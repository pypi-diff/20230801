# Comparing `tmp/macrometa-source-snowflake-0.0.9.tar.gz` & `tmp/macrometa-source-snowflake-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-snowflake-0.0.9.tar", last modified: Tue Mar 28 17:20:08 2023, max compression
+gzip compressed data, was "macrometa-source-snowflake-1.0.0.tar", last modified: Tue Aug  1 08:45:21 2023, max compression
```

## Comparing `macrometa-source-snowflake-0.0.9.tar` & `macrometa-source-snowflake-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:20:08.942757 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)    28479 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/full_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/incremental.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:21.181206 macrometa-source-snowflake-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-08-01 08:45:21.181206 macrometa-source-snowflake-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:21.177206 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)    32137 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:21.181206 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/sync_strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/sync_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/sync_strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/sync_strategies/full_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/sync_strategies/log_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/sync_strategies/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:21.181206 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-08-01 08:45:21.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-01 08:45:21.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:45:21.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 08:45:21.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-01 08:45:21.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 08:45:21.000000 macrometa-source-snowflake-1.0.0/macrometa_source_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:45:21.181206 macrometa-source-snowflake-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-01 08:45:05.000000 macrometa-source-snowflake-1.0.0/setup.py
```

### Comparing `macrometa-source-snowflake-0.0.9/LICENSE` & `macrometa-source-snowflake-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-snowflake-0.0.9/PKG-INFO` & `macrometa-source-snowflake-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,50 @@
 Metadata-Version: 2.1
 Name: macrometa-source-snowflake
-Version: 0.0.9
-Summary: Macrometa Source for extracting data from Macrometa
+Version: 1.0.0
+Summary: Macrometa Source for extracting data from Snowflake
 Home-page: https://github.com/Macrometacorp/macrometa-source-snowflake
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # macrometa-source-snowflake
 
