# Comparing `tmp/km-walk-2.2.0.tar.gz` & `tmp/km-walk-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "km-walk-2.2.0.tar", last modified: Thu Nov  3 18:59:16 2022, max compression
+gzip compressed data, was "km-walk-2.2.1.tar", last modified: Tue Aug  1 21:02:47 2023, max compression
```

## Comparing `km-walk-2.2.0.tar` & `km-walk-2.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 18:59:15.993565 km-walk-2.2.0/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1066 2022-11-03 17:42:57.000000 km-walk-2.2.0/LICENSE
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    10846 2022-11-03 18:59:15.992565 km-walk-2.2.0/PKG-INFO
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     9963 2022-11-03 18:58:57.000000 km-walk-2.2.0/README.rst
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 18:59:15.877564 km-walk-2.2.0/km/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       17 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/__init__.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       97 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/__main__.py
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 18:59:15.900565 km-walk-2.2.0/km/argparser/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       86 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/argparser/__init__.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      377 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/argparser/common.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1770 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/argparser/find_mutation.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1405 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/argparser/find_report.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      523 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/argparser/linear_kmin.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      302 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/argparser/min_cov.py
--rwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)     2435 2022-11-03 18:00:58.000000 km-walk-2.2.0/km/km.py
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 18:59:15.906565 km-walk-2.2.0/km/tests/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/tests/__init__.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    24988 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/tests/test_main.py
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 18:59:15.923565 km-walk-2.2.0/km/tools/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       72 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/tools/__init__.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1628 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/tools/find_mutation.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    12904 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/tools/find_report.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1670 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/tools/linear_kmin.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      774 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/tools/min_cov.py
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 18:59:15.961565 km-walk-2.2.0/km/utils/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     8575 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/utils/Graph.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1969 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/utils/Jellyfish.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    27876 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/utils/MutationFinder.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     4531 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/utils/PathQuant.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1824 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/utils/Sequence.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       96 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/utils/__init__.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     3079 2022-11-03 17:42:57.000000 km-walk-2.2.0/km/utils/common.py
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 18:59:15.987565 km-walk-2.2.0/km_walk.egg-info/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    10846 2022-11-03 18:59:15.000000 km-walk-2.2.0/km_walk.egg-info/PKG-INFO
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      720 2022-11-03 18:59:15.000000 km-walk-2.2.0/km_walk.egg-info/SOURCES.txt
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)        1 2022-11-03 18:59:15.000000 km-walk-2.2.0/km_walk.egg-info/dependency_links.txt
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       35 2022-11-03 18:59:15.000000 km-walk-2.2.0/km_walk.egg-info/entry_points.txt
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       80 2022-11-03 18:59:15.000000 km-walk-2.2.0/km_walk.egg-info/requires.txt
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)        3 2022-11-03 18:59:15.000000 km-walk-2.2.0/km_walk.egg-info/top_level.txt
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       38 2022-11-03 18:59:15.994565 km-walk-2.2.0/setup.cfg
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     3981 2022-11-03 18:02:43.000000 km-walk-2.2.0/setup.py
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 21:02:47.769150 km-walk-2.2.1/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1066 2023-07-28 02:11:33.000000 km-walk-2.2.1/LICENSE
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    10895 2023-08-01 21:02:47.768150 km-walk-2.2.1/PKG-INFO
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     9652 2023-08-01 21:00:27.000000 km-walk-2.2.1/README.rst
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 21:02:47.648149 km-walk-2.2.1/km/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       17 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/__init__.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       97 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/__main__.py
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 21:02:47.674149 km-walk-2.2.1/km/argparser/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       86 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/argparser/__init__.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      377 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/argparser/common.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1764 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/argparser/find_mutation.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1405 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/argparser/find_report.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      523 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/argparser/linear_kmin.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      302 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/argparser/min_cov.py
+-rwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)     2435 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/km.py
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 21:02:47.683149 km-walk-2.2.1/km/tests/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)        0 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/tests/__init__.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    24988 2023-08-01 21:00:27.000000 km-walk-2.2.1/km/tests/test_main.py
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 21:02:47.708150 km-walk-2.2.1/km/tools/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       72 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/tools/__init__.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1628 2023-08-01 19:49:00.000000 km-walk-2.2.1/km/tools/find_mutation.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    12904 2023-08-01 19:49:00.000000 km-walk-2.2.1/km/tools/find_report.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1670 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/tools/linear_kmin.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      774 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/tools/min_cov.py
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 21:02:47.737150 km-walk-2.2.1/km/utils/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     8575 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/utils/Graph.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1969 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/utils/Jellyfish.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    28118 2023-08-01 21:00:27.000000 km-walk-2.2.1/km/utils/MutationFinder.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     4531 2023-08-01 21:00:27.000000 km-walk-2.2.1/km/utils/PathQuant.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1824 2023-08-01 19:49:00.000000 km-walk-2.2.1/km/utils/Sequence.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       96 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/utils/__init__.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     3078 2023-07-28 02:11:34.000000 km-walk-2.2.1/km/utils/common.py
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 21:02:47.763150 km-walk-2.2.1/km_walk.egg-info/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    10895 2023-08-01 21:02:47.000000 km-walk-2.2.1/km_walk.egg-info/PKG-INFO
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      720 2023-08-01 21:02:47.000000 km-walk-2.2.1/km_walk.egg-info/SOURCES.txt
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)        1 2023-08-01 21:02:47.000000 km-walk-2.2.1/km_walk.egg-info/dependency_links.txt
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       34 2023-08-01 21:02:47.000000 km-walk-2.2.1/km_walk.egg-info/entry_points.txt
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       80 2023-08-01 21:02:47.000000 km-walk-2.2.1/km_walk.egg-info/requires.txt
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)        3 2023-08-01 21:02:47.000000 km-walk-2.2.1/km_walk.egg-info/top_level.txt
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       38 2023-08-01 21:02:47.770150 km-walk-2.2.1/setup.cfg
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     4365 2023-08-01 21:00:27.000000 km-walk-2.2.1/setup.py
```

### Comparing `km-walk-2.2.0/LICENSE` & `km-walk-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/PKG-INFO` & `km-walk-2.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 Metadata-Version: 2.1
 Name: km-walk
