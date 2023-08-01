# Comparing `tmp/macrometa-source-mongo-0.0.47.tar.gz` & `tmp/macrometa-source-mongo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.47.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-1.0.0.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.47.tar` & `macrometa-source-mongo-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/LICENSE
--rw-r--r--   0        0        0    23259 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6577 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0      895 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     7252 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     7239 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1577 2023-07-17 10:18:35.690125 macrometa-source-mongo-0.0.47/pyproject.toml
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.47/setup.py
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.47/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-08-01 08:29:58.500559 macrometa-source-mongo-1.0.0/LICENSE
+-rw-r--r--   0        0        0    23259 2023-08-01 08:29:58.500559 macrometa-source-mongo-1.0.0/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6577 2023-08-01 08:29:58.500559 macrometa-source-mongo-1.0.0/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0      895 2023-08-01 08:29:58.500559 macrometa-source-mongo-1.0.0/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     7252 2023-08-01 08:29:58.500559 macrometa-source-mongo-1.0.0/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-08-01 08:29:58.500559 macrometa-source-mongo-1.0.0/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-08-01 08:29:58.500559 macrometa-source-mongo-1.0.0/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     7239 2023-08-01 08:29:58.500559 macrometa-source-mongo-1.0.0/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-08-01 08:29:58.500559 macrometa-source-mongo-1.0.0/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1576 2023-08-01 08:29:58.756559 macrometa-source-mongo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 macrometa-source-mongo-1.0.0/setup.py
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 macrometa-source-mongo-1.0.0/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.47/LICENSE` & `macrometa-source-mongo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.47/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-1.0.0/macrometa_source_mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.47/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-1.0.0/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.47/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-1.0.0/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.47/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-1.0.0/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-1.0.0/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-1.0.0/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-1.0.0/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-1.0.0/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.47/pyproject.toml` & `macrometa-source-mongo-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.47'
+version='1.0.0'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.47/setup.py` & `macrometa-source-mongo-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.47',
+    'version': '1.0.0',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.47/PKG-INFO` & `macrometa-source-mongo-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.47
+Version: 1.0.0
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

