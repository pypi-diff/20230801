# Comparing `tmp/py-doc-0.0.2.tar.gz` & `tmp/py_doc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-doc-0.0.2.tar", last modified: Sun Jul 30 20:48:51 2023, max compression
+gzip compressed data, was "py_doc-0.0.3.tar", last modified: Tue Aug  1 14:22:27 2023, max compression
```

## Comparing `py-doc-0.0.2.tar` & `py_doc-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-07-30 20:48:51.478728 py-doc-0.0.2/
--rw-r--r--   0 connor    (1000) connor    (1000)      987 2023-07-30 20:48:51.478728 py-doc-0.0.2/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      325 2023-07-30 20:17:38.000000 py-doc-0.0.2/README.md
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-07-30 20:48:51.477728 py-doc-0.0.2/py_doc.egg-info/
--rw-r--r--   0 connor    (1000) connor    (1000)      987 2023-07-30 20:48:51.000000 py-doc-0.0.2/py_doc.egg-info/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      209 2023-07-30 20:48:51.000000 py-doc-0.0.2/py_doc.egg-info/SOURCES.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-07-30 20:48:51.000000 py-doc-0.0.2/py_doc.egg-info/dependency_links.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        6 2023-07-30 20:48:51.000000 py-doc-0.0.2/py_doc.egg-info/requires.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        6 2023-07-30 20:48:51.000000 py-doc-0.0.2/py_doc.egg-info/top_level.txt
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-07-30 20:48:51.477728 py-doc-0.0.2/pydoc/
--rw-r--r--   0 connor    (1000) connor    (1000)       53 2023-07-30 20:04:47.000000 py-doc-0.0.2/pydoc/__init__.py
--rw-r--r--   0 connor    (1000) connor    (1000)      599 2023-07-30 20:08:59.000000 py-doc-0.0.2/pydoc/multiplication.py
--rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-07-30 20:48:51.478728 py-doc-0.0.2/setup.cfg
--rw-r--r--   0 connor    (1000) connor    (1000)     1269 2023-07-30 20:47:23.000000 py-doc-0.0.2/setup.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 14:22:27.446340 py_doc-0.0.3/
+-rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 14:22:27.445340 py_doc-0.0.3/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      328 2023-08-01 14:14:55.000000 py_doc-0.0.3/README.md
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 14:22:27.445340 py_doc-0.0.3/py_doc/
+-rw-r--r--   0 connor    (1000) connor    (1000)       48 2023-08-01 14:14:55.000000 py_doc-0.0.3/py_doc/__init__.py
+-rw-r--r--   0 connor    (1000) connor    (1000)      886 2023-07-30 21:46:54.000000 py_doc-0.0.3/py_doc/multiplication.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 14:22:27.445340 py_doc-0.0.3/py_doc.egg-info/
+-rw-r--r--   0 connor    (1000) connor    (1000)      990 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      211 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        6 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/requires.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        7 2023-08-01 14:22:27.000000 py_doc-0.0.3/py_doc.egg-info/top_level.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-08-01 14:22:27.446340 py_doc-0.0.3/setup.cfg
+-rw-r--r--   0 connor    (1000) connor    (1000)     1270 2023-08-01 14:21:26.000000 py_doc-0.0.3/setup.py
```

### Comparing `py-doc-0.0.2/PKG-INFO` & `py_doc-0.0.3/py_doc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-doc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,21 +18,22 @@
 Description-Content-Type: text/markdown
 
 # PyDoc
 A library for interacting with pdf documents.
 
 ### Installation
 ```
-pip install pydoc
+pip install py_doc
 ```
 
 ### Get Started
 How to use the library:
+
 ```python
-from pydoc import Multiplication
+from py_doc import Multiplication
 
 # Instantiate a Multiplication object
 multiplication = Multiplication(2)
 
 # Call the multiply method
 result = multiplication.multiply(5)
 ```
```

### Comparing `py-doc-0.0.2/py_doc.egg-info/PKG-INFO` & `py_doc-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-doc
-Version: 0.0.2
+Name: py_doc
+Version: 0.0.3
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,21 +18,22 @@
 Description-Content-Type: text/markdown
 
 # PyDoc
 A library for interacting with pdf documents.
 
 ### Installation
 ```
-pip install pydoc
+pip install py_doc
 ```
 
 ### Get Started
 How to use the library:
+
 ```python
-from pydoc import Multiplication
+from py_doc import Multiplication
 
 # Instantiate a Multiplication object
 multiplication = Multiplication(2)
 
 # Call the multiply method
 result = multiplication.multiply(5)
 ```
```

### Comparing `py-doc-0.0.2/setup.py` & `py_doc-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
-    name="py-doc",
-    version="0.0.2",
+    name="py_doc",
+    version="0.0.3",
     description="Used for working with documentations in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Connor Holm",
     author_email="connorjholm@gmail.com",
     license="MIT",
@@ -30,11 +30,11 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
-    packages=["pydoc"],
+    packages=["py_doc"],
     include_package_data=True,
     install_requires=["numpy"]
 )
```

