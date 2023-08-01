# Comparing `tmp/cybrex-1.1.3.tar.gz` & `tmp/cybrex-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.1.3.tar", last modified: Tue Aug  1 19:58:06 2023, max compression
+gzip compressed data, was "cybrex-1.1.4.tar", last modified: Tue Aug  1 20:04:35 2023, max compression
```

## Comparing `cybrex-1.1.3.tar` & `cybrex-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:58:06.694486 cybrex-1.1.3/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.3/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 19:58:06.694137 cybrex-1.1.3/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.3/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:58:06.691311 cybrex-1.1.3/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.3/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 19:57:30.000000 cybrex-1.1.3/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    11678 2023-08-01 19:57:40.000000 cybrex-1.1.3/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.3/cybrex/models.py
--rw-r--r--   0 pasha      (501) staff       (20)    13911 2023-08-01 13:45:04.000000 cybrex-1.1.3/cybrex/test.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:58:06.693571 cybrex-1.1.3/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      320 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      204 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 19:57:48.000000 cybrex-1.1.3/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      204 2023-08-01 19:51:35.000000 cybrex-1.1.3/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 19:58:06.694630 cybrex-1.1.3/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:04:35.153126 cybrex-1.1.4/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.4/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:04:35.152810 cybrex-1.1.4/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.4/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:04:35.150243 cybrex-1.1.4/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.4/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 19:57:30.000000 cybrex-1.1.4/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    11678 2023-08-01 19:57:40.000000 cybrex-1.1.4/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.4/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:04:35.152232 cybrex-1.1.4/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      219 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 20:04:17.000000 cybrex-1.1.4/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      219 2023-08-01 20:03:15.000000 cybrex-1.1.4/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 20:04:35.153227 cybrex-1.1.4/setup.cfg
```

### Comparing `cybrex-1.1.3/PKG-INFO` & `cybrex-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.3
+Version: 1.1.4
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.3/README.md` & `cybrex-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.3/cybrex/cli.py` & `cybrex-1.1.4/cybrex/cli.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.3/cybrex/cybrex_ai.py` & `cybrex-1.1.4/cybrex/cybrex_ai.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.3/cybrex/models.py` & `cybrex-1.1.4/cybrex/models.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.3/cybrex.egg-info/PKG-INFO` & `cybrex-1.1.4/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.3
+Version: 1.1.4
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.3/pyproject.toml` & `cybrex-1.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.1.3"
+version = "1.1.4"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

