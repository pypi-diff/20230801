# Comparing `tmp/py_doc-0.0.3.tar.gz` & `tmp/py_doc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_doc-0.0.3.tar", last modified: Tue Aug  1 14:22:27 2023, max compression
+gzip compressed data, was "py_doc-0.0.4.tar", last modified: Tue Aug  1 14:32:39 2023, max compression
```

## Comparing `py_doc-0.0.3.tar` & `py_doc-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 14:22:27.446340 py_doc-0.0.3/
--rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 14:22:27.445340 py_doc-0.0.3/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      328 2023-08-01 14:14:55.000000 py_doc-0.0.3/README.md
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 14:22:27.445340 py_doc-0.0.3/py_doc/
--rw-r--r--   0 connor    (1000) connor    (1000)       48 2023-08-01 14:14:55.000000 py_doc-0.0.3/py_doc/__init__.py
--rw-r--r--   0 connor    (1000) connor    (1000)      886 2023-07-30 21:46:54.000000 py_doc-0.0.3/py_doc/multiplication.py
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 14:22:27.445340 py_doc-0.0.3/py_doc.egg-info/
--rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      211 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/SOURCES.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/dependency_links.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        6 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/requires.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        7 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/top_level.txt
--rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-08-01 14:22:27.446340 py_doc-0.0.3/setup.cfg
--rw-r--r--   0 connor    (1000) connor    (1000)     1270 2023-08-01 14:21:26.000000 py_doc-0.0.3/setup.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 14:32:39.744029 py_doc-0.0.4/
+-rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 14:32:39.744029 py_doc-0.0.4/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      328 2023-08-01 14:14:55.000000 py_doc-0.0.4/README.md
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 14:32:39.743028 py_doc-0.0.4/py_doc/
+-rw-r--r--   0 connor    (1000) connor    (1000)       48 2023-08-01 14:14:55.000000 py_doc-0.0.4/py_doc/__init__.py
+-rw-r--r--   0 connor    (1000) connor    (1000)      886 2023-07-30 21:46:54.000000 py_doc-0.0.4/py_doc/multiplication.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 14:32:39.743028 py_doc-0.0.4/py_doc.egg-info/
+-rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 14:32:39.000000 py_doc-0.0.4/py_doc.egg-info/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      211 2023-08-01 14:32:39.000000 py_doc-0.0.4/py_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-08-01 14:32:39.000000 py_doc-0.0.4/py_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        6 2023-08-01 14:32:39.000000 py_doc-0.0.4/py_doc.egg-info/requires.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        7 2023-08-01 14:32:39.000000 py_doc-0.0.4/py_doc.egg-info/top_level.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-08-01 14:32:39.744029 py_doc-0.0.4/setup.cfg
+-rw-r--r--   0 connor    (1000) connor    (1000)     1270 2023-08-01 14:32:26.000000 py_doc-0.0.4/setup.py
```

### Comparing `py_doc-0.0.3/PKG-INFO` & `py_doc-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_doc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py_doc-0.0.3/py_doc/multiplication.py` & `py_doc-0.0.4/py_doc/multiplication.py`

 * *Files identical despite different names*

### Comparing `py_doc-0.0.3/py_doc.egg-info/PKG-INFO` & `py_doc-0.0.4/py_doc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-doc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py_doc-0.0.3/setup.py` & `py_doc-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="py_doc",
-    version="0.0.3",
+    version="0.0.4",
     description="Used for working with documentations in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Connor Holm",
     author_email="connorjholm@gmail.com",
     license="MIT",
```

