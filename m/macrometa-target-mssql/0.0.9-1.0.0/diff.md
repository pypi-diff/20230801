# Comparing `tmp/macrometa-target-mssql-0.0.9.tar.gz` & `tmp/macrometa-target-mssql-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mssql-0.0.9.tar", max compression
+gzip compressed data, was "macrometa-target-mssql-1.0.0.tar", max compression
```

## Comparing `macrometa-target-mssql-0.0.9.tar` & `macrometa-target-mssql-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-29 18:29:02.540852 macrometa-target-mssql-0.0.9/LICENSE
--rw-r--r--   0        0        0    24117 2023-06-29 18:29:02.540852 macrometa-target-mssql-0.0.9/macrometa_target_mssql/__init__.py
--rw-r--r--   0        0        0    34144 2023-06-29 18:29:02.540852 macrometa-target-mssql-0.0.9/macrometa_target_mssql/db_sync.py
--rw-r--r--   0        0        0     1554 2023-06-29 18:29:02.800850 macrometa-target-mssql-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.9/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 08:38:06.842513 macrometa-target-mssql-1.0.0/LICENSE
+-rw-r--r--   0        0        0    25172 2023-08-01 08:38:06.842513 macrometa-target-mssql-1.0.0/macrometa_target_mssql/__init__.py
+-rw-r--r--   0        0        0    31181 2023-08-01 08:38:06.842513 macrometa-target-mssql-1.0.0/macrometa_target_mssql/db_sync.py
+-rw-r--r--   0        0        0     1583 2023-08-01 08:38:07.082509 macrometa-target-mssql-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 macrometa-target-mssql-1.0.0/setup.py
+-rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 macrometa-target-mssql-1.0.0/PKG-INFO
```

### Comparing `macrometa-target-mssql-0.0.9/LICENSE` & `macrometa-target-mssql-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.9/macrometa_target_mssql/__init__.py` & `macrometa-target-mssql-1.0.0/macrometa_target_mssql/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,49 @@
 import argparse
 import asyncio
 import copy
 import json
 import os
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
 
 from macrometa_target_mssql.db_sync import DbSync
 
 LOGGER = get_logger('macrometa_target_mssql')
 
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
 
 class MicrosoftSQLServerTargetConnector(C8Connector):
     """MicrosoftSQLServerTargetConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
         return "Microsoft SQL Server"
@@ -88,50 +101,41 @@
                            placeholder_value='username'),
             ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, True, False,
                            description='Microsoft SQL Server password.',
                            placeholder_value='password'),
             ConfigProperty('database', 'Database Name', ConfigAttributeType.STRING, True, False,
                            description='Microsoft SQL Server database name.',
                            default_value='master'),
-            ConfigProperty('default_target_schema', 'Target Schema', ConfigAttributeType.STRING, True, True,
+            ConfigProperty('target_schema', 'Target Schema', ConfigAttributeType.STRING, True, True,
                            description='Destination Schema name.',
-                           placeholder_value='public'),
+                           placeholder_value='dbo'),
             ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, True,
                            description='Destination table name.',
                            placeholder_value='my_table'),
-            ConfigProperty('prefer_float_over_numeric', 'Prefer Float over Numeric',
-                           ConfigAttributeType.INT, False, False,
-                           description='Use float data type for numbers (otherwise number type is used)',
-                           default_value='0'),
             ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, False, False,
                            description='When `hard_delete` option is true then DELETE SQL commands will be performed '
-                                       'in MSSQL to delete rows in tables. It is achieved by continuously checking '
-                                       'the `_SDC_DELETED_AT` metadata column sent by the data source. Due to deleting '
-                                       'rows requires metadata columns, `hard_delete` option automatically enables the'
-                                       ' `add_metadata_columns` option as well.',
+                                       'in MS SQL Server to delete rows from the table. It is achieved by continuously checking '
+                                       'the `_SDC_DELETED_AT` metadata column sent by the data source.',
                            default_value='false'),
+            ConfigProperty('characterset', 'Character Set', ConfigAttributeType.STRING, False, False,
+                           description='The characterset of the Microsoft SQL Server database.', default_value='utf8'),
+            ConfigProperty('tds_version', 'TDS Version', ConfigAttributeType.STRING, False, False,
+                           description='Set the version of TDS to use when communicating with MS SQL Server.',
+                           default_value='7.3'),
             ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
                            description='Maximum number of rows inserted per batch.',
                            default_value='10000'),
             ConfigProperty('batch_flush_interval', 'Batch Flush Interval (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Time between batch flush executions.',
                            default_value='60'),
             ConfigProperty('batch_flush_min_time_gap', 'Batch Flush Minimum Time Gap (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Minimum time gap between two batch flush tasks.',
-                           default_value='60'),
-            ConfigProperty('add_metadata_columns', 'Add Metadata Columns', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Metadata columns add extra row level information about data ingestion, '
-                                       '(i.e. when was the row read in source, when was it inserted or deleted in '
-                                       'mssql etc.) Metadata columns are created automatically by adding extra '
-                                       'columns to the tables with a column prefix `_SDC_`. The column names are '
-                                       'following the stitch naming conventions documented at '
-                                       'https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns.',
-                           default_value='false'),
+                           default_value='60')
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
         return []
@@ -160,31 +164,38 @@
 def add_metadata_columns_to_schema(schema_message):
     """Metadata _sdc columns according to the stitch documentation at
     https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns
 
     Metadata columns gives information about data injections
     """
     extended_schema_message = schema_message
-    extended_schema_message['schema']['properties']['_sdc_extracted_at'] = {'type': ['null', 'string'],
-                                                                            'format': 'date-time'}
-    extended_schema_message['schema']['properties']['_sdc_batched_at'] = {'type': ['null', 'string'],
+    extended_schema_message['schema']['properties']['_sdc_deleted_at'] = {'type': ['null', 'string'],
                                                                           'format': 'date-time'}
-    extended_schema_message['schema']['properties']['_sdc_deleted_at'] = {'type': ['null', 'string']}
 
     return extended_schema_message
 
 
 def add_metadata_values_to_record(record_message):
     """Populate metadata _sdc columns from incoming record message
     The location of the required attributes are fixed in the stream
     """
     extended_record = record_message['record']
-    extended_record['_sdc_extracted_at'] = record_message.get('time_extracted')
-    extended_record['_sdc_batched_at'] = datetime.now().isoformat()
-    extended_record['_sdc_deleted_at'] = record_message.get('record', {}).get('_sdc_deleted_at')
+    sdc_deleted_at = record_message.get('record', {}).get('_sdc_deleted_at')
+    if sdc_deleted_at:
+        try:
+            input_format = "%Y-%m-%dT%H:%M:%S.%fZ"
+            # Convert string to datetime object
+            datetime_obj = datetime.strptime(record_message.get('record', {}).get('_sdc_deleted_at'), input_format)
+            output_format = "%Y-%m-%d %H:%M:%S"
+
+            # Convert datetime object to SQL Server datetime format
+            sdc_deleted_at = datetime_obj.strftime(output_format)
+        except Exception as e:
+            LOGGER.warn(f"Cannot convert _sdc_deleted_at to valid datetime format for MsSql. {e}")
+    extended_record['_sdc_deleted_at'] = sdc_deleted_at
 
     return extended_record
 
 
 def emit_state(state):
     """Emit state message to standard output then it can be
     consumed by other components"""
@@ -197,15 +208,15 @@
 
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
@@ -245,18 +256,20 @@
 
                 # increment row count only when a new PK is encountered in the current batch
                 if primary_key_string not in records_to_load[stream]:
                     row_count[stream] += 1
                     total_row_count[stream] += 1
 
                 # append record
-                if config.get('add_metadata_columns') or hard_delete:
-                    records_to_load[stream][primary_key_string] = add_metadata_values_to_record(o)
+                records_to_load[stream][primary_key_string] = add_metadata_values_to_record(o)
+                if 'time_extracted' in o:
+                    time_extracted_list.append(ensure_datetime(o["time_extracted"]))
                 else:
-                    records_to_load[stream][primary_key_string] = o['record']
+                    time_extracted_list.append(datetime.now(timezone.utc))
+
                 row_count[stream] = len(records_to_load[stream])
 
                 if row_count[stream] >= batch_size_rows:
                     # flush all streams, delete records if needed, reset counts and then emit current state
                     if config.get('flush_all_streams'):
                         filter_streams = None
                     else:
@@ -265,14 +278,15 @@
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
@@ -290,15 +304,16 @@
 
             schemas[stream] = float_to_decimal(o['schema'])
             validators[stream] = Draft7Validator(schemas[stream], format_checker=FormatChecker())
 
             with flush_lock:
                 # flush records from previous stream SCHEMA
                 if row_count.get(stream, 0) > 0:
-                    flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state, flushed_state)
+                    flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config,
+                                                   state, flushed_state, time_extracted_list)
                     # emit latest encountered state
                     emit_state(flushed_state)
                     time_schedule['last_executed_time'] = datetime.now()
 
                 # key_properties key must be available in the SCHEMA message.
                 if 'key_properties' not in o:
                     raise Exception("key_properties field is required")
@@ -311,18 +326,15 @@
                 #  1) Set ` 'primary_key_required': false ` in the macrometa-target-mssql config.json
                 if config.get('primary_key_required', True) and len(o['key_properties']) == 0:
                     LOGGER.critical("Primary key is set to mandatory but not defined in the [%s] stream", stream)
                     raise Exception("key_properties field is required")
 
                 key_properties[stream] = o['key_properties']
 
-                if config.get('add_metadata_columns') or hard_delete:
-                    stream_to_sync[stream] = DbSync(config, add_metadata_columns_to_schema(o))
-                else:
-                    stream_to_sync[stream] = DbSync(config, o)
+                stream_to_sync[stream] = DbSync(config, add_metadata_columns_to_schema(o))
 
                 stream_to_sync[stream].create_schema_if_not_exists()
                 stream_to_sync[stream].sync_table()
 
                 row_count[stream] = 0
                 total_row_count[stream] = 0
 
@@ -343,14 +355,15 @@
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
     :param stream_to_sync: Mssql db sync instance per stream
     :param config: dictionary containing the configuration
@@ -383,21 +396,23 @@
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
@@ -410,47 +425,52 @@
             flushed_state = copy.deepcopy(state)
 
     # Return with state message with flushed positions
     return flushed_state
 
 
 # pylint: disable=too-many-arguments
-def load_stream_batch(stream, records_to_load, row_count, db_sync, delete_rows=False, temp_dir=None):
+def load_stream_batch(stream, records_to_load, row_count, db_sync, time_extracted_list, delete_rows=False, temp_dir=None):
     """Load a batch of records and do post load operations, like creating
     or deleting rows"""
     # Load into Mssql
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
-    db_sync.process_bacth(records_to_load)
+    db_sync.process_batch(records_to_load)
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
@@ -464,45 +484,45 @@
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
@@ -520,26 +540,35 @@
     lines = read_stdin()
     async for line in lines:
         await persist_line(line, message_queue)
 
 
 async def main_impl():
     """Main implementation"""
+    # Start the Prometheus HTTP server for exposing metrics
+    LOGGER.info("Mssql target is starting the metrics server.")
+    start_http_server(8001, registry=registry_package)
+
     arg_parser = argparse.ArgumentParser()
     arg_parser.add_argument('-c', '--config', help='Config file')
     args = arg_parser.parse_args()
 
-    if args.config:
-        with open(args.config) as config_input:
-            config = json.load(config_input)
-    else:
-        config = {}
+    try:
+        if args.config:
+            with open(args.config) as config_input:
+                config = json.load(config_input)
+        else:
+            config = {}
 
-    await setup_flush_task(config)
-    LOGGER.debug("Exiting normally")
+        await setup_flush_task(config)
+        LOGGER.debug("Exiting normally")
+    except Exception as e:
+        # Increment export_errors metric
+        export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+        raise e
     return
 
 
 def main():
     """Main entry point"""
     try:
         asyncio.run(main_impl())
```

### Comparing `macrometa-target-mssql-0.0.9/macrometa_target_mssql/db_sync.py` & `macrometa-target-mssql-1.0.0/macrometa_target_mssql/db_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 import json
 import sys
 import pymssql
 import inflection
 import re
-import uuid
 import itertools
 import sqlalchemy
 import time
 
 from collections.abc import MutableMapping
 from singer import get_logger
-from sqlalchemy import Column
-from textwrap import dedent
-from typing import Any, cast, Dict, Iterable, List, Optional
+from typing import cast, Dict, List, Optional
 
 
 # pylint: disable=missing-function-docstring,missing-class-docstring
 def validate_config(config):
     errors = []
     required_config_keys = [
         'host',
         'port',
         'user',
         'password',
         'database',
-        'default_target_schema',
+        'target_schema',
         'target_table',
     ]
 
     # Check if mandatory keys exist
     for k in required_config_keys:
         if not config.get(k, None):
             errors.append("Required key is missing from config: [{}]".format(k))
 
     # Check target schema config
-    config_default_target_schema = config.get('default_target_schema', None)
+    config_default_target_schema = config.get('target_schema', None)
     config_schema_mapping = config.get('schema_mapping', None)
     if not config_default_target_schema and not config_schema_mapping:
-        errors.append("Neither 'default_target_schema' (string) nor 'schema_mapping' (object) keys set in config.")
+        errors.append("Neither 'target_schema' (string) nor 'schema_mapping' (object) keys set in config.")
 
     return errors
 
 
 def safe_column_name(name):
     return '"{}"'.format(name).lower()
 
@@ -174,16 +171,17 @@
         self.logger = get_logger('macrometa_target_mssql')
 
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
@@ -204,15 +202,15 @@
             #           "schema_mapping": {
             #               "my_tap_stream_id": {
             #                   "target_schema": "my_mssql_schema",
             #                   "target_schema_select_permissions": [ "role_with_select_privs" ],
             #                   "indices": ["column_1", "column_2s"]
             #               }
             #           }
-            config_default_target_schema = self.connection_config.get('default_target_schema', '').strip()
+            config_default_target_schema = self.connection_config.get('target_schema', '').strip()
             config_schema_mapping = self.connection_config.get('schema_mapping', {})
             config_target_table = self.connection_config.get('target_table', '').strip()
 
             stream_name = stream_schema_message['stream']
             stream_schema_name = stream_name_to_dict(stream_name, table_name=config_target_table)['schema_name']
             stream_table_name = stream_name_to_dict(stream_name, table_name=config_target_table)['table_name']
             if config_schema_mapping and stream_schema_name in config_schema_mapping:
@@ -223,15 +221,15 @@
                 if stream_table_name in indices:
                     self.indices.extend(indices.get(stream_table_name, []))
 
             elif config_default_target_schema:
                 self.schema_name = config_default_target_schema
 
             if not self.schema_name:
-                raise Exception("Target schema name not defined in config. Neither 'default_target_schema' (string)"
+                raise Exception("Target schema name not defined in config. Neither 'target_schema' (string)"
                                 "nor 'schema_mapping' (object) defines target schema for {} stream."
                                 .format(stream_name))
 
             #  Define grantees
             #  ---------------
             #  Grantees can be defined in multiple ways:
             #
@@ -252,50 +250,50 @@
                 self.grantees = config_schema_mapping[stream_schema_name].get('target_schema_select_permissions',
                                                                               self.grantees)
 
             self.data_flattening_max_level = self.connection_config.get('data_flattening_max_level', 0)
             self.flatten_schema = flatten_schema(stream_schema_message['schema'],
                                                  max_level=self.data_flattening_max_level)
 
-    def open_connection(self, require_database=True):
+    def open_connection(self):
         args = {
             "user": self.connection_config.get("user"),
             "password": self.connection_config.get("password"),
             "server": self.connection_config["host"],
+            "database": self.connection_config.get("database", "master"),
             "charset": self.connection_config.get("characterset", "utf8"),
+            "autocommit": True,
             "port": self.connection_config.get("port", "1433"),
             "tds_version": self.connection_config.get("tds_version", "7.3")
         }
-        if require_database:
-            args["database"] = self.connection_config["database"]
         return pymssql.connect(**args)
 
-    def query(self, query, params=None, require_database=True):
-        self.logger.info("Running query: %s , params: %s", query, params)
-        with self.open_connection(require_database=require_database) as connection:
+    def query(self, query, params=None, ignore_rowcount=False):
+        self.logger.debug("Running query: %s , params: %s", query, params)
+        with self.open_connection() as connection:
             with connection.cursor(as_dict=True) as cur:
                 cur.execute(
                     query,
                     params
                 )
-
-                if cur.rowcount > 0:
-                    self.logger.info(f"rowcount:{cur.rowcount}")
-                    return cur.fetchall()
-
+                if cur.rowcount > 0 or ignore_rowcount:
+                    try:
+                        return cur.fetchall()
+                    except pymssql.OperationalError as e:
+                        self.logger.warn(f"Exception raised while fetching from cursor. {e}")
                 return []
 
     def table_name(self, stream_name, is_temporary=False, without_schema=False):
         config_target_table = self.connection_config.get('target_table', '').strip()
         stream_dict = stream_name_to_dict(stream_name, table_name=config_target_table)
         table_name = stream_dict['table_name']
         mssql_table_name = table_name.replace('.', '_').replace('-', '_').lower()
 
         if is_temporary:
-            return 'tmp_{}'.format(str(uuid.uuid4()).replace('-', '_'))
+            return f'{self.schema_name}."#{mssql_table_name.lower()}"'
 
         if without_schema:
             return f'"{mssql_table_name.lower()}"'
 
         return f'{self.schema_name}."{mssql_table_name.lower()}"'
 
     def record_primary_key_string(self, record):
@@ -307,99 +305,36 @@
         except Exception as exc:
             self.logger.info("Cannot find %s primary key(s) in record: %s",
                              self.stream_schema_message['key_properties'],
                              flatten)
             raise exc
         return ','.join(key_props)
 
-    def generate_insert_statement(
-        self,
-        full_table_name: str,
-        schema: dict,
-    ):
-        """Generate an insert statement for the given records.
-
-        Args:
-            full_table_name: the target table name.
-            schema: the JSON schema for the new table.
-
-        Returns:
-            An insert statement.
-        """
-        property_names = list(schema["properties"].keys())
-        statement = dedent(
-            f"""\
-            INSERT INTO {full_table_name}
-            ({", ".join(property_names)})
-            VALUES ({", ".join([f":{name}" for name in property_names])})
-            """,  # noqa: S608
-        )
-        return statement.rstrip()
-
     def bulk_insert_records(
         self,
         full_table_name: str,
         schema: dict,
-        records: Iterable[Dict[str, Any]],
-        is_temp_table: bool = False,
-    ) -> Optional[int]:
-        """Bulk insert records to an existing destination table.
-        The default implementation uses a generic SQLAlchemy bulk insert operation.
-        This method may optionally be overridden by developers in order to provide
-        faster, native bulk uploads.
-        Args:
-            full_table_name: the target table name.
-            schema: the JSON schema for the new table, to be used when inferring column
-                names.
-            records: the input records.
-            is_temp_table: whether the table is a temp table.
-        Returns:
-            True if table exists, False if not, None if unsure or undetectable.
-        """
-        insert_sql = self.generate_insert_statement(
-            full_table_name,
-            schema,
-        )
-        if isinstance(insert_sql, str):
-            insert_sql = sqlalchemy.text(insert_sql)
-
-        self.logger.info("Inserting with SQL: %s", insert_sql)
-
-        columns = self.column_representation(schema)
+        records,
+    ):
+        """Bulk insert records to an existing destination table."""
 
-        # temporary fix to ensure missing properties are added
-        insert_records = []
-        for record in records:
-            insert_record = {}
+        columns = list(self.flatten_schema.keys())
+        self.logger.info(f"Bulk inserting records into table {full_table_name} with columns {columns}.")
+        # Create the list of tuples for bulk insert
+        values = []
+        for record in records.values():
+            record_values = []
             for column in columns:
-                insert_record[column.name] = record.get(column.name)
-            insert_records.append(insert_record)
-
-        self.query(insert_sql, insert_records)
-
-        if isinstance(records, list):
-            return len(records)  # If list, we can quickly return record count.
-
-        return None  # Unknown record count.
-
-    def column_representation(
-        self,
-        schema: dict,
-    ) -> List[Column]:
-        """Returns a sql alchemy table representation for the current schema."""
-        columns: list[Column] = []
-        conformed_properties = schema["properties"]
-        for property_name, property_jsonschema in conformed_properties.items():
-            columns.append(
-                Column(
-                    property_name,
-                    self.to_sql_type(property_jsonschema),
-                )
-            )
-        return columns
+                value = record.get(column)
+                # Serialize dictionaries and lists to JSON strings
+                if isinstance(value, (dict, list)):
+                    value = json.dumps(value)
+                record_values.append(value)
+            values.append(tuple(record_values))
+        return values
 
     def _jsonschema_type_check(
         self, jsonschema_type: dict, type_check: tuple[str]
     ) -> bool:
         """Return True if the jsonschema_type supports the provided type.
         Args:
             jsonschema_type: The type dict.
