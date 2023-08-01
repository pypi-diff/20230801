# Comparing `tmp/macrometa-target-postgres-0.0.9.tar.gz` & `tmp/macrometa-target-postgres-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-postgres-0.0.9.tar", max compression
+gzip compressed data, was "macrometa-target-postgres-1.0.0.tar", max compression
```

## Comparing `macrometa-target-postgres-0.0.9.tar` & `macrometa-target-postgres-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10765 2023-02-14 09:25:46.818995 macrometa-target-postgres-0.0.9/LICENSE
--rw-r--r--   0        0        0    26584 2023-02-14 09:25:46.818995 macrometa-target-postgres-0.0.9/macrometa_target_postgres/__init__.py
--rw-r--r--   0        0        0    26335 2023-02-14 09:25:46.818995 macrometa-target-postgres-0.0.9/macrometa_target_postgres/db_sync.py
--rw-r--r--   0        0        0     1580 2023-02-14 09:25:47.066997 macrometa-target-postgres-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 macrometa-target-postgres-0.0.9/setup.py
--rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 macrometa-target-postgres-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-08-01 08:32:21.788717 macrometa-target-postgres-1.0.0/LICENSE
+-rw-r--r--   0        0        0    32130 2023-08-01 08:32:21.788717 macrometa-target-postgres-1.0.0/macrometa_target_postgres/__init__.py
+-rw-r--r--   0        0        0    27938 2023-08-01 08:32:21.788717 macrometa-target-postgres-1.0.0/macrometa_target_postgres/db_sync.py
+-rw-r--r--   0        0        0     1611 2023-08-01 08:32:22.048720 macrometa-target-postgres-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 macrometa-target-postgres-1.0.0/setup.py
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 macrometa-target-postgres-1.0.0/PKG-INFO
```

### Comparing `macrometa-target-postgres-0.0.9/LICENSE` & `macrometa-target-postgres-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-postgres-0.0.9/macrometa_target_postgres/__init__.py` & `macrometa-target-postgres-1.0.0/macrometa_target_postgres/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,54 @@
 #!/usr/bin/env python3
 import argparse
 import asyncio
 import copy
-import io
 import json
 import os
 import sys
-from asyncio import AbstractEventLoop
-from datetime import datetime
+import uuid
+from asyncio import Queue as AsyncQueue
+from datetime import datetime, timezone
 from decimal import Decimal
+from pathlib import Path
 from tempfile import mkstemp
-from threading import Thread
+from threading import Lock
+from typing import AsyncIterable
+from typing import Dict
 
 import pkg_resources
 from c8connector import C8Connector, Sample, ConfigAttributeType, Schema
-from c8connector import ConfigProperty
+from c8connector import ConfigProperty, ensure_datetime
 from joblib import Parallel, delayed, parallel_backend
 from jsonschema import Draft7Validator, FormatChecker
+from prometheus_client import CollectorRegistry, Counter, Gauge, start_http_server
 from singer import get_logger
 
 from macrometa_target_postgres.db_sync import DbSync
 
 LOGGER = get_logger('macrometa_target_postgres')
 
