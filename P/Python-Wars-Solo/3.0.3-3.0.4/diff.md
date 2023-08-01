# Comparing `tmp/Python-Wars-Solo-3.0.3.tar.gz` & `tmp/Python-Wars-Solo-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python-Wars-Solo-3.0.3.tar", last modified: Tue Aug  1 13:15:08 2023, max compression
+gzip compressed data, was "Python-Wars-Solo-3.0.4.tar", last modified: Tue Aug  1 13:20:02 2023, max compression
```

## Comparing `Python-Wars-Solo-3.0.3.tar` & `Python-Wars-Solo-3.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:15:08.360908 Python-Wars-Solo-3.0.3/
--rw-r--r--   0 drg        (501) staff       (20)      667 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.3/LICENSE.txt
--rw-r--r--   0 drg        (501) staff       (20)     4331 2023-08-01 13:15:08.360565 Python-Wars-Solo-3.0.3/PKG-INFO
--rw-r--r--   0 drg        (501) staff       (20)     2683 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.3/README.rst
--rw-r--r--   0 drg        (501) staff       (20)      981 2023-08-01 13:14:56.000000 Python-Wars-Solo-3.0.3/pyproject.toml
--rw-r--r--   0 drg        (501) staff       (20)       38 2023-08-01 13:15:08.361039 Python-Wars-Solo-3.0.3/setup.cfg
-drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:15:08.357351 Python-Wars-Solo-3.0.3/src/
-drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:15:08.360079 Python-Wars-Solo-3.0.3/src/Python_Wars_Solo.egg-info/
--rw-r--r--   0 drg        (501) staff       (20)     4331 2023-08-01 13:15:08.000000 Python-Wars-Solo-3.0.3/src/Python_Wars_Solo.egg-info/PKG-INFO
--rw-r--r--   0 drg        (501) staff       (20)      283 2023-08-01 13:15:08.000000 Python-Wars-Solo-3.0.3/src/Python_Wars_Solo.egg-info/SOURCES.txt
--rw-r--r--   0 drg        (501) staff       (20)        1 2023-08-01 13:15:08.000000 Python-Wars-Solo-3.0.3/src/Python_Wars_Solo.egg-info/dependency_links.txt
--rw-r--r--   0 drg        (501) staff       (20)       42 2023-08-01 13:15:08.000000 Python-Wars-Solo-3.0.3/src/Python_Wars_Solo.egg-info/entry_points.txt
--rw-r--r--   0 drg        (501) staff       (20)        9 2023-08-01 13:15:08.000000 Python-Wars-Solo-3.0.3/src/Python_Wars_Solo.egg-info/top_level.txt
--rw-r--r--   0 drg        (501) staff       (20)     4218 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.3/src/go.py
--rw-r--r--   0 drg        (501) staff       (20)     5269 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.3/src/stuff.py
+drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:20:02.523768 Python-Wars-Solo-3.0.4/
+-rw-r--r--   0 drg        (501) staff       (20)      667 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.4/LICENSE.txt
+-rw-r--r--   0 drg        (501) staff       (20)     4462 2023-08-01 13:20:02.523373 Python-Wars-Solo-3.0.4/PKG-INFO
+-rw-r--r--   0 drg        (501) staff       (20)     2683 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.4/README.rst
+-rw-r--r--   0 drg        (501) staff       (20)     1092 2023-08-01 13:18:47.000000 Python-Wars-Solo-3.0.4/pyproject.toml
+-rw-r--r--   0 drg        (501) staff       (20)       38 2023-08-01 13:20:02.523898 Python-Wars-Solo-3.0.4/setup.cfg
+drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:20:02.519939 Python-Wars-Solo-3.0.4/src/
+drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 13:20:02.522656 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/
+-rw-r--r--   0 drg        (501) staff       (20)     4462 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/PKG-INFO
+-rw-r--r--   0 drg        (501) staff       (20)      283 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/SOURCES.txt
+-rw-r--r--   0 drg        (501) staff       (20)        1 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/dependency_links.txt
+-rw-r--r--   0 drg        (501) staff       (20)       42 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/entry_points.txt
+-rw-r--r--   0 drg        (501) staff       (20)        9 2023-08-01 13:20:02.000000 Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/top_level.txt
+-rw-r--r--   0 drg        (501) staff       (20)     4218 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.4/src/go.py
+-rw-r--r--   0 drg        (501) staff       (20)     5269 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.4/src/stuff.py
```

### Comparing `Python-Wars-Solo-3.0.3/LICENSE.txt` & `Python-Wars-Solo-3.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Python-Wars-Solo-3.0.3/PKG-INFO` & `Python-Wars-Solo-3.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Wars-Solo
-Version: 3.0.3
+Version: 3.0.4
 Summary: A retro-style Apple ][ Basic game cooked up in 45 minutes.
 Author-email: Daniel Roy Greenfeld <pydanny@gmail.com>
 License: Python Wars Solo
         Copyright (C) 2017  Daniel Greenfeld
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
@@ -16,16 +16,18 @@
         MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
         GNU General Public License for more details.
         
         You should have received a copy of the GNU General Public License
         along with this program.  If not, see <http://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/pydanny/Python-Wars-Solo
-Project-URL: documentation, https://github.com/pydanny/Python-Wars-Solo#readme
-Project-URL: changelog, https://github.com/pydanny/Python-Wars-Solo/blob/main/changelog.md
+Project-URL: Documentation, https://github.com/pydanny/Python-Wars-Solo#readme
+Project-URL: Changelog, https://github.com/pydanny/Python-Wars-Solo/blob/main/changelog.md
+Project-URL: Sponsors, https://github.com/sponsors/pydanny
+Project-URL: Issues, https://github.com/pydanny/Python-Wars-Solo/issues
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python
```

### Comparing `Python-Wars-Solo-3.0.3/README.rst` & `Python-Wars-Solo-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `Python-Wars-Solo-3.0.3/pyproject.toml` & `Python-Wars-Solo-3.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Python-Wars-Solo"
-version = "3.0.3"
+version = "3.0.4"
 description = "A retro-style Apple ][ Basic game cooked up in 45 minutes."
 readme = "README.rst"
 requires-python = ">=3.8"
 authors = [
     { name = "Daniel Roy Greenfeld", email = "pydanny@gmail.com" },
 ]
 classifiers = [
@@ -22,12 +22,14 @@
 ]
 
 [project.license]
 file = 'LICENSE.txt'
 
 [project.urls]
 Homepage = "https://github.com/pydanny/Python-Wars-Solo"
-documentation = "https://github.com/pydanny/Python-Wars-Solo#readme"
-changelog = "https://github.com/pydanny/Python-Wars-Solo/blob/main/changelog.md"
+Documentation = "https://github.com/pydanny/Python-Wars-Solo#readme"
+Changelog = "https://github.com/pydanny/Python-Wars-Solo/blob/main/changelog.md"
+Sponsors = "https://github.com/sponsors/pydanny"
+Issues = "https://github.com/pydanny/Python-Wars-Solo/issues"
 
 [project.scripts]
 pythonwarsolo = "go:main"
```

### Comparing `Python-Wars-Solo-3.0.3/src/Python_Wars_Solo.egg-info/PKG-INFO` & `Python-Wars-Solo-3.0.4/src/Python_Wars_Solo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Wars-Solo
-Version: 3.0.3
+Version: 3.0.4
 Summary: A retro-style Apple ][ Basic game cooked up in 45 minutes.
 Author-email: Daniel Roy Greenfeld <pydanny@gmail.com>
 License: Python Wars Solo
         Copyright (C) 2017  Daniel Greenfeld
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
@@ -16,16 +16,18 @@
         MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
         GNU General Public License for more details.
         
         You should have received a copy of the GNU General Public License
         along with this program.  If not, see <http://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/pydanny/Python-Wars-Solo
-Project-URL: documentation, https://github.com/pydanny/Python-Wars-Solo#readme
-Project-URL: changelog, https://github.com/pydanny/Python-Wars-Solo/blob/main/changelog.md
+Project-URL: Documentation, https://github.com/pydanny/Python-Wars-Solo#readme
+Project-URL: Changelog, https://github.com/pydanny/Python-Wars-Solo/blob/main/changelog.md
+Project-URL: Sponsors, https://github.com/sponsors/pydanny
+Project-URL: Issues, https://github.com/pydanny/Python-Wars-Solo/issues
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python
```

### Comparing `Python-Wars-Solo-3.0.3/src/go.py` & `Python-Wars-Solo-3.0.4/src/go.py`

 * *Files identical despite different names*

### Comparing `Python-Wars-Solo-3.0.3/src/stuff.py` & `Python-Wars-Solo-3.0.4/src/stuff.py`

 * *Files identical despite different names*