@@ -445,204 +380,168 @@
     def to_sql_type(self, jsonschema_type: dict) -> sqlalchemy.types.TypeEngine:  # noqa
         """Convert JSON Schema type to a SQL type.
         Args:
             jsonschema_type: The JSON Schema object.
         Returns:
             The SQL type.
         """
+        maxlength = jsonschema_type.get("maxLength")
+        if not maxlength:
+            maxlength = 8000
         if self._jsonschema_type_check(jsonschema_type, ("string",)):
             datelike_type = self.get_datelike_property_type(jsonschema_type)
             if datelike_type:
                 if datelike_type == "date-time":
                     return cast(
                         sqlalchemy.types.TypeEngine, sqlalchemy.types.DATETIME()
                     )
                 if datelike_type in "time":
                     return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.TIME())
                 if datelike_type == "date":
                     return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.DATE())
 
-            maxlength = jsonschema_type.get("maxLength")
             if maxlength is not None:
                 if maxlength > 8000:
                     return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.TEXT())
 
             return cast(
                 sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR(maxlength)
             )
 
         if self._jsonschema_type_check(jsonschema_type, ("integer",)):
             return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.BIGINT())
 
         if self._jsonschema_type_check(jsonschema_type, ("number",)):
-            if self.config.get("prefer_float_over_numeric", False):
-                return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.FLOAT())
-            return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.NUMERIC(38, 16))
+            return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.FLOAT())
 
         if self._jsonschema_type_check(jsonschema_type, ("boolean",)):
