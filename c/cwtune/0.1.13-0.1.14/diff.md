# Comparing `tmp/cwtune-0.1.13.tar.gz` & `tmp/cwtune-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwtune-0.1.13.tar", last modified: Tue Aug  1 11:43:46 2023, max compression
+gzip compressed data, was "cwtune-0.1.14.tar", last modified: Tue Aug  1 11:47:42 2023, max compression
```

## Comparing `cwtune-0.1.13.tar` & `cwtune-0.1.14.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:43:46.622956 cwtune-0.1.13/
--rw-r--r--   0 arran      (501) staff       (20)     1204 2023-07-25 11:17:40.000000 cwtune-0.1.13/.gitignore
--rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.1.13/LICENSE
--rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:43:46.624147 cwtune-0.1.13/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      860 2023-07-11 11:02:07.000000 cwtune-0.1.13/README.rst
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:43:46.605327 cwtune-0.1.13/cwtune/
--rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.1.13/cwtune/__init__.py
--rw-r--r--   0 arran      (501) staff       (20)     9126 2023-07-25 15:12:09.000000 cwtune-0.1.13/cwtune/analyze.py
--rw-r--r--   0 arran      (501) staff       (20)     5599 2023-07-25 10:25:39.000000 cwtune-0.1.13/cwtune/aws.py
--rw-r--r--   0 arran      (501) staff       (20)     1067 2023-08-01 11:42:12.000000 cwtune-0.1.13/cwtune/cli.py
--rw-r--r--   0 arran      (501) staff       (20)     2400 2023-07-24 12:37:41.000000 cwtune-0.1.13/cwtune/timeseries.py
--rw-r--r--   0 arran      (501) staff       (20)     2760 2023-07-25 12:45:29.000000 cwtune-0.1.13/cwtune/utils.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:43:46.613891 cwtune-0.1.13/cwtune.egg-info/
--rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:43:46.000000 cwtune-0.1.13/cwtune.egg-info/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      565 2023-08-01 11:43:46.000000 cwtune-0.1.13/cwtune.egg-info/SOURCES.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:43:46.000000 cwtune-0.1.13/cwtune.egg-info/dependency_links.txt
--rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-01 11:43:46.000000 cwtune-0.1.13/cwtune.egg-info/entry_points.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:43:19.000000 cwtune-0.1.13/cwtune.egg-info/not-zip-safe
--rw-r--r--   0 arran      (501) staff       (20)       65 2023-08-01 11:43:46.000000 cwtune-0.1.13/cwtune.egg-info/requires.txt
--rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-01 11:43:46.000000 cwtune-0.1.13/cwtune.egg-info/top_level.txt
--rw-r--r--   0 arran      (501) staff       (20)       66 2023-07-25 12:31:11.000000 cwtune-0.1.13/requirements.txt
--rw-r--r--   0 arran      (501) staff       (20)      424 2023-08-01 11:43:46.625424 cwtune-0.1.13/setup.cfg
--rw-r--r--   0 arran      (501) staff       (20)     1338 2023-08-01 11:43:40.000000 cwtune-0.1.13/setup.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:43:46.616038 cwtune-0.1.13/tests/
--rw-r--r--   0 arran      (501) staff       (20)       36 2023-07-11 11:02:07.000000 cwtune-0.1.13/tests/__init__.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:43:46.621904 cwtune-0.1.13/tests/__pycache__/
--rw-r--r--   0 arran      (501) staff       (20)      208 2023-07-11 11:10:33.000000 cwtune-0.1.13/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     4029 2023-07-11 11:10:33.000000 cwtune-0.1.13/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc
--rw-r--r--   0 arran      (501) staff       (20)     7071 2023-07-17 14:03:14.000000 cwtune-0.1.13/tests/__pycache__/test_cwtune.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     3754 2023-07-17 14:03:13.000000 cwtune-0.1.13/tests/test_cwtune.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.245481 cwtune-0.1.14/
+-rw-r--r--   0 arran      (501) staff       (20)     1204 2023-07-25 11:17:40.000000 cwtune-0.1.14/.gitignore
+-rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.1.14/LICENSE
+-rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:47:42.245772 cwtune-0.1.14/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      860 2023-07-11 11:02:07.000000 cwtune-0.1.14/README.rst
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.155293 cwtune-0.1.14/cwtune/
+-rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.1.14/cwtune/__init__.py
+-rw-r--r--   0 arran      (501) staff       (20)     9129 2023-08-01 11:46:42.000000 cwtune-0.1.14/cwtune/analyze.py
+-rw-r--r--   0 arran      (501) staff       (20)     5599 2023-07-25 10:25:39.000000 cwtune-0.1.14/cwtune/aws.py
+-rw-r--r--   0 arran      (501) staff       (20)     1067 2023-08-01 11:42:12.000000 cwtune-0.1.14/cwtune/cli.py
+-rw-r--r--   0 arran      (501) staff       (20)     2400 2023-07-24 12:37:41.000000 cwtune-0.1.14/cwtune/timeseries.py
+-rw-r--r--   0 arran      (501) staff       (20)     2760 2023-07-25 12:45:29.000000 cwtune-0.1.14/cwtune/utils.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.165642 cwtune-0.1.14/cwtune.egg-info/
+-rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      565 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/SOURCES.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/dependency_links.txt
+-rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/entry_points.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/not-zip-safe
+-rw-r--r--   0 arran      (501) staff       (20)       65 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/requires.txt
+-rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/top_level.txt
+-rw-r--r--   0 arran      (501) staff       (20)       66 2023-07-25 12:31:11.000000 cwtune-0.1.14/requirements.txt
+-rw-r--r--   0 arran      (501) staff       (20)      424 2023-08-01 11:47:42.248702 cwtune-0.1.14/setup.cfg
+-rw-r--r--   0 arran      (501) staff       (20)     1338 2023-08-01 11:46:52.000000 cwtune-0.1.14/setup.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.171811 cwtune-0.1.14/tests/
+-rw-r--r--   0 arran      (501) staff       (20)       36 2023-07-11 11:02:07.000000 cwtune-0.1.14/tests/__init__.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.243670 cwtune-0.1.14/tests/__pycache__/
+-rw-r--r--   0 arran      (501) staff       (20)      208 2023-07-11 11:10:33.000000 cwtune-0.1.14/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     4029 2023-07-11 11:10:33.000000 cwtune-0.1.14/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     7071 2023-07-17 14:03:14.000000 cwtune-0.1.14/tests/__pycache__/test_cwtune.cpython-311.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     3754 2023-07-17 14:03:13.000000 cwtune-0.1.14/tests/test_cwtune.py
```

### Comparing `cwtune-0.1.13/.gitignore` & `cwtune-0.1.14/.gitignore`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/LICENSE` & `cwtune-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/PKG-INFO` & `cwtune-0.1.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.1.13
+Version: 0.1.14
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.1.13/README.rst` & `cwtune-0.1.14/README.rst`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/cwtune/analyze.py` & `cwtune-0.1.14/cwtune/analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import click
 from datetime import timedelta
 from terminaltables import AsciiTable
 from thefuzz import fuzz
 import json
 import math
