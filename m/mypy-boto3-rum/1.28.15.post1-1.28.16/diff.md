# Comparing `tmp/mypy-boto3-rum-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-rum-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rum-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:04 2023, max compression
+gzip compressed data, was "mypy-boto3-rum-1.28.16.tar", last modified: Tue Aug  1 11:37:44 2023, max compression
```

## Comparing `mypy-boto3-rum-1.28.15.post1.tar` & `mypy-boto3-rum-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.657377 mypy-boto3-rum-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-29 10:04:04.657377 mypy-boto3-rum-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.653377 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21314 2023-07-29 09:57:34.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21277 2023-07-29 09:57:34.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.657377 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:04.657377 mypy-boto3-rum-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:44.116759 mypy-boto3-rum-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-08-01 11:37:44.116759 mypy-boto3-rum-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:44.116759 mypy-boto3-rum-1.28.16/mypy_boto3_rum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-08-01 11:30:58.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-08-01 11:30:58.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-08-01 11:30:58.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21599 2023-08-01 11:30:58.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:44.116759 mypy-boto3-rum-1.28.16/mypy_boto3_rum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-08-01 11:37:43.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:37:43.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:43.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:43.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:43.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:43.000000 mypy-boto3-rum-1.28.16/mypy_boto3_rum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:44.116759 mypy-boto3-rum-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:30:57.000000 mypy-boto3-rum-1.28.16/setup.py
```

### Comparing `mypy-boto3-rum-1.28.15.post1/LICENSE` & `mypy-boto3-rum-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15.post1/PKG-INFO` & `mypy-boto3-rum-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatchRUM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rum type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 rum type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rum)](https://pepy.tech/project/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
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
@@ -329,30 +329,29 @@
 )
 
 
 def check_value(value: BatchGetRumMetricDefinitionsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rum.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rum.type_defs import (
     AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
     CustomEventsTypeDef,
     MetricDefinitionRequestOutputTypeDef,
-    MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
     CwLogTypeDef,
@@ -361,45 +360,49 @@
     QueryFilterTypeDef,
     TimeRangeTypeDef,
     GetAppMonitorRequestRequestTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
     ListRumMetricsDestinationsRequestRequestTypeDef,
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RumEventTypeDef,
+    MetricDefinitionRequestTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
+    TimestampTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AppMonitorConfigurationUnionTypeDef,
     CreateAppMonitorRequestRequestTypeDef,
     UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
-    BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-    UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     GetAppMonitorDataResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
     ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
-    PutRumEventsRequestRequestTypeDef,
+    MetricDefinitionRequestUnionTypeDef,
+    UpdateRumMetricDefinitionRequestRequestTypeDef,
+    RumEventTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
+    BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+    PutRumEventsRequestRequestTypeDef,
     GetAppMonitorResponseTypeDef,
 )
 
 
-def get_structure() -> AppMonitorConfigurationOutputTypeDef:
+def get_value() -> AppMonitorConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rum-1.28.15.post1/README.md` & `mypy-boto3-rum-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rum)](https://pepy.tech/project/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
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
@@ -297,30 +297,29 @@
 )
 
 
 def check_value(value: BatchGetRumMetricDefinitionsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rum.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rum.type_defs import (
     AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
     CustomEventsTypeDef,
     MetricDefinitionRequestOutputTypeDef,
-    MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
     CwLogTypeDef,
@@ -329,45 +328,49 @@
     QueryFilterTypeDef,
     TimeRangeTypeDef,
     GetAppMonitorRequestRequestTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
     ListRumMetricsDestinationsRequestRequestTypeDef,
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RumEventTypeDef,
+    MetricDefinitionRequestTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
+    TimestampTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AppMonitorConfigurationUnionTypeDef,
     CreateAppMonitorRequestRequestTypeDef,
     UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
-    BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-    UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     GetAppMonitorDataResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
     ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
-    PutRumEventsRequestRequestTypeDef,
+    MetricDefinitionRequestUnionTypeDef,
+    UpdateRumMetricDefinitionRequestRequestTypeDef,
+    RumEventTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
+    BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+    PutRumEventsRequestRequestTypeDef,
     GetAppMonitorResponseTypeDef,
 )
 
 
-def get_structure() -> AppMonitorConfigurationOutputTypeDef:
+def get_value() -> AppMonitorConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__init__.py` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__init__.pyi` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__main__.py` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchRUM 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CloudWatchRUM 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM\nOther"
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

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/client.py` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,41 +10,39 @@
     from mypy_boto3_rum.client import CloudWatchRUMClient
 
     session = Session()
     client: CloudWatchRUMClient = session.client("rum")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MetricDestinationType
 from .paginator import (
     BatchGetRumMetricDefinitionsPaginator,
     GetAppMonitorDataPaginator,
     ListAppMonitorsPaginator,
     ListRumMetricsDestinationsPaginator,
 )
 from .type_defs import (
-    AppMonitorConfigurationOutputTypeDef,
-    AppMonitorConfigurationTypeDef,
+    AppMonitorConfigurationUnionTypeDef,
     AppMonitorDetailsTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     CustomEventsTypeDef,
     GetAppMonitorDataResponseTypeDef,
     GetAppMonitorResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricDefinitionRequestOutputTypeDef,
-    MetricDefinitionRequestTypeDef,
+    MetricDefinitionRequestUnionTypeDef,
     QueryFilterTypeDef,
     RumEventTypeDef,
     TimeRangeTypeDef,
     UserDetailsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -93,17 +91,15 @@
         """
 
     def batch_create_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinitions: Sequence[
-            Union[MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef]
-        ],
+        MetricDefinitions: Sequence[MetricDefinitionRequestUnionTypeDef],
         DestinationArn: str = ...
     ) -> BatchCreateRumMetricDefinitionsResponseTypeDef:
         """
         Specifies the extended metrics and custom metrics that you want a CloudWatch RUM
         app monitor to send to a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_create_rum_metric_definitions)
@@ -160,17 +156,15 @@
         """
 
     def create_app_monitor(
         self,
         *,
         Domain: str,
         Name: str,
-        AppMonitorConfiguration: Union[
-            AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
-        ] = ...,
+        AppMonitorConfiguration: AppMonitorConfigurationUnionTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateAppMonitorResponseTypeDef:
         """
         Creates a Amazon CloudWatch RUM app monitor, which collects telemetry data from
         your application and sends that data to RUM.
@@ -316,17 +310,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#untag_resource)
         """
 
     def update_app_monitor(
         self,
         *,
         Name: str,
-        AppMonitorConfiguration: Union[
-            AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
-        ] = ...,
+        AppMonitorConfiguration: AppMonitorConfigurationUnionTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Domain: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration of an existing app monitor.
 
@@ -335,17 +327,15 @@
         """
 
     def update_rum_metric_definition(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinition: Union[
-            MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef
-        ],
+        MetricDefinition: MetricDefinitionRequestUnionTypeDef,
         MetricDefinitionId: str,
         DestinationArn: str = ...
     ) -> Dict[str, Any]:
         """
         Modifies one existing metric definition for CloudWatch RUM extended metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_rum_metric_definition)
```

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/client.pyi` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,41 +10,39 @@
     from mypy_boto3_rum.client import CloudWatchRUMClient
 
     session = Session()
     client: CloudWatchRUMClient = session.client("rum")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MetricDestinationType
 from .paginator import (
     BatchGetRumMetricDefinitionsPaginator,
     GetAppMonitorDataPaginator,
     ListAppMonitorsPaginator,
     ListRumMetricsDestinationsPaginator,
 )
 from .type_defs import (
-    AppMonitorConfigurationOutputTypeDef,
-    AppMonitorConfigurationTypeDef,
+    AppMonitorConfigurationUnionTypeDef,
     AppMonitorDetailsTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     CustomEventsTypeDef,
     GetAppMonitorDataResponseTypeDef,
     GetAppMonitorResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricDefinitionRequestOutputTypeDef,
-    MetricDefinitionRequestTypeDef,
+    MetricDefinitionRequestUnionTypeDef,
     QueryFilterTypeDef,
     RumEventTypeDef,
     TimeRangeTypeDef,
     UserDetailsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -88,17 +86,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#exceptions)
         """
     def batch_create_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinitions: Sequence[
-            Union[MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef]
-        ],
+        MetricDefinitions: Sequence[MetricDefinitionRequestUnionTypeDef],
         DestinationArn: str = ...
     ) -> BatchCreateRumMetricDefinitionsResponseTypeDef:
         """
         Specifies the extended metrics and custom metrics that you want a CloudWatch RUM
         app monitor to send to a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_create_rum_metric_definitions)
@@ -150,17 +146,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#close)
         """
     def create_app_monitor(
         self,
         *,
         Domain: str,
         Name: str,
-        AppMonitorConfiguration: Union[
-            AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
-        ] = ...,
+        AppMonitorConfiguration: AppMonitorConfigurationUnionTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateAppMonitorResponseTypeDef:
         """
         Creates a Amazon CloudWatch RUM app monitor, which collects telemetry data from
         your application and sends that data to RUM.
@@ -293,17 +287,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#untag_resource)
         """
     def update_app_monitor(
         self,
         *,
         Name: str,
-        AppMonitorConfiguration: Union[
-            AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
-        ] = ...,
+        AppMonitorConfiguration: AppMonitorConfigurationUnionTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Domain: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration of an existing app monitor.
 
@@ -311,17 +303,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#update_app_monitor)
         """
     def update_rum_metric_definition(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinition: Union[
-            MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef
-        ],
+        MetricDefinition: MetricDefinitionRequestUnionTypeDef,
         MetricDefinitionId: str,
         DestinationArn: str = ...
     ) -> Dict[str, Any]:
         """
         Modifies one existing metric definition for CloudWatch RUM extended metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_rum_metric_definition)
```

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/literals.py` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/literals.pyi` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/paginator.py` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/paginator.pyi` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/type_defs.py` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_rum.type_defs import AppMonitorConfigurationOutputTypeDef
 
-    data: AppMonitorConfigurationOutputTypeDef = {...}
+    data: AppMonitorConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import CustomEventsStatusType, MetricDestinationType, StateEnumType, TelemetryType
@@ -26,15 +26,14 @@
 __all__ = (
     "AppMonitorConfigurationOutputTypeDef",
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
     "CustomEventsTypeDef",
     "MetricDefinitionRequestOutputTypeDef",
-    "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
     "CwLogTypeDef",
@@ -43,40 +42,44 @@
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
     "ListRumMetricsDestinationsRequestRequestTypeDef",
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RumEventTypeDef",
+    "MetricDefinitionRequestTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AppMonitorConfigurationUnionTypeDef",
     "CreateAppMonitorRequestRequestTypeDef",
     "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
-    "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     "CreateAppMonitorResponseTypeDef",
     "GetAppMonitorDataResponseTypeDef",
     "ListAppMonitorsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
-    "PutRumEventsRequestRequestTypeDef",
+    "MetricDefinitionRequestUnionTypeDef",
+    "UpdateRumMetricDefinitionRequestRequestTypeDef",
+    "RumEventTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
+    "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    "PutRumEventsRequestRequestTypeDef",
     "GetAppMonitorResponseTypeDef",
 )
 
 AppMonitorConfigurationOutputTypeDef = TypedDict(
     "AppMonitorConfigurationOutputTypeDef",
     {
         "AllowCookies": bool,
@@ -159,39 +162,14 @@
 
 class MetricDefinitionRequestOutputTypeDef(
     _RequiredMetricDefinitionRequestOutputTypeDef, _OptionalMetricDefinitionRequestOutputTypeDef
 ):
     pass
 
 
-_RequiredMetricDefinitionRequestTypeDef = TypedDict(
-    "_RequiredMetricDefinitionRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalMetricDefinitionRequestTypeDef = TypedDict(
-    "_OptionalMetricDefinitionRequestTypeDef",
-    {
-        "DimensionKeys": Mapping[str, str],
-        "EventPattern": str,
-        "Namespace": str,
-        "UnitLabel": str,
-        "ValueKey": str,
-    },
-    total=False,
-)
-
-
-class MetricDefinitionRequestTypeDef(
-    _RequiredMetricDefinitionRequestTypeDef, _OptionalMetricDefinitionRequestTypeDef
-):
-    pass
-
-
 _RequiredMetricDefinitionTypeDef = TypedDict(
     "_RequiredMetricDefinitionTypeDef",
     {
         "MetricDefinitionId": str,
         "Name": str,
     },
 )
@@ -410,33 +388,36 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredRumEventTypeDef = TypedDict(
-    "_RequiredRumEventTypeDef",
+_RequiredMetricDefinitionRequestTypeDef = TypedDict(
+    "_RequiredMetricDefinitionRequestTypeDef",
     {
-        "details": str,
-        "id": str,
-        "timestamp": Union[datetime, str],
-        "type": str,
+        "Name": str,
     },
 )
-_OptionalRumEventTypeDef = TypedDict(
-    "_OptionalRumEventTypeDef",
+_OptionalMetricDefinitionRequestTypeDef = TypedDict(
+    "_OptionalMetricDefinitionRequestTypeDef",
     {
-        "metadata": str,
+        "DimensionKeys": Mapping[str, str],
+        "EventPattern": str,
+        "Namespace": str,
+        "UnitLabel": str,
+        "ValueKey": str,
     },
     total=False,
 )
 
 
-class RumEventTypeDef(_RequiredRumEventTypeDef, _OptionalRumEventTypeDef):
+class MetricDefinitionRequestTypeDef(
+    _RequiredMetricDefinitionRequestTypeDef, _OptionalMetricDefinitionRequestTypeDef
+):
     pass
 
 
 UserDetailsTypeDef = TypedDict(
     "UserDetailsTypeDef",
     {
         "sessionId": str,
@@ -465,14 +446,15 @@
 class PutRumMetricsDestinationRequestRequestTypeDef(
     _RequiredPutRumMetricsDestinationRequestRequestTypeDef,
     _OptionalPutRumMetricsDestinationRequestRequestTypeDef,
 ):
     pass
 
 
+TimestampTypeDef = Union[datetime, str]
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -481,14 +463,17 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AppMonitorConfigurationUnionTypeDef = Union[
+    AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
+]
 _RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppMonitorRequestRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
     },
 )
@@ -539,65 +524,14 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "MetricDefinition": MetricDefinitionRequestOutputTypeDef,
     },
 )
 
-_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-        "MetricDefinitions": Sequence[
-            Union[MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef]
-        ],
-    },
-)
-_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    {
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
-
-class BatchCreateRumMetricDefinitionsRequestRequestTypeDef(
-    _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-    _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-        "MetricDefinition": MetricDefinitionRequestTypeDef,
-        "MetricDefinitionId": str,
-    },
-)
-_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef",
-    {
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
-
-class UpdateRumMetricDefinitionRequestRequestTypeDef(
-    _RequiredUpdateRumMetricDefinitionRequestRequestTypeDef,
-    _OptionalUpdateRumMetricDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
 BatchGetRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     {
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -762,25 +696,64 @@
     {
         "Destinations": List[MetricDestinationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutRumEventsRequestRequestTypeDef = TypedDict(
-    "PutRumEventsRequestRequestTypeDef",
+MetricDefinitionRequestUnionTypeDef = Union[
+    MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef
+]
+_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef",
     {
-        "AppMonitorDetails": AppMonitorDetailsTypeDef,
-        "BatchId": str,
-        "Id": str,
-        "RumEvents": Sequence[RumEventTypeDef],
-        "UserDetails": UserDetailsTypeDef,
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+        "MetricDefinition": MetricDefinitionRequestTypeDef,
+        "MetricDefinitionId": str,
+    },
+)
+_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+
+class UpdateRumMetricDefinitionRequestRequestTypeDef(
+    _RequiredUpdateRumMetricDefinitionRequestRequestTypeDef,
+    _OptionalUpdateRumMetricDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredRumEventTypeDef = TypedDict(
+    "_RequiredRumEventTypeDef",
+    {
+        "details": str,
+        "id": str,
+        "timestamp": TimestampTypeDef,
+        "type": str,
+    },
+)
+_OptionalRumEventTypeDef = TypedDict(
+    "_OptionalRumEventTypeDef",
+    {
+        "metadata": str,
     },
+    total=False,
 )
 
+
+class RumEventTypeDef(_RequiredRumEventTypeDef, _OptionalRumEventTypeDef):
+    pass
+
+
 BatchCreateRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchCreateRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -799,14 +772,49 @@
         "Name": str,
         "State": StateEnumType,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    {
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+        "MetricDefinitions": Sequence[MetricDefinitionRequestUnionTypeDef],
+    },
+)
+_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+
+class BatchCreateRumMetricDefinitionsRequestRequestTypeDef(
+    _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+    _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+):
+    pass
+
+
+PutRumEventsRequestRequestTypeDef = TypedDict(
+    "PutRumEventsRequestRequestTypeDef",
+    {
+        "AppMonitorDetails": AppMonitorDetailsTypeDef,
+        "BatchId": str,
+        "Id": str,
+        "RumEvents": Sequence[RumEventTypeDef],
+        "UserDetails": UserDetailsTypeDef,
+    },
+)
+
 GetAppMonitorResponseTypeDef = TypedDict(
     "GetAppMonitorResponseTypeDef",
     {
         "AppMonitor": AppMonitorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/type_defs.pyi` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_rum.type_defs import AppMonitorConfigurationOutputTypeDef
 
-    data: AppMonitorConfigurationOutputTypeDef = {...}
+    data: AppMonitorConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import CustomEventsStatusType, MetricDestinationType, StateEnumType, TelemetryType
@@ -25,15 +25,14 @@
 __all__ = (
     "AppMonitorConfigurationOutputTypeDef",
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
     "CustomEventsTypeDef",
     "MetricDefinitionRequestOutputTypeDef",
-    "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
     "CwLogTypeDef",
@@ -42,40 +41,44 @@
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
     "ListRumMetricsDestinationsRequestRequestTypeDef",
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RumEventTypeDef",
+    "MetricDefinitionRequestTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AppMonitorConfigurationUnionTypeDef",
     "CreateAppMonitorRequestRequestTypeDef",
     "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
-    "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     "CreateAppMonitorResponseTypeDef",
     "GetAppMonitorDataResponseTypeDef",
     "ListAppMonitorsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
-    "PutRumEventsRequestRequestTypeDef",
+    "MetricDefinitionRequestUnionTypeDef",
+    "UpdateRumMetricDefinitionRequestRequestTypeDef",
+    "RumEventTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
+    "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    "PutRumEventsRequestRequestTypeDef",
     "GetAppMonitorResponseTypeDef",
 )
 
 AppMonitorConfigurationOutputTypeDef = TypedDict(
     "AppMonitorConfigurationOutputTypeDef",
     {
         "AllowCookies": bool,
@@ -156,37 +159,14 @@
 )
 
 class MetricDefinitionRequestOutputTypeDef(
     _RequiredMetricDefinitionRequestOutputTypeDef, _OptionalMetricDefinitionRequestOutputTypeDef
 ):
     pass
 
-_RequiredMetricDefinitionRequestTypeDef = TypedDict(
-    "_RequiredMetricDefinitionRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalMetricDefinitionRequestTypeDef = TypedDict(
-    "_OptionalMetricDefinitionRequestTypeDef",
-    {
-        "DimensionKeys": Mapping[str, str],
-        "EventPattern": str,
-        "Namespace": str,
-        "UnitLabel": str,
-        "ValueKey": str,
-    },
-    total=False,
-)
-
-class MetricDefinitionRequestTypeDef(
-    _RequiredMetricDefinitionRequestTypeDef, _OptionalMetricDefinitionRequestTypeDef
-):
-    pass
-
 _RequiredMetricDefinitionTypeDef = TypedDict(
     "_RequiredMetricDefinitionTypeDef",
     {
         "MetricDefinitionId": str,
         "Name": str,
     },
 )
@@ -393,32 +373,35 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredRumEventTypeDef = TypedDict(
-    "_RequiredRumEventTypeDef",
+_RequiredMetricDefinitionRequestTypeDef = TypedDict(
+    "_RequiredMetricDefinitionRequestTypeDef",
     {
-        "details": str,
-        "id": str,
-        "timestamp": Union[datetime, str],
-        "type": str,
+        "Name": str,
     },
 )
-_OptionalRumEventTypeDef = TypedDict(
-    "_OptionalRumEventTypeDef",
+_OptionalMetricDefinitionRequestTypeDef = TypedDict(
+    "_OptionalMetricDefinitionRequestTypeDef",
     {
-        "metadata": str,
+        "DimensionKeys": Mapping[str, str],
+        "EventPattern": str,
+        "Namespace": str,
+        "UnitLabel": str,
+        "ValueKey": str,
     },
     total=False,
 )
 
-class RumEventTypeDef(_RequiredRumEventTypeDef, _OptionalRumEventTypeDef):
+class MetricDefinitionRequestTypeDef(
+    _RequiredMetricDefinitionRequestTypeDef, _OptionalMetricDefinitionRequestTypeDef
+):
     pass
 
 UserDetailsTypeDef = TypedDict(
     "UserDetailsTypeDef",
     {
         "sessionId": str,
         "userId": str,
@@ -444,14 +427,15 @@
 
 class PutRumMetricsDestinationRequestRequestTypeDef(
     _RequiredPutRumMetricsDestinationRequestRequestTypeDef,
     _OptionalPutRumMetricsDestinationRequestRequestTypeDef,
 ):
     pass
 
+TimestampTypeDef = Union[datetime, str]
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -460,14 +444,17 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AppMonitorConfigurationUnionTypeDef = Union[
+    AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
+]
 _RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppMonitorRequestRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
     },
 )
@@ -514,61 +501,14 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "MetricDefinition": MetricDefinitionRequestOutputTypeDef,
     },
 )
 
-_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-        "MetricDefinitions": Sequence[
-            Union[MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef]
-        ],
-    },
-)
-_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    {
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
-class BatchCreateRumMetricDefinitionsRequestRequestTypeDef(
-    _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-    _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-        "MetricDefinition": MetricDefinitionRequestTypeDef,
-        "MetricDefinitionId": str,
-    },
-)
-_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef",
-    {
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
-class UpdateRumMetricDefinitionRequestRequestTypeDef(
-    _RequiredUpdateRumMetricDefinitionRequestRequestTypeDef,
-    _OptionalUpdateRumMetricDefinitionRequestRequestTypeDef,
-):
-    pass
-
 BatchGetRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     {
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -725,24 +665,59 @@
     {
         "Destinations": List[MetricDestinationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutRumEventsRequestRequestTypeDef = TypedDict(
-    "PutRumEventsRequestRequestTypeDef",
+MetricDefinitionRequestUnionTypeDef = Union[
+    MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef
+]
+_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef",
     {
-        "AppMonitorDetails": AppMonitorDetailsTypeDef,
-        "BatchId": str,
-        "Id": str,
-        "RumEvents": Sequence[RumEventTypeDef],
-        "UserDetails": UserDetailsTypeDef,
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+        "MetricDefinition": MetricDefinitionRequestTypeDef,
+        "MetricDefinitionId": str,
+    },
+)
+_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+class UpdateRumMetricDefinitionRequestRequestTypeDef(
+    _RequiredUpdateRumMetricDefinitionRequestRequestTypeDef,
+    _OptionalUpdateRumMetricDefinitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredRumEventTypeDef = TypedDict(
+    "_RequiredRumEventTypeDef",
+    {
+        "details": str,
+        "id": str,
+        "timestamp": TimestampTypeDef,
+        "type": str,
     },
 )
+_OptionalRumEventTypeDef = TypedDict(
+    "_OptionalRumEventTypeDef",
+    {
+        "metadata": str,
+    },
+    total=False,
+)
+
+class RumEventTypeDef(_RequiredRumEventTypeDef, _OptionalRumEventTypeDef):
+    pass
 
 BatchCreateRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchCreateRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -762,14 +737,47 @@
         "Name": str,
         "State": StateEnumType,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    {
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+        "MetricDefinitions": Sequence[MetricDefinitionRequestUnionTypeDef],
+    },
+)
+_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+class BatchCreateRumMetricDefinitionsRequestRequestTypeDef(
+    _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+    _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+):
+    pass
+
+PutRumEventsRequestRequestTypeDef = TypedDict(
+    "PutRumEventsRequestRequestTypeDef",
+    {
+        "AppMonitorDetails": AppMonitorDetailsTypeDef,
+        "BatchId": str,
+        "Id": str,
+        "RumEvents": Sequence[RumEventTypeDef],
+        "UserDetails": UserDetailsTypeDef,
+    },
+)
+
 GetAppMonitorResponseTypeDef = TypedDict(
     "GetAppMonitorResponseTypeDef",
     {
         "AppMonitor": AppMonitorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/PKG-INFO` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatchRUM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rum type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 rum type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rum)](https://pepy.tech/project/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
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
@@ -329,30 +329,29 @@
 )
 
 
 def check_value(value: BatchGetRumMetricDefinitionsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rum.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rum.type_defs import (
     AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
     CustomEventsTypeDef,
     MetricDefinitionRequestOutputTypeDef,
-    MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
     CwLogTypeDef,
@@ -361,45 +360,49 @@
     QueryFilterTypeDef,
     TimeRangeTypeDef,
     GetAppMonitorRequestRequestTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
     ListRumMetricsDestinationsRequestRequestTypeDef,
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RumEventTypeDef,
+    MetricDefinitionRequestTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
+    TimestampTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AppMonitorConfigurationUnionTypeDef,
     CreateAppMonitorRequestRequestTypeDef,
     UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
-    BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-    UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     GetAppMonitorDataResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
     ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
-    PutRumEventsRequestRequestTypeDef,
+    MetricDefinitionRequestUnionTypeDef,
+    UpdateRumMetricDefinitionRequestRequestTypeDef,
+    RumEventTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
+    BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+    PutRumEventsRequestRequestTypeDef,
     GetAppMonitorResponseTypeDef,
 )
 
 
-def get_structure() -> AppMonitorConfigurationOutputTypeDef:
+def get_value() -> AppMonitorConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/SOURCES.txt` & `mypy-boto3-rum-1.28.16/mypy_boto3_rum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15.post1/setup.py` & `mypy-boto3-rum-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rum",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_rum"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CloudWatchRUM 1.28.16 service generated with mypy-boto3-builder"
+        " 7.17.1"
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
-    keywords="boto3 rum type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 rum type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_rum": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

