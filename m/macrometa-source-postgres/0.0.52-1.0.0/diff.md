# Comparing `tmp/macrometa-source-postgres-0.0.52.tar.gz` & `tmp/macrometa-source-postgres-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.52.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-1.0.0.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.52.tar` & `macrometa-source-postgres-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/LICENSE
--rw-r--r--   0        0        0    36495 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8690 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     9019 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    28173 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3698 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1541 2023-07-17 14:10:35.028486 macrometa-source-postgres-0.0.52/pyproject.toml
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.52/setup.py
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.52/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-08-01 08:32:13.298869 macrometa-source-postgres-1.0.0/LICENSE
+-rw-r--r--   0        0        0    36495 2023-08-01 08:32:13.298869 macrometa-source-postgres-1.0.0/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8690 2023-08-01 08:32:13.298869 macrometa-source-postgres-1.0.0/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-08-01 08:32:13.298869 macrometa-source-postgres-1.0.0/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-08-01 08:32:13.298869 macrometa-source-postgres-1.0.0/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-08-01 08:32:13.298869 macrometa-source-postgres-1.0.0/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     9019 2023-08-01 08:32:13.298869 macrometa-source-postgres-1.0.0/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    28173 2023-08-01 08:32:13.298869 macrometa-source-postgres-1.0.0/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3698 2023-08-01 08:32:13.298869 macrometa-source-postgres-1.0.0/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1540 2023-08-01 08:32:13.542872 macrometa-source-postgres-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 macrometa-source-postgres-1.0.0/setup.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 macrometa-source-postgres-1.0.0/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.52/LICENSE` & `macrometa-source-postgres-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.52/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-1.0.0/macrometa_source_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.52/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-1.0.0/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.52/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-1.0.0/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-1.0.0/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-1.0.0/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-1.0.0/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-1.0.0/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.52/pyproject.toml` & `macrometa-source-postgres-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.52'
+version='1.0.0'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-postgres-0.0.52/setup.py` & `macrometa-source-postgres-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.52',
+    'version': '1.0.0',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.52/PKG-INFO` & `macrometa-source-postgres-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.52
+Version: 1.0.0
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

