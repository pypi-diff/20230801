# Comparing `tmp/shareddata-2.2.6.tar.gz` & `tmp/shareddata-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.2.6.tar", last modified: Mon Jul 31 17:39:29 2023, max compression
+gzip compressed data, was "shareddata-2.2.7.tar", last modified: Tue Aug  1 10:28:45 2023, max compression
```

## Comparing `shareddata-2.2.6.tar` & `shareddata-2.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 17:39:29.304295 shareddata-2.2.6/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.2.6/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 17:39:29.304295 shareddata-2.2.6/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.2.6/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.2.6/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-31 17:39:29.304295 shareddata-2.2.6/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 17:39:29.304295 shareddata-2.2.6/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 17:39:29.304295 shareddata-2.2.6/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.2.6/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.2.6/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-07-29 20:08:59.000000 shareddata-2.2.6/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-07-29 18:19:38.000000 shareddata-2.2.6/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-07-29 20:09:03.000000 shareddata-2.2.6/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-07-31 11:49:07.000000 shareddata-2.2.6/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11195 2023-07-31 11:51:26.000000 shareddata-2.2.6/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.2.6/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-07-29 20:09:00.000000 shareddata-2.2.6/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-07-31 11:51:47.000000 shareddata-2.2.6/src/SharedData/RealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-07-31 09:53:00.000000 shareddata-2.2.6/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9030 2023-07-31 12:46:43.000000 shareddata-2.2.6/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28818 2023-07-31 10:09:34.000000 shareddata-2.2.6/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-07-31 12:53:11.000000 shareddata-2.2.6/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.2.6/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-07-31 10:19:55.000000 shareddata-2.2.6/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-07-31 17:38:51.000000 shareddata-2.2.6/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.2.6/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.2.6/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 17:39:29.304295 shareddata-2.2.6/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 17:39:29.000000 shareddata-2.2.6/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-07-31 17:39:29.000000 shareddata-2.2.6/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 17:39:29.000000 shareddata-2.2.6/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-31 17:39:29.000000 shareddata-2.2.6/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-31 17:39:29.000000 shareddata-2.2.6/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-01 10:28:45.418496 shareddata-2.2.7/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.2.7/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-01 10:28:45.418496 shareddata-2.2.7/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.2.7/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.2.7/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-01 10:28:45.418496 shareddata-2.2.7/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-01 10:28:45.418496 shareddata-2.2.7/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-01 10:28:45.418496 shareddata-2.2.7/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.2.7/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.2.7/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-07-29 20:08:59.000000 shareddata-2.2.7/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-07-29 18:19:38.000000 shareddata-2.2.7/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-07-29 20:09:03.000000 shareddata-2.2.7/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-07-31 11:49:07.000000 shareddata-2.2.7/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 10:28:18.000000 shareddata-2.2.7/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.2.7/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-07-29 20:09:00.000000 shareddata-2.2.7/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-07-31 11:51:47.000000 shareddata-2.2.7/src/SharedData/RealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-07-31 09:53:00.000000 shareddata-2.2.7/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9030 2023-07-31 12:46:43.000000 shareddata-2.2.7/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28818 2023-07-31 10:09:34.000000 shareddata-2.2.7/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-07-31 12:53:11.000000 shareddata-2.2.7/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.2.7/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-07-31 10:19:55.000000 shareddata-2.2.7/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-07-31 17:38:51.000000 shareddata-2.2.7/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.2.7/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.2.7/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-01 10:28:45.418496 shareddata-2.2.7/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.2.6/LICENSE` & `shareddata-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/PKG-INFO` & `shareddata-2.2.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.2.6
+Version: 2.2.7
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.2.6/README.md` & `shareddata-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/setup.cfg` & `shareddata-2.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.2.6
+version = 2.2.7
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.2.6/src/SharedData/AWSKinesis.py` & `shareddata-2.2.7/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/AWSS3.py` & `shareddata-2.2.7/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/DataFrame.py` & `shareddata-2.2.7/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/Defaults.py` & `shareddata-2.2.7/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/Logger.py` & `shareddata-2.2.7/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.2.7/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/Metadata.py` & `shareddata-2.2.7/src/SharedData/Metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import pandas as pd
 import numpy as np
 import time
 import subprocess
 from datetime import datetime, timedelta
 import gzip,io,shutil,hashlib
 
+
+import SharedData.Defaults as Defaults 
 from SharedData.Logger import Logger
 from SharedData.AWSS3 import S3Upload, S3ListFolder, S3Download, UpdateModTime
 
 class Metadata():
     
     def __init__(self, name, mode='rw', user='master'):
```

### Comparing `shareddata-2.2.6/src/SharedData/MultiProc.py` & `shareddata-2.2.7/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/RealTime.py` & `shareddata-2.2.7/src/SharedData/RealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/RealTimeProcess.py` & `shareddata-2.2.7/src/SharedData/RealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/SharedData.py` & `shareddata-2.2.7/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/SharedNumpy.py` & `shareddata-2.2.7/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/Table.py` & `shareddata-2.2.7/src/SharedData/Table.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/TableIndex.py` & `shareddata-2.2.7/src/SharedData/TableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/TableIndexJit.py` & `shareddata-2.2.7/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/TimeSeries.py` & `shareddata-2.2.7/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/TimeseriesContainer.py` & `shareddata-2.2.7/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/SharedData/Utils.py` & `shareddata-2.2.7/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.6/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.2.7/src/shareddata.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.2.6
+Version: 2.2.7
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.2.6/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.2.7/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

