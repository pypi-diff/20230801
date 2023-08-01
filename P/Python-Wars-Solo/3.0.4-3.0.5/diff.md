# Comparing `tmp/Python-Wars-Solo-3.0.4.tar.gz` & `tmp/Python-Wars-Solo-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python-Wars-Solo-3.0.4.tar", last modified: Tue Aug  1 13:20:02 2023, max compression
+gzip compressed data, was "Python-Wars-Solo-3.0.5.tar", last modified: Tue Aug  1 13:30:55 2023, max compression
```

## Comparing `Python-Wars-Solo-3.0.4.tar` & `Python-Wars-Solo-3.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:20:02.523768 Python-Wars-Solo-3.0.4/
--rw-r--r--   0 drg        (501) staff       (20)      667 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.4/LICENSE.txt
--rw-r--r--   0 drg        (501) staff       (20)     4462 2023-08-01 13:20:02.523373 Python-Wars-Solo-3.0.4/PKG-INFO
--rw-r--r--   0 drg        (501) staff       (20)     2683 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.4/README.rst
--rw-r--r--   0 drg        (501) staff       (20)     1092 2023-08-01 13:18:47.000000 Python-Wars-Solo-3.0.4/pyproject.toml
--rw-r--r--   0 drg        (501) staff       (20)       38 2023-08-01 13:20:02.523898 Python-Wars-Solo-3.0.4/setup.cfg
-drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:20:02.519939 Python-Wars-Solo-3.0.4/src/
-drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:20:02.522656 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/
--rw-r--r--   0 drg        (501) staff       (20)     4462 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/PKG-INFO
--rw-r--r--   0 drg        (501) staff       (20)      283 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/SOURCES.txt
--rw-r--r--   0 drg        (501) staff       (20)        1 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/dependency_links.txt
--rw-r--r--   0 drg        (501) staff       (20)       42 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/entry_points.txt
--rw-r--r--   0 drg        (501) staff       (20)        9 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/top_level.txt
--rw-r--r--   0 drg        (501) staff       (20)     4218 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.4/src/go.py
--rw-r--r--   0 drg        (501) staff       (20)     5269 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.4/src/stuff.py
+drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:30:55.242354 Python-Wars-Solo-3.0.5/
+-rw-r--r--   0 drg        (501) staff       (20)      667 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.5/LICENSE.txt
+-rw-r--r--   0 drg        (501) staff       (20)     4564 2023-08-01 13:30:55.241957 Python-Wars-Solo-3.0.5/PKG-INFO
+-rw-r--r--   0 drg        (501) staff       (20)     2683 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.5/README.rst
+-rw-r--r--   0 drg        (501) staff       (20)     1184 2023-08-01 13:29:16.000000 Python-Wars-Solo-3.0.5/pyproject.toml
+-rw-r--r--   0 drg        (501) staff       (20)       38 2023-08-01 13:30:55.242500 Python-Wars-Solo-3.0.5/setup.cfg
+drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:30:55.238346 Python-Wars-Solo-3.0.5/src/
+drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:30:55.241333 Python-Wars-Solo-3.0.5/src/Python_Wars_Solo.egg-info/
+-rw-r--r--   0 drg        (501) staff       (20)     4564 2023-08-01 13:30:55.000000 Python-Wars-Solo-3.0.5/src/Python_Wars_Solo.egg-info/PKG-INFO
+-rw-r--r--   0 drg        (501) staff       (20)      283 2023-08-01 13:30:55.000000 Python-Wars-Solo-3.0.5/src/Python_Wars_Solo.egg-info/SOURCES.txt
+-rw-r--r--   0 drg        (501) staff       (20)        1 2023-08-01 13:30:55.000000 Python-Wars-Solo-3.0.5/src/Python_Wars_Solo.egg-info/dependency_links.txt
+-rw-r--r--   0 drg        (501) staff       (20)       42 2023-08-01 13:30:55.000000 Python-Wars-Solo-3.0.5/src/Python_Wars_Solo.egg-info/entry_points.txt
+-rw-r--r--   0 drg        (501) staff       (20)        9 2023-08-01 13:30:55.000000 Python-Wars-Solo-3.0.5/src/Python_Wars_Solo.egg-info/top_level.txt
+-rw-r--r--   0 drg        (501) staff       (20)     4218 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.5/src/go.py
+-rw-r--r--   0 drg        (501) staff       (20)     5269 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.5/src/stuff.py
```

### Comparing `Python-Wars-Solo-3.0.4/LICENSE.txt` & `Python-Wars-Solo-3.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Python-Wars-Solo-3.0.4/PKG-INFO` & `Python-Wars-Solo-3.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Wars-Solo
-Version: 3.0.4
+Version: 3.0.5
 Summary: A retro-style Apple ][ Basic game cooked up in 45 minutes.
 Author-email: Daniel Roy Greenfeld <pydanny@gmail.com>
 License: Python Wars Solo
         Copyright (C) 2017  Daniel Greenfeld
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
@@ -24,16 +24,18 @@
 Project-URL: Changelog, https://github.com/pydanny/Python-Wars-Solo/blob/main/changelog.md
 Project-URL: Sponsors, https://github.com/sponsors/pydanny
 Project-URL: Issues, https://github.com/pydanny/Python-Wars-Solo/issues
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 =============
 README
```

### Comparing `Python-Wars-Solo-3.0.4/README.rst` & `Python-Wars-Solo-3.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `Python-Wars-Solo-3.0.4/pyproject.toml` & `Python-Wars-Solo-3.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Python-Wars-Solo"
-version = "3.0.4"
+version = "3.0.5"
 description = "A retro-style Apple ][ Basic game cooked up in 45 minutes."
 readme = "README.rst"
 requires-python = ">=3.8"
 authors = [
     { name = "Daniel Roy Greenfeld", email = "pydanny@gmail.com" },
 ]
 classifiers = [
     'Development Status :: 6 - Mature',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU General Public License (GPL)',
     'Natural Language :: English',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Programming Language :: Python'
 ]
 
 [project.license]
 file = 'LICENSE.txt'
 
 [project.urls]
```

### Comparing `Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/PKG-INFO` & `Python-Wars-Solo-3.0.5/src/Python_Wars_Solo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Wars-Solo
-Version: 3.0.4
+Version: 3.0.5
 Summary: A retro-style Apple ][ Basic game cooked up in 45 minutes.
 Author-email: Daniel Roy Greenfeld <pydanny@gmail.com>
 License: Python Wars Solo
         Copyright (C) 2017  Daniel Greenfeld
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
@@ -24,16 +24,18 @@
 Project-URL: Changelog, https://github.com/pydanny/Python-Wars-Solo/blob/main/changelog.md
 Project-URL: Sponsors, https://github.com/sponsors/pydanny
 Project-URL: Issues, https://github.com/pydanny/Python-Wars-Solo/issues
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 =============
 README
```

### Comparing `Python-Wars-Solo-3.0.4/src/go.py` & `Python-Wars-Solo-3.0.5/src/go.py`

 * *Files identical despite different names*

### Comparing `Python-Wars-Solo-3.0.4/src/stuff.py` & `Python-Wars-Solo-3.0.5/src/stuff.py`

 * *Files identical despite different names*