-[![PyPI version](https://badge.fury.io/py/pipelinewise-tap-snowflake.svg)](https://badge.fury.io/py/pipelinewise-tap-snowflake)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pipelinewise-tap-snowflake.svg)](https://pypi.org/project/pipelinewise-tap-snowflake/)
-[![License: Apache2](https://img.shields.io/badge/License-Apache2-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
-
-[Singer](https://www.singer.io/) tap that extracts data from a [Snowflake](https://www.snowflake.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
+A macrometa source that extracts data from a [Snowflake](https://www.snowflake.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
 
 ## How to use it
 
 TODO: Add proper context
-
-If you want to run this [Singer Tap](https://singer.io) independently please read further.
+If you want to run this macrometa-source-snowflake connector independently please read further.
 
 ### Install and Run
 
 First, make sure Python 3 is installed on your system or follow these
 installation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or
 [Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).
-
 It's recommended to use a virtualenv:
 
 ```bash
 make venv
 ```
 
 ### Configuration
 
 1. Create a `config.json` file with connection details to snowflake, here is a [sample config file](./config_sample.json).
-
-**Note**: `tables` is a mandatory parameter as well to avoid a long-running catalog discovery process.
-Please specify fully qualified table and view names and only that ones that you need to extract otherwise you can
-end up with very long running discovery mode of this tap. Discovery mode is analysing table structures but
-Snowflake doesn't like selecting lot of rows from `INFORMATION_SCHEMA` or running `SHOW` commands that returns lot of
-rows. Please be as specific as possible.
-
+   **Note**: `table` is a mandatory parameter as well to avoid a long-running catalog discovery process.
+   Please specify fully qualified table and view names and only that ones that you need to extract otherwise you can
+   end up with very long running discovery mode of this source connector. Discovery mode is analysing table structures but
+   Snowflake doesn't like selecting lot of rows from `INFORMATION_SCHEMA` or running `SHOW` commands that returns lot of
+   rows. Please be as specific as possible.
 2. Run it in discovery mode to generate a `properties.json`
-
 3. Edit the `properties.json` and select the streams to replicate
-
-4. Run the tap like any other singer compatible tap:
+4. Run the source connector like any other singer compatible tap:
 
 ```
   macrometa-source-snowflake --config config.json --properties properties.json --state state.json
 ```
 
 ### Authentication Methods
 
@@ -62,67 +52,62 @@
 
 #### User / Password authentication
 
 Populate `user` and `password` in the `config.json` file
 
 #### Key Pair authentication
 
-To use key pair authentication, omit the `password` and instead provide the `private_key_path` to the unencrypted version of the private key and, optionally, the `private_key_passphrase`.
+To use key pair authentication, omit the `password` and instead provide the `private_key` to the unencrypted version of the private key and, optionally, the `private_key_passphrase`.
 
 ### Discovery mode
 
-The tap can be invoked in discovery mode to find the available tables and
-columns in the database:
+The macrometa-source-snowflake connector can be invoked in discovery mode to find the available table and columns in the database:
 
 ```bash
 $ macrometa-source-snowflake --config config.json --discover
-
 ```
 
 A discovered catalog is output, with a JSON-schema description of each table. A
 source table directly corresponds to a Singer stream.
 
 ## Replication methods
 
-The two ways to replicate a given table are `FULL_TABLE` and `INCREMENTAL`.
+The two ways to replicate a given table are `FULL_TABLE` and `LOG_BASED`.
 
 ### Full Table
 
-Full-table replication extracts all data from the source table each time the tap
+Full-table replication extracts all data from the source table each time the connector
 is invoked.
 
-### Incremental
+### LogBased
 
-Incremental replication works in conjunction with a state file to only extract
-new records each time the tap is invoked. This requires a replication key to be
-specified in the table's metadata as well.
+Macrometa source Snowflake connector can be used as a CDC (Change Data Capture) connector by specifying the Replication Method as LOG_BASED to capture any changes done at source and identify what records were inserted or updated or deleted, it will extract first all the records (i.e. FULL_TABLE) and then it will continuously listen to a Stream created on the Table to extract only the changes done.
 
 ### To run tests:
 
 1. Define environment variables that requires running the tests
 
 ```
   export MACROMETA_SOURCE_SNOWFLAKE_ACCOUNT=<snowflake-account-name>
   export MACROMETA_SOURCE_SNOWFLAKE_DBNAME=<snowflake-database-name>
   export MACROMETA_SOURCE_SNOWFLAKE_USER=<snowflake-user>
   export MACROMETA_SOURCE_SNOWFLAKE_PASSWORD=<snowflake-password>
-  export MACROMETA_SOURCE_SNOWFLAKE_PRIVATE_KEY_PATH=<snowflake-pk-path>
+  export MACROMETA_SOURCE_SNOWFLAKE_PRIVATE_KEY=<snowflake-pk-path>
   export MACROMETA_SOURCE_SNOWFLAKE_PRIVATE_KEY_PASSPHRASE=<snowflake-passphrase>
   export MACROMETA_SOURCE_SNOWFLAKE_WAREHOUSE=<snowflake-warehouse>
 ```
 
 2. Install python dependencies
 
 ```bash
 make venv
 ```
 
 3. To run unit tests:
-
-**PS**: There are no unit tests at the time of writing this document
+   **PS**: There are no unit tests at the time of writing this document
 
 ```bash
 make unit_test
 ```
 
 4. To run Integration tests
 
@@ -135,9 +120,8 @@
 ```bash
 make venv format pylint
 ```
 
 ## License
 
 Apache License Version 2.0
-
 See [LICENSE](LICENSE) to see the full text.
```

### Comparing `macrometa-source-snowflake-0.0.9/README.md` & `macrometa-source-snowflake-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 # macrometa-source-snowflake
 
-[![PyPI version](https://badge.fury.io/py/pipelinewise-tap-snowflake.svg)](https://badge.fury.io/py/pipelinewise-tap-snowflake)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pipelinewise-tap-snowflake.svg)](https://pypi.org/project/pipelinewise-tap-snowflake/)
-[![License: Apache2](https://img.shields.io/badge/License-Apache2-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
-
-[Singer](https://www.singer.io/) tap that extracts data from a [Snowflake](https://www.snowflake.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
+A macrometa source that extracts data from a [Snowflake](https://www.snowflake.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
 
 ## How to use it
 
 TODO: Add proper context
-
-If you want to run this [Singer Tap](https://singer.io) independently please read further.
+If you want to run this macrometa-source-snowflake connector independently please read further.
 
 ### Install and Run
 
 First, make sure Python 3 is installed on your system or follow these
 installation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or
 [Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).
-
 It's recommended to use a virtualenv:
 
 ```bash
 make venv
 ```
 
 ### Configuration
 
 1. Create a `config.json` file with connection details to snowflake, here is a [sample config file](./config_sample.json).
-
-**Note**: `tables` is a mandatory parameter as well to avoid a long-running catalog discovery process.
-Please specify fully qualified table and view names and only that ones that you need to extract otherwise you can
-end up with very long running discovery mode of this tap. Discovery mode is analysing table structures but
-Snowflake doesn't like selecting lot of rows from `INFORMATION_SCHEMA` or running `SHOW` commands that returns lot of
-rows. Please be as specific as possible.
-
+   **Note**: `table` is a mandatory parameter as well to avoid a long-running catalog discovery process.
+   Please specify fully qualified table and view names and only that ones that you need to extract otherwise you can
+   end up with very long running discovery mode of this source connector. Discovery mode is analysing table structures but
+   Snowflake doesn't like selecting lot of rows from `INFORMATION_SCHEMA` or running `SHOW` commands that returns lot of
+   rows. Please be as specific as possible.
 2. Run it in discovery mode to generate a `properties.json`
-
 3. Edit the `properties.json` and select the streams to replicate
-
-4. Run the tap like any other singer compatible tap:
+4. Run the source connector like any other singer compatible tap:
 
 ```
   macrometa-source-snowflake --config config.json --properties properties.json --state state.json
 ```
 
 ### Authentication Methods
 
@@ -50,67 +40,62 @@
 
 #### User / Password authentication
 
 Populate `user` and `password` in the `config.json` file
 
 #### Key Pair authentication
 
-To use key pair authentication, omit the `password` and instead provide the `private_key_path` to the unencrypted version of the private key and, optionally, the `private_key_passphrase`.
+To use key pair authentication, omit the `password` and instead provide the `private_key` to the unencrypted version of the private key and, optionally, the `private_key_passphrase`.
 
 ### Discovery mode
 
-The tap can be invoked in discovery mode to find the available tables and
-columns in the database:
+The macrometa-source-snowflake connector can be invoked in discovery mode to find the available table and columns in the database:
 
 ```bash
 $ macrometa-source-snowflake --config config.json --discover
-
 ```
 
 A discovered catalog is output, with a JSON-schema description of each table. A
 source table directly corresponds to a Singer stream.
 
 ## Replication methods
 
-The two ways to replicate a given table are `FULL_TABLE` and `INCREMENTAL`.
+The two ways to replicate a given table are `FULL_TABLE` and `LOG_BASED`.
 
 ### Full Table
 
-Full-table replication extracts all data from the source table each time the tap
+Full-table replication extracts all data from the source table each time the connector
 is invoked.
 
-### Incremental
+### LogBased
 
-Incremental replication works in conjunction with a state file to only extract
-new records each time the tap is invoked. This requires a replication key to be
-specified in the table's metadata as well.
+Macrometa source Snowflake connector can be used as a CDC (Change Data Capture) connector by specifying the Replication Method as LOG_BASED to capture any changes done at source and identify what records were inserted or updated or deleted, it will extract first all the records (i.e. FULL_TABLE) and then it will continuously listen to a Stream created on the Table to extract only the changes done.
 
 ### To run tests:
 
 1. Define environment variables that requires running the tests
 
 ```
   export MACROMETA_SOURCE_SNOWFLAKE_ACCOUNT=<snowflake-account-name>
   export MACROMETA_SOURCE_SNOWFLAKE_DBNAME=<snowflake-database-name>
   export MACROMETA_SOURCE_SNOWFLAKE_USER=<snowflake-user>
   export MACROMETA_SOURCE_SNOWFLAKE_PASSWORD=<snowflake-password>
-  export MACROMETA_SOURCE_SNOWFLAKE_PRIVATE_KEY_PATH=<snowflake-pk-path>
+  export MACROMETA_SOURCE_SNOWFLAKE_PRIVATE_KEY=<snowflake-pk-path>
   export MACROMETA_SOURCE_SNOWFLAKE_PRIVATE_KEY_PASSPHRASE=<snowflake-passphrase>
   export MACROMETA_SOURCE_SNOWFLAKE_WAREHOUSE=<snowflake-warehouse>
 ```
 
 2. Install python dependencies
 
 ```bash
 make venv
 ```
 
 3. To run unit tests:
-
-**PS**: There are no unit tests at the time of writing this document
+   **PS**: There are no unit tests at the time of writing this document
 
 ```bash
 make unit_test
 ```
 
 4. To run Integration tests
 
@@ -123,9 +108,8 @@
 ```bash
 make venv format pylint
 ```
 
 ## License
 
 Apache License Version 2.0
-
 See [LICENSE](LICENSE) to see the full text.
```

### Comparing `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/__init__.py` & `macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 #!/usr/bin/env python3
 # pylint: disable=missing-docstring,not-an-iterable,too-many-locals,too-many-arguments,too-many-branches,invalid-name,duplicate-code,too-many-statements
 
 import collections
 import copy
 import itertools
-import re
-import sys
 import logging
 import pkg_resources
+import os
 
 from c8connector import (
     C8Connector, ConfigProperty, Sample,
-    ConfigAttributeType, SchemaAttributeType, SchemaAttribute)
-
+    ConfigAttributeType, SchemaAttributeType, SchemaAttribute, ValidationException)
 from c8connector import Schema as C8Schema
 
 import singer
 import singer.metrics as metrics
 import singer.schema
-import snowflake.connector
 from singer import metadata
 from singer import utils
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema
 
-from macrometa_source_snowflake.sync_strategies.sample_data import fetch_samples
+from prometheus_client import CollectorRegistry, start_http_server, Counter
+from macrometa_source_snowflake.sync_strategies.sample_data import fetch_samples, modify_reserved_keys
 import macrometa_source_snowflake.sync_strategies.common as common
 import macrometa_source_snowflake.sync_strategies.full_table as full_table
-import macrometa_source_snowflake.sync_strategies.incremental as incremental
-from macrometa_source_snowflake.connection import SnowflakeConnection
+import macrometa_source_snowflake.sync_strategies.log_based as log_based
+from macrometa_source_snowflake.connection import SnowflakeConnection, create_private_key_file, delete_private_key_file
 
 LOGGER = singer.get_logger('macrometa_source_snowflake')
 
-# Max number of rows that a SHOW SCHEMAS|TABLES|COLUMNS can return.
-# If more than this number of rows returned then tap-snowflake will raise TooManyRecordsException
+# Max number of rows that a SHOW SCHEMAS|TABLE|COLUMNS can return.
+# If more than this number of rows returned then macrometa-source-snowflake will raise TooManyRecordsException
 SHOW_COMMAND_MAX_ROWS = 9999
 
 
 # Tone down snowflake connector logs noise
 logging.getLogger('snowflake.connector').setLevel(logging.WARNING)
 
 Column = collections.namedtuple('Column', [
@@ -51,27 +49,32 @@
     'numeric_scale'])
 
 REQUIRED_CONFIG_KEYS = [
     'account',
     'dbname',
     'user',
     'warehouse',
-    'tables'
+    'table'
 ]
 
 # Snowflake data types
 STRING_TYPES = set(['varchar', 'char', 'character', 'string', 'text'])
 NUMBER_TYPES = set(['number', 'decimal', 'numeric'])
 INTEGER_TYPES = set(['int', 'integer', 'bigint', 'smallint'])
 FLOAT_TYPES = set(['float', 'float4', 'float8', 'real',
                   'double', 'double precision'])
 DATETIME_TYPES = set(['datetime', 'timestamp', 'date',
                      'timestamp_ltz', 'timestamp_ntz', 'timestamp_tz'])
 BINARY_TYPE = set(['binary', 'varbinary'])
 
+region_label = os.getenv("GDN_FEDERATION", "NA")
+tenant_label = os.getenv("GDN_TENANT", "NA")
+fabric_label = os.getenv("GDN_FABRIC", "NA")
+workflow_label = os.getenv("WORKFLOW_UUID", "NA")
+
 
 def schema_for_column(c):
     '''Returns the Schema object for the given Column.'''
     data_type = c.data_type.lower()
 
     inclusion = 'available'
     result = Schema(inclusion=inclusion)
@@ -125,15 +128,15 @@
                                'sql-datatype',
                                c.data_type.lower())
 
     return metadata.to_list(mdata)
 
 
 def get_table_columns(snowflake_conn, tables):
-    """Get column definitions of a list of tables
+    """Get column definition of a table
 
        It's using SHOW commands instead of INFORMATION_SCHEMA views because information_schemas views are slow
        and can cause unexpected exception of:
             Information schema query returned too much data. Please repeat query with more selective predicates.
     """
     table_columns = []
     for table in tables:
@@ -177,85 +180,101 @@
         table_columns.extend(columns)
 
     return table_columns
 
 
 def discover_catalog(snowflake_conn, config):
     """Returns a Catalog describing the structure of the database."""
-    tables = config.get('tables').split(',')
-    sql_columns = get_table_columns(snowflake_conn, tables)
-
-    table_info = {}
-    columns = []
-    for sql_col in sql_columns:
-        catalog = sql_col['TABLE_CATALOG']
-        schema = sql_col['TABLE_SCHEMA']
-        table_name = sql_col['TABLE_NAME']
-
-        if catalog not in table_info:
-            table_info[catalog] = {}
-
-        if schema not in table_info[catalog]:
-            table_info[catalog][schema] = {}
-
-        table_info[catalog][schema][table_name] = {
-            'row_count': sql_col.get('ROW_COUNT'),
-            'is_view': sql_col.get('TABLE_TYPE') == 'VIEW'
-        }
-
-        columns.append(Column(
-            table_catalog=catalog,
-            table_schema=schema,
-            table_name=table_name,
-            column_name=sql_col['COLUMN_NAME'],
-            data_type=sql_col['DATA_TYPE'],
-            character_maximum_length=sql_col['CHARACTER_MAXIMUM_LENGTH'],
-            numeric_precision=sql_col['NUMERIC_PRECISION'],
-            numeric_scale=sql_col['NUMERIC_SCALE']
-        ))
-
-    entries = []
-    for (k, cols) in itertools.groupby(columns, lambda c: (c.table_catalog, c.table_schema, c.table_name)):
-        cols = list(cols)
-        (table_catalog, table_schema, table_name) = k
-        schema = Schema(type='object',
-                        properties={c.column_name: schema_for_column(c) for c in cols})
-        md = create_column_metadata(cols)
-        md_map = metadata.to_map(md)
-
-        md_map = metadata.write(md_map, (), 'database-name', table_catalog)
-        md_map = metadata.write(md_map, (), 'schema-name', table_schema)
-
-        if (
-                table_catalog in table_info and
-                table_schema in table_info[table_catalog] and
-                table_name in table_info[table_catalog][table_schema]
-        ):
-            # Row Count of views returns NULL - Transform it to not null integer by defaults to 0
-            row_count = table_info[table_catalog][table_schema][table_name].get(
-                'row_count', 0) or 0
-            is_view = table_info[table_catalog][table_schema][table_name]['is_view']
-
-            md_map = metadata.write(md_map, (), 'row-count', row_count)
-            md_map = metadata.write(md_map, (), 'is-view', is_view)
-
-            entry = CatalogEntry(
-                table=table_name,
-                stream=table_name,
-                metadata=metadata.to_list(md_map),
-                tap_stream_id=common.generate_tap_stream_id(
-                    table_catalog, table_schema, table_name),
-                schema=schema)
+    try:
+        table = [config.get('table')]
+        sql_columns = get_table_columns(snowflake_conn, table)
 
-            entries.append(entry)
+        table_info = {}
+        columns = []
+        for sql_col in sql_columns:
+            catalog = sql_col['TABLE_CATALOG']
+            schema = sql_col['TABLE_SCHEMA']
+            table_name = sql_col['TABLE_NAME']
+
+            if catalog not in table_info:
+                table_info[catalog] = {}
+
+            if schema not in table_info[catalog]:
+                table_info[catalog][schema] = {}
+
+            table_info[catalog][schema][table_name] = {
+                'row_count': sql_col.get('ROW_COUNT'),
+                'is_view': sql_col.get('TABLE_TYPE') == 'VIEW'
+            }
 
-    return Catalog(entries)
+            columns.append(Column(
+                table_catalog=catalog,
+                table_schema=schema,
+                table_name=table_name,
+                column_name=sql_col['COLUMN_NAME'],
+                data_type=sql_col['DATA_TYPE'],
+                character_maximum_length=sql_col['CHARACTER_MAXIMUM_LENGTH'],
+                numeric_precision=sql_col['NUMERIC_PRECISION'],
+                numeric_scale=sql_col['NUMERIC_SCALE']
+            ))
+
+        entries = []
+        for (k, cols) in itertools.groupby(columns, lambda c: (c.table_catalog, c.table_schema, c.table_name)):
+            cols = list(cols)
+            (table_catalog, table_schema, table_name) = k
+            schema = Schema(type='object',
+                            properties={c.column_name: schema_for_column(c) for c in cols})
+            md = create_column_metadata(cols)
+            md_map = metadata.to_map(md)
+
+            md_map = metadata.write(md_map, (), 'database-name', table_catalog)
+            md_map = metadata.write(md_map, (), 'schema-name', table_schema)
+
+            # Unique primary key provided by user
+            if config.get('primary_key') and any(column.column_name == config.get('primary_key') for column in cols):
+                md_map = metadata.write(
+                    md_map, (), 'table-key-properties', [config.get('primary_key')])
+
+            if (
+                    table_catalog in table_info and
+                    table_schema in table_info[table_catalog] and
+                    table_name in table_info[table_catalog][table_schema]
+            ):
+                # Row Count of views returns NULL - Transform it to not null integer by defaults to 0
+                row_count = table_info[table_catalog][table_schema][table_name].get(
+                    'row_count', 0) or 0
+                is_view = table_info[table_catalog][table_schema][table_name]['is_view']
+
+                md_map = metadata.write(md_map, (), 'row-count', row_count)
+                md_map = metadata.write(md_map, (), 'is-view', is_view)
+
+                entry = CatalogEntry(
+                    table=table_name,
+                    stream=table_name,
+                    metadata=metadata.to_list(md_map),
+                    tap_stream_id=common.generate_tap_stream_id(
+                        table_catalog, table_schema, table_name),
+                    schema=schema)
+
+                entries.append(entry)
+
+        return Catalog(entries)
+    except Exception as e:
+        raise ValidationException(e)
 
 
 def do_discover(snowflake_conn, config):
+    db = config['dbname']
+    db_exists_query = f"SHOW DATABASES LIKE '{db}'"
+    db_exists = snowflake_conn.query(
+            db_exists_query)
+    if not db_exists:
+        raise ValidationException(f'Database: {db} does not exist')
+    if config['replication_method'] not in ["FULL_TABLE", "LOG_BASED"]:
+        raise ValidationException('Invalid replication method provided. It should be either FULL_TABLE or LOG_BASED.')
     discover_catalog(snowflake_conn, config).dump()
 
 
 # pylint: disable=fixme
 # TODO: Maybe put in a singer-db-utils library.
 def desired_columns(selected, table_schema):
     """Return the set of column names we need to include in the SELECT.
@@ -338,19 +357,19 @@
         ))
 
     return result
 
 
 def get_streams(snowflake_conn, catalog, config, state):
     """Returns the Catalog of data we're going to sync for all SELECT-based
-    streams (i.e. INCREMENTAL and FULL_TABLE that require a historical
+    streams (i.e. FULL_TABLE that require a historical
     sync).
 
     Using the Catalog provided from the input file, this function will return a
-    Catalog representing exactly which tables and columns that will be emitted
+    Catalog representing exactly which table and columns that will be emitted
     by SELECT-based syncs. This is achieved by comparing the input Catalog to a
     freshly discovered Catalog to determine the resulting Catalog.
 
     The resulting Catalog will include the following any streams marked as
     "selected" that currently exist in the database. Columns marked as "selected"
     and those labled "automatic" (e.g. primary keys and replication keys) will be
     included. Streams will be prioritized in the following order:
@@ -393,50 +412,19 @@
     else:
         # prioritize streams that have not been processed
         streams_to_sync = ordered_streams
 
     return resolve_catalog(discovered, streams_to_sync)
 
 
-def write_schema_message(catalog_entry, bookmark_properties=None):
-    key_properties = common.get_key_properties(catalog_entry)
-
-    singer.write_message(singer.SchemaMessage(
-        stream=catalog_entry.stream,
-        schema=catalog_entry.schema.to_dict(),
-        key_properties=key_properties,
-        bookmark_properties=bookmark_properties
-    ))
-
-
-def do_sync_incremental(snowflake_conn, catalog_entry, state, columns, replication_method):
-    LOGGER.info('Stream %s is using incremental replication',
-                catalog_entry.stream)
-
-    md_map = metadata.to_map(catalog_entry.metadata)
-    replication_key = md_map.get((), {}).get('replication-key')
-
-    if not replication_key:
-        raise Exception(f'Cannot use INCREMENTAL replication for table ({catalog_entry.stream}) without a replication '
-                        f'key.')
-
-    write_schema_message(catalog_entry=catalog_entry,
-                         bookmark_properties=[replication_key])
-
-    incremental.sync_table(snowflake_conn, catalog_entry,
-                           state, columns, replication_method)
-
-    singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
-
-
 def do_sync_full_table(snowflake_conn, catalog_entry, state, columns, replication_method):
     LOGGER.info('Stream %s is using full table replication',
                 catalog_entry.stream)
 
-    write_schema_message(catalog_entry)
+    common.write_schema_message(catalog_entry)
 
     stream_version = common.get_stream_version(
         catalog_entry.tap_stream_id, state)
 
     full_table.sync_table(snowflake_conn, catalog_entry,
                           state, columns, stream_version, replication_method)
 
@@ -447,15 +435,27 @@
                                   catalog_entry.tap_stream_id,
                                   'initial_full_table_complete',
                                   True)
 
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
 
+def do_sync_log_based(snowflake_conn, catalog_entry, state, columns, replication_method):
+    LOGGER.info('Stream %s is using LogBased (CDC) replication', catalog_entry.stream)
+
+    common.write_schema_message(catalog_entry)
+
+    log_based.sync_table(snowflake_conn, catalog_entry, state,
+                   columns, replication_method)
+
+    singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
+
+
 def sync_streams(snowflake_conn, catalog, state, replication_method):
+
     for catalog_entry in catalog.streams:
         columns = list(catalog_entry.schema.properties.keys())
 
         if not columns:
             LOGGER.warning(
                 'There are no columns selected for stream %s, skipping it.', catalog_entry.stream)
             continue
@@ -469,59 +469,75 @@
         md_map = metadata.to_map(catalog_entry.metadata)
 
         replication_method = md_map.get((), {}).get(
             'replication-method', replication_method)
 
         database_name = common.get_database_name(catalog_entry)
         schema_name = common.get_schema_name(catalog_entry)
+        stream_name = catalog_entry.table
 
         with metrics.job_timer('sync_table') as timer:
             timer.tags['database'] = database_name
             timer.tags['table'] = catalog_entry.table
 
             LOGGER.info('Beginning to sync %s.%s.%s', database_name,
                         schema_name, catalog_entry.table)
 
-            if replication_method == 'INCREMENTAL':
-                do_sync_incremental(
-                    snowflake_conn, catalog_entry, state, columns, replication_method)
-            elif replication_method == 'FULL_TABLE':
+            if replication_method == 'FULL_TABLE':
                 do_sync_full_table(
                     snowflake_conn, catalog_entry, state, columns, replication_method)
+            elif replication_method == 'LOG_BASED':
+                do_sync_log_based(
+                    snowflake_conn, catalog_entry, state, columns, replication_method)
             else:
                 raise Exception(
-                    'Only INCREMENTAL and FULL TABLE replication methods are supported')
+                    'Only FULL TABLE, and LOG_BASED replication methods are supported')
 
     state = singer.set_currently_syncing(state, None)
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
 
 def do_sync(snowflake_conn, config, catalog, state, replication_method):
     catalog = get_streams(snowflake_conn, catalog, config, state)
     sync_streams(snowflake_conn, catalog, state, replication_method)
 
 
 def main_impl():
-    args = utils.parse_args(REQUIRED_CONFIG_KEYS)
+    # Create a custom CollectorRegistry
+    registry_package = CollectorRegistry()
+    ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
+                        ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
+    LOGGER.info("Snowflake source is starting the metrics server.")
+    start_http_server(8000, registry=registry_package)
 
-    snowflake_conn = SnowflakeConnection(args.config)
-    replication_method = args.config.get('replication_method')
-    if args.discover:
-        do_discover(snowflake_conn, args.config)
-    elif args.catalog:
-        state = args.state or {}
-        do_sync(snowflake_conn, args.config,
-                args.catalog, state, replication_method)
-    elif args.properties:
-        catalog = Catalog.from_dict(args.properties)
-        state = args.state or {}
-        do_sync(snowflake_conn, args.config,
-                catalog, state, replication_method)
-    else:
-        LOGGER.info('No properties were selected')
+    args = utils.parse_args(REQUIRED_CONFIG_KEYS)
+    config = args.config
+    snowflake_conn = SnowflakeConnection(config)
+    replication_method = config.get('replication_method', 'FULL_TABLE')
+    try:
+        config = create_private_key_file(config)
+        if args.discover:
+            do_discover(snowflake_conn, config)
+        elif args.catalog:
+            state = args.state or {}
+            do_sync(snowflake_conn, config,
+                    args.catalog, state, replication_method)
+        elif args.properties:
+            catalog = Catalog.from_dict(args.properties)
+            state = args.state or {}
+            do_sync(snowflake_conn, config,
+                    catalog, state, replication_method)
+        else:
+            LOGGER.info('No properties were selected')
+    except Exception as e:
+        LOGGER.warn('Exception raised: %s', e)
+        ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+        delete_private_key_file(config)
+        raise e
+    delete_private_key_file(config)
 
 
 class SnowflakeSourceConnector(C8Connector):
     """SnowflakeSourceConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
@@ -548,74 +564,102 @@
         return ""
 
     def validate(self, integration: dict) -> None:
         """Validate given configurations against the connector.
         If invalid, throw an exception with the cause.
         """
         config = self.get_config(integration)
-        snowflake_conn = SnowflakeConnection(config)
         try:
+            config = create_private_key_file(config)
+            snowflake_conn = SnowflakeConnection(config)
             do_discover(snowflake_conn, config)
         except Exception as e:
+            LOGGER.warn('Exception raised: %s', e)
+            delete_private_key_file(config)
             raise e
+        delete_private_key_file(config)
 
-    # TODO: Need to add handling of reserved keys
     def samples(self, integration: dict) -> list[Sample]:
         """Fetch sample data using the provided configurations."""
         config = self.get_config(integration)
         try:
+            config = create_private_key_file(config)
             snowflake_conn = SnowflakeConnection(config)
-            LOGGER.info('DEBUG SAMPLE 1: %s', config)
-            catalog = do_discover(snowflake_conn, config)
-            LOGGER.info('DEBUG SAMPLE 2: %s', catalog)
+            catalog = discover_catalog(snowflake_conn, config)
             results = []
-            
+
             for stream in catalog.streams:
                 s_attribs = []
                 s_schema = stream.schema
-                LOGGER.info('DEBUG SAMPLE 3: %s', s_schema)
                 data = fetch_samples(config, stream)[:10]
-                LOGGER.info('DEBUG SAMPLE 4: %s', data)
+
+                # Appending _ to keys for preserving values of reserved keys in source data
+                reserved_keys = ['_key', '_id', '_rev']
+                metadata_obj = stream.metadata[0]
+                if metadata_obj['metadata'].get('table-key-properties'):
+                    key_properties = metadata_obj['metadata'].get(
+                        'table-key-properties')
+                    if key_properties[0] == '_key':
+                        reserved_keys.remove('_key')
+                properties = s_schema.properties
+                modified_properties = modify_reserved_keys(
+                    properties, reserved_keys)
+                s_schema.properties = modified_properties
+
                 for k, v in s_schema.properties.items():
-                    t = v['type'][-1]
+                    t = v.type[-1]
                     s_attribs.append(SchemaAttribute(
                         k, self.get_attribute_type(t)))
                 schema = C8Schema(stream.stream, s_attribs)
-                LOGGER.info('DEBUG SAMPLE 5: %s', schema)
-                LOGGER.info('DEBUG SAMPLE 6: %s', s_attribs)
                 results.append(Sample(
                     schema=schema,
                     data=data)
                 )
         except Exception as e:
+            LOGGER.warn('Exception raised: %s', e)
+            delete_private_key_file(config)
             raise e
+        delete_private_key_file(config)
         return results
 
-    # TODO: Need to add handling of reserved keys
     def schemas(self, integration: dict) -> list[C8Schema]:
         """Get supported schemas using the given configurations."""
         config = self.get_config(integration)
         try:
+            config = create_private_key_file(config)
             snowflake_conn = SnowflakeConnection(config)
-            LOGGER.info('DEBUG 1: %s', config)
-            catalog = do_discover(snowflake_conn, config)
-            LOGGER.info('DEBUG 2: %s', catalog)
+            catalog = discover_catalog(snowflake_conn, config)
             results = []
             for stream in catalog.streams:
                 s_attribs = []
                 s_schema = stream.schema
-                LOGGER.info('DEBUG 3: %s', s_schema)
+
+                # Appending _ to keys for preserving values of reserved keys in source data
+                reserved_keys = ['_key', '_id', '_rev']
+                metadata_obj = stream.metadata[0]
+                if metadata_obj['metadata'].get('table-key-properties'):
+                    key_properties = metadata_obj['metadata'].get(
+                        'table-key-properties')
+                    if key_properties[0] == '_key':
+                        reserved_keys.remove('_key')
+                properties = s_schema.properties
+                modified_properties = modify_reserved_keys(
+                    properties, reserved_keys)
+                s_schema.properties = modified_properties
+
                 for k, v in s_schema.properties.items():
-                    t = v['type'][-1]
+                    t = v.type[-1]
                     s_attribs.append(SchemaAttribute(
                         k, self.get_attribute_type(t)))
-                LOGGER.info('DEBUG 4: %s', s_attribs)
                 results.append(C8Schema(stream.stream, s_attribs))
         except Exception as e:
+            LOGGER.warn('Exception raised: %s', e)
+            delete_private_key_file(config)
             raise e
+        delete_private_key_file(config)
         return results
 
     def reserved_keys(self) -> list[str]:
         """List of reserved keys for the connector."""
         return []
 
     @staticmethod
@@ -630,48 +674,56 @@
             return SchemaAttributeType.DOUBLE
         else:
             return SchemaAttributeType.OBJECT
 
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
-            ConfigProperty('account', 'Account', ConfigAttributeType.STRING, True, False,
-                           description='Snowflake account',
-                           placeholder_value='snowflake_account'),
+            ConfigProperty('account', 'Account ID', ConfigAttributeType.STRING, True, False,
+                           description='Snowflake account identifier. Refer here for more info: '
+                                       'https://docs.snowflake.com/en/user-guide/admin-account-identifier.',
+                           placeholder_value='my_org-my_account'),
             ConfigProperty('dbname', 'Database Name', ConfigAttributeType.STRING, True, False,
-                           description='Snowflake database name',
-                           placeholder_value='snowflake'),
+                           description='Snowflake database name (Case-sensitive).',
+                           placeholder_value='SNOWFLAKE'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
-                           description='Snowflake user',
-                           placeholder_value='user'),
-            ConfigProperty('password', 'Password', ConfigAttributeType.STRING, True, False,
-                           description='Snowflake password',
-                           placeholder_value='password'),
-            ConfigProperty('warehouse', 'Warehouse', ConfigAttributeType.STRING, True, False,
-                           description='Snowflake virtual warehouse name',
-                           placeholder_value='my_schema'),
-            ConfigProperty('tables', 'Tables', ConfigAttributeType.STRING, True, False,
-                           description='A comma separated list of the table names that you want to sync. The table names should be fully qualified including the db and schema name. For example, syncing table1 and table2 would look like `db.schema.table1,db.schema.table2`',
-                           placeholder_value='my_table'),
+                           description='Snowflake username.',
+                           placeholder_value='my_user'),
+            ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, False, False,
+                           description='Snowflake password. It is required when using user/pass authentication and '
+                                       'not using Key/Pair (Private Key) authentication.',
+                           placeholder_value='my_password'),
+            ConfigProperty('warehouse', 'Warehouse', ConfigAttributeType.STRING, True, True,
+                           description='Snowflake virtual warehouse name.',
+                           placeholder_value='my_warehouse'),
+            ConfigProperty('table', 'Table', ConfigAttributeType.STRING, True, True,
+                           description='Name of the table that you want to sync.'
+                                       ' The table name should be fully qualified including the db and schema name.',
+                           placeholder_value='my_db.my_schema.my_table'),
             ConfigProperty('replication_method', 'Replication Method',
                            ConfigAttributeType.STRING, True, False,
-                           description='Choose from INCREMENTAL, FULL_TABLE',
+                           description='Choose from FULL_TABLE, LOG_BASED.',
                            default_value='FULL_TABLE'),
+            ConfigProperty('primary_key', 'Unique Primary Key (to be used as _key for the collection)', ConfigAttributeType.STRING, False, True,
+                           description='A unique primary key from the snowflake table which needs be used as _key for the collection.'
+                                       ' If the columns does not have any column with unique values then do not specify anything here,'
+                                       ' _key for the collection will be autogenerated in this case. Primary key is case sensitive.',
+                           placeholder_value='my_primary_key'),
             ConfigProperty('role', 'Role',
                            ConfigAttributeType.STRING, False, False,
-                           description='Snowflake role to use',
+                           description='Snowflake role to use.',
                            placeholder_value='my_role'),
-            ConfigProperty('private_key_path', 'Private Key Path', ConfigAttributeType.STRING, False, False,
-                           description='A path to your private key used for authenticating using Key Pair authentication instead of user/pass',
-                           placeholder_value='private_key_path'),
-            ConfigProperty('private_key_passphrase', 'Private Key Passphrase', ConfigAttributeType.STRING, False, False,
-                           description='The private key passphrase used for authenticating using Key Pair authentication instead of user/pass',
-                           placeholder_value='private_key_passphrase'),
+            ConfigProperty('private_key', 'Private Key', ConfigAttributeType.FILE, False, False,
+                           description='Private key used for authentication using Key Pair authentication instead of user/pass. At the moment, only PEM format is supported.',
+                           placeholder_value='my_private_key'),
+            ConfigProperty('private_key_passphrase', 'Private Key Passphrase', ConfigAttributeType.PASSWORD, False, False,
+                           description='The private key passphrase used for authenticating using Key Pair authentication instead of user/pass.',
+                           placeholder_value='my_private_key_passphrase'),
             ConfigProperty('insecure_mode', 'Insecure Mode', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Use insecure mode to avoid "Failed to get OCSP response" warnings',
+                           description='Use insecure mode to avoid "Failed to get OCSP response" warnings.',
                            default_value=False)
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
@@ -681,29 +733,27 @@
     def get_config(integration: dict) -> dict:
         try:
             return {
                 # Required config keys
                 'account': integration['account'],
                 'dbname': integration['dbname'],
                 'user': integration['user'],
-                'password': integration['password'],
                 'warehouse': integration['warehouse'],
-                'tables': integration['tables'],
+                'table': integration['table'],
                 # Optional config keys
-
-                # TODO: Check if this is necessery
-                'tap_id': integration.get('tap_id'),
-
+                'replication_method': integration.get('replication_method', 'FULL_TABLE'),
+                'primary_key': integration.get('primary_key'),
                 'role': integration.get('role'),
-                'private_key_path': integration.get('private_key_path'),
+                'password': integration.get('password'),
+                'private_key': integration.get('private_key'),
                 'private_key_passphrase': integration.get('private_key_passphrase'),
                 'insecure_mode': integration.get('insecure_mode', False),
             }
         except KeyError as e:
-            raise KeyError(f'Integration property `{e}` not found.')
+            raise ValidationException(f'Integration property `{e}` not found.')
 
 
 def main():
     try:
         main_impl()
     except Exception as exc:
         LOGGER.critical(exc)
```

### Comparing `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/full_table.py` & `macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/sync_strategies/full_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # pylint: disable=duplicate-code,too-many-locals,simplifiable-if-expression
 
 import singer
 import macrometa_source_snowflake.sync_strategies.common as common
 
-LOGGER = singer.get_logger('macrometa_source_snowflake_snowflake')
+LOGGER = singer.get_logger('macrometa_source_snowflake')
 
 BOOKMARK_KEYS = {'last_pk_fetched', 'max_pk_values',
                  'version', 'initial_full_table_complete'}
 
 
 def get_max_pk_values(cursor, catalog_entry):
     """Get actual max primary key values from database"""
```

### Comparing `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/sample_data.py` & `macrometa-source-snowflake-1.0.0/macrometa_source_snowflake/sync_strategies/sample_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from singer import metadata
 
 from macrometa_source_snowflake.connection import SnowflakeConnection
-
 import macrometa_source_snowflake.sync_strategies.common as common
 
 
-# pylint: disable=invalid-name,missing-function-docstring,too-many-locals,duplicate-code
-def fetch_view(conn_config, catalog_entry, columns):
-    samples = []
-    snowflake_conn = SnowflakeConnection(conn_config)
-    with snowflake_conn.connect_with_backoff() as open_conn:
-        with open_conn.cursor() as cur:
-            select_sql = common.generate_select_sql(catalog_entry, columns)
-            cur.execute(select_sql)
-            count = 0
-            for rec in cur:
-                rec_msg = common.row_to_singer_record(catalog_entry, None, rec, columns, None)
-                samples.append(rec_msg.record)
-                count += 1
-                if count >= 10:
-                    break
-    return samples
-
-# pylint: disable=too-many-statements,duplicate-code
 def fetch_table(conn_config, catalog_entry, columns):
     samples = []
     snowflake_conn = SnowflakeConnection(conn_config)
     with snowflake_conn.connect_with_backoff() as open_conn:
         with open_conn.cursor() as cur:
             select_sql = common.generate_select_sql(catalog_entry, columns)
-            select_sql += "LIMIT 10"
+            select_sql += " LIMIT 10"
             cur.execute(select_sql)
             for rec in cur:
                 rec_msg = common.row_to_singer_record(catalog_entry, None, rec, columns, None)
                 samples.append(rec_msg.record)
     return samples
 
 def fetch_samples(conn_config, catalog_entry):
     """
     Fetch samples for the stream.
     """
     md_map = metadata.to_map(catalog_entry.metadata)
     conn_config['dbname'] = md_map.get(()).get('database-name')
-    columns = [c for c in catalog_entry.schema.properties.keys() if common.property_is_selected(md_map, c)]
+    columns = [c for c in catalog_entry.schema.properties.keys() if common.property_is_selected(catalog_entry, c)]
     columns.sort()
-    if len(columns) == 0:
+    if not columns:
         # There are no columns selected for stream. So, skipping it.
         return []
-    if md_map.get((), {}).get('is-view'):
-        state = fetch_view(conn_config, catalog_entry, columns)
-    else:
-        state = fetch_table(conn_config, catalog_entry, columns)
+    state = fetch_table(conn_config, catalog_entry, columns)
+
+    # Appending _ to keys for preserving values of reserved keys in source data
+    reserved_keys = ['_key', '_id', '_rev']
+    if md_map.get((), {}).get('table-key-properties'):
+        key_properties = md_map.get((), {}).get('table-key-properties')
+        if key_properties[0] == '_key':
+                reserved_keys.remove('_key')
+    if any(key in set(columns) for key in reserved_keys):
+        for record in state:
+            record = modify_reserved_keys(record, reserved_keys)
     return state
+
+def modify_reserved_keys(record, reserved_keys):
+    for reserved_key in reserved_keys:
+        if record.get(reserved_key):
+            new_key = f"_{reserved_key}"
+            while True:
+                if record.get(new_key):
+                    new_key = f"_{new_key}"
+                else:
+                    break
+            record[new_key] = record.pop(reserved_key)
+    return record
```

### Comparing `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/PKG-INFO` & `macrometa-source-snowflake-1.0.0/macrometa_source_snowflake.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,50 @@
 Metadata-Version: 2.1
 Name: macrometa-source-snowflake
-Version: 0.0.9
-Summary: Macrometa Source for extracting data from Macrometa
+Version: 1.0.0
+Summary: Macrometa Source for extracting data from Snowflake
 Home-page: https://github.com/Macrometacorp/macrometa-source-snowflake
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # macrometa-source-snowflake
 
-[![PyPI version](https://badge.fury.io/py/pipelinewise-tap-snowflake.svg)](https://badge.fury.io/py/pipelinewise-tap-snowflake)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pipelinewise-tap-snowflake.svg)](https://pypi.org/project/pipelinewise-tap-snowflake/)
-[![License: Apache2](https://img.shields.io/badge/License-Apache2-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
-
-[Singer](https://www.singer.io/) tap that extracts data from a [Snowflake](https://www.snowflake.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
+A macrometa source that extracts data from a [Snowflake](https://www.snowflake.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
 
 ## How to use it
 
 TODO: Add proper context
-
-If you want to run this [Singer Tap](https://singer.io) independently please read further.
+If you want to run this macrometa-source-snowflake connector independently please read further.
 
 ### Install and Run
 
 First, make sure Python 3 is installed on your system or follow these
 installation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or
 [Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).
-
 It's recommended to use a virtualenv:
 
 ```bash
 make venv
 ```
 
 ### Configuration
 
 1. Create a `config.json` file with connection details to snowflake, here is a [sample config file](./config_sample.json).
-
-**Note**: `tables` is a mandatory parameter as well to avoid a long-running catalog discovery process.
-Please specify fully qualified table and view names and only that ones that you need to extract otherwise you can
-end up with very long running discovery mode of this tap. Discovery mode is analysing table structures but
-Snowflake doesn't like selecting lot of rows from `INFORMATION_SCHEMA` or running `SHOW` commands that returns lot of
-rows. Please be as specific as possible.
-
+   **Note**: `table` is a mandatory parameter as well to avoid a long-running catalog discovery process.
+   Please specify fully qualified table and view names and only that ones that you need to extract otherwise you can
+   end up with very long running discovery mode of this source connector. Discovery mode is analysing table structures but
+   Snowflake doesn't like selecting lot of rows from `INFORMATION_SCHEMA` or running `SHOW` commands that returns lot of
+   rows. Please be as specific as possible.
 2. Run it in discovery mode to generate a `properties.json`
-
 3. Edit the `properties.json` and select the streams to replicate
-
-4. Run the tap like any other singer compatible tap:
+4. Run the source connector like any other singer compatible tap:
 
 ```
   macrometa-source-snowflake --config config.json --properties properties.json --state state.json
 ```
 
 ### Authentication Methods
 
@@ -62,67 +52,62 @@
 
 #### User / Password authentication
 
 Populate `user` and `password` in the `config.json` file
 
 #### Key Pair authentication
 
-To use key pair authentication, omit the `password` and instead provide the `private_key_path` to the unencrypted version of the private key and, optionally, the `private_key_passphrase`.
+To use key pair authentication, omit the `password` and instead provide the `private_key` to the unencrypted version of the private key and, optionally, the `private_key_passphrase`.
 
 ### Discovery mode
 
-The tap can be invoked in discovery mode to find the available tables and
-columns in the database:
+The macrometa-source-snowflake connector can be invoked in discovery mode to find the available table and columns in the database:
 
 ```bash
 $ macrometa-source-snowflake --config config.json --discover
-
 ```
 
 A discovered catalog is output, with a JSON-schema description of each table. A
 source table directly corresponds to a Singer stream.
 
 ## Replication methods
 
-The two ways to replicate a given table are `FULL_TABLE` and `INCREMENTAL`.
+The two ways to replicate a given table are `FULL_TABLE` and `LOG_BASED`.
 
 ### Full Table
 
-Full-table replication extracts all data from the source table each time the tap
+Full-table replication extracts all data from the source table each time the connector
 is invoked.
 
-### Incremental
+### LogBased
 
-Incremental replication works in conjunction with a state file to only extract
-new records each time the tap is invoked. This requires a replication key to be
-specified in the table's metadata as well.
+Macrometa source Snowflake connector can be used as a CDC (Change Data Capture) connector by specifying the Replication Method as LOG_BASED to capture any changes done at source and identify what records were inserted or updated or deleted, it will extract first all the records (i.e. FULL_TABLE) and then it will continuously listen to a Stream created on the Table to extract only the changes done.
 
 ### To run tests:
 
 1. Define environment variables that requires running the tests
 
 ```
   export MACROMETA_SOURCE_SNOWFLAKE_ACCOUNT=<snowflake-account-name>
   export MACROMETA_SOURCE_SNOWFLAKE_DBNAME=<snowflake-database-name>
   export MACROMETA_SOURCE_SNOWFLAKE_USER=<snowflake-user>
   export MACROMETA_SOURCE_SNOWFLAKE_PASSWORD=<snowflake-password>
-  export MACROMETA_SOURCE_SNOWFLAKE_PRIVATE_KEY_PATH=<snowflake-pk-path>
+  export MACROMETA_SOURCE_SNOWFLAKE_PRIVATE_KEY=<snowflake-pk-path>
   export MACROMETA_SOURCE_SNOWFLAKE_PRIVATE_KEY_PASSPHRASE=<snowflake-passphrase>
   export MACROMETA_SOURCE_SNOWFLAKE_WAREHOUSE=<snowflake-warehouse>
 ```
 
 2. Install python dependencies
 
 ```bash
 make venv
 ```
 
 3. To run unit tests:
-
-**PS**: There are no unit tests at the time of writing this document
+   **PS**: There are no unit tests at the time of writing this document
 
 ```bash
 make unit_test
 ```
 
 4. To run Integration tests
 
@@ -135,9 +120,8 @@
 ```bash
 make venv format pylint
 ```
 
 ## License
 
 Apache License Version 2.0
-
 See [LICENSE](LICENSE) to see the full text.
```

### Comparing `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/SOURCES.txt` & `macrometa-source-snowflake-1.0.0/macrometa_source_snowflake.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 macrometa_source_snowflake.egg-info/dependency_links.txt
 macrometa_source_snowflake.egg-info/entry_points.txt
 macrometa_source_snowflake.egg-info/requires.txt
 macrometa_source_snowflake.egg-info/top_level.txt
 macrometa_source_snowflake/sync_strategies/__init__.py
 macrometa_source_snowflake/sync_strategies/common.py
 macrometa_source_snowflake/sync_strategies/full_table.py
-macrometa_source_snowflake/sync_strategies/incremental.py
+macrometa_source_snowflake/sync_strategies/log_based.py
 macrometa_source_snowflake/sync_strategies/sample_data.py
```

### Comparing `macrometa-source-snowflake-0.0.9/setup.py` & `macrometa-source-snowflake-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='macrometa-source-snowflake',
-      version='0.0.9',
-      description='Macrometa Source for extracting data from Macrometa',
+      version='1.0.0',
+      description='Macrometa Source for extracting data from Snowflake',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-source-snowflake',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
           'Programming Language :: Python :: 3 :: Only'
       ],
       py_modules=['macrometa_source_snowflake'],
       install_requires=[
           'pipelinewise-singer-python==1.2.0',
           'snowflake-connector-python[pandas]==2.7.*',
           'pendulum==1.2.0',
-          'c8connector==0.0.15'
+          'c8connector>=0.0.24',
+          'prometheus-client==0.16.0'
       ],
       extras_require={
           'test': [
               'pylint==2.12.*',
               'pytest==7.0.1',
               'pytest-cov==4.0.0',
               'unify==0.5'
```

