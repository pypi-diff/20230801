# Comparing `tmp/mypy-boto3-internetmonitor-1.28.16.tar.gz` & `tmp/mypy-boto3-internetmonitor-1.28.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-internetmonitor-1.28.16.tar", last modified: Tue Aug  1 11:36:57 2023, max compression
+gzip compressed data, was "mypy-boto3-internetmonitor-1.28.17.tar", last modified: Tue Aug  1 19:33:25 2023, max compression
```

## Comparing `mypy-boto3-internetmonitor-1.28.16.tar` & `mypy-boto3-internetmonitor-1.28.17.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:57.776870 mypy-boto3-internetmonitor-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-08-01 11:36:57.776870 mypy-boto3-internetmonitor-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:57.760870 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-08-01 11:20:04.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-08-01 11:20:04.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-01 11:20:04.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-08-01 11:20:06.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-08-01 11:20:04.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:57.760870 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:57.776870 mypy-boto3-internetmonitor-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.447423 mypy-boto3-internetmonitor-1.28.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-08-01 19:33:25.447423 mypy-boto3-internetmonitor-1.28.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.447423 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-08-01 19:32:23.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-08-01 19:32:23.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-01 19:32:23.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-08-01 19:32:23.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-08-01 19:32:23.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.447423 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-08-01 19:33:25.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 19:33:25.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:33:25.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:33:25.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 19:33:25.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 19:33:25.000000 mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:33:25.447423 mypy-boto3-internetmonitor-1.28.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-01 19:32:22.000000 mypy-boto3-internetmonitor-1.28.17/setup.py
```

### Comparing `mypy-boto3-internetmonitor-1.28.16/LICENSE` & `mypy-boto3-internetmonitor-1.28.17/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.16/PKG-INFO` & `mypy-boto3-internetmonitor-1.28.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.28.16
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.17
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.17 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -303,14 +303,15 @@
 
 ```python
 from mypy_boto3_internetmonitor.literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
     ListHealthEventsPaginatorName,
     ListMonitorsPaginatorName,
+    LocalHealthEventsConfigStatusType,
     LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
     CloudWatchInternetMonitorServiceName,
     ServiceName,
     ResourceServiceName,
@@ -329,32 +330,33 @@
 
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
-    HealthEventsConfigTypeDef,
     ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
+    LocalHealthEventsConfigTypeDef,
     S3ConfigTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     NetworkTypeDef,
     RoundTripTimeTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateMonitorOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
+    HealthEventsConfigTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
     ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListHealthEventsInputRequestTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
```

### Comparing `mypy-boto3-internetmonitor-1.28.16/README.md` & `mypy-boto3-internetmonitor-1.28.17/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -271,14 +271,15 @@
 
 ```python
 from mypy_boto3_internetmonitor.literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
     ListHealthEventsPaginatorName,
     ListMonitorsPaginatorName,
+    LocalHealthEventsConfigStatusType,
     LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
     CloudWatchInternetMonitorServiceName,
     ServiceName,
     ResourceServiceName,
@@ -297,32 +298,33 @@
 
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
-    HealthEventsConfigTypeDef,
     ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
+    LocalHealthEventsConfigTypeDef,
     S3ConfigTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     NetworkTypeDef,
     RoundTripTimeTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateMonitorOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
+    HealthEventsConfigTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
     ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListHealthEventsInputRequestTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
```

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__init__.py` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__init__.pyi` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__main__.py` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.16\nVersion:        "
-        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.17\nVersion:        "
+        " 1.28.17\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.17")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/client.py` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/client.pyi` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/literals.py` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,34 @@
 
 
 __all__ = (
     "HealthEventImpactTypeType",
     "HealthEventStatusType",
     "ListHealthEventsPaginatorName",
     "ListMonitorsPaginatorName",
+    "LocalHealthEventsConfigStatusType",
     "LogDeliveryStatusType",
     "MonitorConfigStateType",
     "MonitorProcessingStatusCodeType",
     "TriangulationEventTypeType",
     "CloudWatchInternetMonitorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
-HealthEventImpactTypeType = Literal["AVAILABILITY", "PERFORMANCE"]
+HealthEventImpactTypeType = Literal[
+    "AVAILABILITY", "LOCAL_AVAILABILITY", "LOCAL_PERFORMANCE", "PERFORMANCE"
+]
 HealthEventStatusType = Literal["ACTIVE", "RESOLVED"]
 ListHealthEventsPaginatorName = Literal["list_health_events"]
 ListMonitorsPaginatorName = Literal["list_monitors"]
+LocalHealthEventsConfigStatusType = Literal["DISABLED", "ENABLED"]
 LogDeliveryStatusType = Literal["DISABLED", "ENABLED"]
 MonitorConfigStateType = Literal["ACTIVE", "ERROR", "INACTIVE", "PENDING"]
 MonitorProcessingStatusCodeType = Literal[
     "COLLECTING_DATA",
     "FAULT_ACCESS_CLOUDWATCH",
     "FAULT_SERVICE",
     "INACTIVE",
@@ -437,14 +441,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/literals.pyi` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,33 @@
     from typing_extensions import Literal
 
 __all__ = (
     "HealthEventImpactTypeType",
     "HealthEventStatusType",
     "ListHealthEventsPaginatorName",
     "ListMonitorsPaginatorName",
+    "LocalHealthEventsConfigStatusType",
     "LogDeliveryStatusType",
     "MonitorConfigStateType",
     "MonitorProcessingStatusCodeType",
     "TriangulationEventTypeType",
     "CloudWatchInternetMonitorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-HealthEventImpactTypeType = Literal["AVAILABILITY", "PERFORMANCE"]
+HealthEventImpactTypeType = Literal[
+    "AVAILABILITY", "LOCAL_AVAILABILITY", "LOCAL_PERFORMANCE", "PERFORMANCE"
+]
 HealthEventStatusType = Literal["ACTIVE", "RESOLVED"]
 ListHealthEventsPaginatorName = Literal["list_health_events"]
 ListMonitorsPaginatorName = Literal["list_monitors"]
+LocalHealthEventsConfigStatusType = Literal["DISABLED", "ENABLED"]
 LogDeliveryStatusType = Literal["DISABLED", "ENABLED"]
 MonitorConfigStateType = Literal["ACTIVE", "ERROR", "INACTIVE", "PENDING"]
 MonitorProcessingStatusCodeType = Literal[
     "COLLECTING_DATA",
     "FAULT_ACCESS_CLOUDWATCH",
     "FAULT_SERVICE",
     "INACTIVE",
@@ -435,14 +439,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/paginator.py` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/paginator.pyi` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/type_defs.py` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,46 +14,48 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
+    LocalHealthEventsConfigStatusType,
     LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AvailabilityMeasurementTypeDef",
-    "HealthEventsConfigTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
+    "LocalHealthEventsConfigTypeDef",
     "S3ConfigTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "NetworkTypeDef",
     "RoundTripTimeTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateMonitorOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
+    "HealthEventsConfigTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
@@ -73,23 +75,14 @@
         "ExperienceScore": float,
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
     },
     total=False,
 )
 
