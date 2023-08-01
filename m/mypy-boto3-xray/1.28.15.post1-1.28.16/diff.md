# Comparing `tmp/mypy-boto3-xray-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-xray-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-xray-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:27 2023, max compression
+gzip compressed data, was "mypy-boto3-xray-1.28.16.tar", last modified: Tue Aug  1 11:38:06 2023, max compression
```

## Comparing `mypy-boto3-xray-1.28.15.post1.tar` & `mypy-boto3-xray-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25939 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44015 2023-07-29 10:02:00.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43964 2023-07-29 10:02:00.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:06.808653 mypy-boto3-xray-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:35:39.000000 mypy-boto3-xray-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-08-01 11:38:06.808653 mypy-boto3-xray-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-08-01 11:35:39.000000 mypy-boto3-xray-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:06.808653 mypy-boto3-xray-1.28.16/mypy_boto3_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-01 11:35:39.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-01 11:35:39.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 11:35:39.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25852 2023-08-01 11:35:40.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25805 2023-08-01 11:35:39.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-08-01 11:35:40.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-08-01 11:35:40.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-08-01 11:35:40.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-08-01 11:35:40.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:39.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44118 2023-08-01 11:35:41.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44067 2023-08-01 11:35:40.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:35:39.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:06.808653 mypy-boto3-xray-1.28.16/mypy_boto3_xray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-08-01 11:38:06.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-01 11:38:06.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:06.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:06.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:06.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 11:38:06.000000 mypy-boto3-xray-1.28.16/mypy_boto3_xray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:06.808653 mypy-boto3-xray-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-01 11:35:39.000000 mypy-boto3-xray-1.28.16/setup.py
```

### Comparing `mypy-boto3-xray-1.28.15.post1/LICENSE` & `mypy-boto3-xray-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15.post1/PKG-INFO` & `mypy-boto3-xray-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.XRay 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 xray type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 xray type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-xray)](https://pepy.tech/project/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
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
@@ -354,20 +354,20 @@
 )
 
 
 def check_value(value: BatchGetTracesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_xray.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
@@ -386,25 +386,21 @@
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
-    GetInsightImpactGraphRequestRequestTypeDef,
+    TimestampTypeDef,
     GetInsightRequestRequestTypeDef,
-    GetInsightSummariesRequestRequestTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
-    SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
-    GetServiceGraphRequestRequestTypeDef,
-    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
@@ -419,21 +415,18 @@
     SamplingRuleOutputTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
-    TelemetryRecordTypeDef,
     BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
     GetGroupsRequestGetGroupsPaginateTypeDef,
     GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     GroupSummaryTypeDef,
     GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -442,39 +435,48 @@
     CreateSamplingRuleRequestRequestTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
+    GetInsightImpactGraphRequestRequestTypeDef,
+    GetInsightSummariesRequestRequestTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    GetServiceGraphRequestRequestTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    SamplingStatisticsDocumentTypeDef,
+    TelemetryRecordTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
-    GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
     SamplingRuleRecordTypeDef,
+    SamplingRuleUnionTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
-    PutTelemetryRecordsRequestRequestTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
     EdgeTypeDef,
     TimeSeriesServiceStatisticsTypeDef,
     ErrorRootCauseServiceTypeDef,
     FaultRootCauseServiceTypeDef,
+    GetSamplingTargetsRequestRequestTypeDef,
+    PutTelemetryRecordsRequestRequestTypeDef,
     GetInsightImpactGraphResultTypeDef,
     ResponseTimeRootCauseTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetSamplingRulesResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
     BatchGetTracesResultTypeDef,
@@ -488,15 +490,15 @@
     GetServiceGraphResultTypeDef,
     GetTraceGraphResultTypeDef,
     TraceSummaryTypeDef,
     GetTraceSummariesResultTypeDef,
 )
 
 
