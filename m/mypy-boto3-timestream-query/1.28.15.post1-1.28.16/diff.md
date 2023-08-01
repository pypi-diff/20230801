# Comparing `tmp/mypy-boto3-timestream-query-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-timestream-query-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-query-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:21 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-query-1.28.16.tar", last modified: Tue Aug  1 11:38:00 2023, max compression
```

## Comparing `mypy-boto3-timestream-query-1.28.15.post1.tar` & `mypy-boto3-timestream-query-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:21.801442 mypy-boto3-timestream-query-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-07-29 10:04:21.801442 mypy-boto3-timestream-query-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:21.789441 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-07-29 10:00:49.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-29 10:00:49.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-07-29 10:00:49.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21640 2023-07-29 10:00:49.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:21.801442 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:21.801442 mypy-boto3-timestream-query-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:00.720706 mypy-boto3-timestream-query-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-08-01 11:38:00.720706 mypy-boto3-timestream-query-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:00.716706 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21882 2023-08-01 11:34:26.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-08-01 11:34:26.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:00.720706 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-08-01 11:38:00.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:38:00.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:00.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:00.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:00.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:38:00.000000 mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:00.720706 mypy-boto3-timestream-query-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-01 11:34:25.000000 mypy-boto3-timestream-query-1.28.16/setup.py
```

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/LICENSE` & `mypy-boto3-timestream-query-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/PKG-INFO` & `mypy-boto3-timestream-query-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.TimestreamQuery 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.TimestreamQuery 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 timestream-query type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 timestream-query type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
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
@@ -329,20 +329,20 @@
 )
 
 
 def check_value(value: DimensionValueTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_timestream_query.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
@@ -351,15 +351,15 @@
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
     DimensionMappingTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
-    ExecuteScheduledQueryRequestRequestTypeDef,
+    TimestampTypeDef,
     ExecutionStatsTypeDef,
     PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     SnsConfigurationTypeDef,
     ParameterMappingTypeDef,
@@ -376,14 +376,15 @@
     EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
+    ExecuteScheduledQueryRequestRequestTypeDef,
     ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     QueryRequestQueryPaginateTypeDef,
     MixedMeasureMappingOutputTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
@@ -396,19 +397,20 @@
     TimestreamConfigurationTypeDef,
     ScheduledQueryTypeDef,
     TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
     ScheduledQueryDescriptionTypeDef,
     CreateScheduledQueryRequestRequestTypeDef,
+    TargetConfigurationUnionTypeDef,
     DescribeScheduledQueryResponseTypeDef,
 )
 
 
-def get_structure() -> CancelQueryRequestRequestTypeDef:
+def get_value() -> CancelQueryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/README.md` & `mypy-boto3-timestream-query-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
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
@@ -297,20 +297,20 @@
 )
 
 
 def check_value(value: DimensionValueTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_timestream_query.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
@@ -319,15 +319,15 @@
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
     DimensionMappingTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
-    ExecuteScheduledQueryRequestRequestTypeDef,
+    TimestampTypeDef,
     ExecutionStatsTypeDef,
     PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     SnsConfigurationTypeDef,
     ParameterMappingTypeDef,
@@ -344,14 +344,15 @@
     EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
+    ExecuteScheduledQueryRequestRequestTypeDef,
     ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     QueryRequestQueryPaginateTypeDef,
     MixedMeasureMappingOutputTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
@@ -364,19 +365,20 @@
     TimestreamConfigurationTypeDef,
     ScheduledQueryTypeDef,
     TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
     ScheduledQueryDescriptionTypeDef,
     CreateScheduledQueryRequestRequestTypeDef,
+    TargetConfigurationUnionTypeDef,
     DescribeScheduledQueryResponseTypeDef,
 )
 
 
-def get_structure() -> CancelQueryRequestRequestTypeDef:
+def get_value() -> CancelQueryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__init__.py` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__init__.pyi` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__main__.py` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamQuery 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.TimestreamQuery 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
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

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/client.py` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_timestream_query.client import TimestreamQueryClient
 
     session = Session()
     client: TimestreamQueryClient = session.client("timestream-query")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ScheduledQueryStateType
 from .paginator import ListScheduledQueriesPaginator, ListTagsForResourcePaginator, QueryPaginator
 from .type_defs import (
     CancelQueryResponseTypeDef,
@@ -31,16 +30,16 @@
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    TargetConfigurationOutputTypeDef,
-    TargetConfigurationTypeDef,
+    TargetConfigurationUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -115,17 +114,15 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: Union[
-            TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
-        ] = ...,
+        TargetConfiguration: TargetConfigurationUnionTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
@@ -158,19 +155,15 @@
         Provides detailed information about a scheduled query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_scheduled_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#describe_scheduled_query)
         """
 
     def execute_scheduled_query(
-        self,
-        *,
-        ScheduledQueryArn: str,
-        InvocationTime: Union[datetime, str],
-        ClientToken: str = ...
+        self, *, ScheduledQueryArn: str, InvocationTime: TimestampTypeDef, ClientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         You can use this API to run a scheduled query manually.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.execute_scheduled_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#execute_scheduled_query)
         """
```

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/client.pyi` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_timestream_query.client import TimestreamQueryClient
 
     session = Session()
     client: TimestreamQueryClient = session.client("timestream-query")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ScheduledQueryStateType
 from .paginator import ListScheduledQueriesPaginator, ListTagsForResourcePaginator, QueryPaginator
 from .type_defs import (
     CancelQueryResponseTypeDef,
@@ -31,16 +30,16 @@
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    TargetConfigurationOutputTypeDef,
-    TargetConfigurationTypeDef,
+    TargetConfigurationUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -107,17 +106,15 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: Union[
-            TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
-        ] = ...,
+        TargetConfiguration: TargetConfigurationUnionTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
@@ -146,19 +143,15 @@
         """
         Provides detailed information about a scheduled query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_scheduled_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#describe_scheduled_query)
         """
     def execute_scheduled_query(
-        self,
-        *,
-        ScheduledQueryArn: str,
-        InvocationTime: Union[datetime, str],
-        ClientToken: str = ...
+        self, *, ScheduledQueryArn: str, InvocationTime: TimestampTypeDef, ClientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         You can use this API to run a scheduled query manually.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.execute_scheduled_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#execute_scheduled_query)
         """
```

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/literals.py` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/literals.pyi` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/paginator.py` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/paginator.pyi` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/type_defs.py` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_timestream_query.type_defs import CancelQueryRequestRequestTypeDef
 
-    data: CancelQueryRequestRequestTypeDef = {...}
+    data: CancelQueryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
@@ -44,15 +44,15 @@
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
     "DimensionMappingTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
-    "ExecuteScheduledQueryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ExecutionStatsTypeDef",
     "PaginatorConfigTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
     "SnsConfigurationTypeDef",
     "ParameterMappingTypeDef",
@@ -69,14 +69,15 @@
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
+    "ExecuteScheduledQueryRequestRequestTypeDef",
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "QueryRequestQueryPaginateTypeDef",
     "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
@@ -89,14 +90,15 @@
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
     "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
     "ScheduledQueryDescriptionTypeDef",
     "CreateScheduledQueryRequestRequestTypeDef",
+    "TargetConfigurationUnionTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
@@ -147,15 +149,15 @@
         "Value": str,
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
-        "Data": List[Dict[str, Any]],
+        "Data": List["DatumTypeDef"],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
@@ -218,37 +220,15 @@
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
-_RequiredExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredExecuteScheduledQueryRequestRequestTypeDef",
-    {
-        "ScheduledQueryArn": str,
-        "InvocationTime": Union[datetime, str],
-    },
-)
-_OptionalExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class ExecuteScheduledQueryRequestRequestTypeDef(
-    _RequiredExecuteScheduledQueryRequestRequestTypeDef,
-    _OptionalExecuteScheduledQueryRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": int,
         "DataWrites": int,
         "BytesMetered": int,
         "RecordsIngested": int,
@@ -509,14 +489,37 @@
     "ErrorReportLocationTypeDef",
     {
         "S3ReportLocation": S3ReportLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredExecuteScheduledQueryRequestRequestTypeDef",
+    {
+        "ScheduledQueryArn": str,
+        "InvocationTime": TimestampTypeDef,
+    },
+)
+_OptionalExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class ExecuteScheduledQueryRequestRequestTypeDef(
+    _RequiredExecuteScheduledQueryRequestRequestTypeDef,
+    _OptionalExecuteScheduledQueryRequestRequestTypeDef,
+):
+    pass
+
+
 ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -866,14 +869,17 @@
 class CreateScheduledQueryRequestRequestTypeDef(
     _RequiredCreateScheduledQueryRequestRequestTypeDef,
     _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
 
+TargetConfigurationUnionTypeDef = Union[
+    TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
+]
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/type_defs.pyi` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_timestream_query.type_defs import CancelQueryRequestRequestTypeDef
 
