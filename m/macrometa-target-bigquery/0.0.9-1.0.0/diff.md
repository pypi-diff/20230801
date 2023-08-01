# Comparing `tmp/macrometa-target-bigquery-0.0.9.tar.gz` & `tmp/macrometa-target-bigquery-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-bigquery-0.0.9.tar", last modified: Wed May 31 06:19:00 2023, max compression
+gzip compressed data, was "macrometa-target-bigquery-1.0.0.tar", last modified: Tue Aug  1 08:48:45 2023, max compression
```

## Comparing `macrometa-target-bigquery-0.0.9.tar` & `macrometa-target-bigquery-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)    26318 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24991 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/db_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/flattening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/stream_ref_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:48:45.850306 macrometa-target-bigquery-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-08-01 08:48:45.850306 macrometa-target-bigquery-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:48:45.846306 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    29743 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25555 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/db_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/flattening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/stream_ref_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:48:45.850306 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-08-01 08:48:45.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-01 08:48:45.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:48:45.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-01 08:48:45.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-01 08:48:45.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 08:48:45.000000 macrometa-target-bigquery-1.0.0/macrometa_target_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:48:45.850306 macrometa-target-bigquery-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-01 08:48:31.000000 macrometa-target-bigquery-1.0.0/setup.py
```

### Comparing `macrometa-target-bigquery-0.0.9/LICENSE` & `macrometa-target-bigquery-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.9/PKG-INFO` & `macrometa-target-bigquery-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.9
+Version: 1.0.0
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.9/README.md` & `macrometa-target-bigquery-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/__init__.py` & `macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
-from datetime import datetime, timedelta
+from datetime import datetime
 import copy
-import io
 import json
 import logging
 import os
 import sys
 import uuid
 from multiprocessing.pool import ThreadPool as Pool
 
 import pkg_resources
-from asyncio import AbstractEventLoop
 from c8connector import C8Connector, Sample, ConfigAttributeType, Schema
-from c8connector import ConfigProperty
+from c8connector import ConfigProperty, ensure_datetime
+from datetime import datetime, timezone
 from tempfile import mkstemp
 from fastavro import writer, parse_schema
 from jsonschema import Draft7Validator, FormatChecker
 from pathlib import Path
+from prometheus_client import CollectorRegistry, Counter, Gauge, start_http_server
 from singer import get_logger
-from threading import Thread
-from typing import Dict
+from threading import Lock
+from typing import AsyncIterable, Dict
 
 from macrometa_target_bigquery import stream_utils
 from macrometa_target_bigquery.db_sync import DbSync
 from macrometa_target_bigquery.exceptions import (
     RecordValidationException,
     InvalidValidationOperationException
 )