-HealthEventsConfigTypeDef = TypedDict(
-    "HealthEventsConfigTypeDef",
-    {
-        "AvailabilityScoreThreshold": float,
-        "PerformanceScoreThreshold": float,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -115,14 +108,24 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
+LocalHealthEventsConfigTypeDef = TypedDict(
+    "LocalHealthEventsConfigTypeDef",
+    {
+        "Status": LocalHealthEventsConfigStatusType,
+        "HealthScoreThreshold": float,
+        "MinTrafficImpact": float,
+    },
+    total=False,
+)
+
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
@@ -234,14 +237,25 @@
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+HealthEventsConfigTypeDef = TypedDict(
+    "HealthEventsConfigTypeDef",
+    {
+        "AvailabilityScoreThreshold": float,
+        "PerformanceScoreThreshold": float,
+        "AvailabilityLocalHealthEventsConfig": LocalHealthEventsConfigTypeDef,
+        "PerformanceLocalHealthEventsConfig": LocalHealthEventsConfigTypeDef,
+    },
+    total=False,
+)
+
 InternetMeasurementsLogDeliveryTypeDef = TypedDict(
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/type_defs.pyi` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,45 +14,47 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
+    LocalHealthEventsConfigStatusType,
     LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AvailabilityMeasurementTypeDef",
-    "HealthEventsConfigTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
+    "LocalHealthEventsConfigTypeDef",
     "S3ConfigTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "NetworkTypeDef",
     "RoundTripTimeTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateMonitorOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
+    "HealthEventsConfigTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
@@ -72,23 +74,14 @@
         "ExperienceScore": float,
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
     },
     total=False,
 )
 
-HealthEventsConfigTypeDef = TypedDict(
-    "HealthEventsConfigTypeDef",
-    {
-        "AvailabilityScoreThreshold": float,
-        "PerformanceScoreThreshold": float,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -114,14 +107,24 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
+LocalHealthEventsConfigTypeDef = TypedDict(
+    "LocalHealthEventsConfigTypeDef",
+    {
+        "Status": LocalHealthEventsConfigStatusType,
+        "HealthScoreThreshold": float,
+        "MinTrafficImpact": float,
+    },
+    total=False,
+)
+
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
@@ -231,14 +234,25 @@
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+HealthEventsConfigTypeDef = TypedDict(
+    "HealthEventsConfigTypeDef",
+    {
+        "AvailabilityScoreThreshold": float,
+        "PerformanceScoreThreshold": float,
+        "AvailabilityLocalHealthEventsConfig": LocalHealthEventsConfigTypeDef,
+        "PerformanceLocalHealthEventsConfig": LocalHealthEventsConfigTypeDef,
+    },
+    total=False,
+)
+
 InternetMeasurementsLogDeliveryTypeDef = TypedDict(
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/PKG-INFO` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.28.16
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.17
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.17 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -303,14 +303,15 @@
 
 ```python
 from mypy_boto3_internetmonitor.literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
     ListHealthEventsPaginatorName,
     ListMonitorsPaginatorName,
+    LocalHealthEventsConfigStatusType,
     LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
     CloudWatchInternetMonitorServiceName,
     ServiceName,
     ResourceServiceName,
@@ -329,32 +330,33 @@
 
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
-    HealthEventsConfigTypeDef,
     ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
+    LocalHealthEventsConfigTypeDef,
     S3ConfigTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     NetworkTypeDef,
     RoundTripTimeTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateMonitorOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
+    HealthEventsConfigTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
     ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListHealthEventsInputRequestTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
```

### Comparing `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/SOURCES.txt` & `mypy-boto3-internetmonitor-1.28.17/mypy_boto3_internetmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.16/setup.py` & `mypy-boto3-internetmonitor-1.28.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-internetmonitor",
-    version="1.28.16",
+    version="1.28.17",
     packages=["mypy_boto3_internetmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.16 service generated with"
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.17 service generated with"
         " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

