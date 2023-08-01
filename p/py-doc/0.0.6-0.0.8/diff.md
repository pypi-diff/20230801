# Comparing `tmp/py-doc-0.0.6.tar.gz` & `tmp/py-doc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-doc-0.0.6.tar", last modified: Tue Aug  1 18:21:57 2023, max compression
+gzip compressed data, was "py-doc-0.0.8.tar", last modified: Tue Aug  1 21:49:15 2023, max compression
```

## Comparing `py-doc-0.0.6.tar` & `py-doc-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 18:21:57.674495 py-doc-0.0.6/
--rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 18:21:57.674495 py-doc-0.0.6/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      328 2023-08-01 14:14:55.000000 py-doc-0.0.6/README.md
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 18:21:57.674495 py-doc-0.0.6/py_doc/
--rw-r--r--   0 connor    (1000) connor    (1000)       90 2023-08-01 18:21:42.000000 py-doc-0.0.6/py_doc/__init__.py
--rw-r--r--   0 connor    (1000) connor    (1000)      923 2023-08-01 18:20:38.000000 py-doc-0.0.6/py_doc/multiplication.py
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 18:21:57.674495 py-doc-0.0.6/py_doc.egg-info/
--rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      211 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/SOURCES.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/dependency_links.txt
--rw-r--r--   0 connor    (1000) connor    (1000)       13 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/requires.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        7 2023-08-01 18:21:57.000000 py-doc-0.0.6/py_doc.egg-info/top_level.txt
--rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-08-01 18:21:57.674495 py-doc-0.0.6/setup.cfg
--rw-r--r--   0 connor    (1000) connor    (1000)     1281 2023-08-01 18:21:52.000000 py-doc-0.0.6/setup.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 21:49:15.307024 py-doc-0.0.8/
+-rw-r--r--   0 connor    (1000) connor    (1000)     1119 2023-08-01 21:49:15.307024 py-doc-0.0.8/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      457 2023-08-01 20:49:33.000000 py-doc-0.0.8/README.md
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 21:49:15.307024 py-doc-0.0.8/py_doc/
+-rw-r--r--   0 connor    (1000) connor    (1000)      126 2023-08-01 21:47:22.000000 py-doc-0.0.8/py_doc/__init__.py
+-rw-r--r--   0 connor    (1000) connor    (1000)      369 2023-08-01 21:46:07.000000 py-doc-0.0.8/py_doc/document.py
+-rw-r--r--   0 connor    (1000) connor    (1000)      923 2023-08-01 18:20:38.000000 py-doc-0.0.8/py_doc/multiplication.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 21:49:15.307024 py-doc-0.0.8/py_doc.egg-info/
+-rw-r--r--   0 connor    (1000) connor    (1000)     1119 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      230 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)       13 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/requires.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        7 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/top_level.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-08-01 21:49:15.307024 py-doc-0.0.8/setup.cfg
+-rw-r--r--   0 connor    (1000) connor    (1000)     1281 2023-08-01 21:46:52.000000 py-doc-0.0.8/setup.py
```

### Comparing `py-doc-0.0.6/PKG-INFO` & `py-doc-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-doc
-Version: 0.0.6
+Version: 0.0.8
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 
 # PyDoc
 A library for interacting with pdf documents.
 
 ### Installation
 ```
-pip install py_doc
+pip install py-doc
 ```
 
 ### Get Started
 How to use the library:
 
 ```python
 from py_doc import Multiplication
@@ -34,7 +34,11 @@
 # Instantiate a Multiplication object
 multiplication = Multiplication(2)
 
 # Call the multiply method
 result = multiplication.multiply(5)
 ```
 
+### Documentation
+The documentation for this library can be found [here](https://py-doc.readthedocs.io/en/latest/index.html#).
+
+
```

### Comparing `py-doc-0.0.6/py_doc/multiplication.py` & `py-doc-0.0.8/py_doc/multiplication.py`

 * *Files identical despite different names*

### Comparing `py-doc-0.0.6/py_doc.egg-info/PKG-INFO` & `py-doc-0.0.8/py_doc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-doc
-Version: 0.0.6
+Version: 0.0.8
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 
 # PyDoc
 A library for interacting with pdf documents.
 
 ### Installation
 ```
-pip install py_doc
+pip install py-doc
 ```
 
 ### Get Started
 How to use the library:
 
 ```python
 from py_doc import Multiplication
@@ -34,7 +34,11 @@
 # Instantiate a Multiplication object
 multiplication = Multiplication(2)
 
 # Call the multiply method
 result = multiplication.multiply(5)
 ```
 
+### Documentation
+The documentation for this library can be found [here](https://py-doc.readthedocs.io/en/latest/index.html#).
+
+
```

### Comparing `py-doc-0.0.6/setup.py` & `py-doc-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="py-doc",
-    version="0.0.6",
+    version="0.0.8",
     description="Used for working with documentations in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Connor Holm",
     author_email="connorjholm@gmail.com",
     license="MIT",
```

