# Comparing `tmp/mypy-boto3-internetmonitor-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-internetmonitor-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-internetmonitor-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:17 2023, max compression
+gzip compressed data, was "mypy-boto3-internetmonitor-1.28.16.tar", last modified: Tue Aug  1 11:36:57 2023, max compression
```

## Comparing `mypy-boto3-internetmonitor-1.28.15.post1.tar` & `mypy-boto3-internetmonitor-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:17.809175 mypy-boto3-internetmonitor-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-07-29 10:03:17.805175 mypy-boto3-internetmonitor-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:17.797175 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-29 09:47:24.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:17.805175 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-07-29 10:03:17.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:03:17.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:17.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:17.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:17.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:03:17.000000 mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:17.809175 mypy-boto3-internetmonitor-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-29 09:47:23.000000 mypy-boto3-internetmonitor-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:57.776870 mypy-boto3-internetmonitor-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-08-01 11:36:57.776870 mypy-boto3-internetmonitor-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:57.760870 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-08-01 11:20:04.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-08-01 11:20:04.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-01 11:20:04.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-08-01 11:20:06.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-08-01 11:20:04.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:57.760870 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:36:57.000000 mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:57.776870 mypy-boto3-internetmonitor-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-01 11:20:03.000000 mypy-boto3-internetmonitor-1.28.16/setup.py
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/LICENSE` & `mypy-boto3-internetmonitor-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/PKG-INFO` & `mypy-boto3-internetmonitor-1.28.16/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 internetmonitor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 internetmonitor type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -319,60 +319,61 @@
 )
 
 
 def check_value(value: HealthEventImpactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
     HealthEventsConfigTypeDef,
     ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
     S3ConfigTypeDef,
     PaginatorConfigTypeDef,
-    ListHealthEventsInputRequestTypeDef,
+    TimestampTypeDef,
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
     InternetMeasurementsLogDeliveryTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
+    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    ListHealthEventsInputRequestTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
     CreateMonitorInputRequestTypeDef,
     GetMonitorOutputTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
 
 
-def get_structure() -> AvailabilityMeasurementTypeDef:
+def get_value() -> AvailabilityMeasurementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/README.md` & `mypy-boto3-internetmonitor-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -287,60 +287,61 @@
 )
 
 
 def check_value(value: HealthEventImpactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
     HealthEventsConfigTypeDef,
     ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
     S3ConfigTypeDef,
     PaginatorConfigTypeDef,
-    ListHealthEventsInputRequestTypeDef,
+    TimestampTypeDef,
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
     InternetMeasurementsLogDeliveryTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
+    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    ListHealthEventsInputRequestTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
     CreateMonitorInputRequestTypeDef,
     GetMonitorOutputTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
 
 
-def get_structure() -> AvailabilityMeasurementTypeDef:
+def get_value() -> AvailabilityMeasurementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/__init__.py` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/__init__.pyi` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/__main__.py` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.16")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/client.py` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     from mypy_boto3_internetmonitor.client import CloudWatchInternetMonitorClient
 
     session = Session()
     client: CloudWatchInternetMonitorClient = session.client("internetmonitor")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import HealthEventStatusType, MonitorConfigStateType
 from .paginator import ListHealthEventsPaginator, ListMonitorsPaginator
 from .type_defs import (
     CreateMonitorOutputTypeDef,
     GetHealthEventOutputTypeDef,
     GetMonitorOutputTypeDef,
     HealthEventsConfigTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TimestampTypeDef,
     UpdateMonitorOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -157,16 +157,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_monitor)
         """
 
     def list_health_events(
         self,
         *,
         MonitorName: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         EventStatus: HealthEventStatusType = ...
     ) -> ListHealthEventsOutputTypeDef:
         """
         Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/client.pyi` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     from mypy_boto3_internetmonitor.client import CloudWatchInternetMonitorClient
 
     session = Session()
     client: CloudWatchInternetMonitorClient = session.client("internetmonitor")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import HealthEventStatusType, MonitorConfigStateType
 from .paginator import ListHealthEventsPaginator, ListMonitorsPaginator
 from .type_defs import (
     CreateMonitorOutputTypeDef,
     GetHealthEventOutputTypeDef,
     GetMonitorOutputTypeDef,
     HealthEventsConfigTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TimestampTypeDef,
     UpdateMonitorOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -145,16 +145,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_monitor)
         """
     def list_health_events(
         self,
         *,
         MonitorName: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         EventStatus: HealthEventStatusType = ...
     ) -> ListHealthEventsOutputTypeDef:
         """
         Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/literals.py` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/literals.pyi` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/paginator.py` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     session = Session()
     client: CloudWatchInternetMonitorClient = session.client("internetmonitor")
 
     list_health_events_paginator: ListHealthEventsPaginator = client.get_paginator("list_health_events")
     list_monitors_paginator: ListMonitorsPaginator = client.get_paginator("list_monitors")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import HealthEventStatusType
 from .type_defs import (
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListHealthEventsPaginator", "ListMonitorsPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -52,16 +52,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listhealtheventspaginator)
     """
 
     def paginate(
         self,
         *,
         MonitorName: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventStatus: HealthEventStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHealthEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listhealtheventspaginator)
         """
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/paginator.pyi` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     session = Session()
     client: CloudWatchInternetMonitorClient = session.client("internetmonitor")
 
     list_health_events_paginator: ListHealthEventsPaginator = client.get_paginator("list_health_events")
     list_monitors_paginator: ListMonitorsPaginator = client.get_paginator("list_monitors")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import HealthEventStatusType
 from .type_defs import (
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListHealthEventsPaginator", "ListMonitorsPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -49,16 +49,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listhealtheventspaginator)
     """
 
     def paginate(
         self,
         *,
         MonitorName: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventStatus: HealthEventStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHealthEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listhealtheventspaginator)
         """
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/type_defs.py` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_internetmonitor.type_defs import AvailabilityMeasurementTypeDef
 
-    data: AvailabilityMeasurementTypeDef = {...}
+    data: AvailabilityMeasurementTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -25,38 +25,38 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AvailabilityMeasurementTypeDef",
     "HealthEventsConfigTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
     "S3ConfigTypeDef",
     "PaginatorConfigTypeDef",
-    "ListHealthEventsInputRequestTypeDef",
+    "TimestampTypeDef",
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
     "InternetMeasurementsLogDeliveryTypeDef",
-    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
+    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
+    "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
     "CreateMonitorInputRequestTypeDef",
     "GetMonitorOutputTypeDef",
     "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
@@ -134,39 +134,15 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListHealthEventsInputRequestTypeDef = TypedDict(
-    "_RequiredListHealthEventsInputRequestTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalListHealthEventsInputRequestTypeDef = TypedDict(
-    "_OptionalListHealthEventsInputRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-        "EventStatus": HealthEventStatusType,
-    },
-    total=False,
-)
-
-
-class ListHealthEventsInputRequestTypeDef(
-    _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ListMonitorsInputRequestTypeDef = TypedDict(
     "ListMonitorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "MonitorStatus": str,
     },
@@ -185,19 +161,17 @@
     "_OptionalMonitorTypeDef",
     {
         "ProcessingStatus": MonitorProcessingStatusCodeType,
     },
     total=False,
 )
 
