# Comparing `tmp/slice_to_py_dist-0.3.0.tar.gz` & `tmp/slice_to_py_dist-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slice_to_py_dist-0.3.0.tar", max compression
+gzip compressed data, was "slice_to_py_dist-0.3.1.tar", max compression
```

## Comparing `slice_to_py_dist-0.3.0.tar` & `slice_to_py_dist-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6376 2023-07-12 09:02:11.606973 slice_to_py_dist-0.3.0/README.md
--rw-r--r--   0        0        0     1375 2023-07-23 17:47:06.115104 slice_to_py_dist-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 17:45:55.490474 slice_to_py_dist-0.3.0/slice_to_py_dist/__init__.py
--rw-r--r--   0        0        0     3114 2023-07-23 17:24:38.852989 slice_to_py_dist-0.3.0/slice_to_py_dist/__main__.py
--rw-r--r--   0        0        0     4547 2023-07-14 03:59:36.872429 slice_to_py_dist-0.3.0/slice_to_py_dist/build_sdist.py
--rw-r--r--   0        0        0     2735 2023-07-14 03:59:36.872429 slice_to_py_dist-0.3.0/slice_to_py_dist/custom_build_backend/backend.py
--rw-r--r--   0        0        0      247 2023-07-12 09:02:11.606973 slice_to_py_dist-0.3.0/slice_to_py_dist/types.py
--rw-r--r--   0        0        0      852 2023-07-12 09:02:11.606973 slice_to_py_dist-0.3.0/slice_to_py_dist/utils.py
--rw-r--r--   0        0        0     7140 1970-01-01 00:00:00.000000 slice_to_py_dist-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6376 2023-07-12 09:02:11.606973 slice_to_py_dist-0.3.1/README.md
+-rw-r--r--   0        0        0     1375 2023-08-01 05:18:30.152132 slice_to_py_dist-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 05:17:14.106804 slice_to_py_dist-0.3.1/slice_to_py_dist/__init__.py
+-rw-r--r--   0        0        0     3114 2023-07-23 17:24:38.852989 slice_to_py_dist-0.3.1/slice_to_py_dist/__main__.py
+-rw-r--r--   0        0        0     4547 2023-07-14 03:59:36.872429 slice_to_py_dist-0.3.1/slice_to_py_dist/build_sdist.py
+-rw-r--r--   0        0        0     2735 2023-07-14 03:59:36.872429 slice_to_py_dist-0.3.1/slice_to_py_dist/custom_build_backend/backend.py
+-rw-r--r--   0        0        0      247 2023-07-12 09:02:11.606973 slice_to_py_dist-0.3.1/slice_to_py_dist/types.py
+-rw-r--r--   0        0        0      852 2023-07-12 09:02:11.606973 slice_to_py_dist-0.3.1/slice_to_py_dist/utils.py
+-rw-r--r--   0        0        0     7140 1970-01-01 00:00:00.000000 slice_to_py_dist-0.3.1/PKG-INFO
```

### Comparing `slice_to_py_dist-0.3.0/README.md` & `slice_to_py_dist-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.3.0/pyproject.toml` & `slice_to_py_dist-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slice_to_py_dist"
-version = "0.3.0"  # a placeholder; will be set dynamically by poetry-dynamic-versioning
+version = "0.3.1"  # a placeholder; will be set dynamically by poetry-dynamic-versioning
 description = "Pack a set of ZeroC/ICE slice files (.ice) into python distribution package."
 authors = ["Evgeny Klunko <eklunko@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/evgk/slice_to_py_dist"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `slice_to_py_dist-0.3.0/slice_to_py_dist/__main__.py` & `slice_to_py_dist-0.3.1/slice_to_py_dist/__main__.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.3.0/slice_to_py_dist/build_sdist.py` & `slice_to_py_dist-0.3.1/slice_to_py_dist/build_sdist.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.3.0/slice_to_py_dist/custom_build_backend/backend.py` & `slice_to_py_dist-0.3.1/slice_to_py_dist/custom_build_backend/backend.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.3.0/slice_to_py_dist/utils.py` & `slice_to_py_dist-0.3.1/slice_to_py_dist/utils.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.3.0/PKG-INFO` & `slice_to_py_dist-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slice-to-py-dist
-Version: 0.3.0
+Version: 0.3.1
 Summary: Pack a set of ZeroC/ICE slice files (.ice) into python distribution package.
 Home-page: https://gitlab.com/evgk/slice_to_py_dist
 Author: Evgeny Klunko
 Author-email: eklunko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