-def get_structure() -> AliasTypeDef:
+def get_value() -> AliasTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-xray-1.28.15.post1/README.md` & `mypy-boto3-xray-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-xray)](https://pepy.tech/project/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
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
@@ -322,20 +322,20 @@
 )
 
 
 def check_value(value: BatchGetTracesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_xray.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
@@ -354,25 +354,21 @@
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
-    GetInsightImpactGraphRequestRequestTypeDef,
+    TimestampTypeDef,
     GetInsightRequestRequestTypeDef,
-    GetInsightSummariesRequestRequestTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
-    SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
-    GetServiceGraphRequestRequestTypeDef,
-    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
@@ -387,21 +383,18 @@
     SamplingRuleOutputTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
-    TelemetryRecordTypeDef,
     BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
     GetGroupsRequestGetGroupsPaginateTypeDef,
     GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     GroupSummaryTypeDef,
     GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -410,39 +403,48 @@
     CreateSamplingRuleRequestRequestTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
+    GetInsightImpactGraphRequestRequestTypeDef,
+    GetInsightSummariesRequestRequestTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    GetServiceGraphRequestRequestTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    SamplingStatisticsDocumentTypeDef,
+    TelemetryRecordTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
-    GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
     SamplingRuleRecordTypeDef,
+    SamplingRuleUnionTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
-    PutTelemetryRecordsRequestRequestTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
     EdgeTypeDef,
     TimeSeriesServiceStatisticsTypeDef,
     ErrorRootCauseServiceTypeDef,
     FaultRootCauseServiceTypeDef,
+    GetSamplingTargetsRequestRequestTypeDef,
+    PutTelemetryRecordsRequestRequestTypeDef,
     GetInsightImpactGraphResultTypeDef,
     ResponseTimeRootCauseTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetSamplingRulesResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
     BatchGetTracesResultTypeDef,
@@ -456,15 +458,15 @@
     GetServiceGraphResultTypeDef,
     GetTraceGraphResultTypeDef,
     TraceSummaryTypeDef,
     GetTraceSummariesResultTypeDef,
 )
 
 
-def get_structure() -> AliasTypeDef:
+def get_value() -> AliasTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__init__.py` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__init__.pyi` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__main__.py` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.XRay 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.XRay 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay\nOther"
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

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/client.py` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_xray.client import XRayClient
 
     session = Session()
     client: XRayClient = session.client("xray")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EncryptionTypeType, InsightStateType, TimeRangeTypeType
 from .paginator import (
     BatchGetTracesPaginator,
     GetGroupsPaginator,
@@ -53,21 +52,21 @@
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
-    SamplingRuleOutputTypeDef,
-    SamplingRuleTypeDef,
+    SamplingRuleUnionTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
+    TimestampTypeDef,
     UpdateGroupResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -154,18 +153,15 @@
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_group)
         """
 
     def create_sampling_rule(
-        self,
-        *,
-        SamplingRule: Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        self, *, SamplingRule: SamplingRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_sampling_rule)
         """
@@ -255,30 +251,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_events)
         """
 
     def get_insight_impact_graph(
         self,
         *,
         InsightId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...
     ) -> GetInsightImpactGraphResultTypeDef:
         """
         Retrieves a service graph structure filtered by the specified insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_impact_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_impact_graph)
         """
 
     def get_insight_summaries(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         States: Sequence[InsightStateType] = ...,
         GroupARN: str = ...,
         GroupName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetInsightSummariesResultTypeDef:
         """
@@ -317,16 +313,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_sampling_targets)
         """
 
     def get_service_graph(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         NextToken: str = ...
     ) -> GetServiceGraphResultTypeDef:
         """
         Retrieves a document that describes services that process incoming requests, and
         downstream services that they call as a result.
@@ -334,16 +330,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_service_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_service_graph)
         """
 
     def get_time_series_service_statistics(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
         NextToken: str = ...
     ) -> GetTimeSeriesServiceStatisticsResultTypeDef:
@@ -363,16 +359,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_trace_graph)
         """
 
     def get_trace_summaries(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
         NextToken: str = ...
     ) -> GetTraceSummariesResultTypeDef:
         """
```

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/client.pyi` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_xray.client import XRayClient
 
     session = Session()
     client: XRayClient = session.client("xray")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EncryptionTypeType, InsightStateType, TimeRangeTypeType
 from .paginator import (
     BatchGetTracesPaginator,
     GetGroupsPaginator,
@@ -53,21 +52,21 @@
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
-    SamplingRuleOutputTypeDef,
-    SamplingRuleTypeDef,
+    SamplingRuleUnionTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
+    TimestampTypeDef,
     UpdateGroupResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -145,18 +144,15 @@
         """
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_group)
         """
     def create_sampling_rule(
-        self,
-        *,
-        SamplingRule: Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        self, *, SamplingRule: SamplingRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_sampling_rule)
         """
@@ -236,29 +232,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_events)
         """
     def get_insight_impact_graph(
         self,
         *,
         InsightId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...
     ) -> GetInsightImpactGraphResultTypeDef:
         """
         Retrieves a service graph structure filtered by the specified insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_impact_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_impact_graph)
         """
     def get_insight_summaries(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         States: Sequence[InsightStateType] = ...,
         GroupARN: str = ...,
         GroupName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetInsightSummariesResultTypeDef:
         """