-Version: 2.2.0
+Version: 2.2.1
 Summary: A software for RNA-seq investigation using k-mer decomposition
 Home-page: https://github.com/iric-soft/km
 Author: Albert Feghaly, Eric Audemard, Patrick Gendron, Sebastien Lemieux
 Author-email: bioinformatique@iric.ca
 License: MIT
 Keywords: k-mer RNA-seq variant sequencing
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 
 ===================================================================
 km : a software for RNA-seq investigation using k-mer decomposition
 ===================================================================
 
-+-------------------------------------------------------------+-----------------------------------------------------------------+-----------------------------------------------------------------------------+
-| .. image:: https://img.shields.io/badge/python-3.6-blue.svg | .. image:: https://travis-ci.org/iric-soft/km.svg?branch=master | .. image:: https://codecov.io/gh/iric-soft/km/branch/master/graph/badge.svg |
-|    :target: https://www.python.org/download/releases/3.6.0/ |    :target: https://travis-ci.org/iric-soft/km                  |    :target: https://codecov.io/gh/iric-soft/km/                             |
-+-------------------------------------------------------------+-----------------------------------------------------------------+-----------------------------------------------------------------------------+
++-------------+-----------+
+| |pyversion| | |codecov| |
++-------------+-----------+
+
+.. |pyversion| image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg
+   :target: https://pypi.org/project/km-walk/
+
+.. |codecov| image:: https://codecov.io/gh/iric-soft/km/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/iric-soft/km/
+
+.. |travis| image:: https://travis-ci.org/iric-soft/km.svg?branch=master
+   :target: https://travis-ci.org/iric-soft/km
 
 -------------
 Introduction:
 -------------
 
 This tool was developed to identify and quantify the occurence of single
 nucleotide variants, insertions, deletions and duplications in RNA-seq data.  Contrary to most tools that try to report all variants in a complete genome, here we instead propose to focus the analysis on small regions of interest.