-DEFAULT_BATCH_SIZE_ROWS = 100000
+DEFAULT_BATCH_SIZE_ROWS = 10000
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
 
 class PostgresTargetConnector(C8Connector):
     """PostgresTargetConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
         return "PostgreSQL"
@@ -67,100 +83,91 @@
         """Fetch sample data using the given configurations."""
         return []
 
     def schemas(self, integration: dict) -> list[Schema]:
         """Get supported schemas using the given configurations."""
         return []
 
+    def reserved_keys(self) -> list[str]:
+        """List of reserved keys for the connector."""
+        return []
+
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
             ConfigProperty('host', 'Host', ConfigAttributeType.STRING, True, False,
                            description='PostgreSQL host.',
                            placeholder_value='postgres_host'),
             ConfigProperty('port', 'Port', ConfigAttributeType.INT, True, False,
                            description='PostgreSQL port.',
                            default_value='5432'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
                            description='PostgreSQL user.',
                            default_value='postgres'),
-            ConfigProperty('password', 'Password', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, True, False,
                            description='PostgreSQL password.',
                            placeholder_value='password'),
             ConfigProperty('dbname', 'Database Name', ConfigAttributeType.STRING, True, False,
                            description='PostgreSQL database name.',
                            default_value='postgres'),
-            ConfigProperty('default_target_schema', 'Target Schema', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('default_target_schema', 'Target Schema', ConfigAttributeType.STRING, True, True,
                            description='Destination Schema name.',
                            placeholder_value='public'),
-            ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, True,
                            description='Destination table name.',
                            placeholder_value='my_table'),
             ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, False, False,
                            description='When `hard_delete` option is true then DELETE SQL commands will be performed '
                                        'in Postgres to delete rows in tables. It is achieved by continuously checking '
-                                       'the `_SDC_DELETED_AT` metadata column sent by the singer tap. Due to deleting '
+                                       'the `_SDC_DELETED_AT` metadata column sent by the data source. Due to deleting '
                                        'rows requires metadata columns, `hard_delete` option automatically enables the'
                                        ' `add_metadata_columns` option as well.',
                            default_value='false'),
+            ConfigProperty('ssl', 'Use SSL', ConfigAttributeType.BOOLEAN, False, False,
+                           description='If set to `true` then use SSL via postgres sslmode `require` option.'
+			   	                       ' If the server does not accept SSL connections or the client certificate is not recognized'
+			                           ' then the connection will fail.',
+                           default_value='false'),
+            ConfigProperty('ssl_root_ca_cert', 'SSL CA Certificate', ConfigAttributeType.FILE, False, False,
+                           description='Specific CA certificate in PEM string format. This is most often the case '
+                                       'when using `self-signed` server certificate.',
+                           placeholder_value="my_ca_certificate"),
+            ConfigProperty('ssl_client_certificate', 'SSL Client Certificate', ConfigAttributeType.FILE, False, False,
+                           description='Specific client certificate in PEM string format. The private key for client '
+                                       'certificate should be specfied in a different parameter, SSL Client Key.',
+                           placeholder_value="my_client_certificate"),
+            ConfigProperty('ssl_client_key', 'SSL Client Key', ConfigAttributeType.FILE, False, False,
+                           description='Specific client key in PEM string format.',
+                           placeholder_value="my_client_key"),
+            ConfigProperty('ssl_client_password', 'SSL Client Password', ConfigAttributeType.PASSWORD, False, False,
+                           description='If the private key contained in the SSL Client Key is encrypted, users can provide a '
+                                       'password or passphrase to decrypt the encrypted private keys.',
+                           placeholder_value="my_client_password"),
+            ConfigProperty('connect_timeout', 'Connection Timeout (Seconds)', ConfigAttributeType.INT, False, False,
+                           description='Maximum time to wait while connecting, in seconds (write as a decimal integer, e.g., 10). '
+                                       'Zero or negative means wait indefinitely.',
+                           default_value='30'),
             ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
                            description='Maximum number of rows inserted per batch.',
-                           default_value='100000'),
+                           default_value='10000'),
             ConfigProperty('batch_flush_interval', 'Batch Flush Interval (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Time between batch flush executions.',
                            default_value='60'),
             ConfigProperty('batch_flush_min_time_gap', 'Batch Flush Minimum Time Gap (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Minimum time gap between two batch flush tasks.',
                            default_value='60'),
-            ConfigProperty('flush_all_streams', 'Flush All Streams', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Flush and load every stream into Postgres when one batch is full. '
-                                       'This may trigger the COPY command to use files with low number of records.',
-                           default_value='False'),
-            ConfigProperty('parallelism', 'Parallelism', ConfigAttributeType.INT, False, False,
-                           description='Number of threads used to flush tables. "0" will create a thread for each '
-                                       'stream, up to parallelism_max. "-1" will create a thread for each CPU core. '
-                                       'Any other positive number will create that number of threads, up to '
-                                       'parallelism_max.',
-                           default_value='0'),
-            ConfigProperty('max_parallelism', 'Maximum Parallelism', ConfigAttributeType.INT, False, False,
-                           description='Maximum number of parallel threads used to flush tables.',
-                           default_value='16'),
-            ConfigProperty('default_target_schema_select_permission', 'Target Schema Privileges',
-                           ConfigAttributeType.STRING, False, False,
-                           description='Grant privileges to newly created schemas. Choose from USAGE, SELECT.',
-                           placeholder_value='SELECT'),
             ConfigProperty('add_metadata_columns', 'Add Metadata Columns', ConfigAttributeType.BOOLEAN, False, False,
                            description='Metadata columns add extra row level information about data ingestion, '
                                        '(i.e. when was the row read in source, when was inserted or deleted in '
-                                       'postgres etc.) Metadata columns are creating automatically by adding extra '
+                                       'postgres etc.) Metadata columns are created automatically by adding extra '
                                        'columns to the tables with a column prefix `_SDC_`. The column names are '
                                        'following the stitch naming conventions documented at '
-                                       'https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns '
-                                       'Enabling metadata columns will flag the deleted rows by setting the '
-                                       '`_SDC_DELETED_AT` metadata column. Without the `add_metadata_columns` option '
-                                       'the deleted rows from singer taps will not be recognisable in Postgres.',
-                           default_value='false'),
-            ConfigProperty('data_flattening_max_level', 'Data Flattening Maximum Level', ConfigAttributeType.INT, False,
-                           False,
-                           description='Object type RECORD items from taps can be transformed to flattened columns by '
-                                       'creating columns automatically.<br><br>When value is 0 (default) then '
-                                       'flattening functionality is turned off.',
-                           default_value='0'),
-            ConfigProperty('primary_key_required', 'Primary Key Required', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Log based and Incremental replications on tables with no Primary Key cause '
-                                       'duplicates when merging UPDATE events. When set to true, stop loading data '
-                                       'if no Primary Key is defined.',
-                           default_value='true'),
-            ConfigProperty('validate_records', 'Validate Records', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Validate every single record message to the corresponding JSON schema. '
-                                       'This option is disabled by default and invalid RECORD messages will fail only '
-                                       'at load time by Postgres. Enabling this option will detect invalid records '
-                                       'earlier but could cause performance degradation.',
+                                       'https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns.',
                            default_value='false'),
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
@@ -221,38 +228,24 @@
     if state is not None:
         line = json.dumps(state)
         LOGGER.debug('Emitting state %s', line)
         sys.stdout.write("{}\n".format(line))
         sys.stdout.flush()
 
 
-# pylint: disable=too-many-locals,too-many-branches,too-many-statements,invalid-name,consider-iterating-dictionary
-def persist_lines(config, lines) -> None:
-    """Read singer messages and process them line by line"""
-    state = None
-    flushed_state = None
-    hard_delete = config.get('hard_delete', False)
-    schemas = {}
-    key_properties = {}
-    validators = {}
-    records_to_load = {}
-    row_count = {}
-    stream_to_sync = {}
-    total_row_count = {}
-    batch_size_rows = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
-    time_schedule = {
-        'interval': config.get('batch_flush_interval', DEFAULT_BATCH_FLUSH_INTERVAL),
-        'last_executed_time': datetime.now(),
-        'min_time_gap': config.get('batch_flush_min_time_gap', DEFAULT_MIN_BATCH_FLUSH_TIME_GAP)
-    }
-    event_loop = setup_flush_task(time_schedule, records_to_load, row_count, stream_to_sync, config,
-                                  state, flushed_state)
+async def persist_line(line, message_queue) -> None:
+    await message_queue.put(line)
 
-    # Loop over lines from stdin
-    for line in lines:
+
+async def process_messages(event_loop, message_queue, state, flushed_state, flush_lock, schemas, key_properties,
+                         validators, records_to_load, row_count, stream_to_sync, total_row_count, 
+                         hard_delete, batch_size_rows, time_schedule, config, time_extracted_list) -> None:
+    """Read stdin messages and process them line by line"""
+    while True:
+        line = await message_queue.get()
         try:
             o = json.loads(line)
         except json.decoder.JSONDecodeError:
             LOGGER.error('Unable to parse:\n%s', line)
             raise
 
         if 'type' not in o:
@@ -261,152 +254,148 @@
 
         if t == 'RECORD':
             if 'stream' not in o:
                 raise Exception("Line is missing required key 'stream': {}".format(line))
             if o['stream'] not in schemas:
                 raise Exception(
                     "A record for stream {} was encountered before a corresponding schema".format(o['stream']))
-
             # Get schema for this record's stream
             stream = o['stream']
-
             # Validate record
             if config.get('validate_records'):
                 try:
                     validators[stream].validate(float_to_decimal(o['record']))
                 except Exception as ex:
                     if type(ex).__name__ == "InvalidOperation":
                         raise InvalidValidationOperationException(
                             f"Data validation failed and cannot load to destination. RECORD: {o['record']}\n"
                             "multipleOf validations that allows long precisions are not supported (i.e. with 15 digits"
                             "or more) Try removing 'multipleOf' methods from JSON schema.") from ex
                     raise RecordValidationException(
                         f"Record does not pass schema validation. RECORD: {o['record']}") from ex
 
-            primary_key_string = stream_to_sync[stream].record_primary_key_string(o['record'])
-            if not primary_key_string:
-                primary_key_string = 'RID-{}'.format(total_row_count[stream])
-
-            if stream not in records_to_load:
-                records_to_load[stream] = {}
-
-            # increment row count only when a new PK is encountered in the current batch
-            if primary_key_string not in records_to_load[stream]:
-                row_count[stream] += 1
-                total_row_count[stream] += 1
-
-            # append record
-            if config.get('add_metadata_columns') or hard_delete:
-                records_to_load[stream][primary_key_string] = add_metadata_values_to_record(o)
-            else:
-                records_to_load[stream][primary_key_string] = o['record']
-
-            row_count[stream] = len(records_to_load[stream])
-
-            if row_count[stream] >= batch_size_rows:
-                # flush all streams, delete records if needed, reset counts and then emit current state
-                if config.get('flush_all_streams'):
-                    filter_streams = None
+            with flush_lock:
+                primary_key_string = stream_to_sync[stream].record_primary_key_string(o['record'])
+                if not primary_key_string:
+                    primary_key_string = 'RID-{}'.format(total_row_count[stream])
+                if stream not in records_to_load:
+                    records_to_load[stream] = {}
+
+                # increment row count only when a new PK is encountered in the current batch
+                if primary_key_string not in records_to_load[stream]:
+                    row_count[stream] += 1
+                    total_row_count[stream] += 1
+
+                # append record
+                if config.get('add_metadata_columns') or hard_delete:
+                    records_to_load[stream][primary_key_string] = add_metadata_values_to_record(o)
                 else:
-                    filter_streams = [stream]
+                    records_to_load[stream][primary_key_string] = o['record']
+                if 'time_extracted' in o:
+                    time_extracted_list.append(ensure_datetime(o["time_extracted"]))
+                else:
+                    time_extracted_list.append(datetime.now(timezone.utc))
 
-                # Flush and return a new state dict with new positions only for the flushed streams
-                flushed_state = flush_streams(records_to_load,
-                                              row_count,
-                                              stream_to_sync,
-                                              config,
-                                              state,
-                                              flushed_state,
-                                              filter_streams=filter_streams)
-                # emit last encountered state
-                emit_state(copy.deepcopy(flushed_state))
-                time_schedule['last_executed_time'] = datetime.now()
+                row_count[stream] = len(records_to_load[stream])
 
-        elif t == 'STATE':
-            LOGGER.debug('Setting state to %s', o['value'])
-            state = o['value']
+                if row_count[stream] >= batch_size_rows:
+                    # flush all streams, delete records if needed, reset counts and then emit current state
+                    if config.get('flush_all_streams'):
+                        filter_streams = None
+                    else:
+                        filter_streams = [stream]
+
+                    # Flush and return a new state dict with new positions only for the flushed streams
+                    flushed_state = flush_streams(records_to_load,
+                                                  row_count,
+                                                  stream_to_sync,
+                                                  config,
+                                                  state,
+                                                  flushed_state,
+                                                  time_extracted_list,
+                                                  filter_streams=filter_streams)
+                    # emit last encountered state
+                    emit_state(copy.deepcopy(flushed_state))
+                    time_schedule['last_executed_time'] = datetime.now()
 
-            # Initially set flushed state
-            if not flushed_state:
-                flushed_state = copy.deepcopy(state)
+        elif t == 'STATE':
+            with flush_lock:
+                LOGGER.debug('Setting state to %s', o['value'])
+                state = o['value']
+
+                # Initially set flushed state
+                if not flushed_state:
+                    flushed_state = copy.deepcopy(state)
 
         elif t == 'SCHEMA':
             if 'stream' not in o:
                 raise Exception("Line is missing required key 'stream': {}".format(line))
             stream = o['stream']
 
             schemas[stream] = float_to_decimal(o['schema'])
             validators[stream] = Draft7Validator(schemas[stream], format_checker=FormatChecker())
 
-            # flush records from previous stream SCHEMA
-            if row_count.get(stream, 0) > 0:
-                flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state, flushed_state)
-                # emit latest encountered state
-                emit_state(flushed_state)
-                time_schedule['last_executed_time'] = datetime.now()
-
-            # key_properties key must be available in the SCHEMA message.
-            if 'key_properties' not in o:
-                raise Exception("key_properties field is required")
-
-            # Log based and Incremental replications on tables with no Primary Key
-            # cause duplicates when merging UPDATE events.
-            # Stop loading data by default if no Primary Key.
-            #
-            # If you want to load tables with no Primary Key:
-            #  1) Set ` 'primary_key_required': false ` in the macrometa-target-postgres config.json
-            #  or
-            #  2) Use fastsync [postgres-to-postgres, mysql-to-postgres, etc.]
-            if config.get('primary_key_required', True) and len(o['key_properties']) == 0:
-                LOGGER.critical("Primary key is set to mandatory but not defined in the [%s] stream", stream)
-                raise Exception("key_properties field is required")
-
-            key_properties[stream] = o['key_properties']
-
-            if config.get('add_metadata_columns') or hard_delete:
-                stream_to_sync[stream] = DbSync(config, add_metadata_columns_to_schema(o))
-            else:
-                stream_to_sync[stream] = DbSync(config, o)
+            with flush_lock:
+                # flush records from previous stream SCHEMA
+                if row_count.get(stream, 0) > 0:
+                    flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state,
+                                                   flushed_state, time_extracted_list)
+                    # emit latest encountered state
+                    emit_state(flushed_state)
+                    time_schedule['last_executed_time'] = datetime.now()
+
+                # key_properties key must be available in the SCHEMA message.
+                if 'key_properties' not in o:
+                    raise Exception("key_properties field is required")
+
+                # Log based and Incremental replications on tables with no Primary Key
+                # cause duplicates when merging UPDATE events.
+                # Stop loading data by default if no Primary Key.
+                #
+                # If you want to load tables with no Primary Key:
+                #  1) Set ` 'primary_key_required': false ` in the macrometa-target-postgres config.json
+                if config.get('primary_key_required', True) and len(o['key_properties']) == 0:
+                    LOGGER.critical("Primary key is set to mandatory but not defined in the [%s] stream", stream)
+                    raise Exception("key_properties field is required")
+
+                key_properties[stream] = o['key_properties']
 
-            stream_to_sync[stream].create_schema_if_not_exists()
-            stream_to_sync[stream].sync_table()
+                if config.get('add_metadata_columns') or hard_delete:
+                    stream_to_sync[stream] = DbSync(config, add_metadata_columns_to_schema(o))
+                else:
+                    stream_to_sync[stream] = DbSync(config, o)
+
+                stream_to_sync[stream].create_schema_if_not_exists()
+                stream_to_sync[stream].sync_table()
 
-            row_count[stream] = 0
-            total_row_count[stream] = 0
+                row_count[stream] = 0
+                total_row_count[stream] = 0
 
         elif t == 'ACTIVATE_VERSION':
-            LOGGER.debug('ACTIVATE_VERSION message')
+            with flush_lock:
+                LOGGER.debug('ACTIVATE_VERSION message')
 
-            # Initially set flushed state
-            if not flushed_state:
-                flushed_state = copy.deepcopy(state)
+                # Initially set flushed state
+                if not flushed_state:
+                    flushed_state = copy.deepcopy(state)
 
         else:
             raise Exception("Unknown message type {} in message {}"
                             .format(o['type'], o))
 
-    # if some bucket has records that need to be flushed but haven't reached batch size
-    # then flush all buckets.
-    if sum(row_count.values()) > 0:
-        # flush all streams one last time, delete records if needed, reset counts and then emit current state
-        flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state, flushed_state)
-        time_schedule['last_executed_time'] = datetime.now()
-    # emit latest state
-    emit_state(copy.deepcopy(flushed_state))
-    event_loop.stop()
-
 
 # pylint: disable=too-many-arguments
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
     :param stream_to_sync: Postgres db sync instance per stream
     :param config: dictionary containing the configuration
@@ -439,21 +428,23 @@
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
@@ -466,34 +457,34 @@
             flushed_state = copy.deepcopy(state)
 
     # Return with state message with flushed positions
     return flushed_state
 
 
 # pylint: disable=too-many-arguments
-def load_stream_batch(stream, records_to_load, row_count, db_sync, delete_rows=False, temp_dir=None):
+def load_stream_batch(stream, records_to_load, row_count, db_sync, time_extracted_list, delete_rows=False, temp_dir=None):
     """Load a batch of records and do post load operations, like creating
     or deleting rows"""
     # Load into Postgres
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
     if temp_dir:
         temp_dir = os.path.expanduser(temp_dir)
         os.makedirs(temp_dir, exist_ok=True)
 
     size_bytes = 0
     csv_fd, csv_file = mkstemp(suffix='.csv', prefix=f'{stream}_', dir=temp_dir)
@@ -501,63 +492,220 @@
         for record in records_to_load.values():
             csv_line = db_sync.record_to_csv_line(record)
             f.write(bytes(csv_line + '\n', 'UTF-8'))
 
     size_bytes = os.path.getsize(csv_file)
     db_sync.load_csv(csv_file, row_count, size_bytes)
 
+    event_time = datetime.now(timezone.utc)
+    for time_extracted in time_extracted_list:
+        diff = event_time - time_extracted
+        export_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
+
     # Delete temp file
     os.remove(csv_file)
 
 
-def setup_flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state,
-                     filter_streams=None) -> AbstractEventLoop:
-    event_loop = asyncio.new_event_loop()
-    Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
+async def setup_flush_task(config, filter_streams=None):
+    event_loop = asyncio.get_event_loop()
+    state = None
+    flushed_state = None
+    hard_delete = config.get('hard_delete', False)
+    schemas = {}
+    key_properties = {}
+    validators = {}
+    records_to_load = {}
+    time_extracted_list = []
+    row_count = {}
+    stream_to_sync = {}
+    total_row_count = {}
+    batch_size_rows = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
+    time_schedule = {
+        'interval': config.get('batch_flush_interval', DEFAULT_BATCH_FLUSH_INTERVAL),
+        'last_executed_time': datetime.now(),
+        'min_time_gap': config.get('batch_flush_min_time_gap', DEFAULT_MIN_BATCH_FLUSH_TIME_GAP)
+    }
+    flush_lock = Lock()
+    message_queue = AsyncQueue()
+
+    # Create the stdin_reader task
+    stdin_reader_coro = stdin_reader(message_queue)
+    asyncio.run_coroutine_threadsafe(
+        stdin_reader_coro,
+        event_loop)
+
+    # Create the process_messages task
+    process_messages_coro = process_messages(event_loop, message_queue, state, flushed_state, flush_lock, schemas, key_properties,
+                            validators, records_to_load, row_count, stream_to_sync, total_row_count, 
+                            hard_delete, batch_size_rows, time_schedule, config, time_extracted_list)
     asyncio.run_coroutine_threadsafe(
-        flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state, filter_streams),
+        process_messages_coro,
         event_loop)
-    return event_loop
+
+    # Create the flush_task task
+    flush_task_coro = flush_task(time_schedule, records_to_load, row_count, stream_to_sync, config, state, 
+                                 flushed_state, flush_lock, time_extracted_list, filter_streams)
+    asyncio.run_coroutine_threadsafe(
+        flush_task_coro,
+        event_loop)
+
+    # Wait for all Futures to complete and propagate any exceptions raised
+    await asyncio.gather(
+        stdin_reader_coro,
+        process_messages_coro,
+        flush_task_coro,
+    )
 
 
 async def flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state,
-                     filter_streams=None) -> None:
+                     flush_lock, time_extracted_list, filter_streams=None) -> None:
     while True:
         await asyncio.sleep(time_schedule['interval'])
         timedelta = datetime.now() - time_schedule['last_executed_time']
         if timedelta.total_seconds() >= time_schedule['min_time_gap']:
-            # if some bucket has records that need to be flushed but haven't reached batch size then flush all buckets.
-            if sum(row_count.values()) > 0:
-                # flush all streams one last time, delete records if needed, reset counts and then emit current state.
-                flushed_state = flush_streams(streams, row_count, stream_to_sync, config, state, flushed_state,
-                                              filter_streams)
-                # emit latest state
-                emit_state(copy.deepcopy(flushed_state))
-                time_schedule['last_executed_time'] = datetime.now()
-
+            with flush_lock:
+                # if bucket has records that need to be flushed but haven't reached batch size then flush all buckets.
+                if sum(row_count.values()) > 0:
+                    flushed_state = flush_streams(streams, row_count, stream_to_sync, config, state, flushed_state,
+                                                  time_extracted_list, filter_streams)
+                    # emit latest state
+                    emit_state(copy.deepcopy(flushed_state))
+                    time_schedule['last_executed_time'] = datetime.now()
+
+
+def create_certficate_files(config: Dict) -> Dict:
+    path_uuid = uuid.uuid4().hex
+    try:
+        if config.get('ssl_root_ca_cert'):
+            path = f"/opt/postgresql/{path_uuid}/ca.crt"
+            ca_cert = Path(path)
+            ca_cert.parent.mkdir(exist_ok=True, parents=True)
+            ca_cert.write_text(create_ssl_string(config['ssl_root_ca_cert']))
+            ca_cert.chmod(0o600)
+            config['ssl_root_ca_cert'] = path
+            LOGGER.info(f"CA certificate file created at: {path}")
+
+        if config.get('ssl_client_certificate'):
+            path = f"/opt/postgresql/{path_uuid}/client.crt"
+            client_cert = Path(path)
+            client_cert.parent.mkdir(exist_ok=True, parents=True)
+            client_cert.write_text(create_ssl_string(config['ssl_client_certificate']))
+            client_cert.chmod(0o600)
+            config['ssl_client_certificate'] = path
+            LOGGER.info(f"Client certificate file created at: {path}")
+
+        if config.get('ssl_client_key'):
+            path = f"/opt/postgresql/{path_uuid}/client.key"
+            client_cert = Path(path)
+            client_cert.parent.mkdir(exist_ok=True, parents=True)
+            client_cert.write_text(create_ssl_string(config['ssl_client_key']))
+            client_cert.chmod(0o600)
+            config['ssl_client_key'] = path
+            LOGGER.info(f"Client key file created at: {path}")
+    except Exception as e:
+        LOGGER.warn(f"Failed to create certificate: /opt/postgresql/{path_uuid}/. {e}")
+    return config
+
+def delete_certficate_files(config: Dict) -> None:
+    try:
+        cert = None
+        if config.get('ssl_root_ca_cert'):
+            path = config['ssl_root_ca_cert']
+            cert = Path(path)
+            config['ssl_root_ca_cert'] = cert.read_text()
+            cert.unlink()
+            LOGGER.info(f"CA certificate file deleted from: {path}")
+
+        if config.get('ssl_client_certificate'):
+            path = config['ssl_client_certificate']
+            cert = Path(path)
+            config['ssl_client_certificate'] = cert.read_text()
+            cert.unlink()
+            LOGGER.info(f"Client certificate file deleted from: {path}")
+
+        if config.get('ssl_client_key'):
+            path = config['ssl_client_key']
+            cert = Path(path)
+            config['ssl_client_key'] = cert.read_text()
+            cert.unlink()
+            LOGGER.info(f"Client key file deleted from: {path}")
+
+        if cert is not None:
+            cert.parent.rmdir()
+    except Exception as e:
+        LOGGER.warn(f"Failed to delete certificate: {e}")
+
+def create_ssl_string(ssl_string: str) -> str:
+    tls_certificate_key_list = []
+    split_string = ssl_string.split("-----")
+    if len(split_string) < 4:
+        raise Exception("Invalid PEM format for certificate.")
+    for i in range(len(split_string)):
+        if((i % 2) == 1):
+            tls_certificate_key_list.append("-----")
+            tls_certificate_key_list.append(split_string[i])
+            tls_certificate_key_list.append("-----")
+        else:
+            tls_certificate_key_list.append(split_string[i].replace(' ', '\n'))
 
-def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
-    asyncio.set_event_loop(loop)
-    loop.run_forever()
+    tls_certificate_key_file = ''.join(tls_certificate_key_list)
+    return tls_certificate_key_file
 
 
-def main():
-    """Main entry point"""
+async def read_stdin() -> AsyncIterable[str]:
+    loop = asyncio.get_event_loop()
+    reader = asyncio.StreamReader()
+    reader_protocol = asyncio.StreamReaderProtocol(reader)
+    await loop.connect_read_pipe(lambda: reader_protocol, sys.stdin)
+    while True:
+        line = await reader.readline()
+        if not line:
+            break
+        yield line.decode('utf-8').rstrip('\r\n')
+
+
+async def stdin_reader(message_queue) -> None:
+    lines = read_stdin()
+    async for line in lines:
+        await persist_line(line, message_queue)
+
+
+async def main_impl():
+    """Main implementation"""
+    # Start the Prometheus HTTP server for exposing metrics
+    LOGGER.info("Postgres target is starting the metrics server.")
+    start_http_server(8001, registry=registry_package)
     arg_parser = argparse.ArgumentParser()
     arg_parser.add_argument('-c', '--config', help='Config file')
     args = arg_parser.parse_args()
 
     if args.config:
         with open(args.config) as config_input:
             config = json.load(config_input)
     else:
         config = {}
 
-    # Consume singer messages
-    singer_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
-    persist_lines(config, singer_messages)
+    try:
+        config = create_certficate_files(config)
+        await setup_flush_task(config)
+
+        LOGGER.debug("Exiting normally")
+    except Exception as e:
+        # Increment export_errors metric
+        export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+        delete_certficate_files(config)
+        raise e
+    delete_certficate_files(config)
+    return
+
 
-    LOGGER.debug("Exiting normally")
+def main():
+    """Main entry point"""
+    try:
+        asyncio.run(main_impl())
+    except Exception as exc:
+        LOGGER.critical(exc)
+        raise exc
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `macrometa-target-postgres-0.0.9/macrometa_target_postgres/db_sync.py` & `macrometa-target-postgres-1.0.0/macrometa_target_postgres/db_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import sys
 import psycopg2
 import psycopg2.extras
+import psycopg2.errors
 import inflection
 import re
 import uuid
 import itertools
 import time
 from collections.abc import MutableMapping
 from singer import get_logger
@@ -18,15 +19,14 @@
         'host',
         'port',
         'user',
         'password',
         'dbname',
         'default_target_schema',
         'target_table',
-        'hard_delete',
     ]
 
     # Check if mandatory keys exist
     for k in required_config_keys:
         if not config.get(k, None):
             errors.append("Required key is missing from config: [{}]".format(k))
 
@@ -213,16 +213,17 @@
         self.logger = get_logger('macrometa_target_postgres')
 
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
@@ -300,17 +301,26 @@
             self.connection_config['host'],
             self.connection_config['dbname'],
             self.connection_config['user'],
             self.connection_config['password'],
             self.connection_config['port']
         )
 
-        if 'ssl' in self.connection_config and self.connection_config['ssl'] == 'true':
+        if self.connection_config.get('ssl', False):
             conn_string += " sslmode='require'"
+            if self.connection_config.get('ssl_root_ca_cert'):
+                conn_string += " sslrootcert='{}'".format(self.connection_config['ssl_root_ca_cert'])
+            if self.connection_config.get('ssl_client_certificate'):
+                conn_string += " sslcert='{}'".format(self.connection_config['ssl_client_certificate'])
+                if self.connection_config.get('ssl_client_key'):
+                    conn_string += " sslkey='{}'".format(self.connection_config['ssl_client_key'])
+                if self.connection_config.get('ssl_client_password'):
+                    conn_string += " sslpassword='{}'".format(self.connection_config['ssl_client_password'])
 
+        conn_string += " connect_timeout='{}'".format(self.connection_config.get('connect_timeout', 30))
         return psycopg2.connect(conn_string)
 
     def query(self, query, params=None):
         self.logger.debug("Running query: %s", query)
         with self.open_connection() as connection:
             with connection.cursor(cursor_factory=psycopg2.extras.DictCursor) as cur:
                 cur.execute(
@@ -360,39 +370,50 @@
             ]
         )
 
     def load_csv(self, file, count, size_bytes):
         stream_schema_message = self.stream_schema_message
         stream = stream_schema_message['stream']
         self.logger.info("Loading %d rows into '%s'", count, self.table_name(stream, False))
-
-        with self.open_connection() as connection:
-            with connection.cursor(cursor_factory=psycopg2.extras.DictCursor) as cur:
-                inserts = 0
-                updates = 0
-
-                temp_table = self.table_name(stream_schema_message['stream'], is_temporary=True)
-                cur.execute(self.create_table_query(table_name=temp_table, is_temporary=True))
-
-                copy_sql = "COPY {} ({}) FROM STDIN WITH (FORMAT CSV, ESCAPE '\\')".format(
-                    temp_table,
-                    ', '.join(self.column_names())
-                )
-                self.logger.debug(copy_sql)
-                with open(file, "rb") as f:
-                    cur.copy_expert(copy_sql, f)
-                if len(self.stream_schema_message['key_properties']) > 0:
-                    cur.execute(self.update_from_temp_table(temp_table))
-                    updates = cur.rowcount
-                cur.execute(self.insert_from_temp_table(temp_table))
-                inserts = cur.rowcount
-
-                self.logger.info('Loading into %s: %s',
-                                 self.table_name(stream, False),
-                                 json.dumps({'inserts': inserts, 'updates': updates, 'size_bytes': size_bytes}))
+        # If creating temp table fails due to internal cache error then retry
+        max_retry = 4
+        base_delay = 2
+
+        for retry_count in range(max_retry):
+            try:
+                with self.open_connection() as connection:
+                    with connection.cursor(cursor_factory=psycopg2.extras.DictCursor) as cur:
+                        inserts = 0
+                        updates = 0
+                        temp_table = self.table_name(stream_schema_message['stream'], is_temporary=True)
+                        cur.execute(self.create_table_query(table_name=temp_table, is_temporary=True))
+
+                        copy_sql = "COPY {} ({}) FROM STDIN WITH (FORMAT CSV, ESCAPE '\\')".format(
+                            temp_table,
+                            ', '.join(self.column_names())
+                        )
+                        self.logger.debug(copy_sql)
+                        with open(file, "rb") as f:
+                            cur.copy_expert(copy_sql, f)
+                        if len(self.stream_schema_message['key_properties']) > 0:
+                            cur.execute(self.update_from_temp_table(temp_table))
+                            updates = cur.rowcount
+                        cur.execute(self.insert_from_temp_table(temp_table))
+                        inserts = cur.rowcount
+                        self.logger.info('Loading into %s: %s',
+                                         self.table_name(stream, False),
+                                         json.dumps({'inserts': inserts, 'updates': updates, 'size_bytes': size_bytes}))
+                break
+            except psycopg2.errors.InternalError_ as e:
+                if "cache lookup failed for type" in str(e) and retry_count < (max_retry - 1):
+                    self.logger.warn(f"Failed to create temp table {temp_table}, internal cache "
+                                     f"lookup error. Retrying {retry_count}...")
+                    time.sleep(base_delay)
+                else:
+                    raise e
 
     # pylint: disable=duplicate-string-formatting-argument
     def insert_from_temp_table(self, temp_table):
         stream_schema_message = self.stream_schema_message
         columns = self.column_names()
         table = self.table_name(stream_schema_message['stream'])
```

### Comparing `macrometa-target-postgres-0.0.9/pyproject.toml` & `macrometa-target-postgres-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-postgres"
-version='0.0.9'
+version='1.0.0'
 description = "Pipelinewise target for writing data into Postgres."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -24,21 +24,22 @@
 packages = [
     { include = "macrometa_target_postgres" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = "0.0.14"
+c8connector = ">=0.0.29"
 psycopg2-binary = "2.9.3"
 inflection = "0.3.1"
 joblib = "1.2.0"
 pytest-cov = "2.10.1"
 pytest = "6.2.5"
 pylint = "2.6.0"
+prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-target-postgres = 'macrometa_target_postgres:main'
 
 [tool.poetry.urls]
 "Homepage" = "https://www.macrometa.com/"
```

### Comparing `macrometa-target-postgres-0.0.9/setup.py` & `macrometa-target-postgres-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 packages = \
 ['macrometa_target_postgres']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector==0.0.14',
+['c8connector>=0.0.29',
  'inflection==0.3.1',
  'joblib==1.2.0',
  'pipelinewise-singer-python==1.2.0',
+ 'prometheus-client==0.16.0',
  'psycopg2-binary==2.9.3',
  'pylint==2.6.0',
  'pytest-cov==2.10.1',
  'pytest==6.2.5']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-postgres = '
                      'macrometa_target_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-postgres',
-    'version': '0.0.9',
+    'version': '1.0.0',
     'description': 'Pipelinewise target for writing data into Postgres.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-postgres-0.0.9/PKG-INFO` & `macrometa-target-postgres-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: macrometa-target-postgres
-Version: 0.0.9
+Version: 1.0.0
 Summary: Pipelinewise target for writing data into Postgres.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,Postgres
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
-Requires-Dist: c8connector (==0.0.14)
+Requires-Dist: c8connector (>=0.0.29)
 Requires-Dist: inflection (==0.3.1)
 Requires-Dist: joblib (==1.2.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
+Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: psycopg2-binary (==2.9.3)
 Requires-Dist: pylint (==2.6.0)
 Requires-Dist: pytest (==6.2.5)
 Requires-Dist: pytest-cov (==2.10.1)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-target-postgres/issues
 Project-URL: Homepage, https://www.macrometa.com/
```