@@ -293,32 +289,32 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_sampling_targets)
         """
     def get_service_graph(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         NextToken: str = ...
     ) -> GetServiceGraphResultTypeDef:
         """
         Retrieves a document that describes services that process incoming requests, and
         downstream services that they call as a result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_service_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_service_graph)
         """
     def get_time_series_service_statistics(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
         NextToken: str = ...
     ) -> GetTimeSeriesServiceStatisticsResultTypeDef:
@@ -336,16 +332,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_trace_graph)
         """
     def get_trace_summaries(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
         NextToken: str = ...
     ) -> GetTraceSummariesResultTypeDef:
         """
```

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/literals.py` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/literals.pyi` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/paginator.py` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")
     get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
     get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")
     list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import TimeRangeTypeType
 from .type_defs import (
     BatchGetTracesResultTypeDef,
     GetGroupsResultTypeDef,
@@ -52,14 +51,15 @@
     GetTimeSeriesServiceStatisticsResultTypeDef,
     GetTraceGraphResultTypeDef,
     GetTraceSummariesResultTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     SamplingStrategyTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "BatchGetTracesPaginator",
     "GetGroupsPaginator",
     "GetSamplingRulesPaginator",
     "GetSamplingStatisticSummariesPaginator",
@@ -147,16 +147,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getservicegraphpaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getservicegraphpaginator)
@@ -168,16 +168,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettimeseriesservicestatisticspaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
@@ -207,16 +207,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracesummariespaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTraceSummariesResultTypeDef]:
         """