-
 class MonitorTypeDef(_RequiredMonitorTypeDef, _OptionalMonitorTypeDef):
     pass
 
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -265,48 +239,69 @@
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
 
+ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    {
+        "MonitorStatus": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
     "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
     "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventStatus": HealthEventStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListHealthEventsInputListHealthEventsPaginateTypeDef(
     _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
     _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
 ):
     pass
 
-
-ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
+_RequiredListHealthEventsInputRequestTypeDef = TypedDict(
+    "_RequiredListHealthEventsInputRequestTypeDef",
     {
-        "MonitorStatus": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "MonitorName": str,
+    },
+)
+_OptionalListHealthEventsInputRequestTypeDef = TypedDict(
+    "_OptionalListHealthEventsInputRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "EventStatus": HealthEventStatusType,
     },
     total=False,
 )
 
+class ListHealthEventsInputRequestTypeDef(
+    _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
+):
+    pass
+
 ListMonitorsOutputTypeDef = TypedDict(
     "ListMonitorsOutputTypeDef",
     {
         "Monitors": List[MonitorTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -348,21 +343,19 @@
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
         "HealthEventsConfig": HealthEventsConfigTypeDef,
     },
     total=False,
 )
 
-
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
 ):
     pass
 
-
 GetMonitorOutputTypeDef = TypedDict(
     "GetMonitorOutputTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "Resources": List[str],
         "Status": MonitorConfigStateType,
@@ -396,21 +389,19 @@
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
         "HealthEventsConfig": HealthEventsConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMonitorInputRequestTypeDef(
     _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
 ):
     pass
 
-
 InternetHealthTypeDef = TypedDict(
     "InternetHealthTypeDef",
     {
         "Availability": AvailabilityMeasurementTypeDef,
         "Performance": PerformanceMeasurementTypeDef,
     },
     total=False,
@@ -438,19 +429,17 @@
         "ServiceLocation": str,
         "CausedBy": NetworkImpairmentTypeDef,
         "InternetHealth": InternetHealthTypeDef,
     },
     total=False,
 )
 