-            return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR(1))
+            return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR(5))
 
         if self._jsonschema_type_check(jsonschema_type, ("object",)):
-            return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR())
+            return "VARCHAR(MAX)"
 
         if self._jsonschema_type_check(jsonschema_type, ("array",)):
-            return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.JSON())
+            return "VARCHAR(MAX)"
 
-        return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR())
+        return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR(maxlength))
 
     def column_clause(self, name, schema_property):
         return '{} {}'.format(safe_column_name(name), self.to_sql_type(schema_property))
 
-    def create_temp_table_from_table(self, from_table_name):
+    def create_temp_table_from_table(self, from_table_name, tmp_full_table_name):
         """Temp table from another table."""
-
-        db_name, schema_name, table_name = self.parse_full_table_name(from_table_name)
-        full_table_name = (
-            f"{schema_name}.{table_name}" if schema_name else f"{table_name}"
-        )
-        tmp_full_table_name = (
-            f"{schema_name}.#{table_name}" if schema_name else f"#{table_name}"
-        )
-
         droptable = f"DROP TABLE IF EXISTS {tmp_full_table_name}"
-        self.query(droptable)
 
         ddl = f"""
             SELECT TOP 0 *
             into {tmp_full_table_name}
-            FROM {full_table_name}
+            FROM {from_table_name}
         """  # nosec