@@ -238,9 +253,7 @@
 -------------------------------------------------
 Runing km on a real sample from downloaded fastq:
 -------------------------------------------------
 In the `example`_ folder you can find a script to help you to
 run a km analysis on one Leucegene sample.
 
   .. _example: https://github.com/iric-soft/km/tree/master/example
-
-
```

### Comparing `km-walk-2.2.0/README.rst` & `km-walk-2.2.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 
 ===================================================================
 km : a software for RNA-seq investigation using k-mer decomposition
 ===================================================================
 
-+-------------------------------------------------------------+-----------------------------------------------------------------+-----------------------------------------------------------------------------+
-| .. image:: https://img.shields.io/badge/python-3.6-blue.svg | .. image:: https://travis-ci.org/iric-soft/km.svg?branch=master | .. image:: https://codecov.io/gh/iric-soft/km/branch/master/graph/badge.svg |
-|    :target: https://www.python.org/download/releases/3.6.0/ |    :target: https://travis-ci.org/iric-soft/km                  |    :target: https://codecov.io/gh/iric-soft/km/                             |
-+-------------------------------------------------------------+-----------------------------------------------------------------+-----------------------------------------------------------------------------+
++-------------+-----------+
+| |pyversion| | |codecov| |
++-------------+-----------+
+
+.. |pyversion| image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg
+   :target: https://pypi.org/project/km-walk/
+
+.. |codecov| image:: https://codecov.io/gh/iric-soft/km/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/iric-soft/km/
+
+.. |travis| image:: https://travis-ci.org/iric-soft/km.svg?branch=master
+   :target: https://travis-ci.org/iric-soft/km
 
 -------------
 Introduction:
 -------------
 
 This tool was developed to identify and quantify the occurence of single
 nucleotide variants, insertions, deletions and duplications in RNA-seq data.  Contrary to most tools that try to report all variants in a complete genome, here we instead propose to focus the analysis on small regions of interest.