-
 class ImpactedLocationTypeDef(_RequiredImpactedLocationTypeDef, _OptionalImpactedLocationTypeDef):
     pass
 
-
 GetHealthEventOutputTypeDef = TypedDict(
     "GetHealthEventOutputTypeDef",
     {
         "EventArn": str,
         "EventId": str,
         "StartedAt": datetime,
         "EndedAt": datetime,
@@ -484,19 +473,17 @@
         "CreatedAt": datetime,
         "PercentOfTotalTrafficImpacted": float,
         "HealthScoreThreshold": float,
     },
     total=False,
 )
 
-
 class HealthEventTypeDef(_RequiredHealthEventTypeDef, _OptionalHealthEventTypeDef):
     pass
 
-
 ListHealthEventsOutputTypeDef = TypedDict(
     "ListHealthEventsOutputTypeDef",
     {
         "HealthEvents": List[HealthEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor/type_defs.pyi` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_internetmonitor.type_defs import AvailabilityMeasurementTypeDef
 
-    data: AvailabilityMeasurementTypeDef = {...}
+    data: AvailabilityMeasurementTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -25,37 +25,39 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AvailabilityMeasurementTypeDef",
     "HealthEventsConfigTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
     "S3ConfigTypeDef",
     "PaginatorConfigTypeDef",
-    "ListHealthEventsInputRequestTypeDef",
+    "TimestampTypeDef",
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
     "InternetMeasurementsLogDeliveryTypeDef",
-    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
+    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
+    "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
     "CreateMonitorInputRequestTypeDef",
     "GetMonitorOutputTypeDef",
     "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
@@ -133,37 +135,15 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListHealthEventsInputRequestTypeDef = TypedDict(
-    "_RequiredListHealthEventsInputRequestTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalListHealthEventsInputRequestTypeDef = TypedDict(
-    "_OptionalListHealthEventsInputRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-        "EventStatus": HealthEventStatusType,
-    },
-    total=False,
-)
-
-class ListHealthEventsInputRequestTypeDef(
-    _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 ListMonitorsInputRequestTypeDef = TypedDict(
     "ListMonitorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "MonitorStatus": str,
     },
@@ -182,17 +162,19 @@
     "_OptionalMonitorTypeDef",
     {
         "ProcessingStatus": MonitorProcessingStatusCodeType,
     },
     total=False,
 )
 
+
 class MonitorTypeDef(_RequiredMonitorTypeDef, _OptionalMonitorTypeDef):
     pass
 
+
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -260,46 +242,73 @@
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
 
+ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    {
+        "MonitorStatus": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
     "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
     "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventStatus": HealthEventStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListHealthEventsInputListHealthEventsPaginateTypeDef(
     _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
     _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
 ):
     pass
 
-ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
+
+_RequiredListHealthEventsInputRequestTypeDef = TypedDict(
+    "_RequiredListHealthEventsInputRequestTypeDef",
     {
-        "MonitorStatus": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "MonitorName": str,
+    },
+)
+_OptionalListHealthEventsInputRequestTypeDef = TypedDict(
+    "_OptionalListHealthEventsInputRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "EventStatus": HealthEventStatusType,
     },
     total=False,
 )
 
+
+class ListHealthEventsInputRequestTypeDef(
+    _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
+):
+    pass
+
+
 ListMonitorsOutputTypeDef = TypedDict(
     "ListMonitorsOutputTypeDef",
     {
         "Monitors": List[MonitorTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -341,19 +350,21 @@
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
         "HealthEventsConfig": HealthEventsConfigTypeDef,
     },
     total=False,
 )
 
+
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
 ):
     pass
 
+
 GetMonitorOutputTypeDef = TypedDict(
     "GetMonitorOutputTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "Resources": List[str],
         "Status": MonitorConfigStateType,
@@ -387,19 +398,21 @@
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
         "HealthEventsConfig": HealthEventsConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMonitorInputRequestTypeDef(
     _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
 ):
     pass
 
+
 InternetHealthTypeDef = TypedDict(
     "InternetHealthTypeDef",
     {
         "Availability": AvailabilityMeasurementTypeDef,
         "Performance": PerformanceMeasurementTypeDef,
     },
     total=False,
@@ -427,17 +440,19 @@
         "ServiceLocation": str,
         "CausedBy": NetworkImpairmentTypeDef,
         "InternetHealth": InternetHealthTypeDef,
     },
     total=False,
 )
 
+
 class ImpactedLocationTypeDef(_RequiredImpactedLocationTypeDef, _OptionalImpactedLocationTypeDef):
     pass
 
+
 GetHealthEventOutputTypeDef = TypedDict(
     "GetHealthEventOutputTypeDef",
     {
         "EventArn": str,
         "EventId": str,
         "StartedAt": datetime,
         "EndedAt": datetime,
@@ -471,17 +486,19 @@
         "CreatedAt": datetime,
         "PercentOfTotalTrafficImpacted": float,
         "HealthScoreThreshold": float,
     },
     total=False,
 )
 
+
 class HealthEventTypeDef(_RequiredHealthEventTypeDef, _OptionalHealthEventTypeDef):
     pass
 
+
 ListHealthEventsOutputTypeDef = TypedDict(
     "ListHealthEventsOutputTypeDef",
     {
         "HealthEvents": List[HealthEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor.egg-info/PKG-INFO` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 internetmonitor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 internetmonitor type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -319,60 +319,61 @@
 )
 
 
 def check_value(value: HealthEventImpactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
     HealthEventsConfigTypeDef,
     ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
     S3ConfigTypeDef,
     PaginatorConfigTypeDef,
-    ListHealthEventsInputRequestTypeDef,
+    TimestampTypeDef,
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
     InternetMeasurementsLogDeliveryTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
+    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    ListHealthEventsInputRequestTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
     CreateMonitorInputRequestTypeDef,
     GetMonitorOutputTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
 
 
-def get_structure() -> AvailabilityMeasurementTypeDef:
+def get_value() -> AvailabilityMeasurementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/mypy_boto3_internetmonitor.egg-info/SOURCES.txt` & `mypy-boto3-internetmonitor-1.28.16/mypy_boto3_internetmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.15.post1/setup.py` & `mypy-boto3-internetmonitor-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-internetmonitor",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_internetmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,15 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 internetmonitor type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 internetmonitor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_internetmonitor": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

