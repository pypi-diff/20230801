# Comparing `tmp/macrometa-target-oracle-0.0.9.tar.gz` & `tmp/macrometa-target-oracle-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-oracle-0.0.9.tar", max compression
+gzip compressed data, was "macrometa-target-oracle-1.0.0.tar", max compression
```

## Comparing `macrometa-target-oracle-0.0.9.tar` & `macrometa-target-oracle-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-06 09:40:54.271446 macrometa-target-oracle-0.0.9/LICENSE
--rw-r--r--   0        0        0    23903 2023-07-06 09:40:54.271446 macrometa-target-oracle-0.0.9/macrometa_target_oracle/__init__.py
--rw-r--r--   0        0        0    35237 2023-07-06 09:40:54.271446 macrometa-target-oracle-0.0.9/macrometa_target_oracle/db_sync.py
--rw-r--r--   0        0        0     1538 2023-07-06 09:40:54.523401 macrometa-target-oracle-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.9/setup.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 08:41:16.156628 macrometa-target-oracle-1.0.0/LICENSE
+-rw-r--r--   0        0        0    26064 2023-08-01 08:41:16.160629 macrometa-target-oracle-1.0.0/macrometa_target_oracle/__init__.py
+-rw-r--r--   0        0        0    35359 2023-08-01 08:41:16.160629 macrometa-target-oracle-1.0.0/macrometa_target_oracle/db_sync.py
+-rw-r--r--   0        0        0     1567 2023-08-01 08:41:16.408628 macrometa-target-oracle-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 macrometa-target-oracle-1.0.0/setup.py
+-rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 macrometa-target-oracle-1.0.0/PKG-INFO
```

### Comparing `macrometa-target-oracle-0.0.9/LICENSE` & `macrometa-target-oracle-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.9/macrometa_target_oracle/__init__.py` & `macrometa-target-oracle-1.0.0/macrometa_target_oracle/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 #!/usr/bin/env python3
 import argparse
 import asyncio
 import copy
 import json
+import os
 import sys
 from asyncio import Queue as AsyncQueue
-from datetime import datetime
+from datetime import datetime, timezone
 from decimal import Decimal
 from threading import Lock
 from typing import AsyncIterable
 
 import pkg_resources
 from c8connector import C8Connector, Sample, ConfigAttributeType, Schema
-from c8connector import ConfigProperty
+from c8connector import ConfigProperty, ensure_datetime
 from joblib import Parallel, delayed, parallel_backend
 from jsonschema import Draft7Validator, FormatChecker
+from prometheus_client import CollectorRegistry, Counter, Gauge, start_http_server
 from singer import get_logger
 
 from macrometa_target_oracle.db_sync import DbSync, create_wallet_file, delete_wallet_file
 
 LOGGER = get_logger('macrometa_target_oracle')
 
 DEFAULT_BATCH_SIZE_ROWS = 10000
 DEFAULT_PARALLELISM = 0  # 0 The number of threads used to flush tables
 DEFAULT_MAX_PARALLELISM = 16  # Don't use more than this number of threads by default when flushing streams in parallel
 DEFAULT_BATCH_FLUSH_INTERVAL = 60
 DEFAULT_MIN_BATCH_FLUSH_TIME_GAP = 60
 