-
-        self.query(ddl)
+        return droptable, ddl
 
     def process_batch(self, records) -> None:
         """Process a batch with the given batch context.
         Writes a batch to the SQL target. Developers may override this method
         in order to provide a more efficient upload/upsert process.
         Args:
             records: List of records to load into database.
         """
 
         key_properties = self.stream_schema_message['key_properties']
-        join_keys = list(key_properties)
+        join_keys = primary_column_names(self.stream_schema_message)
         schema = self.stream_schema_message['schema']
 
         stream_schema_message = self.stream_schema_message
         full_table_name = self.table_name(stream_schema_message['stream'], is_temporary=False)
-        if key_properties:
-            # Create a temp table (Creates from the table above)
-            db_name, schema_name, table_name = self.parse_full_table_name(
-                full_table_name
-            )
-            tmp_table_name = (
-                f"{schema_name}.#{table_name}" if schema_name else f"#{table_name}"
-            )
-            self.logger.info(f"Creating temp table {tmp_table_name}")
-            self.create_temp_table_from_table(
-                from_table_name=full_table_name
-            )
-
-            # Insert into temp table
-            self.bulk_insert_records(
-                full_table_name=tmp_table_name,
-                schema=schema,
-                records=records,
-                is_temp_table=True,
-            )
-            # Merge data from Temp table to main table
-            self.logger.info(f"Merging data from temp table to {full_table_name}")
-            self.merge_upsert_from_table(
-                from_table_name=tmp_table_name,
-                to_table_name=full_table_name,
-                schema=schema,
-                join_keys=join_keys,
-            )
+        tmp_table_name = self.table_name(stream_schema_message['stream'], is_temporary=True)
 
