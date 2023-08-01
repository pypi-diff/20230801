# Comparing `tmp/requests_ntlm2-6.5.2.tar.gz` & `tmp/requests_ntlm2-6.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/requests_ntlm2-6.5.2.tar", last modified: Mon Oct 24 12:57:46 2022, max compression
+gzip compressed data, was "dist/requests_ntlm2-6.5.3.tar", last modified: Tue Aug  1 14:46:59 2023, max compression
```

## Comparing `requests_ntlm2-6.5.2.tar` & `requests_ntlm2-6.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/requests_ntlm2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/requests_ntlm2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/requests_ntlm2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/requests_ntlm2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/requests_ntlm2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6748 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/requests_ntlm2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4187 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/requests_ntlm2/
--rw-r--r--   0 runner    (1001) docker     (121)     6219 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/requests_ntlm2/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     5689 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/requests_ntlm2/dance.py
--rw-r--r--   0 runner    (1001) docker     (121)     9912 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/requests_ntlm2/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6337 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/requests_ntlm2/requests_ntlm2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/requests_ntlm2/adapters.py
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-10-24 12:57:42.000000 requests_ntlm2-6.5.2/requests_ntlm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6748 2022-10-24 12:57:46.000000 requests_ntlm2-6.5.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/requests_ntlm2/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/requests_ntlm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/requests_ntlm2/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/requests_ntlm2/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/requests_ntlm2/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/requests_ntlm2/dance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/requests_ntlm2/requests_ntlm2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/requests_ntlm2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/requests_ntlm2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/requests_ntlm2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/requests_ntlm2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/requests_ntlm2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/requests_ntlm2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-01 14:46:59.000000 requests_ntlm2-6.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-01 14:46:54.000000 requests_ntlm2-6.5.3/setup.py
```

### Comparing `requests_ntlm2-6.5.2/requests_ntlm2.egg-info/PKG-INFO` & `requests_ntlm2-6.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: requests-ntlm2
-Version: 6.5.2
+Name: requests_ntlm2
+Version: 6.5.3
 Summary: The HTTP NTLM proxy and/or server authentication library.
 Home-page: https://github.com/dopstar/requests-ntlm2
 Author: Mkhanyisi Madlavana
 Author-email: mmadlavana@gmail.com
 License: ISC
-Download-URL: https://github.com/dopstar/requests-ntlm2/archive/6.5.2.tar.gz
-Project-URL: Source, https://github.com/dopstar/requests-ntlm2
+Download-URL: https://github.com/dopstar/requests-ntlm2/archive/6.5.3.tar.gz
 Project-URL: Documentation, https://dopstar.github.io/requests-ntlm2
+Project-URL: Source, https://github.com/dopstar/requests-ntlm2
 Project-URL: Tracker, https://github.com/dopstar/requests-ntlm2/issues
 Description: <h1 align="center">requests-ntlm2</h1>
         <div align="center">NTLM authentication plugin for Requests</div>
         <br />
         
         [![Build Status](https://github.com/dopstar/requests-ntlm2/workflows/build/badge.svg?branch=master)](https://github.com/dopstar/requests-ntlm2/actions?query=workflow%3Abuild)
         [![codecov](https://codecov.io/gh/dopstar/requests-ntlm2/branch/master/graph/badge.svg)](https://codecov.io/gh/dopstar/requests-ntlm2)
@@ -148,16 +148,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: linting
```

### Comparing `requests_ntlm2-6.5.2/LICENSE` & `requests_ntlm2-6.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_ntlm2-6.5.2/README.md` & `requests_ntlm2-6.5.3/README.md`

 * *Files identical despite different names*

### Comparing `requests_ntlm2-6.5.2/requests_ntlm2/core.py` & `requests_ntlm2-6.5.3/requests_ntlm2/core.py`

 * *Files identical despite different names*

### Comparing `requests_ntlm2-6.5.2/requests_ntlm2/dance.py` & `requests_ntlm2-6.5.3/requests_ntlm2/dance.py`

 * *Files identical despite different names*

### Comparing `requests_ntlm2-6.5.2/requests_ntlm2/connection.py` & `requests_ntlm2-6.5.3/requests_ntlm2/connection.py`

 * *Files identical despite different names*

### Comparing `requests_ntlm2-6.5.2/requests_ntlm2/requests_ntlm2.py` & `requests_ntlm2-6.5.3/requests_ntlm2/requests_ntlm2.py`

 * *Files identical despite different names*

### Comparing `requests_ntlm2-6.5.2/requests_ntlm2/adapters.py` & `requests_ntlm2-6.5.3/requests_ntlm2/adapters.py`

 * *Files identical despite different names*

### Comparing `requests_ntlm2-6.5.2/PKG-INFO` & `requests_ntlm2-6.5.3/requests_ntlm2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: requests_ntlm2
-Version: 6.5.2
+Name: requests-ntlm2
+Version: 6.5.3
 Summary: The HTTP NTLM proxy and/or server authentication library.
 Home-page: https://github.com/dopstar/requests-ntlm2
 Author: Mkhanyisi Madlavana
 Author-email: mmadlavana@gmail.com
 License: ISC
-Download-URL: https://github.com/dopstar/requests-ntlm2/archive/6.5.2.tar.gz
-Project-URL: Source, https://github.com/dopstar/requests-ntlm2
+Download-URL: https://github.com/dopstar/requests-ntlm2/archive/6.5.3.tar.gz
 Project-URL: Documentation, https://dopstar.github.io/requests-ntlm2
+Project-URL: Source, https://github.com/dopstar/requests-ntlm2
 Project-URL: Tracker, https://github.com/dopstar/requests-ntlm2/issues
 Description: <h1 align="center">requests-ntlm2</h1>
         <div align="center">NTLM authentication plugin for Requests</div>
         <br />
         
         [![Build Status](https://github.com/dopstar/requests-ntlm2/workflows/build/badge.svg?branch=master)](https://github.com/dopstar/requests-ntlm2/actions?query=workflow%3Abuild)
         [![codecov](https://codecov.io/gh/dopstar/requests-ntlm2/branch/master/graph/badge.svg)](https://codecov.io/gh/dopstar/requests-ntlm2)
@@ -148,16 +148,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: linting
```

