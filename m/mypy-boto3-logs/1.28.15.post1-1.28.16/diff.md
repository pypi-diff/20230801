# Comparing `tmp/mypy-boto3-logs-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-logs-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-logs-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:33 2023, max compression
+gzip compressed data, was "mypy-boto3-logs-1.28.16.tar", last modified: Tue Aug  1 11:37:13 2023, max compression
```

## Comparing `mypy-boto3-logs-1.28.15.post1.tar` & `mypy-boto3-logs-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.957252 mypy-boto3-logs-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18875 2023-07-29 10:03:33.949252 mypy-boto3-logs-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.949252 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38437 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38370 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37794 2023-07-29 09:50:07.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37759 2023-07-29 09:50:07.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.949252 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18875 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:33.957252 mypy-boto3-logs-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.820836 mypy-boto3-logs-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-08-01 11:37:13.820836 mypy-boto3-logs-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.816836 mypy-boto3-logs-1.28.16/mypy_boto3_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38337 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38270 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-08-01 11:22:57.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-08-01 11:22:57.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-08-01 11:22:57.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37884 2023-08-01 11:23:00.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37849 2023-08-01 11:22:57.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.820836 mypy-boto3-logs-1.28.16/mypy_boto3_logs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-08-01 11:37:13.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-01 11:37:13.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:13.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 11:37:13.000000 mypy-boto3-logs-1.28.16/mypy_boto3_logs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:13.820836 mypy-boto3-logs-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-01 11:22:56.000000 mypy-boto3-logs-1.28.16/setup.py
```

### Comparing `mypy-boto3-logs-1.28.15.post1/LICENSE` & `mypy-boto3-logs-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15.post1/PKG-INFO` & `mypy-boto3-logs-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-logs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatchLogs 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatchLogs 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 logs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 logs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-logs)](https://pepy.tech/project/mypy-boto3-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchLogs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[boto3.CloudWatchLogs 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
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
@@ -358,20 +358,20 @@
 )
 
 
 def check_value(value: DataProtectionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_logs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_logs.type_defs import (
     AccountPolicyTypeDef,
     AssociateKmsKeyRequestRequestTypeDef,
     CancelExportTaskRequestRequestTypeDef,
     CreateExportTaskRequestRequestTypeDef,
@@ -478,22 +478,23 @@
     FilterLogEventsResponseTypeDef,
     GetLogEventsResponseTypeDef,
     GetLogGroupFieldsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     PutLogEventsRequestRequestTypeDef,
     TestMetricFilterResponseTypeDef,
     MetricFilterTypeDef,
-    PutMetricFilterRequestRequestTypeDef,
+    MetricTransformationUnionTypeDef,
     PutLogEventsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeMetricFiltersResponseTypeDef,
+    PutMetricFilterRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountPolicyTypeDef:
+def get_value() -> AccountPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-logs-1.28.15.post1/README.md` & `mypy-boto3-logs-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-logs)](https://pepy.tech/project/mypy-boto3-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchLogs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[boto3.CloudWatchLogs 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
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
@@ -326,20 +326,20 @@
 )
 
 
 def check_value(value: DataProtectionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_logs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_logs.type_defs import (
     AccountPolicyTypeDef,
     AssociateKmsKeyRequestRequestTypeDef,
     CancelExportTaskRequestRequestTypeDef,
     CreateExportTaskRequestRequestTypeDef,
@@ -446,22 +446,23 @@
     FilterLogEventsResponseTypeDef,
     GetLogEventsResponseTypeDef,
     GetLogGroupFieldsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     PutLogEventsRequestRequestTypeDef,
     TestMetricFilterResponseTypeDef,
     MetricFilterTypeDef,
-    PutMetricFilterRequestRequestTypeDef,
+    MetricTransformationUnionTypeDef,
     PutLogEventsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeMetricFiltersResponseTypeDef,
+    PutMetricFilterRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountPolicyTypeDef:
+def get_value() -> AccountPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__init__.py` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__init__.pyi` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__main__.py` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchLogs 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CloudWatchLogs 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs\nOther"
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

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/client.py` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_logs.client import CloudWatchLogsClient
 
     session = Session()
     client: CloudWatchLogsClient = session.client("logs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DistributionType, ExportTaskStatusCodeType, OrderByType, QueryStatusType
 from .paginator import (
     DescribeDestinationsPaginator,
     DescribeExportTasksPaginator,
@@ -49,16 +49,15 @@
     GetLogEventsResponseTypeDef,
     GetLogGroupFieldsResponseTypeDef,
     GetLogRecordResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupResponseTypeDef,
-    MetricTransformationOutputTypeDef,
-    MetricTransformationTypeDef,
+    MetricTransformationUnionTypeDef,
     PutAccountPolicyResponseTypeDef,
     PutDataProtectionPolicyResponseTypeDef,
     PutDestinationResponseTypeDef,
     PutLogEventsResponseTypeDef,
     PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     StartQueryResponseTypeDef,
@@ -613,17 +612,15 @@
 
     def put_metric_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
-        metricTransformations: Sequence[
-            Union[MetricTransformationTypeDef, MetricTransformationOutputTypeDef]
-        ]
+        metricTransformations: Sequence[MetricTransformationUnionTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a metric filter and associates it with the specified log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_metric_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#put_metric_filter)
```

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/client.pyi` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_logs.client import CloudWatchLogsClient
 
     session = Session()
     client: CloudWatchLogsClient = session.client("logs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DistributionType, ExportTaskStatusCodeType, OrderByType, QueryStatusType
 from .paginator import (
     DescribeDestinationsPaginator,
     DescribeExportTasksPaginator,
@@ -49,16 +49,15 @@
     GetLogEventsResponseTypeDef,
     GetLogGroupFieldsResponseTypeDef,
     GetLogRecordResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupResponseTypeDef,
-    MetricTransformationOutputTypeDef,
-    MetricTransformationTypeDef,
+    MetricTransformationUnionTypeDef,
     PutAccountPolicyResponseTypeDef,
     PutDataProtectionPolicyResponseTypeDef,
     PutDestinationResponseTypeDef,
     PutLogEventsResponseTypeDef,
     PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     StartQueryResponseTypeDef,
@@ -566,17 +565,15 @@
         """
     def put_metric_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
-        metricTransformations: Sequence[
-            Union[MetricTransformationTypeDef, MetricTransformationOutputTypeDef]
-        ]
+        metricTransformations: Sequence[MetricTransformationUnionTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a metric filter and associates it with the specified log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_metric_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#put_metric_filter)
```

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/literals.py` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/literals.pyi` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/paginator.py` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/paginator.pyi` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/type_defs.py` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_logs.type_defs import AccountPolicyTypeDef
 
-    data: AccountPolicyTypeDef = {...}
+    data: AccountPolicyTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     DataProtectionStatusType,
@@ -141,18 +141,19 @@
     "FilterLogEventsResponseTypeDef",
     "GetLogEventsResponseTypeDef",
     "GetLogGroupFieldsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "PutLogEventsRequestRequestTypeDef",
     "TestMetricFilterResponseTypeDef",
     "MetricFilterTypeDef",
-    "PutMetricFilterRequestRequestTypeDef",
+    "MetricTransformationUnionTypeDef",
     "PutLogEventsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeMetricFiltersResponseTypeDef",
+    "PutMetricFilterRequestRequestTypeDef",
 )
 
 AccountPolicyTypeDef = TypedDict(
     "AccountPolicyTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
@@ -1455,26 +1456,17 @@
         "metricTransformations": List[MetricTransformationOutputTypeDef],
         "creationTime": int,
         "logGroupName": str,
     },
     total=False,
 )
 
-PutMetricFilterRequestRequestTypeDef = TypedDict(
-    "PutMetricFilterRequestRequestTypeDef",
-    {
-        "logGroupName": str,
-        "filterName": str,
-        "filterPattern": str,
-        "metricTransformations": Sequence[
-            Union[MetricTransformationTypeDef, MetricTransformationOutputTypeDef]
-        ],
-    },
-)
-
+MetricTransformationUnionTypeDef = Union[
+    MetricTransformationTypeDef, MetricTransformationOutputTypeDef
+]
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
         "rejectedLogEventsInfo": RejectedLogEventsInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1493,7 +1485,17 @@
     "DescribeMetricFiltersResponseTypeDef",
     {
         "metricFilters": List[MetricFilterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+PutMetricFilterRequestRequestTypeDef = TypedDict(
+    "PutMetricFilterRequestRequestTypeDef",
+    {
+        "logGroupName": str,
+        "filterName": str,
+        "filterPattern": str,
+        "metricTransformations": Sequence[MetricTransformationUnionTypeDef],
+    },
+)
```

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/type_defs.pyi` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_logs.type_defs import AccountPolicyTypeDef
 
-    data: AccountPolicyTypeDef = {...}
+    data: AccountPolicyTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     DataProtectionStatusType,
@@ -140,18 +140,19 @@
     "FilterLogEventsResponseTypeDef",
     "GetLogEventsResponseTypeDef",
     "GetLogGroupFieldsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "PutLogEventsRequestRequestTypeDef",
     "TestMetricFilterResponseTypeDef",
     "MetricFilterTypeDef",
-    "PutMetricFilterRequestRequestTypeDef",
+    "MetricTransformationUnionTypeDef",
     "PutLogEventsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeMetricFiltersResponseTypeDef",
+    "PutMetricFilterRequestRequestTypeDef",
 )
 
 AccountPolicyTypeDef = TypedDict(
     "AccountPolicyTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
@@ -1420,26 +1421,17 @@
         "metricTransformations": List[MetricTransformationOutputTypeDef],
         "creationTime": int,
         "logGroupName": str,
     },
     total=False,
 )
 
-PutMetricFilterRequestRequestTypeDef = TypedDict(
-    "PutMetricFilterRequestRequestTypeDef",
-    {
-        "logGroupName": str,
-        "filterName": str,
-        "filterPattern": str,
-        "metricTransformations": Sequence[
-            Union[MetricTransformationTypeDef, MetricTransformationOutputTypeDef]
-        ],
-    },
-)
-
+MetricTransformationUnionTypeDef = Union[
+    MetricTransformationTypeDef, MetricTransformationOutputTypeDef
+]
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
         "rejectedLogEventsInfo": RejectedLogEventsInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1458,7 +1450,17 @@
     "DescribeMetricFiltersResponseTypeDef",
     {
         "metricFilters": List[MetricFilterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+PutMetricFilterRequestRequestTypeDef = TypedDict(
+    "PutMetricFilterRequestRequestTypeDef",
+    {
+        "logGroupName": str,
+        "filterName": str,
+        "filterPattern": str,
+        "metricTransformations": Sequence[MetricTransformationUnionTypeDef],
+    },
+)
```

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/PKG-INFO` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-logs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatchLogs 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatchLogs 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 logs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 logs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-logs)](https://pepy.tech/project/mypy-boto3-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchLogs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[boto3.CloudWatchLogs 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
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
@@ -358,20 +358,20 @@
 )
 
 
 def check_value(value: DataProtectionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_logs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_logs.type_defs import (
     AccountPolicyTypeDef,
     AssociateKmsKeyRequestRequestTypeDef,
     CancelExportTaskRequestRequestTypeDef,
     CreateExportTaskRequestRequestTypeDef,
@@ -478,22 +478,23 @@
     FilterLogEventsResponseTypeDef,
     GetLogEventsResponseTypeDef,
     GetLogGroupFieldsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     PutLogEventsRequestRequestTypeDef,
     TestMetricFilterResponseTypeDef,
     MetricFilterTypeDef,
-    PutMetricFilterRequestRequestTypeDef,
+    MetricTransformationUnionTypeDef,
     PutLogEventsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeMetricFiltersResponseTypeDef,
+    PutMetricFilterRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountPolicyTypeDef:
+def get_value() -> AccountPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/SOURCES.txt` & `mypy-boto3-logs-1.28.16/mypy_boto3_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15.post1/setup.py` & `mypy-boto3-logs-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-logs",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_logs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchLogs 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CloudWatchLogs 1.28.16 service generated with"
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
-    keywords="boto3 logs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 logs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_logs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