-        else:
-            self.bulk_insert_records(
-                full_table_name=full_table_name,
-                schema=schema,
-                records=records,
-            )
+        with self.open_connection() as connection:
+            with connection.cursor(as_dict=True) as cur:
+                if key_properties:
+                    # Create a temp table (Creates from the table above)
+                    self.logger.info(f"Creating temp table {tmp_table_name}")
+                    droptable, ddl = self.create_temp_table_from_table(
+                                            from_table_name=full_table_name,
+                                            tmp_full_table_name=tmp_table_name
+                                        )
+                    cur.execute(droptable)
+                    cur.execute(ddl)
+
+                    values = self.bulk_insert_records(
+                                                full_table_name=tmp_table_name,
+                                                schema=schema,
+                                                records=records,
+                                            )
+                    connection.bulk_copy(tmp_table_name, values)
+
+                    # Merge data from Temp table to main table
+                    self.logger.info(f"Bulk insert done. Merging data from temp table to {full_table_name}")
+                    merge_sql, droptable = self.merge_upsert_from_table(
+                                                from_table_name=tmp_table_name,
+                                                to_table_name=full_table_name,
+                                                schema=schema,
+                                                join_keys=join_keys,
+                                            )
+                    cur.execute(merge_sql)
+                    cur.execute(droptable)
+                    self.logger.info("Merge complete.")
+                else:
+                    values = self.bulk_insert_records(
+                                                full_table_name=full_table_name,
+                                                schema=schema,
+                                                records=records,
+                                            )
+                    connection.bulk_copy(full_table_name, values)
+                    self.logger.info("Bulk insert done.")
 
     def merge_upsert_from_table(
         self,
         from_table_name: str,
         to_table_name: str,
         schema: dict,
         join_keys: List[str],
-    ) -> Optional[int]:
+    ):
         """Merge upsert data from one table to another.
         Args:
             from_table_name: The source table name.
             to_table_name: The destination table name.
             join_keys: The merge upsert keys, or `None` to append.
             schema: Singer Schema message.
         Return:
             The number of records copied, if detectable, or `None` if the API does not
             report number of records affected/inserted.
         """