-    data: CancelQueryRequestRequestTypeDef = {...}
+    data: CancelQueryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
@@ -43,15 +43,15 @@
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
     "DimensionMappingTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
-    "ExecuteScheduledQueryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ExecutionStatsTypeDef",
     "PaginatorConfigTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
     "SnsConfigurationTypeDef",
     "ParameterMappingTypeDef",
@@ -68,14 +68,15 @@
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
+    "ExecuteScheduledQueryRequestRequestTypeDef",
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "QueryRequestQueryPaginateTypeDef",
     "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
@@ -88,14 +89,15 @@
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
     "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
     "ScheduledQueryDescriptionTypeDef",
     "CreateScheduledQueryRequestRequestTypeDef",
+    "TargetConfigurationUnionTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
@@ -144,15 +146,15 @@
         "Value": str,
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
-        "Data": List[Dict[str, Any]],
+        "Data": List["DatumTypeDef"],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
@@ -213,35 +215,15 @@
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
-_RequiredExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredExecuteScheduledQueryRequestRequestTypeDef",
-    {
-        "ScheduledQueryArn": str,
-        "InvocationTime": Union[datetime, str],
-    },
-)
-_OptionalExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class ExecuteScheduledQueryRequestRequestTypeDef(
-    _RequiredExecuteScheduledQueryRequestRequestTypeDef,
-    _OptionalExecuteScheduledQueryRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": int,
         "DataWrites": int,
         "BytesMetered": int,
         "RecordsIngested": int,
@@ -494,14 +476,35 @@
     "ErrorReportLocationTypeDef",
     {
         "S3ReportLocation": S3ReportLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredExecuteScheduledQueryRequestRequestTypeDef",
+    {
+        "ScheduledQueryArn": str,
+        "InvocationTime": TimestampTypeDef,
+    },
+)
+_OptionalExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class ExecuteScheduledQueryRequestRequestTypeDef(
+    _RequiredExecuteScheduledQueryRequestRequestTypeDef,
+    _OptionalExecuteScheduledQueryRequestRequestTypeDef,
+):
+    pass
+
 ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -829,14 +832,17 @@
 
 class CreateScheduledQueryRequestRequestTypeDef(
     _RequiredCreateScheduledQueryRequestRequestTypeDef,
     _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
+TargetConfigurationUnionTypeDef = Union[
+    TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
+]
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/PKG-INFO` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.TimestreamQuery 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.TimestreamQuery 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 timestream-query type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 timestream-query type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
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
@@ -329,20 +329,20 @@
 )
 
 
 def check_value(value: DimensionValueTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_timestream_query.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
@@ -351,15 +351,15 @@
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
     DimensionMappingTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
-    ExecuteScheduledQueryRequestRequestTypeDef,
+    TimestampTypeDef,
     ExecutionStatsTypeDef,
     PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     SnsConfigurationTypeDef,
     ParameterMappingTypeDef,
@@ -376,14 +376,15 @@
     EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
+    ExecuteScheduledQueryRequestRequestTypeDef,
     ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     QueryRequestQueryPaginateTypeDef,
     MixedMeasureMappingOutputTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
@@ -396,19 +397,20 @@
     TimestreamConfigurationTypeDef,
     ScheduledQueryTypeDef,
     TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
     ScheduledQueryDescriptionTypeDef,
     CreateScheduledQueryRequestRequestTypeDef,
+    TargetConfigurationUnionTypeDef,
     DescribeScheduledQueryResponseTypeDef,
 )
 
 
-def get_structure() -> CancelQueryRequestRequestTypeDef:
+def get_value() -> CancelQueryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/SOURCES.txt` & `mypy-boto3-timestream-query-1.28.16/mypy_boto3_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15.post1/setup.py` & `mypy-boto3-timestream-query-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-query",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamQuery 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.TimestreamQuery 1.28.16 service generated with"
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
-    keywords="boto3 timestream-query type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 timestream-query type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_timestream_query": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

