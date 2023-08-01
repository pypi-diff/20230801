# Comparing `tmp/mpc_obscodes-2023.7.24.tar.gz` & `tmp/mpc_obscodes-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2023.7.24.tar", last modified: Mon Jul 24 02:29:45 2023, max compression
+gzip compressed data, was "mpc_obscodes-2023.8.1.tar", last modified: Tue Aug  1 17:28:06 2023, max compression
```

## Comparing `mpc_obscodes-2023.7.24.tar` & `mpc_obscodes-2023.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:45.699179 mpc_obscodes-2023.7.24/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-24 02:29:45.699179 mpc_obscodes-2023.7.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:45.695179 mpc_obscodes-2023.7.24/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)   246592 2023-07-24 02:29:34.000000 mpc_obscodes-2023.7.24/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 02:29:34.000000 mpc_obscodes-2023.7.24/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:45.699179 mpc_obscodes-2023.7.24/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:45.695179 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-24 02:29:34.000000 mpc_obscodes-2023.7.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 02:29:45.699179 mpc_obscodes-2023.7.24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:28:06.497356 mpc_obscodes-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-01 17:27:52.000000 mpc_obscodes-2023.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-01 17:28:06.497356 mpc_obscodes-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-01 17:27:52.000000 mpc_obscodes-2023.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:28:06.497356 mpc_obscodes-2023.8.1/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-01 17:27:52.000000 mpc_obscodes-2023.8.1/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-01 17:27:52.000000 mpc_obscodes-2023.8.1/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-08-01 17:27:52.000000 mpc_obscodes-2023.8.1/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246704 2023-08-01 17:27:55.000000 mpc_obscodes-2023.8.1/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-01 17:27:55.000000 mpc_obscodes-2023.8.1/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:28:06.497356 mpc_obscodes-2023.8.1/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:27:52.000000 mpc_obscodes-2023.8.1/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-01 17:27:52.000000 mpc_obscodes-2023.8.1/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 17:27:52.000000 mpc_obscodes-2023.8.1/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-01 17:27:52.000000 mpc_obscodes-2023.8.1/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:28:06.497356 mpc_obscodes-2023.8.1/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-01 17:28:06.000000 mpc_obscodes-2023.8.1/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 17:28:06.000000 mpc_obscodes-2023.8.1/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:28:06.000000 mpc_obscodes-2023.8.1/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 17:28:06.000000 mpc_obscodes-2023.8.1/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 17:28:06.000000 mpc_obscodes-2023.8.1/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-01 17:27:55.000000 mpc_obscodes-2023.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 17:28:06.497356 mpc_obscodes-2023.8.1/setup.cfg
```

### Comparing `mpc_obscodes-2023.7.24/PKG-INFO` & `mpc_obscodes-2023.8.1/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mpc_obscodes
-Version: 2023.7.24
+Name: mpc-obscodes
+Version: 2023.8.1
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.7.24/README.md` & `mpc_obscodes-2023.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.24/mpc_obscodes/compare.py` & `mpc_obscodes-2023.8.1/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.24/mpc_obscodes/fetch.py` & `mpc_obscodes-2023.8.1/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.24/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2023.8.1/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995906672124437%*

 * *Differences: {"'X09'": "OrderedDict([('Longitude', 289.1467), ('cos', 0.862375), ('sin', -0.505108), ('Name', "*

 * *          "'Deep Random Survey, Rio Hurtado')])"}*

```diff
@@ -13777,14 +13777,20 @@
     },
     "X08": {
         "Longitude": 289.235,
         "Name": "ShAO Chile station, El Sauce",
         "cos": 0.862852,
         "sin": -0.504255
     },
+    "X09": {
+        "Longitude": 289.1467,
+        "Name": "Deep Random Survey, Rio Hurtado",
+        "cos": 0.862375,
+        "sin": -0.505108
+    },
     "X10": {
         "Longitude": 291.8204,
         "Name": "OVTLN, San Pedro de Atacama",
         "cos": 0.921644,
         "sin": -0.387717
     },
     "X11": {
```

### Comparing `mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2023.8.1/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2023.8.1/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2023.8.1/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2023.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mpc-obscodes
-Version: 2023.7.24
+Name: mpc_obscodes
+Version: 2023.8.1
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.7.24/pyproject.toml` & `mpc_obscodes-2023.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2023.07.24"
+version = "2023.08.01"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