@@ -36,14 +36,26 @@
 
 DEFAULT_BATCH_SIZE_ROWS = 10000
 DEFAULT_PARALLELISM = 0  # 0 The number of threads used to flush tables
 DEFAULT_MAX_PARALLELISM = 16  # Don't use more than this number of threads by default when flushing streams in parallel
 DEFAULT_HARD_DELETE = False
 DEFAULT_BATCH_AWAIT_TIME = 60
 
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
 
 class BigQueryTargetConnector(C8Connector):
     """BigQueryTargetConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
         return "BigQuery"
@@ -100,14 +112,19 @@
             ConfigProperty('target_schema', 'Target Schema/Dataset', ConfigAttributeType.STRING, True, True,
                            description='Name of the schema/dataset where the tables will be created. '
                                        'The schema will be created if it does not exist (Case-sensitive).',
                            placeholder_value='my_schema'),
             ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, True,
                            description='Name of the bigquery table. The table will be created if it does not exist (Case-sensitive).',
                            placeholder_value='my_table'),
+            ConfigProperty('location', 'Location', ConfigAttributeType.STRING, False, True,
+                           description='If the dataset does not exist, the region where BigQuery creates it will be determined by'
+                                       ' the provided location (default: US). However, if the dataset already exists, the location of the dataset'
+                                       ' will be used eventually.',
+                           placeholder_value='US'),
             ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
                            description='Maximum number of rows in each batch. At the end of each batch, '
                                        'the rows in the batch are loaded into BigQuery.',
                            default_value='10000'),
             ConfigProperty('batch_wait_limit_seconds', 'Batch Wait Limit (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Maximum time to wait for batch to reach batch size rows.',
@@ -121,24 +138,14 @@
             ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, False, False,
                            description='When hard_delete option is true then DELETE SQL commands will be performed in'
                                        ' BigQuery to delete rows in tables. It\'s achieved by continuously checking the'
                                        ' _sdc_deleted_at metadata column sent by the data source. As deleting rows '
                                        'requires metadata columns, hard_delete option automatically enables the '
                                        'add metadata columns option as well.',
                            default_value='false'),
-            ConfigProperty('data_flattening_max_level', 'Data Flattening Max Level',
-                           ConfigAttributeType.INT, False, False,
-                           description='Object type RECORD items from data source can be loaded into VARIANT columns as JSON '
-                                       '(default) or we can flatten the schema by creating columns automatically.'
-                                       ' When value is 0 (default) then flattening functionality is turned off.',
-                           default_value='0'),
-            ConfigProperty('temp_schema', 'Temporary Schema', ConfigAttributeType.STRING, False, False,
-                           description='Name of the schema where the temporary tables will be created. Will default to '
-                                       'the same schema as the target table.',
-                           placeholder_value='my_temp_schema'),
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
         return []
@@ -165,37 +172,34 @@
     if state is not None:
         line = json.dumps(state)
         LOGGER.info('Emitting state {}'.format(line))
         sys.stdout.write("{}\n".format(line))
         sys.stdout.flush()
 
 
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
 # pylint: disable=too-many-locals,too-many-branches,too-many-statements
-def persist_lines(config, lines) -> None:
-    state = None
-    flushed_state = None
-    schemas = {}
-    key_properties = {}
-    validators = {}
-    records_to_load = {}
-    row_count = {}
-    stream_to_sync = {}
-    total_row_count = {}
-    batch_size_rows = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
-    default_hard_delete = config.get('hard_delete', DEFAULT_HARD_DELETE)
-    hard_delete_mapping = config.get('hard_delete_mapping', {})
-    time_schedule = {
-        'batch_wait_limit_seconds': config.get('batch_wait_limit_seconds', DEFAULT_BATCH_AWAIT_TIME),
-        'last_executed_time': datetime.now(),
-    }
-    event_loop = setup_flush_task(time_schedule, records_to_load, row_count, stream_to_sync, config,
-                                  state, flushed_state)
+async def persist_lines(state, flushed_state, schemas, key_properties, validators, records_to_load, row_count,
+                        stream_to_sync, total_row_count, batch_size_rows, default_hard_delete, hard_delete_mapping,
+                        time_schedule, config, flush_lock, time_extracted_list) -> None:
 
     # Loop over lines from stdin
-    for line in lines:
+    lines = read_stdin()
+    async for line in lines:
         try:
             o = json.loads(line)
         except json.decoder.JSONDecodeError:
             LOGGER.error("Unable to parse:\n{}".format(line))
             raise
 
         if 'type' not in o:
@@ -223,151 +227,163 @@
                     if type(ex).__name__ == "InvalidOperation":
                         raise InvalidValidationOperationException(
                             f"Data validation failed and cannot load to destination. RECORD: {o['record']}\n"
                             "multipleOf validations that allows long precisions are not supported (i.e. with 15 digits"
                             "or more) Try removing 'multipleOf' methods from JSON schema.")
                     raise RecordValidationException(f"Record does not pass schema validation. RECORD: {o['record']}")
 
-            primary_key_string = stream_to_sync[stream].record_primary_key_string(o['record'])
-            if not primary_key_string:
-                primary_key_string = 'RID-{}'.format(total_row_count[stream])
-
-            # increment row count only when a new PK is encountered in the current batch
-            if primary_key_string not in records_to_load[stream]:
-                row_count[stream] += 1
-                total_row_count[stream] += 1
-
-            # append record
-            if config.get('add_metadata_columns') or hard_delete_mapping.get(stream, default_hard_delete):
-                records_to_load[stream][primary_key_string] = stream_utils.add_metadata_values_to_record(o)
-            else:
-                records_to_load[stream][primary_key_string] = o['record']
-
-            if row_count[stream] >= batch_size_rows:
-                LOGGER.info("Flush triggered by batch_size_rows (%s) reached in %s",
-                             batch_size_rows, stream)
-
-                # flush all streams, delete records if needed, reset counts and then emit current state
-                if config.get('flush_all_streams'):
-                    filter_streams = None
+            with flush_lock:
+                primary_key_string = stream_to_sync[stream].record_primary_key_string(o['record'])
+                if not primary_key_string:
+                    primary_key_string = 'RID-{}'.format(total_row_count[stream])
+
+                # increment row count only when a new PK is encountered in the current batch
+                if primary_key_string not in records_to_load[stream]:
+                    row_count[stream] += 1
+                    total_row_count[stream] += 1
+
+                # append record
+                if config.get('add_metadata_columns') or hard_delete_mapping.get(stream, default_hard_delete):
+                    records_to_load[stream][primary_key_string] = stream_utils.add_metadata_values_to_record(o)
                 else:
-                    filter_streams = [stream]
+                    records_to_load[stream][primary_key_string] = o['record']
 
-                # Flush and return a new state dict with new positions only for the flushed streams
-                flushed_state = flush_streams(
-                    records_to_load,
-                    row_count,
-                    stream_to_sync,
-                    config,
-                    state,
-                    flushed_state,
-                    filter_streams=filter_streams)
+                if 'time_extracted' in o:
+                    time_extracted_list.append(ensure_datetime(o["time_extracted"]))
+                else:
+                    time_extracted_list.append(datetime.now(timezone.utc))
 
-                # emit last encountered state
-                emit_state(copy.deepcopy(flushed_state))
-                time_schedule['last_executed_time'] = datetime.now()
+                if row_count[stream] >= batch_size_rows and row_count[stream] > 0:
+                    LOGGER.info("Flush triggered by batch_size_rows (%s) reached in %s",
+                                 batch_size_rows, stream)
+
+                    # flush all streams, delete records if needed, reset counts and then emit current state
+                    if config.get('flush_all_streams'):
+                        filter_streams = None
+                    else:
+                        filter_streams = [stream]
+
+                    # Flush and return a new state dict with new positions only for the flushed streams
+                    flushed_state = flush_streams(
+                        records_to_load,
+                        row_count,
+                        stream_to_sync,
+                        config,
+                        state,
+                        flushed_state,
+                        time_extracted_list,
+                        filter_streams=filter_streams)
+
+                    # emit last encountered state
+                    emit_state(copy.deepcopy(flushed_state))
+                    time_schedule['last_executed_time'] = datetime.now()
 
         elif t == 'SCHEMA':
             if 'stream' not in o:
                 raise Exception("Line is missing required key 'stream': {}".format(line))
 
             stream = o['stream']
 
             schemas[stream] = stream_utils.float_to_decimal(o['schema'])
             validators[stream] = Draft7Validator(schemas[stream], format_checker=FormatChecker())
 
-            # flush records from previous stream SCHEMA
-            # if same stream has been encountered again, it means the schema might have been altered
-            # so previous records need to be flushed
-            if row_count.get(stream, 0) > 0:
-                if config.get('flush_all_streams'):
-                    filter_streams = None
-                else:
-                    filter_streams = [stream]
+            with flush_lock:
+                # flush records from previous stream SCHEMA
+                # if same stream has been encountered again, it means the schema might have been altered
+                # so previous records need to be flushed
+                if row_count.get(stream, 0) > 0:
+                    if config.get('flush_all_streams'):
+                        filter_streams = None
+                    else:
+                        filter_streams = [stream]
 
-                flushed_state = flush_streams(
-                    records_to_load, row_count, stream_to_sync, config, state, flushed_state, filter_streams=filter_streams
-                )
+                    flushed_state = flush_streams(
+                        records_to_load, row_count, stream_to_sync, config, state, flushed_state, time_extracted_list, filter_streams=filter_streams
+                    )
+
+                    # emit latest encountered state
+                    emit_state(flushed_state)
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
+                #  1) Set ` 'primary_key_required': false ` in the target-bigquery config.json
+                #  or
+                #  2) Use fastsync [postgres-to-bigquery, mysql-to-bigquery, etc.]
+                if config.get('primary_key_required', True) and len(o['key_properties']) == 0:
+                    LOGGER.critical("Primary key is set to mandatory but not defined in the [{}] stream".format(stream))
+                    raise Exception("key_properties field is required")
+
+                key_properties[stream] = o['key_properties']
 
-                # emit latest encountered state
-                emit_state(flushed_state)
+                if config.get('add_metadata_columns') or hard_delete_mapping.get(stream, default_hard_delete):
+                    stream_to_sync[stream] = DbSync(config, add_metadata_columns_to_schema(o))
+                else:
+                    stream_to_sync[stream] = DbSync(config, o)
 
-            # key_properties key must be available in the SCHEMA message.
-            if 'key_properties' not in o:
-                raise Exception("key_properties field is required")
-
-            # Log based and Incremental replications on tables with no Primary Key
-            # cause duplicates when merging UPDATE events.
-            # Stop loading data by default if no Primary Key.
-            #
-            # If you want to load tables with no Primary Key:
-            #  1) Set ` 'primary_key_required': false ` in the target-bigquery config.json
-            #  or
-            #  2) Use fastsync [postgres-to-bigquery, mysql-to-bigquery, etc.]
-            if config.get('primary_key_required', True) and len(o['key_properties']) == 0:
-                LOGGER.critical("Primary key is set to mandatory but not defined in the [{}] stream".format(stream))
-                raise Exception("key_properties field is required")
-
-            key_properties[stream] = o['key_properties']
-
-            if config.get('add_metadata_columns') or hard_delete_mapping.get(stream, default_hard_delete):
-                stream_to_sync[stream] = DbSync(config, add_metadata_columns_to_schema(o))
-            else:
-                stream_to_sync[stream] = DbSync(config, o)
-
-            try:
-                stream_to_sync[stream].create_schema_if_not_exists()
-                stream_to_sync[stream].sync_table()
-            except Exception as e:
-                LOGGER.error("""
-                    Cannot sync table structure in BigQuery schema: {} .
-                """.format(
-                    stream_to_sync[stream].schema_name))
-                raise e
-
-            records_to_load[stream] = {}
-            row_count[stream] = 0
-            total_row_count[stream] = 0
+                try:
+                    stream_to_sync[stream].create_schema_if_not_exists()
+                    stream_to_sync[stream].sync_table()
+                except Exception as e:
+                    LOGGER.error("""
+                        Cannot sync table structure in BigQuery schema: {} .
+                    """.format(
+                        stream_to_sync[stream].schema_name))
+                    raise e
+
+                records_to_load[stream] = {}
+                row_count[stream] = 0
+                total_row_count[stream] = 0
 
         elif t == 'ACTIVATE_VERSION':
-            stream = o['stream']
-            LOGGER.debug('ACTIVATE_VERSION message - ignoring')
+            with flush_lock:
+                stream = o['stream']
+                LOGGER.debug('ACTIVATE_VERSION message - ignoring')
 
         elif t == 'STATE':
-            LOGGER.debug('Setting state to {}'.format(o['value']))
-            state = o['value']
-
-            # Initially set flushed state
-            if not flushed_state:
-                flushed_state = copy.deepcopy(state)
+            with flush_lock:
+                LOGGER.debug('Setting state to {}'.format(o['value']))
+                state = o['value']
+
+                # Initially set flushed state
+                if not flushed_state:
+                    flushed_state = copy.deepcopy(state)
 
         else:
             raise Exception("Unknown message type {} in message {}"
                             .format(o['type'], o))
 
     # if some bucket has records that need to be flushed but haven't reached batch size
     # then flush all buckets.
     if sum(row_count.values()) > 0:
-        # flush all streams one last time, delete records if needed, reset counts and then emit current state
-        flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state, flushed_state)
-        time_schedule['last_executed_time'] = datetime.now()
-
-    # emit latest state
-    emit_state(copy.deepcopy(flushed_state))
-    event_loop.stop()
+        with flush_lock:
+            # flush all streams one last time, delete records if needed, reset counts and then emit current state
+            flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state, flushed_state, time_extracted_list)
+            time_schedule['last_executed_time'] = datetime.now()
+
+    with flush_lock:
+        # emit latest state
+        emit_state(copy.deepcopy(flushed_state))
 
 
 # pylint: disable=too-many-arguments
 def flush_streams(
         streams,
         row_count,
         stream_to_sync,
         config,
         state,
         flushed_state,
+        time_extracted_list,
         filter_streams=None):
     """
     Flushes all buckets and resets records count to 0 as well as empties records to load list
     :param streams: dictionary with records to load per stream
     :param row_count: dictionary with row count per stream
     :param stream_to_sync: BigQuery db sync instance per stream
     :param config: dictionary containing the configuration
