# Comparing `tmp/py-doc-0.0.5.tar.gz` & `tmp/py-doc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-doc-0.0.5.tar", last modified: Tue Aug  1 18:14:59 2023, max compression
+gzip compressed data, was "py-doc-0.0.6.tar", last modified: Tue Aug  1 18:21:57 2023, max compression
```

## Comparing `py-doc-0.0.5.tar` & `py-doc-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 18:14:59.316865 py-doc-0.0.5/
--rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 18:14:59.316865 py-doc-0.0.5/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      328 2023-08-01 14:14:55.000000 py-doc-0.0.5/README.md
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 18:14:59.316865 py-doc-0.0.5/py_doc/
--rw-r--r--   0 connor    (1000) connor    (1000)       48 2023-08-01 14:14:55.000000 py-doc-0.0.5/py_doc/__init__.py
--rw-r--r--   0 connor    (1000) connor    (1000)      886 2023-07-30 21:46:54.000000 py-doc-0.0.5/py_doc/multiplication.py
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 18:14:59.316865 py-doc-0.0.5/py_doc.egg-info/
--rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 18:14:59.000000 py-doc-0.0.5/py_doc.egg-info/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      211 2023-08-01 18:14:59.000000 py-doc-0.0.5/py_doc.egg-info/SOURCES.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-08-01 18:14:59.000000 py-doc-0.0.5/py_doc.egg-info/dependency_links.txt
--rw-r--r--   0 connor    (1000) connor    (1000)       13 2023-08-01 18:14:59.000000 py-doc-0.0.5/py_doc.egg-info/requires.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        7 2023-08-01 18:14:59.000000 py-doc-0.0.5/py_doc.egg-info/top_level.txt
--rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-08-01 18:14:59.316865 py-doc-0.0.5/setup.cfg
--rw-r--r--   0 connor    (1000) connor    (1000)     1281 2023-08-01 18:14:06.000000 py-doc-0.0.5/setup.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 18:21:57.674495 py-doc-0.0.6/
+-rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 18:21:57.674495 py-doc-0.0.6/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      328 2023-08-01 14:14:55.000000 py-doc-0.0.6/README.md
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 18:21:57.674495 py-doc-0.0.6/py_doc/
+-rw-r--r--   0 connor    (1000) connor    (1000)       90 2023-08-01 18:21:42.000000 py-doc-0.0.6/py_doc/__init__.py
+-rw-r--r--   0 connor    (1000) connor    (1000)      923 2023-08-01 18:20:38.000000 py-doc-0.0.6/py_doc/multiplication.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 18:21:57.674495 py-doc-0.0.6/py_doc.egg-info/
+-rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      211 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)       13 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/requires.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        7 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/top_level.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-08-01 18:21:57.674495 py-doc-0.0.6/setup.cfg
+-rw-r--r--   0 connor    (1000) connor    (1000)     1281 2023-08-01 18:21:52.000000 py-doc-0.0.6/setup.py
```

### Comparing `py-doc-0.0.5/PKG-INFO` & `py-doc-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-doc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-doc-0.0.5/py_doc/multiplication.py` & `py-doc-0.0.6/py_doc/multiplication.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import numpy as np
+
+def double(num):
+    return num * 2
 class Multiplication:
     """
     Instantiate a multiplication operation.
     Numbers will be multiplied by the given multiplier.
 
     :param multiplier: The multiplier.
     :type multiplier: int
```

### Comparing `py-doc-0.0.5/py_doc.egg-info/PKG-INFO` & `py-doc-0.0.6/py_doc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-doc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-doc-0.0.5/setup.py` & `py-doc-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="py-doc",
-    version="0.0.5",
+    version="0.0.6",
     description="Used for working with documentations in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Connor Holm",
     author_email="connorjholm@gmail.com",
     license="MIT",
```

