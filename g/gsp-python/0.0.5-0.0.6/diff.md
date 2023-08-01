# Comparing `tmp/gsp-python-0.0.5.tar.gz` & `tmp/gsp-python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsp-python-0.0.5.tar", last modified: Tue Aug  1 10:06:48 2023, max compression
+gzip compressed data, was "gsp-python-0.0.6.tar", last modified: Tue Aug  1 13:02:46 2023, max compression
```

## Comparing `gsp-python-0.0.5.tar` & `gsp-python-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 10:06:48.622932 gsp-python-0.0.5/
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1065 2023-07-31 17:58:32.000000 gsp-python-0.0.5/LICENSE
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1684 2023-08-01 10:06:48.622436 gsp-python-0.0.5/PKG-INFO
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1274 2023-08-01 09:55:31.000000 gsp-python-0.0.5/README.md
-drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 10:06:48.617807 gsp-python-0.0.5/gsp-python/
--rw-r--r--   0 ilariaritelli   (501) staff       (20)      167 2023-08-01 10:02:33.000000 gsp-python-0.0.5/gsp-python/__init__.py
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     6101 2023-08-01 09:46:34.000000 gsp-python-0.0.5/gsp-python/__main__.py
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     3263 2023-07-31 20:30:17.000000 gsp-python-0.0.5/gsp-python/dataset_gen.py
--rw-r--r--   0 ilariaritelli   (501) staff       (20)    20236 2023-07-31 20:31:04.000000 gsp-python-0.0.5/gsp-python/gsp.py
-drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 10:06:48.621600 gsp-python-0.0.5/gsp_python.egg-info/
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1684 2023-08-01 10:06:48.000000 gsp-python-0.0.5/gsp_python.egg-info/PKG-INFO
--rw-r--r--   0 ilariaritelli   (501) staff       (20)      252 2023-08-01 10:06:48.000000 gsp-python-0.0.5/gsp_python.egg-info/SOURCES.txt
--rw-r--r--   0 ilariaritelli   (501) staff       (20)        1 2023-08-01 10:06:48.000000 gsp-python-0.0.5/gsp_python.egg-info/dependency_links.txt
--rw-r--r--   0 ilariaritelli   (501) staff       (20)       11 2023-08-01 10:06:48.000000 gsp-python-0.0.5/gsp_python.egg-info/top_level.txt
--rw-r--r--   0 ilariaritelli   (501) staff       (20)       38 2023-08-01 10:06:48.623151 gsp-python-0.0.5/setup.cfg
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1000 2023-08-01 10:03:19.000000 gsp-python-0.0.5/setup.py
+drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 13:02:46.032562 gsp-python-0.0.6/
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1065 2023-07-31 17:58:32.000000 gsp-python-0.0.6/LICENSE
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1688 2023-08-01 13:02:46.032290 gsp-python-0.0.6/PKG-INFO
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1278 2023-08-01 13:02:19.000000 gsp-python-0.0.6/README.md
+drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 13:02:46.028625 gsp-python-0.0.6/gsp-python/
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)      167 2023-08-01 10:02:33.000000 gsp-python-0.0.6/gsp-python/__init__.py
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     6101 2023-08-01 09:46:34.000000 gsp-python-0.0.6/gsp-python/__main__.py
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     3263 2023-07-31 20:30:17.000000 gsp-python-0.0.6/gsp-python/dataset_gen.py
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)    20236 2023-07-31 20:31:04.000000 gsp-python-0.0.6/gsp-python/gsp.py
+drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 13:02:46.031754 gsp-python-0.0.6/gsp_python.egg-info/
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1688 2023-08-01 13:02:46.000000 gsp-python-0.0.6/gsp_python.egg-info/PKG-INFO
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)      252 2023-08-01 13:02:46.000000 gsp-python-0.0.6/gsp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)        1 2023-08-01 13:02:46.000000 gsp-python-0.0.6/gsp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)       11 2023-08-01 13:02:46.000000 gsp-python-0.0.6/gsp_python.egg-info/top_level.txt
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)       38 2023-08-01 13:02:46.032666 gsp-python-0.0.6/setup.cfg
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1000 2023-08-01 13:02:36.000000 gsp-python-0.0.6/setup.py
```

### Comparing `gsp-python-0.0.5/LICENSE` & `gsp-python-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gsp-python-0.0.5/PKG-INFO` & `gsp-python-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsp-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: GSP Python implementation
 Author: Slocon
 Author-email: <79758160+Slocon00@users.noreply.github.com>
 Project-URL: Source, https://github.com/Slocon00/GSP-python
 Keywords: python,gsp,data mining,sequential pattern mining,seuence mining
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 dataset. This implementation includes parameters for the _mingap_, _maxgap_, and _maxspan_ time constraints.
 
 The project also features a simple dataset generator.
 
 ### Installation
 
 ```
-python3 -m pip install gsp_py
+python3 -m pip install gsp-python
 ```
 
 ### Usage
 
 To run the gsp algorithm:
 
 ```
```

### Comparing `gsp-python-0.0.5/README.md` & `gsp-python-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 dataset. This implementation includes parameters for the _mingap_, _maxgap_, and _maxspan_ time constraints.
 
 The project also features a simple dataset generator.
 
 ### Installation
 
 ```
-python3 -m pip install gsp_py
+python3 -m pip install gsp-python
 ```
 
 ### Usage
 
 To run the gsp algorithm:
 
 ```
```

### Comparing `gsp-python-0.0.5/gsp-python/__main__.py` & `gsp-python-0.0.6/gsp-python/__main__.py`

 * *Files identical despite different names*

### Comparing `gsp-python-0.0.5/gsp-python/dataset_gen.py` & `gsp-python-0.0.6/gsp-python/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `gsp-python-0.0.5/gsp-python/gsp.py` & `gsp-python-0.0.6/gsp-python/gsp.py`

 * *Files identical despite different names*

### Comparing `gsp-python-0.0.5/gsp_python.egg-info/PKG-INFO` & `gsp-python-0.0.6/gsp_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsp-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: GSP Python implementation
 Author: Slocon
 Author-email: <79758160+Slocon00@users.noreply.github.com>
 Project-URL: Source, https://github.com/Slocon00/GSP-python
 Keywords: python,gsp,data mining,sequential pattern mining,seuence mining
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 dataset. This implementation includes parameters for the _mingap_, _maxgap_, and _maxspan_ time constraints.
 
 The project also features a simple dataset generator.
 
 ### Installation
 
 ```
-python3 -m pip install gsp_py
+python3 -m pip install gsp-python
 ```
 
 ### Usage
 
 To run the gsp algorithm:
 
 ```
```

### Comparing `gsp-python-0.0.5/setup.py` & `gsp-python-0.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'GSP Python implementation'
 LONG_DESCRIPTION = 'A Python implementation of Generalized Sequential Patterns (GSP) algorithm for sequential pattern mining'
 
 # Setting up
 setup(
     name="gsp-python",
     version=VERSION,
```