@@ -409,14 +425,15 @@
                     pool.apply_async(
                         load_stream_batch,
                         kwds={
                             'stream': stream,
                             'records_to_load': streams[stream],
                             'row_count': row_count,
                             'db_sync': stream_to_sync[stream],
+                            'time_extracted_list': time_extracted_list,
                             'delete_rows': hard_delete_mapping.get(
                                 stream, default_hard_delete
                             ),
                         },
                     )
                 )
             for future in jobs:
@@ -425,22 +442,24 @@
         # If we only have one stream to sync let's not introduce overhead.
         # for stream in streams_to_flush:
         load_stream_batch(
             stream=streams_to_flush[0],
             records_to_load=streams[streams_to_flush[0]],
             row_count=row_count,
             db_sync=stream_to_sync[streams_to_flush[0]],
+            time_extracted_list=time_extracted_list,
             delete_rows=hard_delete_mapping.get(streams_to_flush[0], default_hard_delete)
         )
 
     # reset flushed stream records to empty to avoid flushing same records
     # reset row count for flushed streams
     for stream in streams_to_flush:
         streams[stream] = {}
         row_count[stream] = 0
+        time_extracted_list = []
 
         # Update flushed streams
         if filter_streams:
             # update flushed_state position if we have state information for the stream
             if state is not None and stream in state.get('bookmarks', {}):
                 # Create bookmark key if not exists
                 if 'bookmarks' not in flushed_state:
@@ -452,71 +471,97 @@
         else:
             flushed_state = copy.deepcopy(state)
 
     # Return with state message with flushed positions
     return flushed_state
 
 
-def load_stream_batch(stream, records_to_load, row_count, db_sync, delete_rows=False):
+def load_stream_batch(stream, records_to_load, row_count, db_sync, time_extracted_list, delete_rows=False):
     # Load into bigquery
     if row_count[stream] > 0:
-        flush_records(stream, records_to_load, row_count[stream], db_sync)
+        flush_records(stream, records_to_load, row_count[stream], db_sync, time_extracted_list)
 
         # Delete soft-deleted, flagged rows - where _sdc_deleted at is not null
         if delete_rows:
             db_sync.delete_rows(stream)
 
 
-def flush_records(stream, records_to_load, row_count, db_sync):
+def flush_records(stream, records_to_load, row_count, db_sync, time_extracted_list):
     parsed_schema = parse_schema(db_sync.avro_schema())
     csv_fd, csv_file = mkstemp()
     with open(csv_file, 'wb') as out:
         writer(out, parsed_schema, db_sync.records_to_avro(records_to_load.values()))
 
     # Seek to the beginning of the file and load
     with open(csv_file, 'r+b') as f:
         db_sync.load_avro(f, row_count)
 
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
-    asyncio.run_coroutine_threadsafe(
-        flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state, filter_streams),
-        event_loop)
-    return event_loop
+async def setup_flush_task(config, filter_streams=None):
+    state = None
+    flushed_state = None
+    schemas = {}
+    key_properties = {}
+    validators = {}
+    records_to_load = {}
+    row_count = {}
+    stream_to_sync = {}
+    total_row_count = {}
+    time_extracted_list = []
+    batch_size_rows = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
+    default_hard_delete = config.get('hard_delete', DEFAULT_HARD_DELETE)
+    hard_delete_mapping = config.get('hard_delete_mapping', {})
+    time_schedule = {
+        'batch_wait_limit_seconds': config.get('batch_wait_limit_seconds', DEFAULT_BATCH_AWAIT_TIME),
+        'last_executed_time': datetime.now(),
+    }
+    flush_lock = Lock()
+    event_loop = asyncio.get_event_loop()
+    persist_lines_coro = persist_lines(state, flushed_state, schemas, key_properties, validators, records_to_load, row_count,
+                        stream_to_sync, total_row_count, batch_size_rows, default_hard_delete, hard_delete_mapping,
+                        time_schedule, config, flush_lock, time_extracted_list)
+    asyncio.run_coroutine_threadsafe(persist_lines_coro, event_loop)
+    flush_task_coro = flush_task(time_schedule, records_to_load, row_count, stream_to_sync, config, state, flushed_state,
+                                 flush_lock, time_extracted_list, filter_streams)
+    asyncio.run_coroutine_threadsafe(flush_task_coro, event_loop)
+
+    # Wait for all Futures to complete and propagate any exceptions raised
+    await asyncio.gather(
+        persist_lines_coro,
+        flush_task_coro,
+    )
 
 
 async def flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state,