-        # TODO think about sql injeciton,
-        # issue here https://github.com/MeltanoLabs/target-postgres/issues/22
 
+        columns = self.column_names()
         join_condition = " and ".join(
             [f"temp.{key} = target.{key}" for key in join_keys]
         )
 
         update_stmt = ", ".join(
             [
                 f"target.{key} = temp.{key}"
-                for key in schema["properties"].keys()
+                for key in columns
                 if key not in join_keys
             ]
         )  # noqa
 
         merge_sql = f"""
             MERGE INTO {to_table_name} AS target
             USING {from_table_name} AS temp
             ON {join_condition}
             WHEN MATCHED THEN
                 UPDATE SET
                     { update_stmt }
             WHEN NOT MATCHED THEN
-                INSERT ({", ".join(schema["properties"].keys())})
-                VALUES ({", ".join([f"temp.{key}" for key in schema["properties"].keys()])});
+                INSERT ({", ".join(columns)})
+                VALUES ({", ".join([f"temp.{key}" for key in columns])});
         """  # nosec
 
-        self.query(merge_sql)
-
-    def parse_full_table_name(
-        self, full_table_name: str
-    ):
-        """Parse a fully qualified table name into its parts.
-        Developers may override this method if their platform does not support the
-        traditional 3-part convention: `db_name.schema_name.table_name`
-        Args:
-            full_table_name: A table name or a fully qualified table name. Depending on
-                SQL the platform, this could take the following forms:
-                - `<db>.<schema>.<table>` (three part names)
-                - `<db>.<table>` (platforms which do not use schema groupings)
-                - `<schema>.<name>` (if DB name is already in context)
-                - `<table>` (if DB name and schema name are already in context)
-        Returns:
-            A three part tuple (db_name, schema_name, table_name) with any unspecified
-            or unused parts returned as None.
-        """
-        db_name = None
-        schema_name = None
-
-        parts = full_table_name.split(".")
-        if len(parts) == 1:
-            table_name = full_table_name
-        if len(parts) == 2:
-            schema_name, table_name = parts
-        if len(parts) == 3:
-            db_name, schema_name, table_name = parts
-
-        return db_name, schema_name, table_name
+        droptable = f"DROP TABLE IF EXISTS {from_table_name}"
+        return merge_sql, droptable
 
     def column_names(self):
         return [safe_column_name(name) for name in self.flatten_schema]
 
     def create_table_query(self, table_name=None, is_temporary=False):
         stream_schema_message = self.stream_schema_message
         columns = [
@@ -695,67 +594,67 @@
                 FROM sys.indexes
                 WHERE object_id = OBJECT_ID('{table}')
                     AND name = '{index_name}'
             )
             BEGIN
                 CREATE INDEX {index_name} ON {table} ({column});
             END"""
-        self.logger.info("Creating index on '%s' table on '%s' column(s)... %s", table, column, query)
+        self.logger.info("Creating index on '%s' table on '%s' column(s)", table, column)
         try:
-            self.query(query, require_database=False)
+            self.query(query)
         except Exception as e:
             self.logger.warn(f"Failed to create index, error: {e}")
 
     def create_indices(self, stream):
         if isinstance(self.indices, list):
             for index in self.indices:
                 self.create_index(stream, index)
 
     def delete_rows(self, stream):
         table = self.table_name(stream)
         query = "DELETE FROM {} WHERE _sdc_deleted_at IS NOT NULL".format(table)
         self.logger.info("Deleting rows from '%s' table... %s", table, query)
-        self.query(query)
+        with self.open_connection() as connection:
+            with connection.cursor(as_dict=True) as cur:
+                cur.execute(query)
         self.logger.info("Delete query completed.")
 
     def create_schema_if_not_exists(self, table_columns_cache=None):
         schema_name = self.schema_name
         schema_rows = 0
 
         # table_columns_cache is an optional pre-collected list of available objects in mssql
         if table_columns_cache:
             schema_rows = list(filter(lambda x: x['TABLE_SCHEMA'] == schema_name, table_columns_cache))
         # Query realtime if not pre-collected
         else:
-            self.logger.info("reached here..")
             schema_rows = self.query(
                 f"SELECT LOWER(schema_name) schema_name FROM information_schema.schemata WHERE LOWER(schema_name) = '{schema_name.lower()}'",
-                require_database=False
+                ignore_rowcount=True
             )
-            self.logger.info(f"schema rows: {schema_rows}")
 
         if len(schema_rows) == 0:
             query = "CREATE SCHEMA {}".format(schema_name)
             self.logger.info("Schema '%s' does not exist. Creating... %s", schema_name, query)
             self.query(query)
 
             self.grant_privilege(schema_name, self.grantees, self.grant_usage_on_schema)
 
     def get_tables(self):
         return self.query(
             f"SELECT table_name FROM information_schema.tables WHERE table_schema = '{self.schema_name}'",
-            require_database=False
+            ignore_rowcount=True
         )
 
     def get_table_columns(self, table_name):
         return self.query("""SELECT column_name, data_type
       FROM information_schema.columns
       WHERE lower(table_name) = %s AND lower(table_schema) = %s""", params=(table_name.replace("\"", "").lower(),
                                                                      self.schema_name.lower()),
-                                                                     require_database=False)
+                                                                     ignore_rowcount=True)
 
     def update_columns(self):
         stream_schema_message = self.stream_schema_message
         stream = stream_schema_message['stream']
         table_name = self.table_name(stream, without_schema=True)
         columns = self.get_table_columns(table_name)
         columns_dict = {column['column_name'].lower(): column for column in columns}
@@ -775,15 +674,15 @@
         columns_to_replace = [
             (safe_column_name(name), self.column_clause(
                 name,
                 properties_schema
             ))
             for (name, properties_schema) in self.flatten_schema.items()
             if name.lower() in columns_dict and
-            columns_dict[name.lower()]['data_type'].lower() != self.to_sql_type(properties_schema).lower()
+            columns_dict[name.lower()]['data_type'].lower() not in str(self.to_sql_type(properties_schema)).lower()
         ]
 
         for (column_name, column) in columns_to_replace:
             self.version_column(column_name, stream)
             self.add_column(column, stream)
 
     def drop_column(self, column_name, stream):
```

### Comparing `macrometa-target-mssql-0.0.9/pyproject.toml` & `macrometa-target-mssql-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mssql"
-version='0.0.9'
+version='1.0.0'
 description = "Macrometa target connector for writing data into Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -24,19 +24,20 @@
 packages = [
     { include = "macrometa_target_mssql" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = ">=0.0.20"
+c8connector = ">=0.0.29"
 pymssql = ">=2.2.5"
 inflection = "0.3.1"
 joblib = "1.2.0"
 sqlalchemy = "^1.4"
+prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-target-mssql = 'macrometa_target_mssql:main'
 
 [tool.poetry.urls]
 "Homepage" = "https://www.macrometa.com/"
```

### Comparing `macrometa-target-mssql-0.0.9/setup.py` & `macrometa-target-mssql-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 packages = \
 ['macrometa_target_mssql']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector>=0.0.20',
+['c8connector>=0.0.29',
  'inflection==0.3.1',
  'joblib==1.2.0',
  'pipelinewise-singer-python==1.2.0',
+ 'prometheus-client==0.16.0',
  'pymssql>=2.2.5',
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mssql = macrometa_target_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mssql',
-    'version': '0.0.9',
+    'version': '1.0.0',
     'description': 'Macrometa target connector for writing data into Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mssql-0.0.9/PKG-INFO` & `macrometa-target-mssql-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mssql
-Version: 0.0.9
+Version: 1.0.0
 Summary: Macrometa target connector for writing data into Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MicrosoftSQLServer
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
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
+Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: pymssql (>=2.2.5)
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-target-mssql/issues
 Project-URL: Homepage, https://www.macrometa.com/
```

