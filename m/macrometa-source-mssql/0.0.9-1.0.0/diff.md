# Comparing `tmp/macrometa-source-mssql-0.0.9.tar.gz` & `tmp/macrometa-source-mssql-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mssql-0.0.9.tar", max compression
+gzip compressed data, was "macrometa-source-mssql-1.0.0.tar", max compression
```

## Comparing `macrometa-source-mssql-0.0.9.tar` & `macrometa-source-mssql-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11899 2023-05-18 12:22:30.947407 macrometa-source-mssql-0.0.9/LICENSE
--rw-r--r--   0        0        0    35000 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/__init__.py
--rwxr-xr-x   0        0        0     1476 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/connection.py
--rw-r--r--   0        0        0     2287 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sample_data.py
--rwxr-xr-x   0        0        0        0 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     8025 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/common.py
--rwxr-xr-x   0        0        0     2206 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/full_table.py
--rw-r--r--   0        0        0    14533 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1537 2023-05-18 12:22:31.239440 macrometa-source-mssql-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.9/setup.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-08-01 08:37:50.719220 macrometa-source-mssql-1.0.0/LICENSE
+-rw-r--r--   0        0        0    38348 2023-08-01 08:37:50.719220 macrometa-source-mssql-1.0.0/macrometa_source_mssql/__init__.py
+-rwxr-xr-x   0        0        0     1534 2023-08-01 08:37:50.719220 macrometa-source-mssql-1.0.0/macrometa_source_mssql/connection.py
+-rw-r--r--   0        0        0     2287 2023-08-01 08:37:50.719220 macrometa-source-mssql-1.0.0/macrometa_source_mssql/sample_data.py
+-rwxr-xr-x   0        0        0        0 2023-08-01 08:37:50.719220 macrometa-source-mssql-1.0.0/macrometa_source_mssql/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     7934 2023-08-01 08:37:50.719220 macrometa-source-mssql-1.0.0/macrometa_source_mssql/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     2203 2023-08-01 08:37:50.719220 macrometa-source-mssql-1.0.0/macrometa_source_mssql/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    16103 2023-08-01 08:37:50.719220 macrometa-source-mssql-1.0.0/macrometa_source_mssql/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1566 2023-08-01 08:37:51.067218 macrometa-source-mssql-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 macrometa-source-mssql-1.0.0/setup.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 macrometa-source-mssql-1.0.0/PKG-INFO
```

### Comparing `macrometa-source-mssql-0.0.9/LICENSE` & `macrometa-source-mssql-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.9/macrometa_source_mssql/__init__.py` & `macrometa-source-mssql-1.0.0/macrometa_source_mssql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 
 import collections
 import copy
 import itertools
+import os
 import time
 
 import pkg_resources
 import singer
 import singer.schema
 from c8connector import (
     C8Connector, ConfigProperty, Sample, Schema,
-    ConfigAttributeType, SchemaAttributeType, SchemaAttribute)
+    ConfigAttributeType, SchemaAttributeType, SchemaAttribute, ValidationException)
+from prometheus_client import CollectorRegistry, start_http_server, Counter
 from singer import metadata, utils
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema as SingerSchema
 
 import macrometa_source_mssql.sync_strategies.common as common
 import macrometa_source_mssql.sync_strategies.full_table as full_table
 import macrometa_source_mssql.sync_strategies.log_based as log_based
@@ -29,14 +31,19 @@
     'user',
     'password',
     'database',
     'source_schema',
     'source_table'
 ]
 