-                     filter_streams=None) -> None:
+                     flush_lock, time_extracted_list, filter_streams=None) -> None:
     while True:
         timedelta = datetime.now() - time_schedule['last_executed_time']
         if (
             timedelta.total_seconds() >= time_schedule['batch_wait_limit_seconds']
             and sum(row_count.values()) > 0
         ):
-            # flush all streams one last time, delete records if needed, reset counts and then emit current state.
-            flushed_state = flush_streams(streams, row_count, stream_to_sync, config, state, flushed_state,
-                                          filter_streams)
-            # emit latest state
-            emit_state(copy.deepcopy(flushed_state))
-            time_schedule['last_executed_time'] = datetime.now()
+            with flush_lock:
+                # flush all streams one last time, delete records if needed, reset counts and then emit current state.
+                flushed_state = flush_streams(streams, row_count, stream_to_sync, config, state, flushed_state,
+                                              time_extracted_list, filter_streams)
+                # emit latest state
+                emit_state(copy.deepcopy(flushed_state))
+                time_schedule['last_executed_time'] = datetime.now()
         # Add sleep statement to ensure periodic execution
         await asyncio.sleep(time_schedule['batch_wait_limit_seconds'])
 
 
-def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
-    asyncio.set_event_loop(loop)
-    loop.run_forever()
-
-
 def create_credentials_file(config: Dict) -> Dict:
     path_uuid = uuid.uuid4().hex
     try:
         if config.get('credentials_file'):
             path = f"/opt/bigquery/{path_uuid}/client_secrets.json"
             client_secrets = Path(path)
             client_secrets.parent.mkdir(exist_ok=True, parents=True)
