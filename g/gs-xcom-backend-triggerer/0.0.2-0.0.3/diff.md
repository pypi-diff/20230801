# Comparing `tmp/gs_xcom_backend_triggerer-0.0.2.tar.gz` & `tmp/gs_xcom_backend_triggerer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs_xcom_backend_triggerer-0.0.2.tar", last modified: Tue Aug  1 05:22:26 2023, max compression
+gzip compressed data, was "gs_xcom_backend_triggerer-0.0.3.tar", last modified: Tue Aug  1 05:33:08 2023, max compression
```

## Comparing `gs_xcom_backend_triggerer-0.0.2.tar` & `gs_xcom_backend_triggerer-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 05:22:26.719673 gs_xcom_backend_triggerer-0.0.2/
--rw-rw-rw-   0        0        0      536 2023-08-01 05:22:26.718591 gs_xcom_backend_triggerer-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 05:22:26.706654 gs_xcom_backend_triggerer-0.0.2/gs_xcom_backend_triggerer/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:44:48.000000 gs_xcom_backend_triggerer-0.0.2/gs_xcom_backend_triggerer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-01 04:40:19.000000 gs_xcom_backend_triggerer-0.0.2/gs_xcom_backend_triggerer/gs_xcom_backend_triggerer.py
-drwxrwxrwx   0        0        0        0 2023-08-01 05:22:26.717259 gs_xcom_backend_triggerer-0.0.2/gs_xcom_backend_triggerer.egg-info/
--rw-rw-rw-   0        0        0      536 2023-08-01 05:22:26.000000 gs_xcom_backend_triggerer-0.0.2/gs_xcom_backend_triggerer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-08-01 05:22:26.000000 gs_xcom_backend_triggerer-0.0.2/gs_xcom_backend_triggerer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 05:22:26.000000 gs_xcom_backend_triggerer-0.0.2/gs_xcom_backend_triggerer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-08-01 05:22:26.000000 gs_xcom_backend_triggerer-0.0.2/gs_xcom_backend_triggerer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 05:22:26.719673 gs_xcom_backend_triggerer-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-08-01 05:20:41.000000 gs_xcom_backend_triggerer-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:33:08.130306 gs_xcom_backend_triggerer-0.0.3/
+-rw-rw-rw-   0        0        0      536 2023-08-01 05:33:08.129256 gs_xcom_backend_triggerer-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 05:33:08.092982 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:44:48.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend/__init__.py
+-rw-rw-rw-   0        0        0     1289 2023-08-01 05:25:23.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend/triggerer.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:33:08.127228 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/
+-rw-rw-rw-   0        0        0      536 2023-08-01 05:33:07.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-08-01 05:33:08.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:33:07.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-01 05:33:07.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 05:33:08.130306 gs_xcom_backend_triggerer-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      841 2023-08-01 05:33:04.000000 gs_xcom_backend_triggerer-0.0.3/setup.py
```

### Comparing `gs_xcom_backend_triggerer-0.0.2/PKG-INFO` & `gs_xcom_backend_triggerer-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs_xcom_backend_triggerer
-Version: 0.0.2
+Version: 0.0.3
 Summary: triggerer gs_xcom_backend module file
 Author: imvj202
 Author-email: imvj202@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `gs_xcom_backend_triggerer-0.0.2/gs_xcom_backend_triggerer.egg-info/PKG-INFO` & `gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-xcom-backend-triggerer
-Version: 0.0.2
+Version: 0.0.3
 Summary: triggerer gs_xcom_backend module file
 Author: imvj202
 Author-email: imvj202@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `gs_xcom_backend_triggerer-0.0.2/setup.py` & `gs_xcom_backend_triggerer-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'triggerer gs_xcom_backend module file'
 LONG_DESCRIPTION = 'triggerer gs_xcom_backend module file'
 
 # Setting up
 setup(
     name="gs_xcom_backend_triggerer",
     version=VERSION,
```

