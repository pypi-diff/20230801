# Comparing `tmp/uta-gms-engine-0.0.6.tar.gz` & `tmp/uta-gms-engine-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uta-gms-engine-0.0.6.tar", last modified: Tue Jul 18 18:26:42 2023, max compression
+gzip compressed data, was "uta-gms-engine-0.0.7.tar", last modified: Tue Aug  1 16:52:41 2023, max compression
```

## Comparing `uta-gms-engine-0.0.6.tar` & `uta-gms-engine-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:26:42.268895 uta-gms-engine-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-18 18:26:42.268895 uta-gms-engine-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-18 18:26:31.000000 uta-gms-engine-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 18:26:31.000000 uta-gms-engine-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-18 18:26:42.272894 uta-gms-engine-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:26:42.268895 uta-gms-engine-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:26:42.268895 uta-gms-engine-0.0.6/src/uta_gms_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-18 18:26:42.000000 uta-gms-engine-0.0.6/src/uta_gms_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 18:26:42.000000 uta-gms-engine-0.0.6/src/uta_gms_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:26:42.000000 uta-gms-engine-0.0.6/src/uta_gms_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 18:26:42.000000 uta-gms-engine-0.0.6/src/uta_gms_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 18:26:42.000000 uta-gms-engine-0.0.6/src/uta_gms_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:26:42.268895 uta-gms-engine-0.0.6/src/utagms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:26:31.000000 uta-gms-engine-0.0.6/src/utagms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:26:31.000000 uta-gms-engine-0.0.6/src/utagms/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-18 18:26:31.000000 uta-gms-engine-0.0.6/src/utagms/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:52:41.018982 uta-gms-engine-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-01 16:52:41.022982 uta-gms-engine-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-01 16:52:41.022982 uta-gms-engine-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:52:41.018982 uta-gms-engine-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:52:41.018982 uta-gms-engine-0.0.7/src/uta_gms_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-01 16:52:41.000000 uta-gms-engine-0.0.7/src/uta_gms_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-01 16:52:41.000000 uta-gms-engine-0.0.7/src/uta_gms_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:52:41.000000 uta-gms-engine-0.0.7/src/uta_gms_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 16:52:41.000000 uta-gms-engine-0.0.7/src/uta_gms_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 16:52:41.000000 uta-gms-engine-0.0.7/src/uta_gms_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:52:41.018982 uta-gms-engine-0.0.7/src/utagmsengine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/src/utagmsengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/src/utagmsengine/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/src/utagmsengine/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:52:41.018982 uta-gms-engine-0.0.7/src/utagmsengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/src/utagmsengine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/src/utagmsengine/utils/parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/src/utagmsengine/utils/solver_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:52:41.018982 uta-gms-engine-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/tests/test_parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-01 16:52:27.000000 uta-gms-engine-0.0.7/tests/test_solver_utils.py
```

### Comparing `uta-gms-engine-0.0.6/PKG-INFO` & `uta-gms-engine-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uta-gms-engine
-Version: 0.0.6
+Version: 0.0.7
 Summary: Engine for UTA GMS method
 Home-page: https://github.com/UTA-WESOME/uta-gms-engine
 Author: Filip Marciniak
 Author-email: filip.marciniak15@gmail.com
 Project-URL: Bug Tracker, https://github.com/UTA-WESOME/uta-gms-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uta-gms-engine-0.0.6/setup.cfg` & `uta-gms-engine-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uta-gms-engine
-version = 0.0.6
+version = 0.0.7
 author = Filip Marciniak
 author_email = filip.marciniak15@gmail.com
 description = Engine for UTA GMS method
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/UTA-WESOME/uta-gms-engine
 project_urls =
```

### Comparing `uta-gms-engine-0.0.6/src/uta_gms_engine.egg-info/PKG-INFO` & `uta-gms-engine-0.0.7/src/uta_gms_engine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uta-gms-engine
-Version: 0.0.6
+Version: 0.0.7
 Summary: Engine for UTA GMS method
 Home-page: https://github.com/UTA-WESOME/uta-gms-engine
 Author: Filip Marciniak
 Author-email: filip.marciniak15@gmail.com
 Project-URL: Bug Tracker, https://github.com/UTA-WESOME/uta-gms-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