@@ -538,29 +583,42 @@
             LOGGER.info(f"Client credentials file deleted from: {path}")
             client_secrets.parent.rmdir()
     except Exception as e:
         LOGGER.warn(f"Failed to delete client credentials file: {e}")
 
 
 def validate_config(config):
+    def validate_integer(value, error_message, key=None):
+        try:
+            if int(value) < 0 or (key == 'batch_size_rows' and int(value) == 0):
+                raise ValueError
+        except Exception:
+            raise Exception(error_message)
+
     batch_size_rows = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
-    if not batch_size_rows.isdecimal() or int(batch_size_rows) <= 0:
-        raise Exception('The batch size provided is not valid. Only integer values greater'
-                        ' than 0 are supported as batch size.')
+    validate_integer(batch_size_rows, 'The batch size provided is not valid. '
+                                       'Only integer values greater than 0 '
+                                       'are supported as batch size.',
+                                       key='batch_size_rows')
+
     batch_wait_limit = config.get('batch_wait_limit_seconds', DEFAULT_BATCH_AWAIT_TIME)
-    if not batch_wait_limit.isdecimal() or int(batch_wait_limit) < 0:
-        raise Exception('The batch wait limit provided is not valid. Only integer values '
-                        'greater than or equal to 0 are supported as batch wait limit.')
+    validate_integer(batch_wait_limit, 'The batch wait limit provided is not valid. '
+                                        'Only integer values greater than or equal to 0 '
+                                        'are supported as batch wait limit.')
+
     data_flattening_max_level = config.get('data_flattening_max_level', 0)