-from utils import create_cloudwatch_link, format_timestamp, select_range
-from aws import list_metrics, get_metric_data, create_cloudwatch_alarm
-from timeseries import zero_pad, get_breaches, longest_breach
+from .utils import create_cloudwatch_link, format_timestamp, select_range
+from .aws import list_metrics, get_metric_data, create_cloudwatch_alarm
+from .timeseries import zero_pad, get_breaches, longest_breach
 
 # Define constants
 WEIGHTS = {'Namespace': 0.5, 'MetricName': 0.3, 'Dimensions': 0.3}
 MAX_ITERATIONS = 100
 
 
 def prompt_metric_search(metrics):
```

### Comparing `cwtune-0.1.13/cwtune/aws.py` & `cwtune-0.1.14/cwtune/aws.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/cwtune/cli.py` & `cwtune-0.1.14/cwtune/cli.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/cwtune/timeseries.py` & `cwtune-0.1.14/cwtune/timeseries.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/cwtune/utils.py` & `cwtune-0.1.14/cwtune/utils.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/cwtune.egg-info/PKG-INFO` & `cwtune-0.1.14/cwtune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.1.13
+Version: 0.1.14
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.1.13/cwtune.egg-info/SOURCES.txt` & `cwtune-0.1.14/cwtune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/setup.py` & `cwtune-0.1.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords='cwtune',
     name='cwtune',
     packages=find_packages(include=['cwtune', 'cwtune.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/availabl-co/cwtune',
-    version='0.1.13',
+    version='0.1.14',
     zip_safe=False,
 )
```

### Comparing `cwtune-0.1.13/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc` & `cwtune-0.1.14/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/tests/__pycache__/test_cwtune.cpython-311.pyc` & `cwtune-0.1.14/tests/__pycache__/test_cwtune.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.13/tests/test_cwtune.py` & `cwtune-0.1.14/tests/test_cwtune.py`

 * *Files identical despite different names*