```

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/paginator.pyi` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")
     get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
     get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")
     list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import TimeRangeTypeType
 from .type_defs import (
     BatchGetTracesResultTypeDef,
     GetGroupsResultTypeDef,
@@ -52,14 +51,15 @@
     GetTimeSeriesServiceStatisticsResultTypeDef,
     GetTraceGraphResultTypeDef,
     GetTraceSummariesResultTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     SamplingStrategyTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "BatchGetTracesPaginator",
     "GetGroupsPaginator",
     "GetSamplingRulesPaginator",
     "GetSamplingStatisticSummariesPaginator",
@@ -140,16 +140,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getservicegraphpaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getservicegraphpaginator)
@@ -160,16 +160,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettimeseriesservicestatisticspaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
@@ -197,16 +197,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracesummariespaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTraceSummariesResultTypeDef]:
         """
```

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/type_defs.py` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_xray.type_defs import AliasTypeDef
 
-    data: AliasTypeDef = {...}
+    data: AliasTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -53,25 +53,21 @@
     "HistogramEntryTypeDef",
     "EncryptionConfigTypeDef",
     "RootCauseExceptionTypeDef",
     "ForecastStatisticsTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetGroupsRequestRequestTypeDef",
     "GetInsightEventsRequestRequestTypeDef",
-    "GetInsightImpactGraphRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetInsightRequestRequestTypeDef",
-    "GetInsightSummariesRequestRequestTypeDef",
     "GetSamplingRulesRequestRequestTypeDef",
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     "SamplingStatisticSummaryTypeDef",
-    "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
-    "GetServiceGraphRequestRequestTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
     "ListResourcePoliciesRequestRequestTypeDef",
@@ -86,21 +82,18 @@
     "SamplingRuleOutputTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
-    "TelemetryRecordTypeDef",
     "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     "GetGroupsRequestGetGroupsPaginateTypeDef",
     "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "GroupSummaryTypeDef",
     "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
@@ -109,39 +102,48 @@
     "CreateSamplingRuleRequestRequestTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
+    "GetInsightImpactGraphRequestRequestTypeDef",
+    "GetInsightSummariesRequestRequestTypeDef",
+    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    "GetServiceGraphRequestRequestTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    "SamplingStatisticsDocumentTypeDef",
+    "TelemetryRecordTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
-    "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
     "SamplingRuleRecordTypeDef",
+    "SamplingRuleUnionTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
-    "PutTelemetryRecordsRequestRequestTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
     "EdgeTypeDef",
     "TimeSeriesServiceStatisticsTypeDef",
     "ErrorRootCauseServiceTypeDef",
     "FaultRootCauseServiceTypeDef",
+    "GetSamplingTargetsRequestRequestTypeDef",
+    "PutTelemetryRecordsRequestRequestTypeDef",
     "GetInsightImpactGraphResultTypeDef",
     "ResponseTimeRootCauseTypeDef",
     "CreateSamplingRuleResultTypeDef",
     "DeleteSamplingRuleResultTypeDef",
     "GetSamplingRulesResultTypeDef",
     "UpdateSamplingRuleResultTypeDef",
     "BatchGetTracesResultTypeDef",
@@ -430,72 +432,22 @@
 
 class GetInsightEventsRequestRequestTypeDef(
     _RequiredGetInsightEventsRequestRequestTypeDef, _OptionalGetInsightEventsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
-    "_RequiredGetInsightImpactGraphRequestRequestTypeDef",
-    {
-        "InsightId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
-    "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
-    {
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetInsightImpactGraphRequestRequestTypeDef(
-    _RequiredGetInsightImpactGraphRequestRequestTypeDef,
-    _OptionalGetInsightImpactGraphRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 GetInsightRequestRequestTypeDef = TypedDict(
     "GetInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 
-_RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetInsightSummariesRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetInsightSummariesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetInsightSummariesRequestRequestTypeDef",
-    {
-        "States": Sequence[InsightStateType],
-        "GroupARN": str,
-        "GroupName": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetInsightSummariesRequestRequestTypeDef(
-    _RequiredGetInsightSummariesRequestRequestTypeDef,
-    _OptionalGetInsightSummariesRequestRequestTypeDef,
-):
-    pass
-
-
 GetSamplingRulesRequestRequestTypeDef = TypedDict(
     "GetSamplingRulesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -516,39 +468,14 @@
         "RequestCount": int,
         "BorrowCount": int,
         "SampledCount": int,
     },
     total=False,
 )
 
-_RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
-    "_RequiredSamplingStatisticsDocumentTypeDef",
-    {
-        "RuleName": str,
-        "ClientID": str,
-        "Timestamp": Union[datetime, str],
-        "RequestCount": int,
-        "SampledCount": int,
-    },
-)
-_OptionalSamplingStatisticsDocumentTypeDef = TypedDict(
-    "_OptionalSamplingStatisticsDocumentTypeDef",
-    {
-        "BorrowCount": int,
-    },
-    total=False,
-)
-
-
-class SamplingStatisticsDocumentTypeDef(
-    _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
-):
-    pass
-
-
 SamplingTargetDocumentTypeDef = TypedDict(
     "SamplingTargetDocumentTypeDef",
     {
         "RuleName": str,
         "FixedRate": float,
         "ReservoirQuota": int,
         "ReservoirQuotaTTL": datetime,
@@ -563,66 +490,14 @@
         "RuleName": str,
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestRequestTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestRequestTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetServiceGraphRequestRequestTypeDef(
-    _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestRequestTypeDef = TypedDict(
@@ -898,37 +773,14 @@
     {
         "AnnotationValue": AnnotationValueTypeDef,
         "ServiceIds": List[ServiceIdTypeDef],
     },
     total=False,
 )
 
-_RequiredTelemetryRecordTypeDef = TypedDict(
-    "_RequiredTelemetryRecordTypeDef",
-    {
-        "Timestamp": Union[datetime, str],
-    },
-)
-_OptionalTelemetryRecordTypeDef = TypedDict(
-    "_OptionalTelemetryRecordTypeDef",
-    {
-        "SegmentsReceivedCount": int,
-        "SegmentsSentCount": int,
-        "SegmentsSpilloverCount": int,
-        "SegmentsRejectedCount": int,
-        "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
-    },
-    total=False,
-)
-
-
-class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
-    pass
-
-
 _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
     "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
@@ -967,67 +819,14 @@
     "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
-    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
@@ -1227,27 +1026,224 @@
         "Name": str,
         "Exceptions": List[RootCauseExceptionTypeDef],
         "Remote": bool,
     },
     total=False,
 )
 
-GetSamplingStatisticSummariesResultTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesResultTypeDef",
+_RequiredGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
+    "_RequiredGetInsightImpactGraphRequestRequestTypeDef",
+    {
+        "InsightId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
+    "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
     {
-        "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-GetSamplingTargetsRequestRequestTypeDef = TypedDict(
-    "GetSamplingTargetsRequestRequestTypeDef",
+
+class GetInsightImpactGraphRequestRequestTypeDef(
+    _RequiredGetInsightImpactGraphRequestRequestTypeDef,
+    _OptionalGetInsightImpactGraphRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetInsightSummariesRequestRequestTypeDef",
     {
-        "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetInsightSummariesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetInsightSummariesRequestRequestTypeDef",
+    {
+        "States": Sequence[InsightStateType],
+        "GroupARN": str,
+        "GroupName": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class GetInsightSummariesRequestRequestTypeDef(
+    _RequiredGetInsightSummariesRequestRequestTypeDef,
+    _OptionalGetInsightSummariesRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
+    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetServiceGraphRequestRequestTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestRequestTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class GetServiceGraphRequestRequestTypeDef(
+    _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
+    "_RequiredSamplingStatisticsDocumentTypeDef",
+    {
+        "RuleName": str,
+        "ClientID": str,
+        "Timestamp": TimestampTypeDef,
+        "RequestCount": int,
+        "SampledCount": int,
+    },
+)
+_OptionalSamplingStatisticsDocumentTypeDef = TypedDict(
+    "_OptionalSamplingStatisticsDocumentTypeDef",
+    {
+        "BorrowCount": int,
+    },
+    total=False,
+)
+
+
+class SamplingStatisticsDocumentTypeDef(
+    _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
+):
+    pass
+
+
+_RequiredTelemetryRecordTypeDef = TypedDict(
+    "_RequiredTelemetryRecordTypeDef",
+    {
+        "Timestamp": TimestampTypeDef,
+    },
+)
+_OptionalTelemetryRecordTypeDef = TypedDict(
+    "_OptionalTelemetryRecordTypeDef",
+    {
+        "SegmentsReceivedCount": int,
+        "SegmentsSentCount": int,
+        "SegmentsSpilloverCount": int,
+        "SegmentsRejectedCount": int,
+        "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
+    },
+    total=False,
+)
+
+
+class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
+    pass
+
+
+GetSamplingStatisticSummariesResultTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesResultTypeDef",
+    {
+        "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSamplingTargetsResultTypeDef = TypedDict(
     "GetSamplingTargetsResultTypeDef",
     {
         "SamplingTargetDocuments": List[SamplingTargetDocumentTypeDef],
@@ -1256,16 +1252,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
@@ -1283,16 +1279,16 @@
 ):
     pass
 
 
 _RequiredGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestRequestTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestRequestTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
@@ -1367,14 +1363,15 @@
         "SamplingRule": SamplingRuleOutputTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
     },
     total=False,
 )
 
+SamplingRuleUnionTypeDef = Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef]
 UpdateSamplingRuleRequestRequestTypeDef = TypedDict(
     "UpdateSamplingRuleRequestRequestTypeDef",
     {
         "SamplingRuleUpdate": SamplingRuleUpdateTypeDef,
     },
 )
 
@@ -1436,38 +1433,14 @@
         "ClientRequestImpactStatistics": RequestImpactStatisticsTypeDef,
         "RootCauseServiceRequestImpactStatistics": RequestImpactStatisticsTypeDef,
         "TopAnomalousServices": List[AnomalousServiceTypeDef],
     },
     total=False,
 )
 
-_RequiredPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutTelemetryRecordsRequestRequestTypeDef",
-    {
-        "TelemetryRecords": Sequence[TelemetryRecordTypeDef],
-    },
-)
-_OptionalPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutTelemetryRecordsRequestRequestTypeDef",
-    {
-        "EC2InstanceId": str,
-        "Hostname": str,
-        "ResourceARN": str,
-    },
-    total=False,
-)
-
-
-class PutTelemetryRecordsRequestRequestTypeDef(
-    _RequiredPutTelemetryRecordsRequestRequestTypeDef,
-    _OptionalPutTelemetryRecordsRequestRequestTypeDef,
-):
-    pass
-
-
 GetGroupsResultTypeDef = TypedDict(
     "GetGroupsResultTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1546,14 +1519,45 @@
         "AccountId": str,
         "EntityPath": List[FaultRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+GetSamplingTargetsRequestRequestTypeDef = TypedDict(
+    "GetSamplingTargetsRequestRequestTypeDef",
+    {
+        "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
+    },
+)
+
+_RequiredPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutTelemetryRecordsRequestRequestTypeDef",
+    {
+        "TelemetryRecords": Sequence[TelemetryRecordTypeDef],
+    },
+)
+_OptionalPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutTelemetryRecordsRequestRequestTypeDef",
+    {
+        "EC2InstanceId": str,
+        "Hostname": str,
+        "ResourceARN": str,
+    },
+    total=False,
+)
+
+
+class PutTelemetryRecordsRequestRequestTypeDef(
+    _RequiredPutTelemetryRecordsRequestRequestTypeDef,
+    _OptionalPutTelemetryRecordsRequestRequestTypeDef,
+):
+    pass
+
+
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
```

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/type_defs.pyi` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_xray.type_defs import AliasTypeDef
 
-    data: AliasTypeDef = {...}
+    data: AliasTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,25 +52,21 @@
     "HistogramEntryTypeDef",
     "EncryptionConfigTypeDef",
     "RootCauseExceptionTypeDef",
     "ForecastStatisticsTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetGroupsRequestRequestTypeDef",
     "GetInsightEventsRequestRequestTypeDef",
-    "GetInsightImpactGraphRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetInsightRequestRequestTypeDef",
-    "GetInsightSummariesRequestRequestTypeDef",
     "GetSamplingRulesRequestRequestTypeDef",
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     "SamplingStatisticSummaryTypeDef",
-    "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
-    "GetServiceGraphRequestRequestTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
     "ListResourcePoliciesRequestRequestTypeDef",
@@ -85,21 +81,18 @@
     "SamplingRuleOutputTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
-    "TelemetryRecordTypeDef",
     "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     "GetGroupsRequestGetGroupsPaginateTypeDef",
     "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "GroupSummaryTypeDef",
     "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
@@ -108,39 +101,48 @@
     "CreateSamplingRuleRequestRequestTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
+    "GetInsightImpactGraphRequestRequestTypeDef",
+    "GetInsightSummariesRequestRequestTypeDef",
+    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    "GetServiceGraphRequestRequestTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    "SamplingStatisticsDocumentTypeDef",
+    "TelemetryRecordTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
-    "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
     "SamplingRuleRecordTypeDef",
+    "SamplingRuleUnionTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
-    "PutTelemetryRecordsRequestRequestTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
     "EdgeTypeDef",
     "TimeSeriesServiceStatisticsTypeDef",
     "ErrorRootCauseServiceTypeDef",
     "FaultRootCauseServiceTypeDef",
+    "GetSamplingTargetsRequestRequestTypeDef",
+    "PutTelemetryRecordsRequestRequestTypeDef",
     "GetInsightImpactGraphResultTypeDef",
     "ResponseTimeRootCauseTypeDef",
     "CreateSamplingRuleResultTypeDef",
     "DeleteSamplingRuleResultTypeDef",
     "GetSamplingRulesResultTypeDef",
     "UpdateSamplingRuleResultTypeDef",
     "BatchGetTracesResultTypeDef",
@@ -421,68 +423,22 @@
 )
 
 class GetInsightEventsRequestRequestTypeDef(
     _RequiredGetInsightEventsRequestRequestTypeDef, _OptionalGetInsightEventsRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
-    "_RequiredGetInsightImpactGraphRequestRequestTypeDef",
-    {
-        "InsightId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
-    "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
-    {
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetInsightImpactGraphRequestRequestTypeDef(
-    _RequiredGetInsightImpactGraphRequestRequestTypeDef,
-    _OptionalGetInsightImpactGraphRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 GetInsightRequestRequestTypeDef = TypedDict(
     "GetInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 
-_RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetInsightSummariesRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetInsightSummariesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetInsightSummariesRequestRequestTypeDef",
-    {
-        "States": Sequence[InsightStateType],
-        "GroupARN": str,
-        "GroupName": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetInsightSummariesRequestRequestTypeDef(
-    _RequiredGetInsightSummariesRequestRequestTypeDef,
-    _OptionalGetInsightSummariesRequestRequestTypeDef,
-):
-    pass
-
 GetSamplingRulesRequestRequestTypeDef = TypedDict(
     "GetSamplingRulesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -503,37 +459,14 @@
         "RequestCount": int,
         "BorrowCount": int,
         "SampledCount": int,
     },
     total=False,
 )
 
-_RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
-    "_RequiredSamplingStatisticsDocumentTypeDef",
-    {
-        "RuleName": str,
-        "ClientID": str,
-        "Timestamp": Union[datetime, str],
-        "RequestCount": int,
-        "SampledCount": int,
-    },
-)
-_OptionalSamplingStatisticsDocumentTypeDef = TypedDict(
-    "_OptionalSamplingStatisticsDocumentTypeDef",
-    {
-        "BorrowCount": int,
-    },
-    total=False,
-)
-
-class SamplingStatisticsDocumentTypeDef(
-    _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
-):
-    pass
-
 SamplingTargetDocumentTypeDef = TypedDict(
     "SamplingTargetDocumentTypeDef",
     {
         "RuleName": str,
         "FixedRate": float,
         "ReservoirQuota": int,
         "ReservoirQuotaTTL": datetime,
@@ -548,62 +481,14 @@
         "RuleName": str,
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestRequestTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestRequestTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetServiceGraphRequestRequestTypeDef(
-    _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
-):
-    pass
-
-_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-):
-    pass
-
 _RequiredGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestRequestTypeDef = TypedDict(
@@ -869,35 +754,14 @@
     {
         "AnnotationValue": AnnotationValueTypeDef,
         "ServiceIds": List[ServiceIdTypeDef],
     },
     total=False,
 )
 
-_RequiredTelemetryRecordTypeDef = TypedDict(
-    "_RequiredTelemetryRecordTypeDef",
-    {
-        "Timestamp": Union[datetime, str],
-    },
-)
-_OptionalTelemetryRecordTypeDef = TypedDict(
-    "_OptionalTelemetryRecordTypeDef",
-    {
-        "SegmentsReceivedCount": int,
-        "SegmentsSentCount": int,
-        "SegmentsSpilloverCount": int,
-        "SegmentsRejectedCount": int,
-        "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
-    },
-    total=False,
-)
-
-class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
-    pass
-
 _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
     "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
@@ -934,63 +798,14 @@
     "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
-    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-):
-    pass
-
-_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
@@ -1182,27 +997,208 @@
         "Name": str,
         "Exceptions": List[RootCauseExceptionTypeDef],
         "Remote": bool,
     },
     total=False,
 )
 
-GetSamplingStatisticSummariesResultTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesResultTypeDef",
+_RequiredGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
+    "_RequiredGetInsightImpactGraphRequestRequestTypeDef",
+    {
+        "InsightId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
+    "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
     {
-        "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-GetSamplingTargetsRequestRequestTypeDef = TypedDict(
-    "GetSamplingTargetsRequestRequestTypeDef",
+class GetInsightImpactGraphRequestRequestTypeDef(
+    _RequiredGetInsightImpactGraphRequestRequestTypeDef,
+    _OptionalGetInsightImpactGraphRequestRequestTypeDef,
+):
+    pass
+
+_RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetInsightSummariesRequestRequestTypeDef",
     {
-        "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetInsightSummariesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetInsightSummariesRequestRequestTypeDef",
+    {
+        "States": Sequence[InsightStateType],
+        "GroupARN": str,
+        "GroupName": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class GetInsightSummariesRequestRequestTypeDef(
+    _RequiredGetInsightSummariesRequestRequestTypeDef,
+    _OptionalGetInsightSummariesRequestRequestTypeDef,
+):
+    pass
+
+_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
+    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+):
+    pass
+
+_RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetServiceGraphRequestRequestTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestRequestTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class GetServiceGraphRequestRequestTypeDef(
+    _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
+):
+    pass
+
+_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
+    "_RequiredSamplingStatisticsDocumentTypeDef",
+    {
+        "RuleName": str,
+        "ClientID": str,
+        "Timestamp": TimestampTypeDef,
+        "RequestCount": int,
+        "SampledCount": int,
+    },
+)
+_OptionalSamplingStatisticsDocumentTypeDef = TypedDict(
+    "_OptionalSamplingStatisticsDocumentTypeDef",
+    {
+        "BorrowCount": int,
+    },
+    total=False,
+)
+
+class SamplingStatisticsDocumentTypeDef(
+    _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
+):
+    pass
+
+_RequiredTelemetryRecordTypeDef = TypedDict(
+    "_RequiredTelemetryRecordTypeDef",
+    {
+        "Timestamp": TimestampTypeDef,
+    },
+)
+_OptionalTelemetryRecordTypeDef = TypedDict(
+    "_OptionalTelemetryRecordTypeDef",
+    {
+        "SegmentsReceivedCount": int,
+        "SegmentsSentCount": int,
+        "SegmentsSpilloverCount": int,
+        "SegmentsRejectedCount": int,
+        "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
+    },
+    total=False,
+)
+
+class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
+    pass
+
+GetSamplingStatisticSummariesResultTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesResultTypeDef",
+    {
+        "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSamplingTargetsResultTypeDef = TypedDict(
     "GetSamplingTargetsResultTypeDef",
     {
         "SamplingTargetDocuments": List[SamplingTargetDocumentTypeDef],
@@ -1211,16 +1207,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
@@ -1236,16 +1232,16 @@
     _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
 ):
     pass
 
 _RequiredGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestRequestTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestRequestTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
@@ -1318,14 +1314,15 @@
         "SamplingRule": SamplingRuleOutputTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
     },
     total=False,
 )
 
+SamplingRuleUnionTypeDef = Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef]
 UpdateSamplingRuleRequestRequestTypeDef = TypedDict(
     "UpdateSamplingRuleRequestRequestTypeDef",
     {
         "SamplingRuleUpdate": SamplingRuleUpdateTypeDef,
     },
 )
 
@@ -1387,36 +1384,14 @@
         "ClientRequestImpactStatistics": RequestImpactStatisticsTypeDef,
         "RootCauseServiceRequestImpactStatistics": RequestImpactStatisticsTypeDef,
         "TopAnomalousServices": List[AnomalousServiceTypeDef],
     },
     total=False,
 )
 
-_RequiredPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutTelemetryRecordsRequestRequestTypeDef",
-    {
-        "TelemetryRecords": Sequence[TelemetryRecordTypeDef],
-    },
-)
-_OptionalPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutTelemetryRecordsRequestRequestTypeDef",
-    {
-        "EC2InstanceId": str,
-        "Hostname": str,
-        "ResourceARN": str,
-    },
-    total=False,
-)
-
-class PutTelemetryRecordsRequestRequestTypeDef(
-    _RequiredPutTelemetryRecordsRequestRequestTypeDef,
-    _OptionalPutTelemetryRecordsRequestRequestTypeDef,
-):
-    pass
-
 GetGroupsResultTypeDef = TypedDict(
     "GetGroupsResultTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1495,14 +1470,43 @@
         "AccountId": str,
         "EntityPath": List[FaultRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+GetSamplingTargetsRequestRequestTypeDef = TypedDict(
+    "GetSamplingTargetsRequestRequestTypeDef",
+    {
+        "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
+    },
+)
+
+_RequiredPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutTelemetryRecordsRequestRequestTypeDef",
+    {
+        "TelemetryRecords": Sequence[TelemetryRecordTypeDef],
+    },
+)
+_OptionalPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutTelemetryRecordsRequestRequestTypeDef",
+    {
+        "EC2InstanceId": str,
+        "Hostname": str,
+        "ResourceARN": str,
+    },
+    total=False,
+)
+
+class PutTelemetryRecordsRequestRequestTypeDef(
+    _RequiredPutTelemetryRecordsRequestRequestTypeDef,
+    _OptionalPutTelemetryRecordsRequestRequestTypeDef,
+):
+    pass
+
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
```

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/PKG-INFO` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.XRay 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 xray type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 xray type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-xray)](https://pepy.tech/project/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
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
@@ -354,20 +354,20 @@
 )
 
 
 def check_value(value: BatchGetTracesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_xray.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
@@ -386,25 +386,21 @@
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
-    GetInsightImpactGraphRequestRequestTypeDef,
+    TimestampTypeDef,
     GetInsightRequestRequestTypeDef,
-    GetInsightSummariesRequestRequestTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
-    SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
-    GetServiceGraphRequestRequestTypeDef,
-    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
@@ -419,21 +415,18 @@
     SamplingRuleOutputTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
-    TelemetryRecordTypeDef,
     BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
     GetGroupsRequestGetGroupsPaginateTypeDef,
     GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     GroupSummaryTypeDef,
     GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -442,39 +435,48 @@
     CreateSamplingRuleRequestRequestTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
+    GetInsightImpactGraphRequestRequestTypeDef,
+    GetInsightSummariesRequestRequestTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    GetServiceGraphRequestRequestTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    SamplingStatisticsDocumentTypeDef,
+    TelemetryRecordTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
-    GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
     SamplingRuleRecordTypeDef,
+    SamplingRuleUnionTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
-    PutTelemetryRecordsRequestRequestTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
     EdgeTypeDef,
     TimeSeriesServiceStatisticsTypeDef,
     ErrorRootCauseServiceTypeDef,
     FaultRootCauseServiceTypeDef,
+    GetSamplingTargetsRequestRequestTypeDef,
+    PutTelemetryRecordsRequestRequestTypeDef,
     GetInsightImpactGraphResultTypeDef,
     ResponseTimeRootCauseTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetSamplingRulesResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
     BatchGetTracesResultTypeDef,
@@ -488,15 +490,15 @@
     GetServiceGraphResultTypeDef,
     GetTraceGraphResultTypeDef,
     TraceSummaryTypeDef,
     GetTraceSummariesResultTypeDef,
 )
 
 
-def get_structure() -> AliasTypeDef:
+def get_value() -> AliasTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/SOURCES.txt` & `mypy-boto3-xray-1.28.16/mypy_boto3_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15.post1/setup.py` & `mypy-boto3-xray-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-xray",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_xray"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.XRay 1.28.16 service generated with mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -33,15 +33,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 xray type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 xray type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_xray": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