-    if not data_flattening_max_level.isdecimal() or int(data_flattening_max_level) < 0:
-        raise Exception('The data flattening max level provided is not valid. Only integer values '
-                        'greater than or equal to 0 are supported as data flattening max level.')
-    
+    validate_integer(data_flattening_max_level, 'The data flattening max level provided is not valid. '
+                                                 'Only integer values greater than or equal to 0 '
+                                                 'are supported as data flattening max level.')
 
-def main():
+
+async def main_impl():
+    # Start the Prometheus HTTP server for exposing metrics
+    LOGGER.info("Bigquery target is starting the metrics server.")
+    start_http_server(8001, registry=registry_package)
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--config', help='Config file')
     args = parser.parse_args()
 
     if args.config:
         with open(args.config) as config_input:
             config = json.load(config_input)
@@ -568,20 +626,30 @@
         config = {}
 
     try:
         # Field validations
         validate_config(config)
         config = create_credentials_file(config)
         # Consume singer messages
-        singer_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
-        persist_lines(config, singer_messages)
+        await setup_flush_task(config)
 
         LOGGER.debug("Exiting normally")
     except Exception as e:
         LOGGER.info("Exception raised: %s", e)
+        # Increment export_errors metric
+        export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         delete_credentials_file(config)
         raise e
     delete_credentials_file(config)
 
 
+def main():
+    """Main entry point"""
+    try:
+        asyncio.run(main_impl())
+    except Exception as exc:
+        LOGGER.critical(exc)
+        raise exc
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/db_sync.py` & `macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/db_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,21 +196,24 @@
         self.stream_schema_message = stream_schema_message
 
         # Validate connection configuration
         config_errors = validate_config(connection_config)
 
         # Exit if config has errors
         if len(config_errors) > 0:
-            logger.error("Invalid configuration:\n   * {}".format('\n   * '.join(config_errors)))
-            sys.exit(1)
+            error_msg = "Invalid configuration:\n   * {}".format('\n   * '.join(config_errors))
+            logger.error(error_msg)
+            raise Exception(error_msg)
 
