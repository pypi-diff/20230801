# Comparing `tmp/aws-fsx-lifecycle-status-monitor-0.0.7.tar.gz` & `tmp/aws-fsx-lifecycle-status-monitor-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-fsx-lifecycle-status-monitor-0.0.7.tar", last modified: Thu Jul 20 17:39:45 2023, max compression
+gzip compressed data, was "aws-fsx-lifecycle-status-monitor-0.0.8.tar", last modified: Tue Aug  1 04:17:31 2023, max compression
```

## Comparing `aws-fsx-lifecycle-status-monitor-0.0.7.tar` & `aws-fsx-lifecycle-status-monitor-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   452790 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:39:33.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:45.145429 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 17:39:45.000000 aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.759951 aws-fsx-lifecycle-status-monitor-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   452794 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.7/LICENSE` & `aws-fsx-lifecycle-status-monitor-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.7/PKG-INFO` & `aws-fsx-lifecycle-status-monitor-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-fsx-lifecycle-status-monitor
-Version: 0.0.7
+Version: 0.0.8
 Summary: aws-fsx-lifecycle-status-monitor
 Home-page: https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/AWS-FSx-Lifecycle-Status-Monitor
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.7/setup.py` & `aws-fsx-lifecycle-status-monitor-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-fsx-lifecycle-status-monitor",
-    "version": "0.0.7",
+    "version": "0.0.8",
     "description": "aws-fsx-lifecycle-status-monitor",
     "license": "Apache-2.0",
     "url": "https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_fsx_lifecycle_status_monitor",
         "aws_fsx_lifecycle_status_monitor._jsii"
     ],
     "package_data": {
         "aws_fsx_lifecycle_status_monitor._jsii": [
-            "aws-fsx-lifecycle-status-monitor@0.0.7.jsii.tgz"
+            "aws-fsx-lifecycle-status-monitor@0.0.8.jsii.tgz"
         ],
         "aws_fsx_lifecycle_status_monitor": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor/__init__.py` & `aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO` & `aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-fsx-lifecycle-status-monitor
-Version: 0.0.7
+Version: 0.0.8
 Summary: aws-fsx-lifecycle-status-monitor
 Home-page: https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/AWS-FSx-Lifecycle-Status-Monitor
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.7/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt` & `aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_fsx_lifecycle_status_monitor/py.typed
 src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
 src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
 src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
-src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.7.jsii.tgz
+src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.8.jsii.tgz
```

