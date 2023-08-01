# Comparing `tmp/macrometa-target-snowflake-0.0.9.tar.gz` & `tmp/macrometa-target-snowflake-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-snowflake-0.0.9.tar", last modified: Sun Apr  2 07:28:35 2023, max compression
+gzip compressed data, was "macrometa-target-snowflake-1.0.0.tar", last modified: Tue Aug  1 08:45:30 2023, max compression
```

## Comparing `macrometa-target-snowflake-0.0.9.tar` & `macrometa-target-snowflake-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.115972 macrometa-target-snowflake-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22964 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38365 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/db_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/flattening.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/base_upload_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/s3_upload_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/snowflake_upload_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 07:28:35.115972 macrometa-target-snowflake-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:30.040017 macrometa-target-snowflake-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-08-01 08:45:30.040017 macrometa-target-snowflake-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22964 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:30.036018 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)    34402 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41619 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/db_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/file_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:30.040017 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/file_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/file_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/file_formats/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/file_formats/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/flattening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:30.040017 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/upload_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/upload_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/upload_clients/base_upload_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/upload_clients/s3_upload_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/upload_clients/snowflake_upload_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:30.036018 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-08-01 08:45:29.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-01 08:45:30.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:45:29.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 08:45:29.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-01 08:45:29.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 08:45:29.000000 macrometa-target-snowflake-1.0.0/macrometa_target_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:45:30.040017 macrometa-target-snowflake-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 08:45:11.000000 macrometa-target-snowflake-1.0.0/setup.py
```

### Comparing `macrometa-target-snowflake-0.0.9/LICENSE` & `macrometa-target-snowflake-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/PKG-INFO` & `macrometa-target-snowflake-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-snowflake
-Version: 0.0.9
+Version: 1.0.0
 Summary: Macrometa target for loading data to Snowflake
 Home-page: https://github.com/Macrometacorp/macrometa-target-snowflake
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `macrometa-target-snowflake-0.0.9/README.md` & `macrometa-target-snowflake-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/__init__.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
-import io
 import json
-import logging
 import os
 import sys
 import copy
 
-from asyncio import AbstractEventLoop
-from datetime import datetime
+from datetime import datetime, timezone
 from joblib import Parallel, delayed, parallel_backend
 from jsonschema import Draft7Validator, FormatChecker
+from prometheus_client import CollectorRegistry, Counter, Gauge, start_http_server
 from singer import get_logger
-from threading import Thread
-from typing import Dict, List, Optional
+from threading import Lock
+from typing import AsyncIterable, Dict, List, Optional
 
 import pkg_resources
 from c8connector import C8Connector, Sample, ConfigAttributeType, Schema
-from c8connector import ConfigProperty
+from c8connector import ConfigProperty, ensure_datetime
 
 
 from macrometa_target_snowflake.file_formats import csv
 from macrometa_target_snowflake.file_formats import parquet
 from macrometa_target_snowflake import stream_utils
 
-from macrometa_target_snowflake.db_sync import DbSync
+from macrometa_target_snowflake.db_sync import DbSync, create_private_key_file, delete_private_key_file
 from macrometa_target_snowflake.file_format import FileFormatTypes
 from macrometa_target_snowflake.exceptions import (
     RecordValidationException,
     InvalidValidationOperationException
 )
 
 LOGGER = get_logger('macrometa_target_snowflake')
@@ -38,14 +36,26 @@
 
 DEFAULT_BATCH_SIZE_ROWS = 100000
 DEFAULT_BATCH_WAIT_TIME = 60
 DEFAULT_PARALLELISM = 0  # 0 The number of threads used to flush tables
 # Don't use more than this number of threads by default when flushing streams in parallel
 DEFAULT_MAX_PARALLELISM = 16
 
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
 
 def add_metadata_columns_to_schema(schema_message):
     """Metadata _sdc columns according to the stitch documentation at
     https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns
 
     Metadata columns gives information about data injections
     """
@@ -84,16 +94,30 @@
 
     # The file format is detected at DbSync init time
     file_format_type = db.file_format.file_format_type
 
     return table_cache, file_format_type
 
 
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
 # pylint: disable=too-many-locals,too-many-branches,too-many-statements,invalid-name
-def persist_lines(config, lines, table_cache=None, file_format_type: FileFormatTypes = None) -> None:
+async def persist_lines(state, flushed_state, schemas, key_properties, validators, records_to_load, row_count,
+                        stream_to_sync, total_row_count, batch_size_rows, archive_load_files, archive_load_files_data,
+                        time_schedule, config, flush_lock, time_extracted_list, table_cache=None, file_format_type: FileFormatTypes = None) -> None:
     """Main loop to read and consume singer messages from stdin
 
     Params:
         config: configuration dictionary
         lines: iterable of singer messages
         table_cache: Optional dictionary of Snowflake table structures. This is useful to run the less
                      INFORMATION_SCHEMA and SHOW queries as possible.
@@ -102,36 +126,17 @@
         file_format_type: Optional FileFormatTypes value that defines which supported file format to use
                           to load data into Snowflake.
                           If not provided then it will be detected automatically
 
     Returns:
         tuple of retrieved items: table_cache, file_format_type
     """
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
-    archive_load_files = config.get('archive_load_files', False)
-    archive_load_files_data = {}
-
-    time_schedule = {
-        'batch_wait_limit_seconds': config.get('batch_wait_limit_seconds', DEFAULT_BATCH_WAIT_TIME),
-        'last_executed_time': datetime.now(),
-    }
-    event_loop = setup_flush_task(time_schedule, records_to_load, row_count, stream_to_sync, config,
-                                  state, flushed_state)
-
     # Loop over lines from stdin
-    for line in lines:
+    lines = read_stdin()
+    async for line in lines:
         try:
             o = json.loads(line)
         except json.decoder.JSONDecodeError:
             LOGGER.error('Unable to parse:\n%s', line)
             raise
 
         if 'type' not in o:
@@ -163,73 +168,80 @@
                         raise InvalidValidationOperationException(
                             f"Data validation failed and cannot load to destination. RECORD: {o['record']}\n"
                             "multipleOf validations that allows long precisions are not supported (i.e. with 15 digits"
                             "or more) Try removing 'multipleOf' methods from JSON schema.") from ex
                     raise RecordValidationException(f"Record does not pass schema validation. RECORD: {o['record']}") \
                         from ex
 
-            primary_key_string = stream_to_sync[stream].record_primary_key_string(
-                o['record'])
-            if not primary_key_string:
-                primary_key_string = f'RID-{total_row_count[stream]}'
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
-            if config.get('add_metadata_columns') or config.get('hard_delete'):
-                records_to_load[stream][primary_key_string] = stream_utils.add_metadata_values_to_record(
-                    o)
-            else:
-                records_to_load[stream][primary_key_string] = o['record']
-
-            if archive_load_files and stream in archive_load_files_data:
-                # Keep track of min and max of the designated column
-                stream_archive_load_files_values = archive_load_files_data[stream]
-                if 'column' in stream_archive_load_files_values:
-                    incremental_key_column_name = stream_archive_load_files_values['column']
-                    incremental_key_value = o['record'][incremental_key_column_name]
-                    min_value = stream_archive_load_files_values['min']
-                    max_value = stream_archive_load_files_values['max']
-
-                    if min_value is None or min_value > incremental_key_value:
-                        stream_archive_load_files_values['min'] = incremental_key_value
-
-                    if max_value is None or max_value < incremental_key_value:
-                        stream_archive_load_files_values['max'] = incremental_key_value
-
-            if row_count[stream] >= batch_size_rows:
-                LOGGER.info("Flush triggered by batch_size_rows (%s) reached in %s",
-                            batch_size_rows, stream)
-
-                # flush all streams, delete records if needed, reset counts and then emit current state
-                if config.get('flush_all_streams'):
-                    filter_streams = None
+            with flush_lock:
+                primary_key_string = stream_to_sync[stream].record_primary_key_string(
+                    o['record'])
+                if not primary_key_string:
+                    primary_key_string = f'RID-{total_row_count[stream]}'
+
+                if stream not in records_to_load:
+                    records_to_load[stream] = {}
+
+                # increment row count only when a new PK is encountered in the current batch
+                if primary_key_string not in records_to_load[stream]:
+                    row_count[stream] += 1
+                    total_row_count[stream] += 1
+
+                # append record
+                if config.get('add_metadata_columns') or config.get('hard_delete'):
+                    records_to_load[stream][primary_key_string] = stream_utils.add_metadata_values_to_record(
+                        o)
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
-                    archive_load_files_data,
-                    filter_streams=filter_streams)
+                if 'time_extracted' in o:
+                    time_extracted_list.append(ensure_datetime(o["time_extracted"]))
+                else:
+                    time_extracted_list.append(datetime.now(timezone.utc))
 
-                # emit last encountered state
-                emit_state(copy.deepcopy(flushed_state))
-                time_schedule['last_executed_time'] = datetime.now()
+                if archive_load_files and stream in archive_load_files_data:
+                    # Keep track of min and max of the designated column
+                    stream_archive_load_files_values = archive_load_files_data[stream]
+                    if 'column' in stream_archive_load_files_values:
+                        incremental_key_column_name = stream_archive_load_files_values['column']
+                        incremental_key_value = o['record'][incremental_key_column_name]
+                        min_value = stream_archive_load_files_values['min']
+                        max_value = stream_archive_load_files_values['max']
+
+                        if min_value is None or min_value > incremental_key_value:
+                            stream_archive_load_files_values['min'] = incremental_key_value
+
+                        if max_value is None or max_value < incremental_key_value:
+                            stream_archive_load_files_values['max'] = incremental_key_value
+
+                if row_count[stream] >= batch_size_rows:
+                    LOGGER.info("Flush triggered by batch_size_rows (%s) reached in %s",
+                                batch_size_rows, stream)
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
+                        archive_load_files_data,
+                        time_extracted_list,
+                        filter_streams=filter_streams)
+
+                    # emit last encountered state
+                    emit_state(copy.deepcopy(flushed_state))
+                    time_schedule['last_executed_time'] = datetime.now()
 
         elif t == 'SCHEMA':
             if 'stream' not in o:
                 raise Exception(
                     f"Line is missing required key 'stream': {line}")
 
             stream = o['stream']
@@ -239,129 +251,134 @@
             # the previously used version of the schema
             if stream not in schemas or schemas[stream] != new_schema:
 
                 schemas[stream] = new_schema
                 validators[stream] = Draft7Validator(
                     schemas[stream], format_checker=FormatChecker())
 
-                # flush records from previous stream SCHEMA
-                # if same stream has been encountered again, it means the schema might have been altered
-                # so previous records need to be flushed
-                if row_count.get(stream, 0) > 0:
-                    # flush all streams, delete records if needed, reset counts and then emit current state
-                    if config.get('flush_all_streams'):
-                        filter_streams = None
+                with flush_lock:
+                    # flush records from previous stream SCHEMA
+                    # if same stream has been encountered again, it means the schema might have been altered
+                    # so previous records need to be flushed
+                    if row_count.get(stream, 0) > 0:
+                        # flush all streams, delete records if needed, reset counts and then emit current state
+                        if config.get('flush_all_streams'):
+                            filter_streams = None
+                        else:
+                            filter_streams = [stream]
+                        flushed_state = flush_streams(records_to_load,
+                                                      row_count,
+                                                      stream_to_sync,
+                                                      config,
+                                                      state,
+                                                      flushed_state,
+                                                      archive_load_files_data,
+                                                      time_extracted_list,
+                                                      filter_streams=filter_streams)
+
+                        # emit latest encountered state
+                        emit_state(flushed_state)
+
+                    # key_properties key must be available in the SCHEMA message.
+                    if 'key_properties' not in o:
+                        raise Exception("key_properties field is required")
+
+                    # Log based and Incremental replications on tables with no Primary Key
+                    # cause duplicates when merging UPDATE events.
+                    # Stop loading data by default if no Primary Key.
+                    #
+                    # If you want to load tables with no Primary Key:
+                    #  1) Set ` 'primary_key_required': false ` in the macrometa-target-snowflake config.json
+                    #  or
+                    #  2) Use fastsync [postgres-to-snowflake, mysql-to-snowflake, etc.]
+                    if config.get('primary_key_required', True) and len(o['key_properties']) == 0:
+                        LOGGER.critical(
+                            'Primary key is set to mandatory but not defined in the [%s] stream', stream)
+                        raise Exception("key_properties field is required")
+
+                    key_properties[stream] = o['key_properties']
+
+                    if config.get('add_metadata_columns') or config.get('hard_delete'):
+                        stream_to_sync[stream] = DbSync(config,
+                                                        add_metadata_columns_to_schema(
+                                                            o),
+                                                        table_cache,
+                                                        file_format_type)
                     else:
-                        filter_streams = [stream]
-                    flushed_state = flush_streams(records_to_load,
-                                                  row_count,
-                                                  stream_to_sync,
-                                                  config,
-                                                  state,
-                                                  flushed_state,
-                                                  archive_load_files_data,
-                                                  filter_streams=filter_streams)
-
-                    # emit latest encountered state
-                    emit_state(flushed_state)
-
-                # key_properties key must be available in the SCHEMA message.
-                if 'key_properties' not in o:
-                    raise Exception("key_properties field is required")
-
-                # Log based and Incremental replications on tables with no Primary Key
-                # cause duplicates when merging UPDATE events.
-                # Stop loading data by default if no Primary Key.
-                #
-                # If you want to load tables with no Primary Key:
-                #  1) Set ` 'primary_key_required': false ` in the macrometa-target-snowflake config.json
-                #  or
-                #  2) Use fastsync [postgres-to-snowflake, mysql-to-snowflake, etc.]
-                if config.get('primary_key_required', True) and len(o['key_properties']) == 0:
-                    LOGGER.critical(
-                        'Primary key is set to mandatory but not defined in the [%s] stream', stream)
-                    raise Exception("key_properties field is required")
+                        stream_to_sync[stream] = DbSync(
+                            config, o, table_cache, file_format_type)
 
-                key_properties[stream] = o['key_properties']
+                    if archive_load_files:
+                        archive_load_files_data[stream] = {
+                            'tap': config.get('tap_id'),
+                        }
+
+                        # In case of incremental replication, track min/max of the replication key.
+                        # Incremental replication is assumed if o['bookmark_properties'][0] is one of the columns.
+                        incremental_key_column_name = stream_utils.get_incremental_key(
+                            o)
+                        if incremental_key_column_name:
+                            LOGGER.info(
+                                "Using %s as incremental_key_column_name", incremental_key_column_name)
+                            archive_load_files_data[stream].update(
+                                column=incremental_key_column_name,
+                                min=None,
+                                max=None
+                            )
+                        else:
+                            LOGGER.warning(
+                                "archive_load_files is enabled, but no incremental_key_column_name was found. "
+                                "Min/max values will not be added to metadata for stream %s.", stream
+                            )
 
-                if config.get('add_metadata_columns') or config.get('hard_delete'):
-                    stream_to_sync[stream] = DbSync(config,
-                                                    add_metadata_columns_to_schema(
-                                                        o),
-                                                    table_cache,
-                                                    file_format_type)
-                else:
-                    stream_to_sync[stream] = DbSync(
-                        config, o, table_cache, file_format_type)
-
-                if archive_load_files:
-                    archive_load_files_data[stream] = {
-                        'tap': config.get('tap_id'),
-                    }
-
-                    # In case of incremental replication, track min/max of the replication key.
-                    # Incremental replication is assumed if o['bookmark_properties'][0] is one of the columns.
-                    incremental_key_column_name = stream_utils.get_incremental_key(
-                        o)
-                    if incremental_key_column_name:
-                        LOGGER.info(
-                            "Using %s as incremental_key_column_name", incremental_key_column_name)
-                        archive_load_files_data[stream].update(
-                            column=incremental_key_column_name,
-                            min=None,
-                            max=None
-                        )
-                    else:
-                        LOGGER.warning(
-                            "archive_load_files is enabled, but no incremental_key_column_name was found. "
-                            "Min/max values will not be added to metadata for stream %s.", stream
-                        )
+                    stream_to_sync[stream].create_schema_if_not_exists()
+                    stream_to_sync[stream].sync_table()
 
-                stream_to_sync[stream].create_schema_if_not_exists()
-                stream_to_sync[stream].sync_table()
-
-                row_count[stream] = 0
-                total_row_count[stream] = 0
+                    row_count[stream] = 0
+                    total_row_count[stream] = 0
 
         elif t == 'ACTIVATE_VERSION':
             LOGGER.debug('ACTIVATE_VERSION message')
 
         elif t == 'STATE':
-            LOGGER.debug('Setting state to %s', o['value'])
-            state = o['value']
-
-            # # set flushed state if it's not defined or there are no records so far
-            if not flushed_state or sum(row_count.values()) == 0:
-                flushed_state = copy.deepcopy(state)
+            with flush_lock:
+                LOGGER.debug('Setting state to %s', o['value'])
+                state = o['value']
+
+                # # set flushed state if it's not defined or there are no records so far
+                if not flushed_state or sum(row_count.values()) == 0:
+                    flushed_state = copy.deepcopy(state)
 
         else:
             raise Exception(f"Unknown message type {o['type']} in message {o}")
 
     # if some bucket has records that need to be flushed but haven't reached batch size
     # then flush all buckets.
     if sum(row_count.values()) > 0:
-        # flush all streams one last time, delete records if needed, reset counts and then emit current state
-        flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state, flushed_state,
-                                      archive_load_files_data)
-        time_schedule['last_executed_time'] = datetime.now()
-
-    # emit latest state
-    emit_state(copy.deepcopy(flushed_state))
-    event_loop.stop()
+        with flush_lock:
+            # flush all streams one last time, delete records if needed, reset counts and then emit current state
+            flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state, flushed_state,
+                                          archive_load_files_data, time_extracted_list)
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
         archive_load_files_data,
+        time_extracted_list,
         filter_streams=None):
     """
     Flushes all buckets and resets records count to 0 as well as empties records to load list
     :param streams: dictionary with records to load per stream
     :param row_count: dictionary with row count per stream
     :param stream_to_sync: Snowflake db sync instance per stream
     :param config: dictionary containing the configuration
@@ -395,24 +412,26 @@
     # Single-host, thread-based parallelism
     with parallel_backend('threading', n_jobs=parallelism):
         Parallel()(delayed(load_stream_batch)(
             stream=stream,
             records=streams[stream],
             row_count=row_count,
             db_sync=stream_to_sync[stream],
+            time_extracted_list=time_extracted_list,
             no_compression=config.get('no_compression'),
             delete_rows=config.get('hard_delete'),
             temp_dir=config.get('temp_dir'),
             archive_load_files=copy.copy(
                 archive_load_files_data.get(stream, None))
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
@@ -429,33 +448,34 @@
             archive_load_files_data[stream]['min'] = None
             archive_load_files_data[stream]['max'] = None
 
     # Return with state message with flushed positions
     return flushed_state
 
 
-def load_stream_batch(stream, records, row_count, db_sync, no_compression=False, delete_rows=False,
+def load_stream_batch(stream, records, row_count, db_sync, time_extracted_list, no_compression=False, delete_rows=False,
                       temp_dir=None, archive_load_files=None):
     """Load one batch of the stream into target table"""
     # Load into snowflake
     if row_count[stream] > 0:
-        flush_records(stream, records, db_sync, temp_dir,
+        flush_records(stream, records, db_sync, time_extracted_list, temp_dir,
                       no_compression, archive_load_files)
 
         # Delete soft-deleted, flagged rows - where _sdc_deleted at is not null
         if delete_rows:
             db_sync.delete_rows(stream)
 
         # reset row count for the current stream
         row_count[stream] = 0
 
 
 def flush_records(stream: str,
                   records: List[Dict],
                   db_sync: DbSync,
+                  time_extracted_list: list,
                   temp_dir: str = None,
                   no_compression: bool = False,
                   archive_load_files: Dict = None) -> None:
     """
     Takes a list of record messages and loads it into the snowflake target table
 
     Args:
@@ -483,14 +503,19 @@
     size_bytes = os.path.getsize(filepath)
 
     # Upload to s3 and load into Snowflake
     s3_key = db_sync.put_to_stage(
         filepath, stream, row_count, temp_dir=temp_dir)
     db_sync.load_file(s3_key, row_count, size_bytes)
 
+    event_time = datetime.now(timezone.utc)
+    for time_extracted in time_extracted_list:
+        diff = event_time - time_extracted
+        export_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
+
     # Delete file from local disk
     os.remove(filepath)
 
     if archive_load_files:
         stream_name_parts = stream_utils.stream_name_to_dict(stream)
         if 'schema_name' not in stream_name_parts or 'table_name' not in stream_name_parts:
             raise Exception(
@@ -520,43 +545,68 @@
 
         db_sync.copy_to_archive(s3_key, archive_key, archive_metadata)
 
     # Delete file from S3
     db_sync.delete_from_stage(stream, s3_key)
 
 
-def setup_flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state,
-                     filter_streams=None) -> AbstractEventLoop:
-    event_loop = asyncio.new_event_loop()
-    Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
-    asyncio.run_coroutine_threadsafe(
-        flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state, filter_streams),
-        event_loop)
-    return event_loop
+async def setup_flush_task(config, table_cache=None, file_format_type: FileFormatTypes = None, filter_streams=None):
+    state = None
+    flushed_state = None
+    schemas = {}
+    key_properties = {}
+    validators = {}
+    records_to_load = {}
+    time_extracted_list = []
+    row_count = {}
+    stream_to_sync = {}
+    total_row_count = {}
+    batch_size_rows = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
+    archive_load_files = config.get('archive_load_files', False)
+    archive_load_files_data = {}
+
+    time_schedule = {
+        'batch_wait_limit_seconds': config.get('batch_wait_limit_seconds', DEFAULT_BATCH_WAIT_TIME),
+        'last_executed_time': datetime.now(),
+    }
+    flush_lock = Lock()
+    event_loop = asyncio.get_event_loop()
+    persist_lines_coro = persist_lines(state, flushed_state, schemas, key_properties, validators, records_to_load, row_count,
+                        stream_to_sync, total_row_count, batch_size_rows, archive_load_files, archive_load_files_data,
+                        time_schedule, config, flush_lock, time_extracted_list, table_cache, file_format_type)
+    asyncio.run_coroutine_threadsafe(persist_lines_coro, event_loop)
+    flush_task_coro = flush_task(time_schedule, records_to_load, row_count, stream_to_sync, config, state, flushed_state,
+                                 archive_load_files_data, flush_lock, time_extracted_list, filter_streams)
+    asyncio.run_coroutine_threadsafe(flush_task_coro, event_loop)
+
+    # Wait for all Futures to complete and propagate any exceptions raised
+    await asyncio.gather(
+        persist_lines_coro,
+        flush_task_coro,
+    )
 
 
 async def flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state,
-                     filter_streams=None) -> None:
+                     archive_load_files_data, flush_lock, time_extracted_list, filter_streams=None) -> None:
     while True:
         timedelta = datetime.now() - time_schedule['last_executed_time']
         if (
-            timedelta.total_seconds() >= time_schedule['batch_wait_limit_seconds']
+            timedelta.total_seconds(
+            ) >= time_schedule['batch_wait_limit_seconds']
             and sum(row_count.values()) > 0
         ):
-            # flush all streams one last time, delete records if needed, reset counts and then emit current state.
-            flushed_state = flush_streams(streams, row_count, stream_to_sync, config, state, flushed_state,
-                                          filter_streams)
-            # emit latest state
-            emit_state(copy.deepcopy(flushed_state))
-            time_schedule['last_executed_time'] = datetime.now()
-
-
-def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
-    asyncio.set_event_loop(loop)
-    loop.run_forever()
+            with flush_lock:
+                # flush all streams one last time, delete records if needed, reset counts and then emit current state.
+                flushed_state = flush_streams(streams, row_count, stream_to_sync, config, state, flushed_state,
+                                              archive_load_files_data, time_extracted_list, filter_streams)
+                # emit latest state
+                emit_state(copy.deepcopy(flushed_state))
+                time_schedule['last_executed_time'] = datetime.now()
+        # Add sleep statement to ensure periodic execution
+        await asyncio.sleep(time_schedule['batch_wait_limit_seconds'])
 
 
 class SnowflakeTargetConnector(C8Connector):
     """SnowflakeTargetConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
@@ -599,82 +649,110 @@
     def reserved_keys(self) -> list[str]:
         """List of reserved keys for the connector."""
         return []
 
     def config(self) -> List[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
-            ConfigProperty('account', 'Account', ConfigAttributeType.STRING, True, False,
-                           description='Snowflake account.',
-                           placeholder_value='my_account'),
+            ConfigProperty('account', 'Account ID', ConfigAttributeType.STRING, True, False,
+                           description='Snowflake account identifier. Refer here for more info: '
+                                       'https://docs.snowflake.com/en/user-guide/admin-account-identifier.',
+                           placeholder_value='my_org-my_account'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
                            description='Snowflake user name.',
                            placeholder_value='my_username'),
-            ConfigProperty('password', 'Password', ConfigAttributeType.STRING, True, False,
-                           description='Snowflake password.',
+            ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, False, False,
+                           description='Snowflake password. It is required when using user/pass authentication and '
+                                       'not using Key/Pair (Private Key) authentication.',
                            placeholder_value='my_password'),
-            ConfigProperty('dbname', 'Database', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('dbname', 'Database Name', ConfigAttributeType.STRING, True, False,
                            description='Snowflake target database.',
                            placeholder_value='my_database'),
-            ConfigProperty('target_schema', 'Target Schema', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('target_schema', 'Target Schema', ConfigAttributeType.STRING, True, True,
                            description='Snowflake target schema.',
                            placeholder_value='my_schema'),
-            ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, True,
                            description='Snowflake target table.',
                            placeholder_value='my_table'),
-            ConfigProperty('warehouse', 'Warehouse', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('warehouse', 'Warehouse', ConfigAttributeType.STRING, True, True,
                            description='Snowflake target warehouse.',
                            placeholder_value='my_warehouse'),
-            ConfigProperty('file_format', 'File Format', ConfigAttributeType.STRING, True, False,
-                           description='Snowflake file format for loading. Currently supported CSV and PARQUET.',
+            ConfigProperty('file_format', 'File Format', ConfigAttributeType.STRING, True, True,
+                           description='Snowflake file format for loading. Currently only CSV and PARQUET'
+                                       ' file formats are supported.',
                            placeholder_value='my_file_format'),
             ConfigProperty('role', 'Role', ConfigAttributeType.STRING, False, False,
                            description='Snowflake role (optional).',
                            placeholder_value='my_role'),
-            ConfigProperty('primary_key_required', 'Primary Key Required', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Indicates whether primary key is required (optional).',
-                           default_value='false'),
             ConfigProperty('batch_size_rows', 'Batch Size Rows', ConfigAttributeType.INT, False, False,
                            description='Number of rows per batch.',
                            default_value='100000'),
-            ConfigProperty('batch_wait_limit_seconds', 'Batch Wait Limit (seconds)', ConfigAttributeType.INT, False, False,
+            ConfigProperty('batch_wait_limit_seconds', 'Batch Wait Limit (Seconds)', ConfigAttributeType.INT, False, False,
                            description='Maximum time to wait for a batch in seconds.',
                            default_value='60'),
-            ConfigProperty('target_schema_select_permission', 'Target Schema Select Permission', ConfigAttributeType.STRING, False, False,
-                           description='SELECT permission for target schema.',
-                           placeholder_value='SELECT'),
             ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Indicates whether to perform a hard delete on records.',
-                           default_value='false')
+                           description='When `hard_delete` option is true then DELETE SQL commands will be performed '
+                                       'in Snowflake to delete rows in tables. It is achieved by continuously checking '
+                                       'the `_SDC_DELETED_AT` metadata column sent by the data source.',
+                           default_value='false'),
+            ConfigProperty('private_key', 'Private Key', ConfigAttributeType.FILE, False, False,
+                           description='A private key used for authentication using Key Pair authentication instead of user/pass. At the moment, only PEM format is supported.',
+                           placeholder_value='my_private_key'),
+            ConfigProperty('private_key_passphrase', 'Private Key Passphrase', ConfigAttributeType.PASSWORD, False, False,
+                           description='The private key passphrase used for authenticating using Key Pair authentication instead of user/pass.',
+                           placeholder_value='my_private_key_passphrase')
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
         return []
 
 
-def main():
+async def main_impl():
     """Main function"""
+    # Start the Prometheus HTTP server for exposing metrics
+    LOGGER.info("Snowflake target is starting the metrics server.")
+    start_http_server(8001, registry=registry_package)
     arg_parser = argparse.ArgumentParser()
     arg_parser.add_argument('-c', '--config', help='Config file')
     args = arg_parser.parse_args()
 
     if args.config:
         with open(args.config, encoding="utf8") as config_input:
             config = json.load(config_input)
     else:
         config = {}
 
-    # Init columns cache
-    table_cache, file_format_type = get_snowflake_statics(config)
+    # Create private key file
+    config = create_private_key_file(config)
 
-    # Consume singer messages
-    singer_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
-    persist_lines(config, singer_messages, table_cache, file_format_type)
+    try:
+        # Init columns cache
+        table_cache, file_format_type = get_snowflake_statics(config)
+
+        # Consume singer messages
+        await setup_flush_task(config, table_cache, file_format_type)
+    except Exception as e:
+        # Increment export_errors metric
+        export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+        delete_private_key_file(config)
+        raise e
+
+    # Delete private key file
+    delete_private_key_file(config)
 
     LOGGER.debug("Exiting normally")
 
 
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

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/db_sync.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/db_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 import json
 import sys
 import snowflake.connector
 import re
 import time
+import singer
+import uuid
+from pathlib import Path
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import serialization
 
 from typing import List, Dict, Union, Tuple, Set
-from singer import get_logger
 from macrometa_target_snowflake import flattening
 from macrometa_target_snowflake import stream_utils
 from macrometa_target_snowflake.file_format import FileFormat, FileFormatTypes
 
 from macrometa_target_snowflake.exceptions import TooManyRecordsException, PrimaryKeyNotFoundException
 from macrometa_target_snowflake.upload_clients.s3_upload_client import S3UploadClient
 from macrometa_target_snowflake.upload_clients.snowflake_upload_client import SnowflakeUploadClient
 
+LOGGER = singer.get_logger('macrometa_target_snowflake')
+
 
 def validate_config(config):
     """Validate configuration"""
     errors = []
     s3_required_config_keys = [
         'account',
         'dbname',
         'user',
-        'password',
         'warehouse',
         's3_bucket',
         'stage',
         'file_format'
     ]
 
     snowflake_required_config_keys = [
         'account',
         'dbname',
         'user',
-        'password',
         'warehouse',
         'file_format'
     ]
 
     required_config_keys = []
 
+    possible_authentication_keys = [
+        'password',
+        'private_key'
+    ]
+
     # Use external stages if both s3_bucket and stage defined
     if config.get('s3_bucket', None) and config.get('stage', None):
         required_config_keys = s3_required_config_keys
     # Use table stage if none s3_bucket and stage defined
     elif not config.get('s3_bucket', None) and not config.get('stage', None):
         required_config_keys = snowflake_required_config_keys
     else:
@@ -68,14 +77,18 @@
 
     # Check if archive load files option is using external stages
     archive_load_files = config.get('archive_load_files', False)
     if archive_load_files and not config.get('s3_bucket', None):
         errors.append(
             'Archive load files option can be used only with external s3 stages. Please define s3_bucket.')
 
+    if not any(config.get(k, None) for k in possible_authentication_keys):
+        errors.append(
+            f'Required authentication key missing. Existing methods: {",".join(possible_authentication_keys)}')
+
     return errors
 
 
 def column_type(schema_property):
     """Take a specific schema property and return the snowflake equivalent column type"""
     property_type = schema_property['type']
     property_format = schema_property['format'] if 'format' in schema_property else None
@@ -167,14 +180,64 @@
     }.items():
         if k in query_tag:
             query_tag = query_tag.replace(k, v or '')
 
     return query_tag
 
 
+# PRIVATE KEY PATH
+def create_private_key_file(config: Dict) -> Dict:
+    path_uuid = uuid.uuid4().hex
+    try:
+        if config.get('private_key'):
+            path = f"/opt/snowflake/{path_uuid}/rsa_key.p8"
+            private_key = Path(path)
+            private_key.parent.mkdir(exist_ok=True, parents=True)
+            private_key.write_text(
+                create_private_key_string(config['private_key']))
+            config['private_key'] = path
+            LOGGER.info(f"Private key file created at: {path}")
+
+    except Exception as e:
+        LOGGER.warn(
+            f'Failed to create private key: /opt/snowflake/{path_uuid}/rsa_key.p8')
+
+    return config
+
+
+def delete_private_key_file(config: Dict) -> None:
+    try:
+        private_key = None
+        if config.get('private_key'):
+            path = config['private_key']
+            private_key = Path(path)
+            config['private_key'] = private_key.read_text()
+            private_key.unlink()
+            LOGGER.info(f"Private key file deleted from: {path}")
+
+        if private_key is not None:
+            private_key.parent.rmdir()
+    except Exception as e:
+        LOGGER.warn(f"Failed to delete private key file: {e}")
+
+
+def create_private_key_string(private_key_string: str) -> str:
+    private_key_list = []
+    split_string = private_key_string.split("-----")
+    if len(split_string) < 4:
+        raise Exception("Invalid PEM format for private key.")
+    for i in range(len(split_string)):
+        if ((i % 2) == 1):
+            private_key_list.extend(("-----", split_string[i], "-----"))
+        else:
+            private_key_list.append(split_string[i].replace(' ', '\n'))
+
+    return ''.join(private_key_list)
+
+
 # pylint: disable=too-many-public-methods,too-many-instance-attributes
 class DbSync:
     """DbSync class"""
 
     def __init__(self, connection_config, stream_schema_message=None, table_cache=None, file_format_type=None):
         """
             connection_config:      Snowflake connection details
@@ -195,42 +258,43 @@
                                     purposes.
         """
         self.connection_config = connection_config
         self.stream_schema_message = stream_schema_message
         self.table_cache = table_cache
 
         # logger to be used across the class's methods
-        self.logger = get_logger('macrometa_target_snowflake')
+        self.logger = singer.get_logger('macrometa_target_snowflake')
 
         # Validate connection configuration
         config_errors = validate_config(connection_config)
 
         # Exit if config has errors
         if len(config_errors) > 0:
-            self.logger.error('Invalid configuration:\n   * %s',
-                              '\n   * '.join(config_errors))
-            sys.exit(1)
+            error_msg = "Invalid configuration:\n   * {}".format('\n   * '.join(config_errors))
+            self.logger.error(error_msg)
+            raise Exception(error_msg)
 
         if self.connection_config.get('stage', None):
             stage = stream_utils.stream_name_to_dict(
                 self.connection_config['stage'], separator='.')
             if not stage['schema_name']:
-                self.logger.error(
-                    "The named external stage object in config has to use the <schema>.<stage_name> format.")
-                sys.exit(1)
+                error_msg = "The named external stage object in config has to use the <schema>.<stage_name> format."
+                self.logger.error(error_msg)
+                raise Exception(error_msg)
 
         self.schema_name = None
         self.grantees = None
         self.file_format = FileFormat(
             self.connection_config['file_format'], self.query, file_format_type)
 
         if not self.connection_config.get('stage') and self.file_format.file_format_type == FileFormatTypes.PARQUET:
-            self.logger.error("Table stages with Parquet file format is not supported. "
-                              "Use named stages with Parquet file format or table stages with CSV files format")
-            sys.exit(1)
+            error_msg = "Table stages with Parquet file format is not supported. " \
+                        "Use named stages with Parquet file format or table stages with CSV files format."
+            self.logger.error(error_msg)
+            raise Exception(error_msg)
 
         # Init stream schema pylint: disable=line-too-long
         if self.stream_schema_message is not None:
             #  Define target schema name.
             #  --------------------------
             #  Target schema name can be defined in multiple ways:
             #
@@ -268,23 +332,50 @@
         # Use external stage
         if connection_config.get('s3_bucket', None):
             self.upload_client = S3UploadClient(connection_config)
         # Use table stage
         else:
             self.upload_client = SnowflakeUploadClient(connection_config, self)
 
+    def get_private_key(self):
+        """
+        Get private key from the right location
+        """
+        if self.connection_config.get('private_key'):
+            try:
+                encoded_passphrase = self.connection_config['private_key_passphrase'].encode(
+                )
+            except KeyError:
+                encoded_passphrase = None
+
+            with open(self.connection_config['private_key'], 'rb') as key:
+                p_key = serialization.load_pem_private_key(
+                    key.read(),
+                    password=encoded_passphrase,
+                    backend=default_backend()
+                )
+
+            pkb = p_key.private_bytes(
+                encoding=serialization.Encoding.DER,
+                format=serialization.PrivateFormat.PKCS8,
+                encryption_algorithm=serialization.NoEncryption())
+            return pkb
+
+        return None
+
     def open_connection(self):
         """Open snowflake connection"""
         stream = None
         if self.stream_schema_message:
             stream = self.stream_schema_message['stream']
 
         return snowflake.connector.connect(
             user=self.connection_config['user'],
-            password=self.connection_config['password'],
+            password=self.connection_config.get('password'),
+            private_key=self.get_private_key(),
             account=self.connection_config['account'],
             database=self.connection_config['dbname'],
             warehouse=self.connection_config['warehouse'],
             role=self.connection_config.get('role', None),
             autocommit=True,
             session_parameters={
                 # Quoted identifiers should be case sensitive
@@ -807,15 +898,15 @@
         self.logger.info('Adding column: %s', add_column)
         self.query(add_column)
 
     def sync_table(self):
         """Creates or alters the target table according to the schema"""
         stream_schema_message = self.stream_schema_message
         stream = stream_schema_message['stream']
-        table_name = self.table_name(stream, False, True)
+        table_name = self.table_name(self.connection_config.get('target_table'), False, True)
         table_name_with_schema = self.table_name(
             self.connection_config.get('target_table'), False)
 
         if self.table_cache:
             found_tables = list(filter(lambda x: x['SCHEMA_NAME'] == self.schema_name.upper() and
                                        f'"{x["TABLE_NAME"].upper()}"' == table_name,
                                        self.table_cache))
```

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/exceptions.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_format.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/file_format.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/csv.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/file_formats/csv.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/parquet.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/file_formats/parquet.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/flattening.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/flattening.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/stream_utils.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/stream_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/base_upload_client.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/upload_clients/base_upload_client.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/s3_upload_client.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/upload_clients/s3_upload_client.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/snowflake_upload_client.py` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake/upload_clients/snowflake_upload_client.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/PKG-INFO` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-snowflake
-Version: 0.0.9
+Version: 1.0.0
 Summary: Macrometa target for loading data to Snowflake
 Home-page: https://github.com/Macrometacorp/macrometa-target-snowflake
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/SOURCES.txt` & `macrometa-target-snowflake-1.0.0/macrometa_target_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.9/setup.py` & `macrometa-target-snowflake-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name="macrometa-target-snowflake",
-      version='0.0.9',
+      version='1.0.0',
       description="Macrometa target for loading data to Snowflake",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-target-snowflake',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
@@ -23,15 +23,16 @@
       python_requires='>=3.7',
       install_requires=[
           'pipelinewise-singer-python==1.2.0',
           'snowflake-connector-python[pandas]==2.7.*',
           'inflection==0.5.1',
           'joblib==1.2.0',
           'boto3==1.23.10',
-          'c8connector==0.0.15'
+          'c8connector>=0.0.29',
+          'prometheus-client==0.16.0'
       ],
       extras_require={
           "test": [
               "pylint==2.12.*",
               'pytest==7.0.1',
               'pytest-cov==4.0.0',
               "python-dotenv==0.19.*"
```