-        project_id = self.connection_config['project_id']
+        self.project_id = self.connection_config['project_id']
         location = self.connection_config.get('location', None)
-        credentials = service_account.Credentials.from_service_account_file(self.connection_config['credentials_file'])
-        self.client = bigquery.Client(project=project_id, credentials=credentials, location=location)
+        if location:
+            location = str(location).strip()
+        self.credentials = service_account.Credentials.from_service_account_file(self.connection_config['credentials_file'])
+        self.client = bigquery.Client(project=self.project_id, credentials=self.credentials, location=location)
 
         self.schema_name = None
         self.grantees = None
 
         # Init stream schema
         if self.stream_schema_message is not None:
             #  Define target schema name.
@@ -370,15 +373,19 @@
                                                    pk_columns_names)
         else:
             query = sql_utils.insert_from_table_sql(temp_table,
                                                     target_table,
                                                     self.column_names())
         drop_temp_query = sql_utils.drop_table_sql(temp_table)
         results = self.query([query, drop_temp_query])
-        logger.info('LOADED {} rows'.format(results.num_dml_affected_rows))
+        loaded_rows = 0
+        for child_job in self.client.list_jobs(parent_job=results.job_id):
+            if child_job.num_dml_affected_rows is not None:
+                loaded_rows += child_job.num_dml_affected_rows
+        logger.info('LOADED {} rows'.format(loaded_rows))
 
     def column_names(self):
         return [sql_utils.safe_column_name(name) for name in self.flatten_schema]
 
     def create_table(self, is_temporary=False):
         stream_schema_message = self.stream_schema_message
         stream = stream_schema_message['stream']
@@ -436,14 +443,16 @@
         for schema in set([schema_name, temp_schema]):
             try:
                 self.client.create_dataset(bigquery.DatasetReference(project_id, schema))
                 logger.info("Schema '{}' does not exist. Creating...".format(schema))
                 self.grant_privilege(schema, self.grantees, self.grant_usage_on_schema)
             except Conflict:
                 # Already exists.
+                dataset = self.client.get_dataset(bigquery.DatasetReference(project_id, schema))
+                self.client = bigquery.Client(project=self.project_id, credentials=self.credentials, location=dataset.location)
                 pass
 
     # pylint: disable=no-self-use
     def alias_field(self, field, alias):
         api_repr = field.to_api_repr()
         api_repr['name'] = alias
         return SchemaField.from_api_repr(api_repr)
```

### Comparing `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/exceptions.py` & `macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/flattening.py` & `macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/flattening.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/sql_utils.py` & `macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/sql_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/stream_ref_helper.py` & `macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/stream_ref_helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/stream_utils.py` & `macrometa-target-bigquery-1.0.0/macrometa_target_bigquery/stream_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/PKG-INFO` & `macrometa-target-bigquery-1.0.0/macrometa_target_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.9
+Version: 1.0.0
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/SOURCES.txt` & `macrometa-target-bigquery-1.0.0/macrometa_target_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.9/setup.py` & `macrometa-target-bigquery-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name="macrometa-target-bigquery",
-      version='0.0.9',
+      version='1.0.0',
       description="Macrometa target bigquery connector for loading data to BigQuery",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-target-bigquery',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
           'Programming Language :: Python :: 3 :: Only'
       ],
       py_modules=["macrometa_target_bigquery"],
       install_requires=[
           'pipelinewise-singer-python==1.2.0',
           'google-cloud-bigquery>=2.20.0,<3.1.0',
           'fastavro>=0.22.8,<1.4.11',
-          'c8connector>=0.0.20'
+          'c8connector>=0.0.29',
+          'prometheus-client==0.16.0'
       ],
       extras_require={
           "test": [
               'pytest==7.0.1',
               'pylint==2.13.4',
               'pytest-cov==3.0.0',
           ]
```

