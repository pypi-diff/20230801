# Comparing `tmp/macrometa-source-oracle-0.0.38.tar.gz` & `tmp/macrometa-source-oracle-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-oracle-0.0.38.tar", max compression
+gzip compressed data, was "macrometa-source-oracle-1.0.0.tar", max compression
```

## Comparing `macrometa-source-oracle-0.0.38.tar` & `macrometa-source-oracle-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     9713 2023-07-17 14:09:02.028172 macrometa-source-oracle-0.0.38/LICENSE
--rw-r--r--   0        0        0     1707 2023-07-17 14:09:02.028172 macrometa-source-oracle-0.0.38/README.md
--rw-r--r--   0        0        0    43914 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/__init__.py
--rwxr-xr-x   0        0        0     7524 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/connection.py
--rwxr-xr-x   0        0        0        0 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     4779 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/common.py
--rwxr-xr-x   0        0        0     4880 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/full_table.py
--rwxr-xr-x   0        0        0    17662 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1600 2023-07-17 14:09:02.128174 macrometa-source-oracle-0.0.38/pyproject.toml
--rw-r--r--   0        0        0     2777 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.38/setup.py
--rw-r--r--   0        0        0     2759 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.38/PKG-INFO
+-rwxr-xr-x   0        0        0     9713 2023-08-01 08:41:09.523691 macrometa-source-oracle-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1707 2023-08-01 08:41:09.523691 macrometa-source-oracle-1.0.0/README.md
+-rw-r--r--   0        0        0    43914 2023-08-01 08:41:09.523691 macrometa-source-oracle-1.0.0/macrometa_source_oracle/__init__.py
+-rwxr-xr-x   0        0        0     7524 2023-08-01 08:41:09.523691 macrometa-source-oracle-1.0.0/macrometa_source_oracle/connection.py
+-rwxr-xr-x   0        0        0        0 2023-08-01 08:41:09.523691 macrometa-source-oracle-1.0.0/macrometa_source_oracle/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     4779 2023-08-01 08:41:09.523691 macrometa-source-oracle-1.0.0/macrometa_source_oracle/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     4880 2023-08-01 08:41:09.523691 macrometa-source-oracle-1.0.0/macrometa_source_oracle/sync_strategies/full_table.py
+-rwxr-xr-x   0        0        0    17662 2023-08-01 08:41:09.523691 macrometa-source-oracle-1.0.0/macrometa_source_oracle/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1599 2023-08-01 08:41:09.599692 macrometa-source-oracle-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2776 1970-01-01 00:00:00.000000 macrometa-source-oracle-1.0.0/setup.py
+-rw-r--r--   0        0        0     2758 1970-01-01 00:00:00.000000 macrometa-source-oracle-1.0.0/PKG-INFO
```

### Comparing `macrometa-source-oracle-0.0.38/LICENSE` & `macrometa-source-oracle-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.38/README.md` & `macrometa-source-oracle-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.38/macrometa_source_oracle/__init__.py` & `macrometa-source-oracle-1.0.0/macrometa_source_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.38/macrometa_source_oracle/connection.py` & `macrometa-source-oracle-1.0.0/macrometa_source_oracle/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/common.py` & `macrometa-source-oracle-1.0.0/macrometa_source_oracle/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/full_table.py` & `macrometa-source-oracle-1.0.0/macrometa_source_oracle/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/log_based.py` & `macrometa-source-oracle-1.0.0/macrometa_source_oracle/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.38/pyproject.toml` & `macrometa-source-oracle-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-oracle"
-version='0.0.38'
+version='1.0.0'
 description = "Macrometa source oracle connector for reading from oracle databases."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 readme = "README.md"
 homepage = "https://www.macrometa.com/"
 keywords = [
     "ELT",
```

### Comparing `macrometa-source-oracle-0.0.38/setup.py` & `macrometa-source-oracle-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'strict-rfc3339>=0.7,<0.8']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-oracle = macrometa_source_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-oracle',
-    'version': '0.0.38',
+    'version': '1.0.0',
     'description': 'Macrometa source oracle connector for reading from oracle databases.',
     'long_description': '# macrometa-source-oracle\n\nMacrometa source connector that extracts data from a [Oracle](https://www.oracle.com/database/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).\n\n## How to use it\n\n### Install and Run\n\nFirst, make sure Python 3 is installed on your system or follow these\ninstallation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or\n[Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).\n\n\nIt\'s recommended to use a virtualenv:\n\n```bash\n  python3 -m venv venv\n  pip install macrometa-source-oracle\n```\n\nor from source using,\n1. Install poetry using https://python-poetry.org/docs/#installation\n2. Run \n    ```bash\n    poetry build\n    pip install dist/macrometa_source_oracle-<version>*.whl\n    ```\n\n### Configuration\n\nRunning the the macrometa source connector independently requires a `config.json` file. \n\nExample configuration:\n\n```json\n{\n  "host": "dev.oracledb.io",\n  "port": 1521,\n  "user": "C##HELLO",\n  "password": "password",\n  "service_name": "ORCLCDB",\n  "filter_schema": "C##HELLO",\n  "filter_table": "CUSTOMERS",\n  "replication_method": "LOG_BASED",\n  "pdb_name": "ORCLPDB1",\n  "multitenant": true,\n  "scn_window_size": 10\n}\n```\n\nYou can run a discover run using the previous `config.json` file to acquire all the tables definition\n \n```\nmacrometa-source-oracle --config /tmp/config.json --discover >> /tmp/catalog.json\n```\n\nThen use the catalog.json to run a full export:\n\n```\nmacrometa-source-oracle --config /tmp/config.json --catalog /tmp/catalog.json\n```\n\n',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.macrometa.com/',
```

### Comparing `macrometa-source-oracle-0.0.38/PKG-INFO` & `macrometa-source-oracle-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-oracle
-Version: 0.0.38
+Version: 1.0.0
 Summary: Macrometa source oracle connector for reading from oracle databases.
 Home-page: https://www.macrometa.com/
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Oracle,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
```