+region_label = os.getenv("GDN_FEDERATION", "NA")
+tenant_label = os.getenv("GDN_TENANT", "NA")
+fabric_label = os.getenv("GDN_FABRIC", "NA")
+workflow_label = os.getenv("WORKFLOW_UUID", "NA")
+
 
 class MicrosoftSQLServerConnector(C8Connector):
     """MicrosoftSQLServerConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
         return "Microsoft SQL Server"
@@ -63,32 +70,59 @@
 
     def validate(self, integration: dict) -> None:
         """Validate given configurations against the connector.
         If invalid, throw an exception with the cause.
         """
         try:
             config = self.get_config(integration)
-            mssql_conn = MSSQLConnection(config)
+            if config['replication_method'] not in ["FULL_TABLE", "LOG_BASED"]:
+                raise Exception('Invalid replication method provided. It should be either FULL_TABLE or LOG_BASED.')
+            mssql_conn = MSSQLConnection(config, require_database=False)
             with connect_with_backoff(mssql_conn) as open_conn:
                 try:
                     with open_conn.cursor() as cur:
+                        # Check connection
                         cur.execute("""SELECT @@VERSION as version, @@lock_timeout as lock_wait_timeout""")
                         row = cur.fetchone()
                         LOGGER.info(
                             "Server Parameters: " + "version: %s, " + "lock_timeout: %s, ",
                             *row,
                         )
+
+                        # Check database existence
+                        database_name = config.get('database')
+                        cur.execute(f"SELECT name FROM sys.databases WHERE name = '{database_name}'")
+                        database_row = cur.fetchone()
+                        if not database_row:
+                            raise Exception(f"Database '{database_name}' does not exist.")
+
+                        # Check schema existence
+                        schema_name = config.get('source_schema')
+                        cur.execute(f"SELECT name FROM {database_name}.sys.schemas WHERE name = '{schema_name}'")
+                        schema_row = cur.fetchone()
+                        if not schema_row:
+                            raise Exception(f"Schema '{schema_name}' does not exist.")
+
+                        # Check table existence
+                        table_name = config.get('source_table')
+                        cur.execute(
+                            f"SELECT TABLE_NAME FROM {database_name}.INFORMATION_SCHEMA.TABLES WHERE "
+                            f"TABLE_NAME = '{table_name}' AND TABLE_SCHEMA = '{schema_name}'")
+                        table_row = cur.fetchone()
+                        if not table_row:
+                            raise Exception(f"Table '{table_name}' does not exist in schema '{schema_name}'.")
                 except Exception as e:
                     raise e
         except Exception as e:
-            raise e
+            raise ValidationException(e)
 
     def samples(self, integration: dict) -> list[Sample]:
         """Fetch sample data using the provided configurations."""
         try:
+            self.validate(integration)
             config = self.get_config(integration)
             mssql_conn = MSSQLConnection(config)
             catalog = do_discover(mssql_conn, config)
             results = []
             for stream in catalog.streams:
                 s_attribs = []
                 s_schema = stream.schema
@@ -113,14 +147,15 @@
             LOGGER.info("Exception raised: %s", e)
             raise e
         return results
 
     def schemas(self, integration: dict) -> list[Schema]:
         """Get supported schemas using the given configurations."""
         try:
+            self.validate(integration)
             config = self.get_config(integration)
             mssql_conn = MSSQLConnection(config)
             catalog = do_discover(mssql_conn, config)
             results = []
             for stream in catalog.streams:
                 s_attribs = []
                 s_schema = stream.schema
@@ -174,22 +209,28 @@
                            description='Microsoft SQL Server database name.', default_value='master'),
             ConfigProperty('source_schema', 'Source Schema', ConfigAttributeType.STRING, True, True,
                            description='Source Schema to scan.', placeholder_value='my_schema'),
             ConfigProperty('source_table', 'Source Table', ConfigAttributeType.STRING, True, True,
                            description='Source Table to scan.', placeholder_value='my_table'),
             ConfigProperty('replication_method', 'Replication Method', ConfigAttributeType.STRING, True, True,
                            description='Choose from LOG_BASED, FULL_TABLE.', default_value='FULL_TABLE'),
+            ConfigProperty('log_polling_interval', 'Log Polling Interval', ConfigAttributeType.INT, False, False,
+                           description='Polling Interval for Microsoft SQL Server CDC Logs', default_value='10'),
             ConfigProperty('characterset', 'Character Set', ConfigAttributeType.STRING, False, False,
                            description='The characterset of the Microsoft SQL Server database.', default_value='utf8'),
             ConfigProperty('tds_version', 'TDS Version', ConfigAttributeType.STRING, False, False,
                            description='Set the version of TDS to use when communicating with MS SQL Server.',
                            default_value='7.3'),
             ConfigProperty('use_date_datatype', 'Use Date data type', ConfigAttributeType.BOOLEAN, False, False,
                            description='Emit `datetime` type values as a date without a time component or time without '
                                        'an UTC offset.', default_value='false'),
+            ConfigProperty('debug_lsn', 'Debug LSN', ConfigAttributeType.BOOLEAN, False, False,
+                           description='If set to True then add _sdc_lsn properties to the singer messages '
+                                       'to debug MSSQL LSN positions.',
+                           default_value='false'),
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
         return ['catalog', 'discover', 'state']
@@ -207,18 +248,20 @@
                 'source_schema': integration['source_schema'],
                 'source_table': integration['source_table'],
 
                 # Optional config keys
                 'characterset': integration.get('characterset', "utf8"),
                 'tds_version': integration.get('tds_version', "7.3"),
                 'use_date_datatype': integration.get('use_date_datatype', False),
-                'replication_method': integration.get('replication_method', "FULL_TABLE")
+                'replication_method': integration.get('replication_method', "FULL_TABLE"),
+                'log_polling_interval': integration.get('log_polling_interval', 10),
+                'debug_lsn': integration.get('debug_lsn', False)
             }
         except KeyError as e:
-            raise KeyError(f'Integration property `{e}` not found.') from e
+            raise ValidationException(f'Integration property `{e}` not found.') from e
 
 
 Column = collections.namedtuple(
     "Column",
     [
         "table_schema",
         "table_name",
@@ -695,15 +738,15 @@
     )
 
 
 def do_sync_historical_log(mssql_conn, config, catalog_entry, state, columns):
     mssql_conn = MSSQLConnection(config)
 
     # Add additional keys to the schema
-    log_based.add_synthetic_keys_to_schema(catalog_entry)
+    log_based.add_synthetic_keys_to_schema(config, catalog_entry)
 
     write_schema_message(catalog_entry)
 
     stream_version = common.get_stream_version(catalog_entry.tap_stream_id, state)
 
     # full_table.sync_table(mssql_conn, config, catalog_entry, state, columns, stream_version)
     log_based.sync_historic_table(mssql_conn, config, catalog_entry, state, columns, stream_version)
@@ -739,30 +782,29 @@
 
 def do_sync_log_based(mssql_conn, config, catalog_entry, state, columns):
     LOGGER.info(f"inside do_sync_log_based...")
     mssql_conn = MSSQLConnection(config)
     md_map = metadata.to_map(catalog_entry.metadata)
     replication_key = md_map.get((), {}).get("replication-key")
     # Add additional keys to the schema
-    log_based.add_synthetic_keys_to_schema(catalog_entry)
+    log_based.add_synthetic_keys_to_schema(config, catalog_entry)
 
     LOGGER.info("SingerSchema written")
     write_schema_message(catalog_entry=catalog_entry, bookmark_properties=[replication_key])
 
     LOGGER.info("Starting CDC based replication")
     while True:
         try:
             stream_version = common.get_stream_version(catalog_entry.tap_stream_id, state)
             log_based.sync_table(mssql_conn, config, catalog_entry, state, columns, stream_version)
             singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
-            LOGGER.warn("Successful CDC...")
-        except Exception as e:
-            LOGGER.warn("Failed CDC...")
+        except:
+            pass
         finally:
-            time.sleep(5)
+            time.sleep(config.get("log_polling_interval"))
 
 
 def sync_non_cdc_streams(mssql_conn, non_cdc_catalog, config, state):
     mssql_conn = MSSQLConnection(config)
 
     for catalog_entry in non_cdc_catalog.streams:
         columns = list(catalog_entry.schema.properties.keys())
@@ -865,29 +907,41 @@
                     *row,
                 )
         except:
             LOGGER.warning("Encountered error checking server params.")
 
 
 def main_impl():
-    args = utils.parse_args(REQUIRED_CONFIG_KEYS)
-    mssql_conn = MSSQLConnection(args.config)
-    log_server_params(mssql_conn)
-
-    if args.discover:
-        do_discover(mssql_conn, args.config)
-    elif args.catalog:
-        state = args.state or {}
-        do_sync(mssql_conn, args.config, args.catalog, state)
-    elif args.properties:
-        catalog = Catalog.from_dict(args.properties)
-        state = args.state or {}
-        do_sync(mssql_conn, args.config, catalog, state)
-    else:
-        LOGGER.info("No properties were selected")
+    # Create a custom CollectorRegistry
+    registry_package = CollectorRegistry()
+    ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
+                        ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
+    LOGGER.info("Mssql source is starting the metrics server.")
+    start_http_server(8000, registry=registry_package)
+
+    try:
+        args = utils.parse_args(REQUIRED_CONFIG_KEYS)
+        mssql_conn = MSSQLConnection(args.config)
+        log_server_params(mssql_conn)
+
+        if args.discover:
+            do_discover(mssql_conn, args.config)
+        elif args.catalog:
+            state = args.state or {}
+            do_sync(mssql_conn, args.config, args.catalog, state)
+        elif args.properties:
+            catalog = Catalog.from_dict(args.properties)
+            state = args.state or {}
+            do_sync(mssql_conn, args.config, catalog, state)
+        else:
+            LOGGER.info("No properties were selected")
+    except Exception as e:
+        LOGGER.warn("Exception raised: %s", e)
+        ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+        raise e
 
 
 def main():
     try:
         main_impl()
     except Exception as exc:
         LOGGER.critical(exc)
```

### Comparing `macrometa-source-mssql-0.0.9/macrometa_source_mssql/connection.py` & `macrometa-source-mssql-1.0.0/macrometa_source_mssql/connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,24 +20,25 @@
         for w in warnings:
             LOGGER.warning(w)
 
     return connection
 
 
 class MSSQLConnection(pymssql.Connection):
-    def __init__(self, config):
+    def __init__(self, config, require_database=True):
         args = {
             "user": config.get("user"),
             "password": config.get("password"),
             "server": config["host"],
-            "database": config["database"],
             "charset": config.get("characterset", "utf8"),
             "port": config.get("port", "1433"),
             "tds_version": config.get("tds_version", "7.3"),
         }
+        if require_database:
+            args["database"] = config["database"]
         conn = pymssql._mssql.connect(**args)
         super().__init__(conn, False, True)
 
     def __enter__(self):
         return self
 
     def __exit__(self, *exc_info):
```

### Comparing `macrometa-source-mssql-0.0.9/macrometa_source_mssql/sample_data.py` & `macrometa-source-mssql-1.0.0/macrometa_source_mssql/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/common.py` & `macrometa-source-mssql-1.0.0/macrometa_source_mssql/sync_strategies/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,31 +155,28 @@
         for non_whitelisted_bookmark_key in state.get("bookmarks", {}).get(tap_stream_id, {}).keys()
         if non_whitelisted_bookmark_key not in bookmark_key_set
     ]:
         singer.clear_bookmark(state, tap_stream_id, bk)
 
 
 def sync_query(cursor, catalog_entry, state, select_sql, columns, stream_version, params, config):
-    replication_key = singer.get_bookmark(state, catalog_entry.tap_stream_id, "replication_key")
-
     # query_string = cursor.mogrify(select_sql, params)
-
-    time_extracted = utils.now()
     cursor.execute(select_sql, params)
 
     row = cursor.fetchone()
     rows_saved = 0
 
     database_name = get_database_name(catalog_entry)
 
     with metrics.record_counter(None) as counter:
         counter.tags["database"] = database_name
         counter.tags["table"] = catalog_entry.table
 
         while row:
+            time_extracted = utils.now()
             counter.increment()
             rows_saved += 1
             record_message = row_to_singer_record(
                 catalog_entry, stream_version, row, columns, time_extracted, config
             )
             singer.write_message(record_message)
             md_map = metadata.to_map(catalog_entry.metadata)
```

### Comparing `macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/full_table.py` & `macrometa-source-mssql-1.0.0/macrometa_source_mssql/sync_strategies/full_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 def generate_bookmark_keys(catalog_entry):
     base_bookmark_keys = {
         "last_pk_fetched",
         "max_pk_values",
         "version",
         "initial_full_table_complete",
     }
-
     bookmark_keys = base_bookmark_keys
-
     return bookmark_keys
 
 
 def sync_table(mssql_conn, config, catalog_entry, state, columns, stream_version):
     mssql_conn = MSSQLConnection(config)
     common.whitelist_bookmark_keys(
         generate_bookmark_keys(catalog_entry), catalog_entry.tap_stream_id, state
@@ -55,9 +53,8 @@
             common.sync_query(
                 cur, catalog_entry, state, select_sql, columns, stream_version, params, config
             )
 
     # clear max pk value and last pk fetched upon successful sync
     singer.clear_bookmark(state, catalog_entry.tap_stream_id, "max_pk_values")
     singer.clear_bookmark(state, catalog_entry.tap_stream_id, "last_pk_fetched")
-
     singer.write_message(activate_version_message)
```

### Comparing `macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/log_based.py` & `macrometa-source-mssql-1.0.0/macrometa_source_mssql/sync_strategies/log_based.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,45 +101,46 @@
     LOGGER.info(
         "Max LSN ID : %s",
         row[0].hex(),
     )
     return row
 
 
-def add_synthetic_keys_to_schema(catalog_entry):
-    catalog_entry.schema.properties["_sdc_operation_type"] = Schema(
-        description="Source operation I=Insert, D=Delete, U=Update",
-        type=["null", "string"],
-        format="string",
-    )
-    catalog_entry.schema.properties["_sdc_lsn_commit_timestamp"] = Schema(
-        description="Source system commit timestamp", type=["null", "string"], format="date-time"
-    )
-    catalog_entry.schema.properties["_sdc_lsn_deleted_at"] = Schema(
+def add_synthetic_keys_to_schema(config, catalog_entry):
+    catalog_entry.schema.properties["_sdc_deleted_at"] = Schema(
         description="Source system delete timestamp", type=["null", "string"], format="date-time"
     )
-    catalog_entry.schema.properties["_sdc_lsn_value"] = Schema(
-        description="Source system log sequence number (LSN)",
-        type=["null", "string"],
-        format="string",
-    )
-    catalog_entry.schema.properties["_sdc_lsn_seq_value"] = Schema(
-        description="Source sequence number within the system log sequence number (LSN)",
-        type=["null", "string"],
-        format="string",
-    )
-    catalog_entry.schema.properties["_sdc_lsn_operation"] = Schema(
-        description=(
-            "The operation that took place (1=Delete, 2=Insert, 3=Update (Before Image),"
-            "4=Update (After Image) )"
-        ),
-        type=["null", "integer"],
-        format="integer",
-    )
-
+    debug_lsn = config.get("debug_lsn")
+    if debug_lsn:
+        catalog_entry.schema.properties["_sdc_operation_type"] = Schema(
+            description="Source operation I=Insert, D=Delete, U=Update",
+            type=["null", "string"],
+            format="string",
+        )
+        catalog_entry.schema.properties["_sdc_lsn_commit_timestamp"] = Schema(
+            description="Source system commit timestamp", type=["null", "string"], format="date-time"
+        )
+        catalog_entry.schema.properties["_sdc_lsn_value"] = Schema(
+            description="Source system log sequence number (LSN)",
+            type=["null", "string"],
+            format="string",
+        )
+        catalog_entry.schema.properties["_sdc_lsn_seq_value"] = Schema(
+            description="Source sequence number within the system log sequence number (LSN)",
+            type=["null", "string"],
+            format="string",
+        )
+        catalog_entry.schema.properties["_sdc_lsn_operation"] = Schema(
+            description=(
+                "The operation that took place (1=Delete, 2=Insert, 3=Update (Before Image),"
+                "4=Update (After Image) )"
+            ),
+            type=["null", "integer"],
+            format="integer",
+        )
     return catalog_entry
 
 
 def generate_bookmark_keys(catalog_entry):
     # TO_DO:
     # 1. check the use of the top three values above and the parameter value, seem to not be required.
     # 2. check the base_bookmark_keys required
@@ -154,27 +155,29 @@
     bookmark_keys = base_bookmark_keys
 
     return bookmark_keys
 
 
 def sync_historic_table(mssql_conn, config, catalog_entry, state, columns, stream_version):
     mssql_conn = MSSQLConnection(config)
+    debug_lsn = config.get("debug_lsn")
     common.whitelist_bookmark_keys(
         generate_bookmark_keys(catalog_entry), catalog_entry.tap_stream_id, state
     )
 
     # Add additional keys to the columns
-    extended_columns = columns + [
-        "_sdc_operation_type",
-        "_sdc_lsn_commit_timestamp",
-        "_sdc_lsn_deleted_at",
-        "_sdc_lsn_value",
-        "_sdc_lsn_seq_value",
-        "_sdc_lsn_operation",
-    ]
+    extended_columns = columns + ["_sdc_deleted_at"]
+    if debug_lsn:
+        extended_columns = extended_columns + [
+            "_sdc_operation_type",
+            "_sdc_lsn_commit_timestamp",
+            "_sdc_lsn_value",
+            "_sdc_lsn_seq_value",
+            "_sdc_lsn_operation"
+        ]
 
     bookmark = state.get("bookmarks", {}).get(catalog_entry.tap_stream_id, {})
     version_exists = True if "version" in bookmark else False
 
     initial_full_table_complete = singer.get_bookmark(
         state, catalog_entry.tap_stream_id, "initial_full_table_complete"
     )
@@ -207,26 +210,31 @@
             verify_read_isolation_databases(mssql_conn)
 
             # Store the current database lsn number, will use this to store at the end of the initial load.
             # Note: Recommend no transactions loaded when the initial loads are performed.
             # Have captured the to_lsn before the initial load sync in-case records are added during the sync.
             lsn_to = str(get_to_lsn(mssql_conn)[0].hex())
 
-            select_sql = """
-                            SELECT {}
-                                ,'I' _sdc_operation_type
-                                , cast('1900-01-01' as datetime) _sdc_lsn_commit_timestamp
-                                , null _sdc_lsn_deleted_at
-                                , '00000000000000000000' _sdc_lsn_value
-                                , '00000000000000000000' _sdc_lsn_seq_value
-                                , 1 as _sdc_lsn_operation
-                            FROM {}.{}
-                            ;""".format(
-                ",".join(escaped_columns), schema_name, table_name
-            )
+            if debug_lsn:
+                select_sql = f"""
+                                SELECT {",".join(escaped_columns)}
+                                    ,'I' _sdc_operation_type
+                                    , cast('1900-01-01' as datetime) _sdc_lsn_commit_timestamp
+                                    , '00000000000000000000' _sdc_lsn_value
+                                    , '00000000000000000000' _sdc_lsn_seq_value
+                                    , 1 as _sdc_lsn_operation
+                                    , null _sdc_deleted_at
+                                FROM {schema_name}.{table_name}
+                                ;"""
+            else:
+                select_sql = f"""
+                                SELECT {",".join(escaped_columns)}
+                                    , null _sdc_deleted_at
+                                FROM {schema_name}.{table_name}
+                                ;"""
             params = {}
 
             common.sync_query(
                 cur,
                 catalog_entry,
                 state,
                 select_sql,
@@ -245,27 +253,29 @@
     singer.clear_bookmark(state, catalog_entry.tap_stream_id, "last_pk_fetched")
 
     singer.write_message(activate_version_message)
 
 
 def sync_table(mssql_conn, config, catalog_entry, state, columns, stream_version):
     mssql_conn = MSSQLConnection(config)
+    debug_lsn = config.get("debug_lsn")
     common.whitelist_bookmark_keys(
         generate_bookmark_keys(catalog_entry), catalog_entry.tap_stream_id, state
     )
 
     # Add additional keys to the columns
-    extended_columns = columns + [
-        "_sdc_operation_type",
-        "_sdc_lsn_commit_timestamp",
-        "_sdc_lsn_deleted_at",
-        "_sdc_lsn_value",
-        "_sdc_lsn_seq_value",
-        "_sdc_lsn_operation",
-    ]
+    extended_columns = columns + ["_sdc_deleted_at"]
+    if debug_lsn:
+        extended_columns = extended_columns + [
+            "_sdc_operation_type",
+            "_sdc_lsn_commit_timestamp",
+            "_sdc_lsn_value",
+            "_sdc_lsn_seq_value",
+            "_sdc_lsn_operation"
+        ]
 
     bookmark = state.get("bookmarks", {}).get(catalog_entry.tap_stream_id, {})
     version_exists = True if "version" in bookmark else False
 
     initial_full_table_complete = singer.get_bookmark(
         state, catalog_entry.tap_stream_id, "initial_full_table_complete"
     )
@@ -302,15 +312,15 @@
             lsn_range = get_lsn_available_range(mssql_conn, schema_table)
 
             if lsn_range[0] is not None:  # Test to see if there are any change records to process
                 lsn_from = str(lsn_range[0].hex())
                 lsn_to = str(lsn_range[1].hex())
 
                 if lsn_from <= state_last_lsn:
-                    LOGGER.info(
+                    LOGGER.debug(
                         (
                             "The last lsn processed as per the state file %s, minimum available lsn"
                             " for extract table %s, and the maximum lsn is %s."
                         ),
                         state_last_lsn,
                         lsn_from,
                         lsn_to,
@@ -319,42 +329,51 @@
                     raise Exception(
                         (
                             "Error {}.{}: CDC changes have expired, the minimum lsn is {}, the last"
                             " processed lsn is {}. Recommend a full load as there may be missing data."
                         ).format(schema_name, table_name, lsn_from, state_last_lsn)
                     )
 
-                select_sql = """DECLARE @from_lsn binary (10), @to_lsn binary (10)
+                if debug_lsn:
+                    select_sql = f"""DECLARE @from_lsn binary (10), @to_lsn binary (10)
 
-                                SET @from_lsn = sys.fn_cdc_increment_lsn({})
-                                SET @to_lsn = {}
-
-                                SELECT {}
-                                    ,case __$operation
-                                        when 2 then 'I'
-                                        when 4 then 'U'
-                                        when 1 then 'D'
-                                    end _sdc_operation_type
-                                    , sys.fn_cdc_map_lsn_to_time(__$start_lsn) _sdc_lsn_commit_timestamp
-                                    , case __$operation
-                                        when 1 then sys.fn_cdc_map_lsn_to_time(__$start_lsn)
-                                        else null
-                                        end _sdc_lsn_deleted_at
-                                    , __$start_lsn _sdc_lsn_value
-                                    , __$seqval _sdc_lsn_seq_value
-                                    , __$operation _sdc_lsn_operation
-                                FROM cdc.fn_cdc_get_all_changes_{}(@from_lsn, @to_lsn, 'all')
-                                ORDER BY __$start_lsn, __$seqval, __$operation
-                                ;""".format(
-                    py_bin_to_mssql(state_last_lsn),
-                    py_bin_to_mssql(lsn_to),
-                    ",".join(escaped_columns),
-                    schema_table,
-                )
+                                    SET @from_lsn = sys.fn_cdc_increment_lsn({py_bin_to_mssql(state_last_lsn)})
+                                    SET @to_lsn = {py_bin_to_mssql(lsn_to)}
 
