# Comparing `tmp/cwtune-0.1.15.tar.gz` & `tmp/cwtune-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwtune-0.1.15.tar", last modified: Tue Aug  1 11:55:11 2023, max compression
+gzip compressed data, was "cwtune-0.1.16.tar", last modified: Tue Aug  1 12:04:22 2023, max compression
```

## Comparing `cwtune-0.1.15.tar` & `cwtune-0.1.16.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:55:11.216641 cwtune-0.1.15/
--rw-r--r--   0 arran      (501) staff       (20)     1204 2023-07-25 11:17:40.000000 cwtune-0.1.15/.gitignore
--rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.1.15/LICENSE
--rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:55:11.216972 cwtune-0.1.15/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      860 2023-07-11 11:02:07.000000 cwtune-0.1.15/README.rst
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:55:11.170864 cwtune-0.1.15/cwtune/
--rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.1.15/cwtune/__init__.py
--rw-r--r--   0 arran      (501) staff       (20)     9129 2023-08-01 11:54:44.000000 cwtune-0.1.15/cwtune/analyze.py
--rw-r--r--   0 arran      (501) staff       (20)     5600 2023-08-01 11:54:31.000000 cwtune-0.1.15/cwtune/aws.py
--rw-r--r--   0 arran      (501) staff       (20)     1067 2023-08-01 11:42:12.000000 cwtune-0.1.15/cwtune/cli.py
--rw-r--r--   0 arran      (501) staff       (20)     2400 2023-07-24 12:37:41.000000 cwtune-0.1.15/cwtune/timeseries.py
--rw-r--r--   0 arran      (501) staff       (20)     2760 2023-07-25 12:45:29.000000 cwtune-0.1.15/cwtune/utils.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:55:11.191642 cwtune-0.1.15/cwtune.egg-info/
--rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:55:10.000000 cwtune-0.1.15/cwtune.egg-info/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      565 2023-08-01 11:55:10.000000 cwtune-0.1.15/cwtune.egg-info/SOURCES.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:55:10.000000 cwtune-0.1.15/cwtune.egg-info/dependency_links.txt
--rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-01 11:55:10.000000 cwtune-0.1.15/cwtune.egg-info/entry_points.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:55:10.000000 cwtune-0.1.15/cwtune.egg-info/not-zip-safe
--rw-r--r--   0 arran      (501) staff       (20)       65 2023-08-01 11:55:10.000000 cwtune-0.1.15/cwtune.egg-info/requires.txt
--rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-01 11:55:10.000000 cwtune-0.1.15/cwtune.egg-info/top_level.txt
--rw-r--r--   0 arran      (501) staff       (20)       66 2023-07-25 12:31:11.000000 cwtune-0.1.15/requirements.txt
--rw-r--r--   0 arran      (501) staff       (20)      424 2023-08-01 11:55:11.217753 cwtune-0.1.15/setup.cfg
--rw-r--r--   0 arran      (501) staff       (20)     1338 2023-08-01 11:54:53.000000 cwtune-0.1.15/setup.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:55:11.199618 cwtune-0.1.15/tests/
--rw-r--r--   0 arran      (501) staff       (20)       36 2023-07-11 11:02:07.000000 cwtune-0.1.15/tests/__init__.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:55:11.214086 cwtune-0.1.15/tests/__pycache__/
--rw-r--r--   0 arran      (501) staff       (20)      208 2023-07-11 11:10:33.000000 cwtune-0.1.15/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     4029 2023-07-11 11:10:33.000000 cwtune-0.1.15/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc
--rw-r--r--   0 arran      (501) staff       (20)     7071 2023-07-17 14:03:14.000000 cwtune-0.1.15/tests/__pycache__/test_cwtune.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     3754 2023-07-17 14:03:13.000000 cwtune-0.1.15/tests/test_cwtune.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 12:04:22.453888 cwtune-0.1.16/
+-rw-r--r--   0 arran      (501) staff       (20)     1204 2023-07-25 11:17:40.000000 cwtune-0.1.16/.gitignore
+-rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.1.16/LICENSE
+-rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 12:04:22.454079 cwtune-0.1.16/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      860 2023-07-11 11:02:07.000000 cwtune-0.1.16/README.rst
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 12:04:22.412242 cwtune-0.1.16/cwtune/
+-rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.1.16/cwtune/__init__.py
+-rw-r--r--   0 arran      (501) staff       (20)     9129 2023-08-01 11:54:44.000000 cwtune-0.1.16/cwtune/analyze.py
+-rw-r--r--   0 arran      (501) staff       (20)     5600 2023-08-01 11:54:31.000000 cwtune-0.1.16/cwtune/aws.py
+-rw-r--r--   0 arran      (501) staff       (20)     1067 2023-08-01 11:42:12.000000 cwtune-0.1.16/cwtune/cli.py
+-rw-r--r--   0 arran      (501) staff       (20)     2400 2023-07-24 12:37:41.000000 cwtune-0.1.16/cwtune/timeseries.py
+-rw-r--r--   0 arran      (501) staff       (20)     2760 2023-07-25 12:45:29.000000 cwtune-0.1.16/cwtune/utils.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 12:04:22.442402 cwtune-0.1.16/cwtune.egg-info/
+-rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 12:04:21.000000 cwtune-0.1.16/cwtune.egg-info/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      565 2023-08-01 12:04:22.000000 cwtune-0.1.16/cwtune.egg-info/SOURCES.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 12:04:21.000000 cwtune-0.1.16/cwtune.egg-info/dependency_links.txt
+-rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-01 12:04:21.000000 cwtune-0.1.16/cwtune.egg-info/entry_points.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 12:04:21.000000 cwtune-0.1.16/cwtune.egg-info/not-zip-safe
+-rw-r--r--   0 arran      (501) staff       (20)       65 2023-08-01 12:04:21.000000 cwtune-0.1.16/cwtune.egg-info/requires.txt
+-rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-01 12:04:21.000000 cwtune-0.1.16/cwtune.egg-info/top_level.txt
+-rw-r--r--   0 arran      (501) staff       (20)       64 2023-08-01 12:03:14.000000 cwtune-0.1.16/requirements.txt
+-rw-r--r--   0 arran      (501) staff       (20)      424 2023-08-01 12:04:22.456039 cwtune-0.1.16/setup.cfg
+-rw-r--r--   0 arran      (501) staff       (20)     1338 2023-08-01 12:03:29.000000 cwtune-0.1.16/setup.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 12:04:22.447367 cwtune-0.1.16/tests/
+-rw-r--r--   0 arran      (501) staff       (20)       36 2023-07-11 11:02:07.000000 cwtune-0.1.16/tests/__init__.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 12:04:22.452484 cwtune-0.1.16/tests/__pycache__/
+-rw-r--r--   0 arran      (501) staff       (20)      208 2023-07-11 11:10:33.000000 cwtune-0.1.16/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     4029 2023-07-11 11:10:33.000000 cwtune-0.1.16/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     7071 2023-07-17 14:03:14.000000 cwtune-0.1.16/tests/__pycache__/test_cwtune.cpython-311.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     3754 2023-07-17 14:03:13.000000 cwtune-0.1.16/tests/test_cwtune.py
```

### Comparing `cwtune-0.1.15/.gitignore` & `cwtune-0.1.16/.gitignore`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/LICENSE` & `cwtune-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/PKG-INFO` & `cwtune-0.1.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.1.15
+Version: 0.1.16
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.1.15/README.rst` & `cwtune-0.1.16/README.rst`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/cwtune/analyze.py` & `cwtune-0.1.16/cwtune/analyze.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/cwtune/aws.py` & `cwtune-0.1.16/cwtune/aws.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/cwtune/cli.py` & `cwtune-0.1.16/cwtune/cli.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/cwtune/timeseries.py` & `cwtune-0.1.16/cwtune/timeseries.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/cwtune/utils.py` & `cwtune-0.1.16/cwtune/utils.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/cwtune.egg-info/PKG-INFO` & `cwtune-0.1.16/cwtune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.1.15
+Version: 0.1.16
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.1.15/cwtune.egg-info/SOURCES.txt` & `cwtune-0.1.16/cwtune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/setup.py` & `cwtune-0.1.16/setup.py`

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
-    version='0.1.15',
+    version='0.1.16',
     zip_safe=False,
 )
```

### Comparing `cwtune-0.1.15/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc` & `cwtune-0.1.16/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/tests/__pycache__/test_cwtune.cpython-311.pyc` & `cwtune-0.1.16/tests/__pycache__/test_cwtune.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.15/tests/test_cwtune.py` & `cwtune-0.1.16/tests/test_cwtune.py`

 * *Files identical despite different names*

