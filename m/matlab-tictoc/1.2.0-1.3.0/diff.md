# Comparing `tmp/matlab-tictoc-1.2.0.tar.gz` & `tmp/matlab-tictoc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlab-tictoc-1.2.0.tar", last modified: Mon May 29 16:01:52 2023, max compression
+gzip compressed data, was "matlab-tictoc-1.3.0.tar", last modified: Tue Aug  1 18:57:31 2023, max compression
```

## Comparing `matlab-tictoc-1.2.0.tar` & `matlab-tictoc-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:01:52.767171 matlab-tictoc-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-29 16:01:52.767171 matlab-tictoc-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:01:52.767171 matlab-tictoc-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:01:52.763171 matlab-tictoc-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:01:52.763171 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-29 16:01:52.000000 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 16:01:52.000000 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:01:52.000000 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 16:01:52.000000 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:01:52.767171 matlab-tictoc-1.2.0/src/tictoc/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/src/tictoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/src/tictoc/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:57:31.744851 matlab-tictoc-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 18:57:22.000000 matlab-tictoc-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-01 18:57:31.740851 matlab-tictoc-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-01 18:57:22.000000 matlab-tictoc-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-01 18:57:22.000000 matlab-tictoc-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:57:31.744851 matlab-tictoc-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:57:31.740851 matlab-tictoc-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:57:31.740851 matlab-tictoc-1.3.0/src/matlab_tictoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-01 18:57:31.000000 matlab-tictoc-1.3.0/src/matlab_tictoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-01 18:57:31.000000 matlab-tictoc-1.3.0/src/matlab_tictoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:57:31.000000 matlab-tictoc-1.3.0/src/matlab_tictoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 18:57:31.000000 matlab-tictoc-1.3.0/src/matlab_tictoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:57:31.740851 matlab-tictoc-1.3.0/src/tictoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-01 18:57:22.000000 matlab-tictoc-1.3.0/src/tictoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-01 18:57:22.000000 matlab-tictoc-1.3.0/src/tictoc/tictoc.py
```

### Comparing `matlab-tictoc-1.2.0/LICENSE` & `matlab-tictoc-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matlab-tictoc-1.2.0/PKG-INFO` & `matlab-tictoc-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: matlab-tictoc
-Version: 1.2.0
+Version: 1.3.0
 Summary: A timing package that mimics MATLAB's tic and toc functionality
 Author: Matthew Altberg
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MATLAB Tic Toc
 
 A Python module to make timing in python easier by mimicing MATLAB's `tic` and `toc` functions.
 `tic` starts a timer by recording the current time, and `toc` uses the start time to find the elapsed time.
```

### Comparing `matlab-tictoc-1.2.0/README.md` & `matlab-tictoc-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/PKG-INFO` & `matlab-tictoc-1.3.0/src/matlab_tictoc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: matlab-tictoc
-Version: 1.2.0
+Version: 1.3.0
 Summary: A timing package that mimics MATLAB's tic and toc functionality
 Author: Matthew Altberg
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MATLAB Tic Toc
 
 A Python module to make timing in python easier by mimicing MATLAB's `tic` and `toc` functions.
 `tic` starts a timer by recording the current time, and `toc` uses the start time to find the elapsed time.
```

### Comparing `matlab-tictoc-1.2.0/src/tictoc/tictoc.py` & `matlab-tictoc-1.3.0/src/tictoc/tictoc.py`

 * *Files identical despite different names*