```

### Comparing `km-walk-2.2.0/km/argparser/find_mutation.py` & `km-walk-2.2.1/km/argparser/find_mutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         help="Maximum branchs until getback to target sequence (default: -b 10)",
         action="store",
         nargs='?',
         default=10,
         type=int)
     parser.add_argument(
         "-n", "--nodes",
-        help="Maximum nodes/kmers queried from jellyfish database (default: -n 5000)",
+        help="Maximum nodes queried from jellyfish database (default: -n 5000)",
         action="store",
         nargs='?',
         default=10000,
         type=int)
     parser.add_argument(
         "-g", "--graphical",
         help="Display coverage graph.",
```

### Comparing `km-walk-2.2.0/km/argparser/find_report.py` & `km-walk-2.2.1/km/argparser/find_report.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/argparser/linear_kmin.py` & `km-walk-2.2.1/km/argparser/linear_kmin.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/km.py` & `km-walk-2.2.1/km/km.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/tests/test_main.py` & `km-walk-2.2.1/km/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/tools/find_mutation.py` & `km-walk-2.2.1/km/tools/find_mutation.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/tools/find_report.py` & `km-walk-2.2.1/km/tools/find_report.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/tools/linear_kmin.py` & `km-walk-2.2.1/km/tools/linear_kmin.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/tools/min_cov.py` & `km-walk-2.2.1/km/tools/min_cov.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/utils/Graph.py` & `km-walk-2.2.1/km/utils/Graph.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/utils/Jellyfish.py` & `km-walk-2.2.1/km/utils/Jellyfish.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/utils/MutationFinder.py` & `km-walk-2.2.1/km/utils/MutationFinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 from . import Graph as ug
 from . import PathQuant as upq
 from . import Sequence as us
 from . import common as uc
 
 
+sys.setrecursionlimit(10000)
+
+
 PathDiff = namedtuple('PathDiff',
     [
         'start',
         'end_ref',
         'end_var',
         'kmers_ref',
         'kmers_var',
@@ -130,16 +133,14 @@
 
         self.__define_edges()
 
 
     def __extend(self, stack, breaks=0):
         """Recursive depth first search"""
 
-        sys.setrecursionlimit(10000)
-
         if len(stack) > self.max_stack:
             return
 
         if len(self.node_data.keys()) > self.max_node:
             sys.exit(
                 "ERROR: Node query count limit exceeded: max={}".format(
                     self.max_node
@@ -151,20 +152,21 @@
 
         if len(childs) > 1:
             breaks += 1
             if breaks > self.max_break:
                 return
 
         for child in childs:
-            ustack = stack + [child]
-            if child in self.node_data:
+            if child in self.node_data or child in set(stack):
+                if child in set(stack) and child not in self.node_data:
+                    log.info('Broke loop at kmer: %s' % child)
                 for p in stack:
                     self.node_data[p] = self.jf.query(p)
             else:
-                self.__extend(ustack, breaks)
+                self.__extend(stack + [child], breaks)
 
 
     def __define_edges(self):
         self.start_kmers = set()
         self.end_kmers = set()
 
         if type(self.refpath) == us.RefSeq:
@@ -176,17 +178,17 @@
             self.end_kmers.add(last)
 
         self.start_kmers_ix = set([self.kmer.index(k) for k in self.start_kmers])
         self.end_kmers_ix = set([self.kmer.index(k) for k in self.end_kmers])
 
         log.info("BigBang=%d, BigCrunch=%d" % (self.first_seq_ix, self.last_seq_ix))
         for s in self.start_kmers:
-            log.info("Start kmer %d %s" % (self.kmer.index(s), s))
+            log.info("Start kmer %s %d" % (s, self.kmer.index(s)))
         for e in self.end_kmers:
-            log.info("End   kmer %d %s" % (self.kmer.index(e), e))
+            log.info("End   kmer %s %d" % (e, self.kmer.index(e)))
 
 
     @staticmethod
     def diff_path_without_overlap(ref, seq, k):
         """Compare a reference sequence to an alternative path
         discovered through kmer walking.
 
@@ -606,14 +608,17 @@
 
         if graphical:
             for paths in self.alt_groups.values():
                 plot(paths)
 
         for path in self.alt_paths:
             ref_name, ref_index, alt_index = path.ref_name, path.ref_index, path.seq_index
+
+            log.info('Quantifying %s' % ref_name)
+
             quant = upq.PathQuant(
                 all_paths=[alt_index, ref_index],
                 counts=self.counts
             )
             quant.compute_coef()
             quant.refine_coef()
             quant.get_ratio()
@@ -750,14 +755,16 @@
         if graphical:
             import matplotlib.pyplot as plt
 
         for i, cluster in enumerate(clusters):
             ref_name, ref_path, clipped_paths, start_off = cluster
             num_cluster = i + 1
 
+            log.info('Quantifying %s in cluster mode' % ref_name)
+
             if graphical:
                 plt.figure(figsize=(10, 6))
                 plt.plot(
                     self.get_counts(ref_path),
                     label="Reference"
                 )
                 for path in clipped_paths:
```

### Comparing `km-walk-2.2.0/km/utils/PathQuant.py` & `km-walk-2.2.1/km/utils/PathQuant.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/utils/Sequence.py` & `km-walk-2.2.1/km/utils/Sequence.py`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/km/utils/common.py` & `km-walk-2.2.1/km/utils/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 
 def natsortkey(*args, rev_ix=[]):
     """Natural sorting of a string. For example: exon12 would
     come before exon2 with a regular sort, with natural sort
     the order would be exon2, exon12.
     """
 
-
     class reversor:
         def __init__(self, obj):
             self.obj = obj
 
         def __eq__(self, other):
             return other.obj == self.obj
```

### Comparing `km-walk-2.2.0/km_walk.egg-info/PKG-INFO` & `km-walk-2.2.1/km_walk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 Metadata-Version: 2.1
 Name: km-walk
-Version: 2.2.0
+Version: 2.2.1
 Summary: A software for RNA-seq investigation using k-mer decomposition
 Home-page: https://github.com/iric-soft/km
 Author: Albert Feghaly, Eric Audemard, Patrick Gendron, Sebastien Lemieux
 Author-email: bioinformatique@iric.ca
 License: MIT
 Keywords: k-mer RNA-seq variant sequencing
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 
 ===================================================================
 km : a software for RNA-seq investigation using k-mer decomposition
 ===================================================================
 
-+-------------------------------------------------------------+-----------------------------------------------------------------+-----------------------------------------------------------------------------+
-| .. image:: https://img.shields.io/badge/python-3.6-blue.svg | .. image:: https://travis-ci.org/iric-soft/km.svg?branch=master | .. image:: https://codecov.io/gh/iric-soft/km/branch/master/graph/badge.svg |
-|    :target: https://www.python.org/download/releases/3.6.0/ |    :target: https://travis-ci.org/iric-soft/km                  |    :target: https://codecov.io/gh/iric-soft/km/                             |
-+-------------------------------------------------------------+-----------------------------------------------------------------+-----------------------------------------------------------------------------+
++-------------+-----------+
+| |pyversion| | |codecov| |
++-------------+-----------+
+
+.. |pyversion| image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg
+   :target: https://pypi.org/project/km-walk/
+
+.. |codecov| image:: https://codecov.io/gh/iric-soft/km/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/iric-soft/km/
+
+.. |travis| image:: https://travis-ci.org/iric-soft/km.svg?branch=master
+   :target: https://travis-ci.org/iric-soft/km
 
 -------------
 Introduction:
 -------------
 
 This tool was developed to identify and quantify the occurence of single
 nucleotide variants, insertions, deletions and duplications in RNA-seq data.  Contrary to most tools that try to report all variants in a complete genome, here we instead propose to focus the analysis on small regions of interest.
@@ -238,9 +253,7 @@
 -------------------------------------------------
 Runing km on a real sample from downloaded fastq:
 -------------------------------------------------
 In the `example`_ folder you can find a script to help you to
 run a km analysis on one Leucegene sample.
 
   .. _example: https://github.com/iric-soft/km/tree/master/example
-
-
```

### Comparing `km-walk-2.2.0/km_walk.egg-info/SOURCES.txt` & `km-walk-2.2.1/km_walk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `km-walk-2.2.0/setup.py` & `km-walk-2.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 
 setup(
     name='km-walk',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.2.0',
+    version='2.2.1',
 
     description='A software for RNA-seq investigation using k-mer decomposition',
     long_description=long_description,
+    long_description_content_type='text/x-rst',
 
     # The project's main homepage.
     url='https://github.com/iric-soft/km',
 
     # Author details
     author='Albert Feghaly, Eric Audemard, Patrick Gendron, Sebastien Lemieux',
     author_email='bioinformatique@iric.ca',
@@ -50,15 +51,22 @@
         'Topic :: Software Development :: Build Tools',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 
         # Others
         'Natural Language :: English',
     ],
 
     # What does your project relate to?
     keywords='k-mer RNA-seq variant sequencing',
@@ -71,15 +79,15 @@
     # this:
     #   py_modules=["my_module"],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['numpy>=1.18.1', 'matplotlib>=3.3.4', 'pyjellyfish>=1.1.1', 'pytest>=6.2.0'],
+    install_requires=['numpy>=1.18.1', 'matplotlib>=3.3.4', 'pyjellyfish>=1.2.0', 'pytest>=6.2.0'],
     python_requires='>=3.6',
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
```