+# Create a custom CollectorRegistry
+registry_package = CollectorRegistry()
+export_lag = Gauge("export_lag", "The average time from when the data changes in GDN collections are reflected in external data sources",
+                   ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
+export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections",
+                        ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
+
+region_label = os.getenv("GDN_FEDERATION", "NA")
+tenant_label = os.getenv("GDN_TENANT", "NA")
+fabric_label = os.getenv("GDN_FABRIC", "NA")
+workflow_label = os.getenv("WORKFLOW_UUID", "NA")
+
 
 class OracleTargetConnector(C8Connector):
     """OracleTargetConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
         return "OracleDB"
@@ -177,14 +191,16 @@
 
 def add_metadata_values_to_record(record_message):
     """Populate metadata _sdc columns from incoming record message
     The location of the required attributes are fixed in the stream
     """
     extended_record = record_message['record']
     sdc_deleted_at = record_message.get('record', {}).get('_sdc_deleted_at')
+    if sdc_deleted_at:
+        sdc_deleted_at = datetime.strptime(sdc_deleted_at, '%Y-%m-%dT%H:%M:%S.%fZ')
     extended_record['_sdc_deleted_at'] = sdc_deleted_at
 
     return extended_record
 
 
 def emit_state(state):
     """Emit state message to standard output then it can be
@@ -198,15 +214,15 @@
 
 async def persist_line(line, message_queue) -> None:
     await message_queue.put(line)
 
 
 async def process_messages(message_queue, state, flushed_state, flush_lock, schemas, key_properties,
                          validators, records_to_load, row_count, stream_to_sync, total_row_count, 
-                         hard_delete, batch_size_rows, time_schedule, config) -> None:
+                         hard_delete, batch_size_rows, time_schedule, config, time_extracted_list) -> None:
     """Read stdin messages and process them line by line"""
     while True:
         line = await message_queue.get()
         try:
             o = json.loads(line)
         except json.decoder.JSONDecodeError:
             LOGGER.error('Unable to parse:\n%s', line)
@@ -247,14 +263,18 @@
                 # increment row count only when a new PK is encountered in the current batch
                 if primary_key_string not in records_to_load[stream]:
                     row_count[stream] += 1
                     total_row_count[stream] += 1
 
                 # append record
                 records_to_load[stream][primary_key_string] = add_metadata_values_to_record(o)
+                if 'time_extracted' in o:
+                    time_extracted_list.append(ensure_datetime(o["time_extracted"]))
+                else:
+                    time_extracted_list.append(datetime.now(timezone.utc))
 
                 row_count[stream] = len(records_to_load[stream])
 
                 if row_count[stream] >= batch_size_rows:
                     # flush all streams, delete records if needed, reset counts and then emit current state
                     if config.get('flush_all_streams'):
                         filter_streams = None
@@ -264,14 +284,15 @@
                     # Flush and return a new state dict with new positions only for the flushed streams
                     flushed_state = flush_streams(records_to_load,
                                                   row_count,
                                                   stream_to_sync,
                                                   config,
                                                   state,
                                                   flushed_state,
+                                                  time_extracted_list,
                                                   filter_streams=filter_streams)
                     # emit last encountered state
                     emit_state(copy.deepcopy(flushed_state))
                     time_schedule['last_executed_time'] = datetime.now()
 
         elif t == 'STATE':
             with flush_lock:
@@ -289,15 +310,16 @@
 
             schemas[stream] = float_to_decimal(o['schema'])
             validators[stream] = Draft7Validator(schemas[stream], format_checker=FormatChecker())
 
             with flush_lock:
                 # flush records from previous stream SCHEMA
                 if row_count.get(stream, 0) > 0:
-                    flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state, flushed_state)
+                    flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, 
+                                                  state, flushed_state, time_extracted_list)
                     # emit latest encountered state
                     emit_state(flushed_state)
                     time_schedule['last_executed_time'] = datetime.now()
 
                 # key_properties key must be available in the SCHEMA message.
                 if 'key_properties' not in o:
                     raise Exception("key_properties field is required")
