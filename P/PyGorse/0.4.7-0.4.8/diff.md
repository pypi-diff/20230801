# Comparing `tmp/PyGorse-0.4.7.tar.gz` & `tmp/PyGorse-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGorse-0.4.7.tar", last modified: Sun Nov 27 11:01:32 2022, max compression
+gzip compressed data, was "PyGorse-0.4.8.tar", last modified: Tue Aug  1 13:17:34 2023, max compression
```

## Comparing `PyGorse-0.4.7.tar` & `PyGorse-0.4.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 11:01:32.530115 PyGorse-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-11-27 11:01:17.000000 PyGorse-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2022-11-27 11:01:32.526115 PyGorse-0.4.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 11:01:32.526115 PyGorse-0.4.7/PyGorse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2022-11-27 11:01:32.000000 PyGorse-0.4.7/PyGorse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2022-11-27 11:01:32.000000 PyGorse-0.4.7/PyGorse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-27 11:01:32.000000 PyGorse-0.4.7/PyGorse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-11-27 11:01:32.000000 PyGorse-0.4.7/PyGorse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-11-27 11:01:32.000000 PyGorse-0.4.7/PyGorse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2022-11-27 11:01:17.000000 PyGorse-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 11:01:32.526115 PyGorse-0.4.7/gorse/
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2022-11-27 11:01:17.000000 PyGorse-0.4.7/gorse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-27 11:01:32.530115 PyGorse-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      494 2022-11-27 11:01:17.000000 PyGorse-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:17:34.652427 PyGorse-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 13:17:26.000000 PyGorse-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-01 13:17:34.652427 PyGorse-0.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:17:34.652427 PyGorse-0.4.8/PyGorse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-01 13:17:34.000000 PyGorse-0.4.8/PyGorse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 13:17:34.000000 PyGorse-0.4.8/PyGorse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:17:34.000000 PyGorse-0.4.8/PyGorse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 13:17:34.000000 PyGorse-0.4.8/PyGorse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 13:17:34.000000 PyGorse-0.4.8/PyGorse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-01 13:17:26.000000 PyGorse-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:17:34.652427 PyGorse-0.4.8/gorse/
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-08-01 13:17:26.000000 PyGorse-0.4.8/gorse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:17:34.652427 PyGorse-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 13:17:26.000000 PyGorse-0.4.8/setup.py
```

### Comparing `PyGorse-0.4.7/LICENSE` & `PyGorse-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGorse-0.4.7/PKG-INFO` & `PyGorse-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGorse
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python SDK for gorse recommender system
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyGorse
 
 [![CI](https://github.com/gorse-io/PyGorse/actions/workflows/ci.yml/badge.svg)](https://github.com/gorse-io/PyGorse/actions/workflows/ci.yml)
```

### Comparing `PyGorse-0.4.7/PyGorse.egg-info/PKG-INFO` & `PyGorse-0.4.8/PyGorse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGorse
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python SDK for gorse recommender system
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyGorse
 
 [![CI](https://github.com/gorse-io/PyGorse/actions/workflows/ci.yml/badge.svg)](https://github.com/gorse-io/PyGorse/actions/workflows/ci.yml)
```

### Comparing `PyGorse-0.4.7/README.md` & `PyGorse-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `PyGorse-0.4.7/gorse/__init__.py` & `PyGorse-0.4.8/gorse/__init__.py`

 * *Files identical despite different names*