+                                    SELECT {",".join(escaped_columns)}
+                                        ,case __$operation
+                                            when 2 then 'I'
+                                            when 4 then 'U'
+                                            when 1 then 'D'
+                                        end _sdc_operation_type
+                                        , sys.fn_cdc_map_lsn_to_time(__$start_lsn) _sdc_lsn_commit_timestamp
+                                        , __$start_lsn _sdc_lsn_value
+                                        , __$seqval _sdc_lsn_seq_value
+                                        , __$operation _sdc_lsn_operation
+                                        , case __$operation
+                                            when 1 then sys.fn_cdc_map_lsn_to_time(__$start_lsn)
+                                            else null
+                                        end _sdc_deleted_at
+                                    FROM cdc.fn_cdc_get_all_changes_{schema_table}(@from_lsn, @to_lsn, 'all')
+                                    ORDER BY __$start_lsn, __$seqval, __$operation
+                                    ;"""
+                else:
+                    select_sql = f"""DECLARE @from_lsn binary (10), @to_lsn binary (10)
+    
+                                    SET @from_lsn = sys.fn_cdc_increment_lsn({py_bin_to_mssql(state_last_lsn)})
+                                    SET @to_lsn = {py_bin_to_mssql(lsn_to)}
+    
+                                    SELECT {",".join(escaped_columns)}
+                                        , case __$operation
+                                            when 1 then sys.fn_cdc_map_lsn_to_time(__$start_lsn)
+                                            else null
+                                        end _sdc_deleted_at
+                                    FROM cdc.fn_cdc_get_all_changes_{schema_table}(@from_lsn, @to_lsn, 'all')
+                                    ORDER BY __$start_lsn, __$seqval, __$operation
+                                    ;"""
                 params = {}
 
                 common.sync_query(
                     cur,
                     catalog_entry,
                     state,
                     select_sql,
@@ -362,15 +381,15 @@
                     stream_version,
                     params,
                     config,
                 )
 
             else:
                 # Store the current database lsn number, need to store the latest lsn checkpoint because the
-                # CDC logs expire after a point in time. Therefore if there are no records read, then refresh
+                # CDC logs expire after a point in time. Therefore, if there are no records read, then refresh
                 # the max lsn_to to the latest LSN in the database.
                 lsn_to = str(get_to_lsn(mssql_conn)[0].hex())
 
             state = singer.write_bookmark(state, catalog_entry.tap_stream_id, "lsn", lsn_to)
             singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
     # clear max lsn value and last lsn fetched upon successful sync
```

### Comparing `macrometa-source-mssql-0.0.9/pyproject.toml` & `macrometa-source-mssql-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mssql"
-version='0.0.9'
+version='1.0.0'
 description = "Macrometa Source for extracting data from Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -25,18 +25,19 @@
     { include = "macrometa_source_mssql" },
     { include = "sync_strategies", from = "macrometa_source_mssql" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = ">=0.0.20"
+c8connector = ">=0.0.24"
 attrs = ">=16.3.0"
 pendulum = ">=1.2.0"
 pymssql = ">=2.2.1"
+prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-source-mssql = 'macrometa_source_mssql:main'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Macrometacorp/macrometa-source-mssql/issues"
```

### Comparing `macrometa-source-mssql-0.0.9/setup.py` & `macrometa-source-mssql-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,26 @@
  'sync_strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=16.3.0',
- 'c8connector>=0.0.20',
+ 'c8connector>=0.0.24',
  'pendulum>=1.2.0',
  'pipelinewise-singer-python==1.2.0',
+ 'prometheus-client==0.16.0',
  'pymssql>=2.2.1']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mssql = macrometa_source_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mssql',
-    'version': '0.0.9',
+    'version': '1.0.0',
     'description': 'Macrometa Source for extracting data from Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mssql-0.0.9/PKG-INFO` & `macrometa-source-mssql-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mssql
-Version: 0.0.9
+Version: 1.0.0
 Summary: Macrometa Source for extracting data from Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MSSQL,Microsoft SQL Server,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: attrs (>=16.3.0)
-Requires-Dist: c8connector (>=0.0.20)
+Requires-Dist: c8connector (>=0.0.24)
 Requires-Dist: pendulum (>=1.2.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
+Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: pymssql (>=2.2.1)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-mssql/issues
```