@@ -338,14 +360,15 @@
 def flush_streams(
         streams,
         row_count,
         stream_to_sync,
         config,
         state,
         flushed_state,
+        time_extracted_list,
         filter_streams=None) -> dict:
     """
     Flushes all buckets and resets records count to 0 as well as empties records to load list
     :param streams: dictionary with records to load per stream
     :param row_count: dictionary with row count per stream
     :param stream_to_sync: Oracle db sync instance per stream
     :param config: dictionary containing the configuration
@@ -378,21 +401,23 @@
     # Single-host, thread-based parallelism
     with parallel_backend('threading', n_jobs=parallelism):
         Parallel()(delayed(load_stream_batch)(
             stream=stream,
             records_to_load=streams[stream],
             row_count=row_count,
             db_sync=stream_to_sync[stream],
+            time_extracted_list=time_extracted_list,
             delete_rows=config.get('hard_delete', False),
             temp_dir=config.get('temp_dir')
         ) for stream in streams_to_flush)
 
     # reset flushed stream records to empty to avoid flushing same records
     for stream in streams_to_flush:
         streams[stream] = {}
+        time_extracted_list = []
 
         # Update flushed streams
         if filter_streams:
             # update flushed_state position if we have state information for the stream
             if state is not None and stream in state.get('bookmarks', {}):
                 # Create bookmark key if not exists
                 if 'bookmarks' not in flushed_state:
@@ -405,47 +430,52 @@
             flushed_state = copy.deepcopy(state)
 
     # Return with state message with flushed positions
     return flushed_state
 
 
 # pylint: disable=too-many-arguments
-def load_stream_batch(stream, records_to_load, row_count, db_sync, delete_rows=False, temp_dir=None):
+def load_stream_batch(stream, records_to_load, row_count, db_sync, time_extracted_list, delete_rows=False, temp_dir=None):
     """Load a batch of records and do post load operations, like creating
     or deleting rows"""
     # Load into OracleDb
     if row_count[stream] > 0:
-        flush_records(stream, records_to_load, row_count[stream], db_sync, temp_dir)
+        flush_records(stream, records_to_load, row_count[stream], db_sync, time_extracted_list, temp_dir)
 
     # Load finished, create indices if required
     db_sync.create_indices(stream)
 
     # Delete soft-deleted, flagged rows - where _sdc_deleted at is not null
     if delete_rows:
         db_sync.delete_rows(stream)
 
     # reset row count for the current stream
     row_count[stream] = 0
 
 
 # pylint: disable=unused-argument
-def flush_records(stream, records_to_load, row_count, db_sync, temp_dir=None):
+def flush_records(stream, records_to_load, row_count, db_sync, time_extracted_list, temp_dir=None):
     """Take a list of records and load into database"""
     db_sync.process_batch(records_to_load)
+    event_time = datetime.now(timezone.utc)
+    for time_extracted in time_extracted_list:
+        diff = event_time - time_extracted
+        export_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
 
 
 async def setup_flush_task(config, filter_streams=None):
     event_loop = asyncio.get_event_loop()
     state = None
     flushed_state = None
     hard_delete = config.get('hard_delete', False)
     schemas = {}
     key_properties = {}
     validators = {}
     records_to_load = {}
+    time_extracted_list = []
     row_count = {}
     stream_to_sync = {}
     total_row_count = {}
     batch_size_rows = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
     time_schedule = {
         'interval': config.get('batch_flush_interval', DEFAULT_BATCH_FLUSH_INTERVAL),
         'last_executed_time': datetime.now(),
@@ -459,45 +489,45 @@
     asyncio.run_coroutine_threadsafe(
         stdin_reader_coro,
         event_loop)
 
     # Create the process_messages task
     process_messages_coro = process_messages(message_queue, state, flushed_state, flush_lock, schemas, key_properties,
                             validators, records_to_load, row_count, stream_to_sync, total_row_count, 
-                            hard_delete, batch_size_rows, time_schedule, config)
+                            hard_delete, batch_size_rows, time_schedule, config, time_extracted_list)
     asyncio.run_coroutine_threadsafe(
         process_messages_coro,
         event_loop)
 
     # Create the flush_task task
     flush_task_coro = flush_task(time_schedule, records_to_load, row_count, stream_to_sync, config, state, 
-                                 flushed_state, flush_lock, filter_streams)
+                                 flushed_state, flush_lock, time_extracted_list, filter_streams)
     asyncio.run_coroutine_threadsafe(
         flush_task_coro,
         event_loop)
 
     # Wait for all Futures to complete and propagate any exceptions raised
     await asyncio.gather(
         stdin_reader_coro,
         process_messages_coro,
         flush_task_coro,
     )
 
 
 async def flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state,
-                     flush_lock, filter_streams=None) -> None:
+                     flush_lock, time_extracted_list, filter_streams=None) -> None:
     while True:
         await asyncio.sleep(time_schedule['interval'])
         timedelta = datetime.now() - time_schedule['last_executed_time']
         if timedelta.total_seconds() >= time_schedule['min_time_gap']:
             with flush_lock:
                 # if bucket has records that need to be flushed but haven't reached batch size then flush all buckets.
                 if sum(row_count.values()) > 0:
                     flushed_state = flush_streams(streams, row_count, stream_to_sync, config, state, flushed_state,
-                                                  filter_streams)
+                                                  time_extracted_list, filter_streams)
                     # emit latest state
                     emit_state(copy.deepcopy(flushed_state))
                     time_schedule['last_executed_time'] = datetime.now()
 
 
 async def read_stdin() -> AsyncIterable[str]:
     loop = asyncio.get_event_loop()
@@ -515,14 +545,17 @@
     lines = read_stdin()
     async for line in lines:
         await persist_line(line, message_queue)
 
 
 async def main_impl():
     """Main implementation"""
+    # Start the Prometheus HTTP server for exposing metrics
+    LOGGER.info("Oracle target is starting the metrics server.")
+    start_http_server(8001, registry=registry_package)
     arg_parser = argparse.ArgumentParser()
     arg_parser.add_argument('-c', '--config', help='Config file')
     args = arg_parser.parse_args()
 
     if args.config:
         with open(args.config) as config_input:
             config = json.load(config_input)
@@ -531,14 +564,16 @@
 
     try:
         config = create_wallet_file(config)
         await setup_flush_task(config)
 
         LOGGER.debug("Exiting normally")
     except Exception as e:
+        # Increment export_errors metric
+        export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         delete_wallet_file(config)
         raise e
     delete_wallet_file(config)
     return
 
 
 def main():
```

### Comparing `macrometa-target-oracle-0.0.9/macrometa_target_oracle/db_sync.py` & `macrometa-target-oracle-1.0.0/macrometa_target_oracle/db_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,26 +218,27 @@
         self.logger = get_logger('macrometa_target_oracle')
 
         # Validate connection configuration
         config_errors = validate_config(connection_config)
 
         # Exit if config has errors
         if len(config_errors) > 0:
-            self.logger.error("Invalid configuration:\n   * %s", '\n   * '.join(config_errors))
-            sys.exit(1)
+            error_msg = "Invalid configuration:\n   * {}".format('\n   * '.join(config_errors))
+            self.logger.error(error_msg)
+            raise Exception(error_msg)
 
         self.schema_name = None
         self.grantees = None
 
         # Init stream schema
         if stream_schema_message is not None:
             # Define initial list of indices to created
             self.hard_delete = self.connection_config.get('hard_delete', False)
             if self.hard_delete:
-                self.indices = ['_sdc_deleted_at']
+                self.indices = ['"_sdc_deleted_at"']
             else:
                 self.indices = []
 
             #  Define target schema name.
             #  --------------------------
             #  Target schema name can be defined in multiple ways:
             #
@@ -306,15 +307,14 @@
             dsn = dsn.replace("tcp", "tcps", 1)
             dsn = f"{dsn}?wallet_location=" + config.get('ewallet_pem')
 
         return dsn
 
     def open_connection(self):
         dsn = self.make_dsn(self.connection_config)
-        self.logger.info("dsn: %s", dsn)
         wallet_password = None
         wallet_location = None
         if self.connection_config.get('ewallet_pem'):
             wallet_location = self.connection_config["ewallet_pem"]
             if self.connection_config.get('wallet_password'):
                 wallet_password = self.connection_config["wallet_password"]
         return oracledb.connect(
@@ -327,15 +327,15 @@
 
     def query(self, query, params=None, ignore_rowcount=False):
         self.logger.debug("Running query: %s , params: %s", query, params)
         with self.open_connection() as connection:
             with connection.cursor() as cur:
                 cur.execute("ALTER SESSION SET TIME_ZONE = '00:00'")
                 if self.connection_config.get('multitenant'):
-                    cur.execute(f"ALTER SESSION SET CONTAINER = {self.connection_config.get('pdb_name', 'CDB$ROOT')}") #Switch to expected PDB
+                    cur.execute(f'ALTER SESSION SET CONTAINER = "{self.connection_config.get("pdb_name", "CDB$ROOT")}"') #Switch to expected PDB
                 cur.execute("""ALTER SESSION SET NLS_DATE_FORMAT = 'YYYY-MM-DD"T"HH24:MI:SS."00+00:00"'""")
                 cur.execute("""ALTER SESSION SET NLS_TIMESTAMP_FORMAT='YYYY-MM-DD"T"HH24:MI:SSXFF"+00:00"'""")
                 cur.execute("""ALTER SESSION SET NLS_TIMESTAMP_TZ_FORMAT  = 'YYYY-MM-DD"T"HH24:MI:SS.FFTZH:TZM'""")
                 cur.execute(
                     query,
                     params
                 )
@@ -451,27 +451,26 @@
     def to_sql_type(self, jsonschema_type: dict) -> sqlalchemy.types.TypeEngine:  # noqa
         """Convert JSON Schema type to a SQL type.
         Args:
             jsonschema_type: The JSON Schema object.
         Returns:
             The SQL type.
         """
+        maxlength = jsonschema_type.get("maxLength", 4000)
         if self._jsonschema_type_check(jsonschema_type, ("string",)):
             datelike_type = self.get_datelike_property_type(jsonschema_type)
             if datelike_type:
                 if datelike_type == "date-time":
                     return cast(
                         sqlalchemy.types.TypeEngine, sqlalchemy.types.TIMESTAMP()
                     )
                 if datelike_type in "time":
                     return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.TIME())
                 if datelike_type == "date":
                     return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.DATE())
-
-            maxlength = jsonschema_type.get("maxLength", 4000)
             return cast(
                 sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR(maxlength)
             )
 
         if self._jsonschema_type_check(jsonschema_type, ("integer",)):
             return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.INTEGER())
         
@@ -532,15 +531,15 @@
 
         stream_schema_message = self.stream_schema_message
         full_table_name = self.table_name(stream_schema_message['stream'], is_temporary=False)
         with self.open_connection() as connection:
             with connection.cursor() as cur:
                 cur.execute("ALTER SESSION SET TIME_ZONE = '00:00'")
                 if self.connection_config.get('multitenant'):
-                    cur.execute(f"ALTER SESSION SET CONTAINER = {self.connection_config.get('pdb_name', 'CDB$ROOT')}") #Switch to expected PDB
+                    cur.execute(f'ALTER SESSION SET CONTAINER = "{self.connection_config.get("pdb_name", "CDB$ROOT")}"') #Switch to expected PDB
                 cur.execute("""ALTER SESSION SET NLS_DATE_FORMAT = 'YYYY-MM-DD"T"HH24:MI:SS."00+00:00"'""")
                 cur.execute("""ALTER SESSION SET NLS_TIMESTAMP_FORMAT='YYYY-MM-DD"T"HH24:MI:SSXFF"+00:00"'""")
                 cur.execute("""ALTER SESSION SET NLS_TIMESTAMP_TZ_FORMAT  = 'YYYY-MM-DD"T"HH24:MI:SS.FFTZH:TZM'""")
                 if key_properties:
                     # Create a temp table (Creates from the table above)
                     tmp_table_name = self.table_name(stream_schema_message['stream'], is_temporary=True)
                     self.logger.info(f"Creating temp table {tmp_table_name}")
@@ -564,18 +563,19 @@
                     merge_sql, droptable = self.merge_upsert_from_table(
                                                 from_table_name=tmp_table_name,
                                                 to_table_name=full_table_name,
                                                 schema=schema,
                                                 join_keys=join_keys,
                                             )
                     cur.execute(merge_sql)
+                    self.logger.info(f"Merge complete. Upserted {cur.rowcount} rows.")
                     connection.commit()
                     cur.execute(droptable)
                     connection.commit()
-                    self.logger.info("Merge complete.")
+                    self.logger.info("Dropped temp table.")
                 else:
                     insert_query, values = self.bulk_insert_records(
                                                 full_table_name=full_table_name,
                                                 schema=schema,
                                                 records=records,
                                             )
                     cur.executemany(insert_query, values)
@@ -673,51 +673,51 @@
         elif isinstance(grantees, str):
             grant_method(schema, grantees)
 
     def create_index(self, stream, column):
         table = self.table_name(stream)
         table_without_schema = self.table_name(stream, without_schema=True)
         index_name = 'i_{}_{}'.format(table_without_schema[:30].replace(' ', '').replace('"', ''),
-                                      column.replace(',', '_'))
+                                      column.replace(',', '_').replace('"', ''))
         query = f"""DECLARE
                       index_count INTEGER;
                     BEGIN
                       -- Check if the index already exists
                       SELECT COUNT(*)
                       INTO index_count
                       FROM all_indexes
                       WHERE owner = '{self.schema_name}' AND table_name = '{table_without_schema}' AND index_name = '{index_name}';
 
                       -- Create the index if it does not exist
                       IF index_count = 0 THEN
                         EXECUTE IMMEDIATE 'CREATE INDEX {index_name} ON {table} ({column})';
                       END IF;
                     END;"""
-        self.logger.info("Creating index on '%s' table on '%s' column(s)... %s", table, column, query)
+        self.logger.info("Creating index on '%s' table on '%s' column(s).", table, column)
         try:
             self.query(query)
         except Exception as e:
             self.logger.warn(f"Failed to create index, error: {e}")
 
     def create_indices(self, stream):
         if isinstance(self.indices, list):
             for index in self.indices:
                 self.create_index(stream, index)
 
     def delete_rows(self, stream):
         table = self.table_name(stream)
-        query = "DELETE FROM {} WHERE _sdc_deleted_at IS NOT NULL".format(table)
+        query = f'DELETE FROM {table} WHERE "_sdc_deleted_at" IS NOT NULL'
         self.logger.info("Deleting rows from '%s' table... %s", table, query)
         with self.open_connection() as connection:
             with connection.cursor() as cur:
                 if self.connection_config.get('multitenant'):
-                    cur.execute(f"ALTER SESSION SET CONTAINER = {self.connection_config.get('pdb_name', 'CDB$ROOT')}") #Switch to expected PDB
+                    cur.execute(f'ALTER SESSION SET CONTAINER = "{self.connection_config.get("pdb_name", "CDB$ROOT")}"') #Switch to expected PDB
                 cur.execute(query)
+                self.logger.info(f"Deleted {cur.rowcount} rows.")
                 connection.commit()
-        self.logger.info("Delete query completed.")
 
     def get_tables(self):
         return self.query(
             f"SELECT table_name FROM all_tables WHERE owner = '{self.schema_name}'",
             ignore_rowcount=True
         )
```

### Comparing `macrometa-target-oracle-0.0.9/pyproject.toml` & `macrometa-target-oracle-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-oracle"
-version='0.0.9'
+version='1.0.0'
 description = "Macrometa target connector for writing data into Oracle DB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -24,19 +24,20 @@
 packages = [
     { include = "macrometa_target_oracle" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = ">=0.0.20"
+c8connector = ">=0.0.29"
 oracledb = "^1.2.2"
 inflection = "0.3.1"
 joblib = "1.2.0"
 sqlalchemy = "^1.4"
+prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-target-oracle = 'macrometa_target_oracle:main'
 
 [tool.poetry.urls]
 "Homepage" = "https://www.macrometa.com/"
```

### Comparing `macrometa-target-oracle-0.0.9/setup.py` & `macrometa-target-oracle-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 packages = \
 ['macrometa_target_oracle']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector>=0.0.20',
+['c8connector>=0.0.29',
  'inflection==0.3.1',
  'joblib==1.2.0',
  'oracledb>=1.2.2,<2.0.0',
  'pipelinewise-singer-python==1.2.0',
+ 'prometheus-client==0.16.0',
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-oracle = macrometa_target_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-oracle',
-    'version': '0.0.9',
+    'version': '1.0.0',
     'description': 'Macrometa target connector for writing data into Oracle DB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-oracle-0.0.9/PKG-INFO` & `macrometa-target-oracle-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: macrometa-target-oracle
-Version: 0.0.9
+Version: 1.0.0
 Summary: Macrometa target connector for writing data into Oracle DB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,OracleDB
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: c8connector (>=0.0.20)
+Requires-Dist: c8connector (>=0.0.29)
 Requires-Dist: inflection (==0.3.1)
 Requires-Dist: joblib (==1.2.0)
 Requires-Dist: oracledb (>=1.2.2,<2.0.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
+Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-target-oracle/issues
 Project-URL: Homepage, https://www.macrometa.com/
```

