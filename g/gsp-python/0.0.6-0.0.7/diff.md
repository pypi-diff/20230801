# Comparing `tmp/gsp-python-0.0.6.tar.gz` & `tmp/gsp-python-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsp-python-0.0.6.tar", last modified: Tue Aug  1 13:02:46 2023, max compression
+gzip compressed data, was "gsp-python-0.0.7.tar", last modified: Tue Aug  1 21:24:46 2023, max compression
```

## Comparing `gsp-python-0.0.6.tar` & `gsp-python-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 13:02:46.032562 gsp-python-0.0.6/
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1065 2023-07-31 17:58:32.000000 gsp-python-0.0.6/LICENSE
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1688 2023-08-01 13:02:46.032290 gsp-python-0.0.6/PKG-INFO
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1278 2023-08-01 13:02:19.000000 gsp-python-0.0.6/README.md
-drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 13:02:46.028625 gsp-python-0.0.6/gsp-python/
--rw-r--r--   0 ilariaritelli   (501) staff       (20)      167 2023-08-01 10:02:33.000000 gsp-python-0.0.6/gsp-python/__init__.py
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     6101 2023-08-01 09:46:34.000000 gsp-python-0.0.6/gsp-python/__main__.py
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     3263 2023-07-31 20:30:17.000000 gsp-python-0.0.6/gsp-python/dataset_gen.py
--rw-r--r--   0 ilariaritelli   (501) staff       (20)    20236 2023-07-31 20:31:04.000000 gsp-python-0.0.6/gsp-python/gsp.py
-drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 13:02:46.031754 gsp-python-0.0.6/gsp_python.egg-info/
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1688 2023-08-01 13:02:46.000000 gsp-python-0.0.6/gsp_python.egg-info/PKG-INFO
--rw-r--r--   0 ilariaritelli   (501) staff       (20)      252 2023-08-01 13:02:46.000000 gsp-python-0.0.6/gsp_python.egg-info/SOURCES.txt
--rw-r--r--   0 ilariaritelli   (501) staff       (20)        1 2023-08-01 13:02:46.000000 gsp-python-0.0.6/gsp_python.egg-info/dependency_links.txt
--rw-r--r--   0 ilariaritelli   (501) staff       (20)       11 2023-08-01 13:02:46.000000 gsp-python-0.0.6/gsp_python.egg-info/top_level.txt
--rw-r--r--   0 ilariaritelli   (501) staff       (20)       38 2023-08-01 13:02:46.032666 gsp-python-0.0.6/setup.cfg
--rw-r--r--   0 ilariaritelli   (501) staff       (20)     1000 2023-08-01 13:02:36.000000 gsp-python-0.0.6/setup.py
+drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 21:24:46.309503 gsp-python-0.0.7/
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1065 2023-07-31 17:58:32.000000 gsp-python-0.0.7/LICENSE
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1688 2023-08-01 21:24:46.309249 gsp-python-0.0.7/PKG-INFO
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1278 2023-08-01 13:02:19.000000 gsp-python-0.0.7/README.md
+drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 21:24:46.307551 gsp-python-0.0.7/gsp-python/
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)      167 2023-08-01 10:02:33.000000 gsp-python-0.0.7/gsp-python/__init__.py
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     6110 2023-08-01 21:18:39.000000 gsp-python-0.0.7/gsp-python/__main__.py
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     3263 2023-07-31 20:30:17.000000 gsp-python-0.0.7/gsp-python/dataset_gen.py
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)    20236 2023-07-31 20:31:04.000000 gsp-python-0.0.7/gsp-python/gsp.py
+drwxr-xr-x   0 ilariaritelli   (501) staff       (20)        0 2023-08-01 21:24:46.308846 gsp-python-0.0.7/gsp_python.egg-info/
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1688 2023-08-01 21:24:46.000000 gsp-python-0.0.7/gsp_python.egg-info/PKG-INFO
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)      252 2023-08-01 21:24:46.000000 gsp-python-0.0.7/gsp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)        1 2023-08-01 21:24:46.000000 gsp-python-0.0.7/gsp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)       11 2023-08-01 21:24:46.000000 gsp-python-0.0.7/gsp_python.egg-info/top_level.txt
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)       38 2023-08-01 21:24:46.309620 gsp-python-0.0.7/setup.cfg
+-rw-r--r--   0 ilariaritelli   (501) staff       (20)     1000 2023-08-01 21:24:38.000000 gsp-python-0.0.7/setup.py
```

### Comparing `gsp-python-0.0.6/LICENSE` & `gsp-python-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gsp-python-0.0.6/PKG-INFO` & `gsp-python-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsp-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: GSP Python implementation
 Author: Slocon
 Author-email: <79758160+Slocon00@users.noreply.github.com>
 Project-URL: Source, https://github.com/Slocon00/GSP-python
 Keywords: python,gsp,data mining,sequential pattern mining,seuence mining
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `gsp-python-0.0.6/README.md` & `gsp-python-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gsp-python-0.0.6/gsp-python/__main__.py` & `gsp-python-0.0.7/gsp-python/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import math
 import sys
 import os.path
-import gsp
-from gsp import GSP
-from dataset_gen import DatasetGenerator
+from . import gsp
+from .gsp import GSP
+from .dataset_gen import DatasetGenerator
 import logging
 
 logging.basicConfig(level=logging.NOTSET, stream=sys.stdout,
                     format="%(levelname)s:%(module)s:%(message)s", force=True)
 
 
 def setup_subparsers(parser):
```

### Comparing `gsp-python-0.0.6/gsp-python/dataset_gen.py` & `gsp-python-0.0.7/gsp-python/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `gsp-python-0.0.6/gsp-python/gsp.py` & `gsp-python-0.0.7/gsp-python/gsp.py`

 * *Files identical despite different names*

### Comparing `gsp-python-0.0.6/gsp_python.egg-info/PKG-INFO` & `gsp-python-0.0.7/gsp_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsp-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: GSP Python implementation
 Author: Slocon
 Author-email: <79758160+Slocon00@users.noreply.github.com>
 Project-URL: Source, https://github.com/Slocon00/GSP-python
 Keywords: python,gsp,data mining,sequential pattern mining,seuence mining
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `gsp-python-0.0.6/setup.py` & `gsp-python-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'GSP Python implementation'
 LONG_DESCRIPTION = 'A Python implementation of Generalized Sequential Patterns (GSP) algorithm for sequential pattern mining'
 
 # Setting up
 setup(
     name="gsp-python",
     version=VERSION,
```

