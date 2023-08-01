# Comparing `tmp/py-partiql-parser-0.3.6.tar.gz` & `tmp/py-partiql-parser-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.3.6.tar", last modified: Sun Jul 30 11:58:01 2023, max compression
+gzip compressed data, was "py-partiql-parser-0.3.7.tar", last modified: Tue Aug  1 17:59:39 2023, max compression
```

## Comparing `py-partiql-parser-0.3.6.tar` & `py-partiql-parser-0.3.7.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:58:01.452626 py-partiql-parser-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-30 11:58:01.452626 py-partiql-parser-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:58:01.448626 py-partiql-parser-0.3.6/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:58:01.452626 py-partiql-parser-0.3.6/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/case_insensitive_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:58:01.448626 py-partiql-parser-0.3.6/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-30 11:58:01.000000 py-partiql-parser-0.3.6/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-30 11:58:01.000000 py-partiql-parser-0.3.6/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:58:01.000000 py-partiql-parser-0.3.6/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-30 11:58:01.000000 py-partiql-parser-0.3.6/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 11:58:01.000000 py-partiql-parser-0.3.6/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 11:57:53.000000 py-partiql-parser-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 11:58:01.456627 py-partiql-parser-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:58:01.452626 py-partiql-parser-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_dynamodb_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_query_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_s3_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-30 11:57:41.000000 py-partiql-parser-0.3.6/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:59:39.627520 py-partiql-parser-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 17:59:39.627520 py-partiql-parser-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:59:39.623520 py-partiql-parser-0.3.7/py_partiql_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:59:39.623520 py-partiql-parser-0.3.7/py_partiql_parser/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/case_insensitive_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/clause_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/py_partiql_parser/_internal/where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:59:39.623520 py-partiql-parser-0.3.7/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 17:59:39.000000 py-partiql-parser-0.3.7/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-01 17:59:39.000000 py-partiql-parser-0.3.7/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:59:39.000000 py-partiql-parser-0.3.7/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 17:59:39.000000 py-partiql-parser-0.3.7/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 17:59:39.000000 py-partiql-parser-0.3.7/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-01 17:59:32.000000 py-partiql-parser-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 17:59:39.627520 py-partiql-parser-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:59:39.627520 py-partiql-parser-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_query_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_s3_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-01 17:59:22.000000 py-partiql-parser-0.3.7/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.3.6/LICENSE` & `py-partiql-parser-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/PKG-INFO` & `py-partiql-parser-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.6
+Version: 0.3.7
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Project-URL: Homepage, https://github.com/getmoto/py-partiql-parser
 Project-URL: Bug Tracker, https://github.com/getmoto/py-partiql-parser/issues
 Project-URL: ChangeLog, https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md
 Keywords: pypartiql,parser
```

### Comparing `py-partiql-parser-0.3.6/README.md` & `py-partiql-parser-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser/_internal/case_insensitive_dict.py` & `py-partiql-parser-0.3.7/py_partiql_parser/_internal/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser/_internal/clause_tokenizer.py` & `py-partiql-parser-0.3.7/py_partiql_parser/_internal/clause_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser/_internal/csv_converter.py` & `py-partiql-parser-0.3.7/py_partiql_parser/_internal/csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser/_internal/from_parser.py` & `py-partiql-parser-0.3.7/py_partiql_parser/_internal/from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser/_internal/json_parser.py` & `py-partiql-parser-0.3.7/py_partiql_parser/_internal/json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser/_internal/parser.py` & `py-partiql-parser-0.3.7/py_partiql_parser/_internal/parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser/_internal/select_parser.py` & `py-partiql-parser-0.3.7/py_partiql_parser/_internal/select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser/_internal/utils.py` & `py-partiql-parser-0.3.7/py_partiql_parser/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser/_internal/where_parser.py` & `py-partiql-parser-0.3.7/py_partiql_parser/_internal/where_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser.egg-info/PKG-INFO` & `py-partiql-parser-0.3.7/py_partiql_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.6
+Version: 0.3.7
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Project-URL: Homepage, https://github.com/getmoto/py-partiql-parser
 Project-URL: Bug Tracker, https://github.com/getmoto/py-partiql-parser/issues
 Project-URL: ChangeLog, https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md
 Keywords: pypartiql,parser
```

### Comparing `py-partiql-parser-0.3.6/py_partiql_parser.egg-info/SOURCES.txt` & `py-partiql-parser-0.3.7/py_partiql_parser.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 py_partiql_parser/__init__.py
 py_partiql_parser.egg-info/PKG-INFO
 py_partiql_parser.egg-info/SOURCES.txt
 py_partiql_parser.egg-info/dependency_links.txt
```

### Comparing `py-partiql-parser-0.3.6/pyproject.toml` & `py-partiql-parser-0.3.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 [project]
 name = "py-partiql-parser"
-version = "0.3.6"
+version = "0.3.7"
 description = "Pure Python PartiQL Parser"
 readme = "README.md"
 keywords = ["pypartiql", "parser"]
 license = {text = "MIT"}
 authors = [{name="Bert Blommers", email="info@bertblommers.nl"}]
 
 dependencies = []
 
 [project.urls]
 "Homepage" = "https://github.com/getmoto/py-partiql-parser"
 "Bug Tracker" = "https://github.com/getmoto/py-partiql-parser/issues"
 "ChangeLog" = "https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md"
 
-[tool.setuptools]
-packages = [
-    "py_partiql_parser",
-    "py_partiql_parser._internal",
-    "tests"
-]
-
 [project.optional-dependencies]
 dev = [
     "black==22.6.0",
     "flake8",
     "mypy==0.971",
     "pytest"
 ]
```

### Comparing `py-partiql-parser-0.3.6/tests/__init__.py` & `py-partiql-parser-0.3.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_csv_converter.py` & `py-partiql-parser-0.3.7/tests/test_csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_dynamodb_examples.py` & `py-partiql-parser-0.3.7/tests/test_dynamodb_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_from_parser.py` & `py-partiql-parser-0.3.7/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_json_encoder.py` & `py-partiql-parser-0.3.7/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_json_parser.py` & `py-partiql-parser-0.3.7/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_query_metadata.py` & `py-partiql-parser-0.3.7/tests/test_query_metadata.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_s3_examples.py` & `py-partiql-parser-0.3.7/tests/test_s3_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_select_functions.py` & `py-partiql-parser-0.3.7/tests/test_select_functions.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_select_parser.py` & `py-partiql-parser-0.3.7/tests/test_select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_utils.py` & `py-partiql-parser-0.3.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.6/tests/test_where_parser.py` & `py-partiql-parser-0.3.7/tests/test_where_parser.py`

 * *Files identical despite different names*

