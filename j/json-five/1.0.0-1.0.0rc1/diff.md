# Comparing `tmp/json-five-1.0.0.tar.gz` & `tmp/json-five-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-five-1.0.0.tar", last modified: Tue Aug  1 04:56:36 2023, max compression
+gzip compressed data, was "json-five-1.0.0rc1.tar", last modified: Tue Aug  1 04:50:10 2023, max compression
```

## Comparing `json-five-1.0.0.tar` & `json-five-1.0.0rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:56:36.631888 json-five-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 04:56:25.000000 json-five-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 04:56:25.000000 json-five-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-01 04:56:36.631888 json-five-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-01 04:56:25.000000 json-five-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:56:36.631888 json-five-1.0.0/json5/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-01 04:56:25.000000 json-five-1.0.0/json5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-08-01 04:56:25.000000 json-five-1.0.0/json5/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-08-01 04:56:25.000000 json-five-1.0.0/json5/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-08-01 04:56:25.000000 json-five-1.0.0/json5/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21269 2023-08-01 04:56:25.000000 json-five-1.0.0/json5/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:56:25.000000 json-five-1.0.0/json5/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-08-01 04:56:25.000000 json-five-1.0.0/json5/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-01 04:56:25.000000 json-five-1.0.0/json5/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:56:36.631888 json-five-1.0.0/json_five.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-01 04:56:36.000000 json-five-1.0.0/json_five.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 04:56:36.000000 json-five-1.0.0/json_five.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:56:36.000000 json-five-1.0.0/json_five.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 04:56:36.000000 json-five-1.0.0/json_five.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 04:56:36.000000 json-five-1.0.0/json_five.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-01 04:56:36.631888 json-five-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:56:25.000000 json-five-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:56:36.631888 json-five-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_json5_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_json5_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_json5_official_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_json_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_loads_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_model_loader_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_modelizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-01 04:56:25.000000 json-five-1.0.0/tests/test_roundtrip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/json5/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21269 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/json_five.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json5_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json5_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json5_official_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_loads_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_model_loader_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_modelizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_roundtrip.py
```

### Comparing `json-five-1.0.0/LICENSE` & `json-five-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/PKG-INFO` & `json-five-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-five
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: A JSON5 parser that, among other features, supports round-trip preservation of comments
 Home-page: https://github.com/spyoungtech/json-five
 Author: Spencer Phillip Young
 Author-email: spencer.young@spyoung.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `json-five-1.0.0/README.md` & `json-five-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/json5/dumper.py` & `json-five-1.0.0rc1/json5/dumper.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/json5/loader.py` & `json-five-1.0.0rc1/json5/loader.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/json5/model.py` & `json-five-1.0.0rc1/json5/model.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/json5/parser.py` & `json-five-1.0.0rc1/json5/parser.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/json5/tokenizer.py` & `json-five-1.0.0rc1/json5/tokenizer.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/json5/utils.py` & `json-five-1.0.0rc1/json5/utils.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/json_five.egg-info/PKG-INFO` & `json-five-1.0.0rc1/json_five.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-five
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: A JSON5 parser that, among other features, supports round-trip preservation of comments
 Home-page: https://github.com/spyoungtech/json-five
 Author: Spencer Phillip Young
 Author-email: spencer.young@spyoung.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `json-five-1.0.0/json_five.egg-info/SOURCES.txt` & `json-five-1.0.0rc1/json_five.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/setup.cfg` & `json-five-1.0.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json-five
-version = 1.0.0
+version = 1.0.0rc1
 url = https://github.com/spyoungtech/json-five
 license = Apache
 author = Spencer Phillip Young
 author_email = spencer.young@spyoung.com
 description = A JSON5 parser that, among other features, supports round-trip preservation of comments
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `json-five-1.0.0/tests/test_errors.py` & `json-five-1.0.0rc1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/tests/test_json5_dump.py` & `json-five-1.0.0rc1/tests/test_json5_dump.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/tests/test_json5_load.py` & `json-five-1.0.0rc1/tests/test_json5_load.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/tests/test_json5_official_tests.py` & `json-five-1.0.0rc1/tests/test_json5_official_tests.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/tests/test_json_helpers.py` & `json-five-1.0.0rc1/tests/test_json_helpers.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/tests/test_loads_options.py` & `json-five-1.0.0rc1/tests/test_loads_options.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/tests/test_model_loader_dumper.py` & `json-five-1.0.0rc1/tests/test_model_loader_dumper.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/tests/test_modelizer.py` & `json-five-1.0.0rc1/tests/test_modelizer.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/tests/test_regressions.py` & `json-five-1.0.0rc1/tests/test_regressions.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0/tests/test_roundtrip.py` & `json-five-1.0.0rc1/tests/test_roundtrip.py`

 * *Files identical despite different names*

