# Comparing `tmp/pyssp_standard-0.2.tar.gz` & `tmp/pyssp_standard-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyssp_standard-0.2.tar", last modified: Tue Aug  1 16:16:48 2023, max compression
+gzip compressed data, was "pyssp_standard-0.3.tar", last modified: Tue Aug  1 16:25:24 2023, max compression
```

## Comparing `pyssp_standard-0.2.tar` & `pyssp_standard-0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:16:48.835430 pyssp_standard-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 16:16:36.000000 pyssp_standard-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 16:16:48.835430 pyssp_standard-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-01 16:16:36.000000 pyssp_standard-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:16:48.831430 pyssp_standard-0.2/pyssp_standard/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/common_content_ssc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/fmu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/parameter_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/transformation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:16:48.835430 pyssp_standard-0.2/pyssp_standard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 16:16:48.835430 pyssp_standard-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-01 16:16:36.000000 pyssp_standard-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:25:24.429735 pyssp_standard-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 16:25:14.000000 pyssp_standard-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 16:25:24.429735 pyssp_standard-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-01 16:25:14.000000 pyssp_standard-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:25:24.429735 pyssp_standard-0.3/pyssp_standard/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/common_content_ssc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/fmu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/parameter_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/ssb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/ssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/ssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/ssv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/transformation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-01 16:25:14.000000 pyssp_standard-0.3/pyssp_standard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:25:24.429735 pyssp_standard-0.3/pyssp_standard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 16:25:24.000000 pyssp_standard-0.3/pyssp_standard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 16:25:24.000000 pyssp_standard-0.3/pyssp_standard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:25:24.000000 pyssp_standard-0.3/pyssp_standard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 16:25:24.000000 pyssp_standard-0.3/pyssp_standard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 16:25:24.000000 pyssp_standard-0.3/pyssp_standard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 16:25:24.429735 pyssp_standard-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-01 16:25:14.000000 pyssp_standard-0.3/setup.py
```

### Comparing `pyssp_standard-0.2/LICENSE` & `pyssp_standard-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/PKG-INFO` & `pyssp_standard-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyssp_standard
-Version: 0.2
+Version: 0.3
 Summary: Simple python package for reading, modifying and creating files, specified in the SSP Standard
 Home-page: https://github.com/FGHaider/pyssp
 Download-URL: https://github.com/FGHaider/pyssp/archive/refs/tags/v_01.tar.gz
 Author: Fredrik Haider
 Author-email: 
 License: MIT
 Keywords: SSP,system,engineering
```

### Comparing `pyssp_standard-0.2/README.md` & `pyssp_standard-0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/common_content_ssc.py` & `pyssp_standard-0.3/pyssp_standard/common_content_ssc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from typing import TypedDict, List
 from lxml import etree as ET
 from lxml.etree import QName
 from dataclasses import dataclass, asdict, fields
 
-from utils import SSPStandard
+from pyssp_standard.utils import SSPStandard
 
 
 class Annotation(SSPStandard):  # TODO needs to read and not just create
 
     def __init__(self, type_declaration):
         """
         The SSP standard allows for the addition of annotations, when created they must contain at least one annotation.
```

### Comparing `pyssp_standard-0.2/pyssp_standard/fmu.py` & `pyssp_standard-0.3/pyssp_standard/fmu.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/parameter_types.py` & `pyssp_standard-0.3/pyssp_standard/parameter_types.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/ssb.py` & `pyssp_standard-0.3/pyssp_standard/ssb.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/ssd.py` & `pyssp_standard-0.3/pyssp_standard/ssd.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/ssm.py` & `pyssp_standard-0.3/pyssp_standard/ssm.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/ssp.py` & `pyssp_standard-0.3/pyssp_standard/ssp.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/ssv.py` & `pyssp_standard-0.3/pyssp_standard/ssv.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/transformation_types.py` & `pyssp_standard-0.3/pyssp_standard/transformation_types.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/unit.py` & `pyssp_standard-0.3/pyssp_standard/unit.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard/utils.py` & `pyssp_standard-0.3/pyssp_standard/utils.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/pyssp_standard.egg-info/PKG-INFO` & `pyssp_standard-0.3/pyssp_standard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyssp-standard
-Version: 0.2
+Version: 0.3
 Summary: Simple python package for reading, modifying and creating files, specified in the SSP Standard
 Home-page: https://github.com/FGHaider/pyssp
 Download-URL: https://github.com/FGHaider/pyssp/archive/refs/tags/v_01.tar.gz
 Author: Fredrik Haider
 Author-email: 
 License: MIT
 Keywords: SSP,system,engineering
```

### Comparing `pyssp_standard-0.2/pyssp_standard.egg-info/SOURCES.txt` & `pyssp_standard-0.3/pyssp_standard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.2/setup.py` & `pyssp_standard-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='pyssp_standard',
     packages=['pyssp_standard'],
-    version='0.2',
+    version='0.3',
     license='MIT',
     description='Simple python package for reading, modifying and creating files, specified in the SSP Standard',
     long_description='',
     long_description_content_type='text/markdown',
     author='Fredrik Haider',
     author_email='',
     url='https://github.com/FGHaider/pyssp',
```

