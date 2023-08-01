# Comparing `tmp/gsp_python-0.0.8.tar.gz` & `tmp/gsp_python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsp_python-0.0.8.tar", last modified: Tue Aug  1 21:35:22 2023, max compression
+gzip compressed data, was "gsp_python-0.0.9.tar", last modified: Tue Aug  1 21:36:21 2023, max compression
```

## Comparing `gsp_python-0.0.8.tar` & `gsp_python-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 21:35:22.632389 gsp_python-0.0.8/
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1065 2023-07-31 17:58:32.000000 gsp_python-0.0.8/LICENSE
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1697 2023-08-01 21:35:22.632102 gsp_python-0.0.8/PKG-INFO
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1287 2023-08-01 21:33:52.000000 gsp_python-0.0.8/README.md
-drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 21:35:22.629735 gsp_python-0.0.8/gsp_python/
--rw-r--r--   0 ilariaritelli   (501) staff       (20)      167 2023-08-01 10:02:33.000000 gsp_python-0.0.8/gsp_python/__init__.py
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     6110 2023-08-01 21:18:39.000000 gsp_python-0.0.8/gsp_python/__main__.py
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     3263 2023-07-31 20:30:17.000000 gsp_python-0.0.8/gsp_python/dataset_gen.py
--rw-r--r--   0 ilariaritelli   (501) staff       (20)    20236 2023-07-31 20:31:04.000000 gsp_python-0.0.8/gsp_python/gsp.py
-drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 21:35:22.631577 gsp_python-0.0.8/gsp_python.egg-info/
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1697 2023-08-01 21:35:22.000000 gsp_python-0.0.8/gsp_python.egg-info/PKG-INFO
--rw-r--r--   0 ilariaritelli   (501) staff       (20)      252 2023-08-01 21:35:22.000000 gsp_python-0.0.8/gsp_python.egg-info/SOURCES.txt
--rw-r--r--   0 ilariaritelli   (501) staff       (20)        1 2023-08-01 21:35:22.000000 gsp_python-0.0.8/gsp_python.egg-info/dependency_links.txt
--rw-r--r--   0 ilariaritelli   (501) staff       (20)       11 2023-08-01 21:35:22.000000 gsp_python-0.0.8/gsp_python.egg-info/top_level.txt
--rw-r--r--   0 ilariaritelli   (501) staff       (20)       38 2023-08-01 21:35:22.632505 gsp_python-0.0.8/setup.cfg
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1000 2023-08-01 21:32:35.000000 gsp_python-0.0.8/setup.py
+drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 21:36:21.189973 gsp_python-0.0.9/
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1065 2023-07-31 17:58:32.000000 gsp_python-0.0.9/LICENSE
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1696 2023-08-01 21:36:21.189718 gsp_python-0.0.9/PKG-INFO
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1286 2023-08-01 21:36:08.000000 gsp_python-0.0.9/README.md
+drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 21:36:21.187596 gsp_python-0.0.9/gsp_python/
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)      167 2023-08-01 10:02:33.000000 gsp_python-0.0.9/gsp_python/__init__.py
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     6110 2023-08-01 21:18:39.000000 gsp_python-0.0.9/gsp_python/__main__.py
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     3263 2023-07-31 20:30:17.000000 gsp_python-0.0.9/gsp_python/dataset_gen.py
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)    20236 2023-07-31 20:31:04.000000 gsp_python-0.0.9/gsp_python/gsp.py
+drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 21:36:21.189218 gsp_python-0.0.9/gsp_python.egg-info/
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1696 2023-08-01 21:36:21.000000 gsp_python-0.0.9/gsp_python.egg-info/PKG-INFO
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)      252 2023-08-01 21:36:21.000000 gsp_python-0.0.9/gsp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)        1 2023-08-01 21:36:21.000000 gsp_python-0.0.9/gsp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)       11 2023-08-01 21:36:21.000000 gsp_python-0.0.9/gsp_python.egg-info/top_level.txt
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)       38 2023-08-01 21:36:21.190096 gsp_python-0.0.9/setup.cfg
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1000 2023-08-01 21:36:18.000000 gsp_python-0.0.9/setup.py
```

### Comparing `gsp_python-0.0.8/LICENSE` & `gsp_python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gsp_python-0.0.8/PKG-INFO` & `gsp_python-0.0.9/gsp_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gsp_python
-Version: 0.0.8
+Name: gsp-python
+Version: 0.0.9
 Summary: GSP Python implementation
 Author: Slocon
 Author-email: <79758160+Slocon00@users.noreply.github.com>
 Project-URL: Source, https://github.com/Slocon00/GSP-python
 Keywords: python,gsp,data mining,sequential pattern mining,seuence mining
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -27,15 +27,15 @@
 ```
 
 ### Usage
 
 To run the gsp algorithm:
 
 ```
-python3 -m gsp_pythonn GSP infile outfile minsup -t maxgap mingap maxspan
+python3 -m gsp_python GSP infile outfile minsup -t maxgap mingap maxspan
 ```
 
 To generate a random dataset:
 
 ```
 python3 -m gsp_python DatasetGen outfile size nevents maxevents avgelems
 ```
```

### Comparing `gsp_python-0.0.8/README.md` & `gsp_python-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```
 
 ### Usage
 
 To run the gsp algorithm:
 
 ```
-python3 -m gsp_pythonn GSP infile outfile minsup -t maxgap mingap maxspan
+python3 -m gsp_python GSP infile outfile minsup -t maxgap mingap maxspan
 ```
 
 To generate a random dataset:
 
 ```
 python3 -m gsp_python DatasetGen outfile size nevents maxevents avgelems
 ```
```

### Comparing `gsp_python-0.0.8/gsp_python/__main__.py` & `gsp_python-0.0.9/gsp_python/__main__.py`

 * *Files identical despite different names*

### Comparing `gsp_python-0.0.8/gsp_python/dataset_gen.py` & `gsp_python-0.0.9/gsp_python/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `gsp_python-0.0.8/gsp_python/gsp.py` & `gsp_python-0.0.9/gsp_python/gsp.py`

 * *Files identical despite different names*

### Comparing `gsp_python-0.0.8/gsp_python.egg-info/PKG-INFO` & `gsp_python-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gsp-python
-Version: 0.0.8
+Name: gsp_python
+Version: 0.0.9
 Summary: GSP Python implementation
 Author: Slocon
 Author-email: <79758160+Slocon00@users.noreply.github.com>
 Project-URL: Source, https://github.com/Slocon00/GSP-python
 Keywords: python,gsp,data mining,sequential pattern mining,seuence mining
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -27,15 +27,15 @@
 ```
 
 ### Usage
 
 To run the gsp algorithm:
 
 ```
-python3 -m gsp_pythonn GSP infile outfile minsup -t maxgap mingap maxspan
+python3 -m gsp_python GSP infile outfile minsup -t maxgap mingap maxspan
 ```
 
 To generate a random dataset:
 
 ```
 python3 -m gsp_python DatasetGen outfile size nevents maxevents avgelems
 ```
```

### Comparing `gsp_python-0.0.8/setup.py` & `gsp_python-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'GSP Python implementation'
 LONG_DESCRIPTION = 'A Python implementation of Generalized Sequential Patterns (GSP) algorithm for sequential pattern mining'
 
 # Setting up
 setup(
     name="gsp_python",
     version=VERSION,
```

