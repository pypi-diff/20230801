# Comparing `tmp/mypy-boto3-codeguruprofiler-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-codeguruprofiler-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguruprofiler-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:48 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguruprofiler-1.28.16.tar", last modified: Tue Aug  1 11:36:28 2023, max compression
```

## Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1.tar` & `mypy-boto3-codeguruprofiler-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.001075 mypy-boto3-codeguruprofiler-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15627 2023-07-29 10:02:47.997075 mypy-boto3-codeguruprofiler-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:47.993075 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-07-29 09:40:49.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22987 2023-07-29 09:40:49.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:47.997075 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15627 2023-07-29 10:02:47.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:02:47.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:47.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:47.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:47.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:02:47.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:48.001075 mypy-boto3-codeguruprofiler-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:40:48.000000 mypy-boto3-codeguruprofiler-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.628924 mypy-boto3-codeguruprofiler-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:19.000000 mypy-boto3-codeguruprofiler-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-08-01 11:36:28.628924 mypy-boto3-codeguruprofiler-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-08-01 11:13:19.000000 mypy-boto3-codeguruprofiler-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.628924 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-01 11:13:19.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-01 11:13:19.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-01 11:13:19.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-08-01 11:13:20.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-08-01 11:13:20.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-01 11:13:20.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-08-01 11:13:20.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-01 11:13:20.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-01 11:13:20.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:19.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23233 2023-08-01 11:13:20.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23202 2023-08-01 11:13:20.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:19.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.628924 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-08-01 11:36:28.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:36:28.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:28.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:36:28.000000 mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:28.628924 mypy-boto3-codeguruprofiler-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 11:13:19.000000 mypy-boto3-codeguruprofiler-1.28.16/setup.py
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/LICENSE` & `mypy-boto3-codeguruprofiler-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/PKG-INFO` & `mypy-boto3-codeguruprofiler-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguruprofiler
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeGuruProfiler 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeGuruProfiler 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codeguruprofiler type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codeguruprofiler type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguruprofiler)](https://pepy.tech/project/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
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
@@ -319,92 +319,96 @@
 )
 
 
 def check_value(value: ActionGroupType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
-    ChannelOutputTypeDef,
-    ChannelTypeDef,
     ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
-    FrameMetricOutputTypeDef,
-    FrameMetricTypeDef,
+    TimestampTypeDef,
     TimestampStructureTypeDef,
+    BlobTypeDef,
+    ChannelOutputTypeDef,
+    ChannelTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
+    FrameMetricOutputTypeDef,
+    FrameMetricTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetProfileRequestRequestTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
-    ListFindingsReportsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListProfileTimesRequestRequestTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MatchTypeDef,
     PatternTypeDef,
-    PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
-    AddNotificationChannelsRequestRequestTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutPermissionResponseTypeDef,
     RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
-    FrameMetricDatumTypeDef,
-    BatchGetFrameMetricDataRequestRequestTypeDef,
+    GetProfileRequestRequestTypeDef,
+    GetRecommendationsRequestRequestTypeDef,
+    ListFindingsReportsRequestRequestTypeDef,
+    ListProfileTimesRequestRequestTypeDef,
+    PostAgentProfileRequestRequestTypeDef,
+    NotificationConfigurationTypeDef,
+    ChannelUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
+    FrameMetricDatumTypeDef,
+    FrameMetricUnionTypeDef,
     ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
+    ProfilingGroupDescriptionTypeDef,
+    AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
+    AddNotificationChannelsRequestRequestTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
+    BatchGetFrameMetricDataRequestRequestTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     UpdateProfilingGroupResponseTypeDef,
     GetRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> ChannelOutputTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/README.md` & `mypy-boto3-codeguruprofiler-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguruprofiler)](https://pepy.tech/project/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
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
@@ -287,92 +287,96 @@
 )
 
 
 def check_value(value: ActionGroupType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
-    ChannelOutputTypeDef,
-    ChannelTypeDef,
     ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
-    FrameMetricOutputTypeDef,
-    FrameMetricTypeDef,
+    TimestampTypeDef,
     TimestampStructureTypeDef,
+    BlobTypeDef,
+    ChannelOutputTypeDef,
+    ChannelTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
+    FrameMetricOutputTypeDef,
+    FrameMetricTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetProfileRequestRequestTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
-    ListFindingsReportsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListProfileTimesRequestRequestTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MatchTypeDef,
     PatternTypeDef,
-    PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
-    AddNotificationChannelsRequestRequestTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutPermissionResponseTypeDef,
     RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
-    FrameMetricDatumTypeDef,
-    BatchGetFrameMetricDataRequestRequestTypeDef,
+    GetProfileRequestRequestTypeDef,
+    GetRecommendationsRequestRequestTypeDef,
+    ListFindingsReportsRequestRequestTypeDef,
+    ListProfileTimesRequestRequestTypeDef,
+    PostAgentProfileRequestRequestTypeDef,
+    NotificationConfigurationTypeDef,
+    ChannelUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
+    FrameMetricDatumTypeDef,
+    FrameMetricUnionTypeDef,
     ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
+    ProfilingGroupDescriptionTypeDef,
+    AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
+    AddNotificationChannelsRequestRequestTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
+    BatchGetFrameMetricDataRequestRequestTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     UpdateProfilingGroupResponseTypeDef,
     GetRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> ChannelOutputTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/__init__.py` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/__init__.pyi` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/__main__.py` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruProfiler 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CodeGuruProfiler 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler\nOther"
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

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/client.py` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,81 +10,75 @@
     from mypy_boto3_codeguruprofiler.client import CodeGuruProfilerClient
 
     session = Session()
     client: CodeGuruProfilerClient = session.client("codeguruprofiler")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     AggregationPeriodType,
     ComputePlatformType,
     FeedbackTypeType,
     MetadataFieldType,
     OrderByType,
 )
 from .paginator import ListProfileTimesPaginator
 from .type_defs import (
     AddNotificationChannelsResponseTypeDef,
     AgentOrchestrationConfigTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
-    ChannelOutputTypeDef,
-    ChannelTypeDef,
+    BlobTypeDef,
+    ChannelUnionTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
-    FrameMetricOutputTypeDef,
-    FrameMetricTypeDef,
+    FrameMetricUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileResponseTypeDef,
     GetRecommendationsResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
     ListProfileTimesResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutPermissionResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
     RemovePermissionResponseTypeDef,
+    TimestampTypeDef,
     UpdateProfilingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeGuruProfilerClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class CodeGuruProfilerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/)
     """
 
     meta: ClientMeta
@@ -93,77 +87,68 @@
     def exceptions(self) -> Exceptions:
         """
         CodeGuruProfilerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#exceptions)
         """
-
     def add_notification_channels(
-        self,
-        *,
-        channels: Sequence[Union[ChannelTypeDef, ChannelOutputTypeDef]],
-        profilingGroupName: str
+        self, *, channels: Sequence[ChannelUnionTypeDef], profilingGroupName: str
     ) -> AddNotificationChannelsResponseTypeDef:
         """
         Add up to 2 anomaly notifications channels for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.add_notification_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#add_notification_channels)
         """
-
     def batch_get_frame_metric_data(
         self,
         *,
         profilingGroupName: str,
-        endTime: Union[datetime, str] = ...,
-        frameMetrics: Sequence[Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]] = ...,
+        endTime: TimestampTypeDef = ...,
+        frameMetrics: Sequence[FrameMetricUnionTypeDef] = ...,
         period: str = ...,
-        startTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
         targetResolution: AggregationPeriodType = ...
     ) -> BatchGetFrameMetricDataResponseTypeDef:
         """
         Returns the time series of values for a requested list of frame metrics from a
         time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.batch_get_frame_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#batch_get_frame_metric_data)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#close)
         """
-
     def configure_agent(
         self,
         *,
         profilingGroupName: str,
         fleetInstanceId: str = ...,
         metadata: Mapping[MetadataFieldType, str] = ...
     ) -> ConfigureAgentResponseTypeDef:
         """
         Used by profiler agents to report their current state and to receive remote
         configuration updates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.configure_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#configure_agent)
         """
-
     def create_profiling_group(
         self,
         *,
         clientToken: str,
         profilingGroupName: str,
         agentOrchestrationConfig: AgentOrchestrationConfigTypeDef = ...,
         computePlatform: ComputePlatformType = ...,
@@ -171,185 +156,171 @@
     ) -> CreateProfilingGroupResponseTypeDef:
         """
         Creates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.create_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#create_profiling_group)
         """
-
     def delete_profiling_group(self, *, profilingGroupName: str) -> Dict[str, Any]:
         """
         Deletes a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.delete_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#delete_profiling_group)
         """
-
     def describe_profiling_group(
         self, *, profilingGroupName: str
     ) -> DescribeProfilingGroupResponseTypeDef:
         """
         Returns a
         [ProfilingGroupDescription](https://docs.aws.amazon.com/codeguru/latest/profiler-
         api/API_ProfilingGroupDescription.html)_ object that contains information about
         the requested profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.describe_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#describe_profiling_group)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#generate_presigned_url)
         """
-
     def get_findings_report_account_summary(
         self, *, dailyReportsOnly: bool = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetFindingsReportAccountSummaryResponseTypeDef:
         """
         Returns a list of
         [FindingsReportSummary](https://docs.aws.amazon.com/codeguru/latest/profiler-
         api/API_FindingsReportSummary.html)_ objects that contain analysis results for
         all profiling groups in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_findings_report_account_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_findings_report_account_summary)
         """
-
     def get_notification_configuration(
         self, *, profilingGroupName: str
     ) -> GetNotificationConfigurationResponseTypeDef:
         """
         Get the current configuration for anomaly notifications for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_notification_configuration)
         """
-
     def get_policy(self, *, profilingGroupName: str) -> GetPolicyResponseTypeDef:
         """
         Returns the JSON-formatted resource-based policy on a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_policy)
         """
-
     def get_profile(
         self,
         *,
         profilingGroupName: str,
         accept: str = ...,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxDepth: int = ...,
         period: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> GetProfileResponseTypeDef:
         """
         Gets the aggregated profile of a profiling group for a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_profile)
         """
-
     def get_recommendations(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         locale: str = ...
     ) -> GetRecommendationsResponseTypeDef:
         """
         Returns a list of
         [Recommendation](https://docs.aws.amazon.com/codeguru/latest/profiler-
         api/API_Recommendation.html)_ objects that contain recommendations for a
         profiling group for a given time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_recommendations)
         """
-
     def list_findings_reports(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         dailyReportsOnly: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFindingsReportsResponseTypeDef:
         """
         List the available reports for a given profiling group and time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_findings_reports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_findings_reports)
         """
-
     def list_profile_times(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
         orderBy: OrderByType = ...
     ) -> ListProfileTimesResponseTypeDef:
         """
         Lists the start times of the available aggregated profiles of a profiling group
         for an aggregation period within the specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profile_times)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_profile_times)
         """
-
     def list_profiling_groups(
         self, *, includeDescription: bool = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListProfilingGroupsResponseTypeDef:
         """
         Returns a list of profiling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profiling_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_profiling_groups)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags that are assigned to a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_tags_for_resource)
         """
-
     def post_agent_profile(
         self,
         *,
-        agentProfile: Union[str, bytes, IO[Any], StreamingBody],
+        agentProfile: BlobTypeDef,
         contentType: str,
         profilingGroupName: str,
         profileToken: str = ...
     ) -> Dict[str, Any]:
         """
         Submits profiling data to an aggregated profile of a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.post_agent_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#post_agent_profile)
         """
-
     def put_permission(
         self,
         *,
         actionGroup: Literal["agentPermissions"],
         principals: Sequence[str],
         profilingGroupName: str,
         revisionId: str = ...
@@ -357,36 +328,33 @@
         """
         Adds permissions to a profiling group's resource-based policy that are provided
         using an action group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.put_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#put_permission)
         """
-
     def remove_notification_channel(
         self, *, channelId: str, profilingGroupName: str
     ) -> RemoveNotificationChannelResponseTypeDef:
         """
         Remove one anomaly notifications channel for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.remove_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#remove_notification_channel)
         """
-
     def remove_permission(
         self, *, actionGroup: Literal["agentPermissions"], profilingGroupName: str, revisionId: str
     ) -> RemovePermissionResponseTypeDef:
         """
         Removes permissions from a profiling group's resource-based policy that are
         provided using an action group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.remove_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#remove_permission)
         """
-
     def submit_feedback(
         self,
         *,
         anomalyInstanceId: str,
         profilingGroupName: str,
         type: FeedbackTypeType,
         comment: str = ...
@@ -394,41 +362,37 @@
         """
         Sends feedback to CodeGuru Profiler about whether the anomaly detected by the
         analysis is useful or not.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.submit_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#submit_feedback)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Use to assign one or more tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Use to remove one or more tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#untag_resource)
         """
-
     def update_profiling_group(
         self, *, agentOrchestrationConfig: AgentOrchestrationConfigTypeDef, profilingGroupName: str
     ) -> UpdateProfilingGroupResponseTypeDef:
         """
         Updates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.update_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#update_profiling_group)
         """
-
     def get_paginator(
         self, operation_name: Literal["list_profile_times"]
     ) -> ListProfileTimesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/client.pyi` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,77 +10,79 @@
     from mypy_boto3_codeguruprofiler.client import CodeGuruProfilerClient
 
     session = Session()
     client: CodeGuruProfilerClient = session.client("codeguruprofiler")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     AggregationPeriodType,
     ComputePlatformType,
     FeedbackTypeType,
     MetadataFieldType,
     OrderByType,
 )
 from .paginator import ListProfileTimesPaginator
 from .type_defs import (
     AddNotificationChannelsResponseTypeDef,
     AgentOrchestrationConfigTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
-    ChannelOutputTypeDef,
-    ChannelTypeDef,
+    BlobTypeDef,
+    ChannelUnionTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
-    FrameMetricOutputTypeDef,
-    FrameMetricTypeDef,
+    FrameMetricUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileResponseTypeDef,
     GetRecommendationsResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
     ListProfileTimesResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutPermissionResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
     RemovePermissionResponseTypeDef,
+    TimestampTypeDef,
     UpdateProfilingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("CodeGuruProfilerClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class CodeGuruProfilerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/)
     """
 
     meta: ClientMeta
@@ -89,71 +91,74 @@
     def exceptions(self) -> Exceptions:
         """
         CodeGuruProfilerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#exceptions)
         """
+
     def add_notification_channels(
-        self,
-        *,
-        channels: Sequence[Union[ChannelTypeDef, ChannelOutputTypeDef]],
-        profilingGroupName: str
+        self, *, channels: Sequence[ChannelUnionTypeDef], profilingGroupName: str
     ) -> AddNotificationChannelsResponseTypeDef:
         """
         Add up to 2 anomaly notifications channels for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.add_notification_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#add_notification_channels)
         """
+
     def batch_get_frame_metric_data(
         self,
         *,
         profilingGroupName: str,
-        endTime: Union[datetime, str] = ...,
-        frameMetrics: Sequence[Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]] = ...,
+        endTime: TimestampTypeDef = ...,
+        frameMetrics: Sequence[FrameMetricUnionTypeDef] = ...,
         period: str = ...,
-        startTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
         targetResolution: AggregationPeriodType = ...
     ) -> BatchGetFrameMetricDataResponseTypeDef:
         """
         Returns the time series of values for a requested list of frame metrics from a
         time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.batch_get_frame_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#batch_get_frame_metric_data)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#close)
         """
+
     def configure_agent(
         self,
         *,
         profilingGroupName: str,
         fleetInstanceId: str = ...,
         metadata: Mapping[MetadataFieldType, str] = ...
     ) -> ConfigureAgentResponseTypeDef:
         """
         Used by profiler agents to report their current state and to receive remote
         configuration updates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.configure_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#configure_agent)
         """
+
     def create_profiling_group(
         self,
         *,
         clientToken: str,
         profilingGroupName: str,
         agentOrchestrationConfig: AgentOrchestrationConfigTypeDef = ...,
         computePlatform: ComputePlatformType = ...,
@@ -161,171 +166,185 @@
     ) -> CreateProfilingGroupResponseTypeDef:
         """
         Creates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.create_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#create_profiling_group)
         """
+
     def delete_profiling_group(self, *, profilingGroupName: str) -> Dict[str, Any]:
         """
         Deletes a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.delete_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#delete_profiling_group)
         """
+
     def describe_profiling_group(
         self, *, profilingGroupName: str
     ) -> DescribeProfilingGroupResponseTypeDef:
         """
         Returns a
         [ProfilingGroupDescription](https://docs.aws.amazon.com/codeguru/latest/profiler-
         api/API_ProfilingGroupDescription.html)_ object that contains information about
         the requested profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.describe_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#describe_profiling_group)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#generate_presigned_url)
         """
+
     def get_findings_report_account_summary(
         self, *, dailyReportsOnly: bool = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetFindingsReportAccountSummaryResponseTypeDef:
         """
         Returns a list of
         [FindingsReportSummary](https://docs.aws.amazon.com/codeguru/latest/profiler-
         api/API_FindingsReportSummary.html)_ objects that contain analysis results for
         all profiling groups in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_findings_report_account_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_findings_report_account_summary)
         """
+
     def get_notification_configuration(
         self, *, profilingGroupName: str
     ) -> GetNotificationConfigurationResponseTypeDef:
         """
         Get the current configuration for anomaly notifications for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_notification_configuration)
         """
+
     def get_policy(self, *, profilingGroupName: str) -> GetPolicyResponseTypeDef:
         """
         Returns the JSON-formatted resource-based policy on a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_policy)
         """
+
     def get_profile(
         self,
         *,
         profilingGroupName: str,
         accept: str = ...,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxDepth: int = ...,
         period: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> GetProfileResponseTypeDef:
         """
         Gets the aggregated profile of a profiling group for a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_profile)
         """
+
     def get_recommendations(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         locale: str = ...
     ) -> GetRecommendationsResponseTypeDef:
         """
         Returns a list of
         [Recommendation](https://docs.aws.amazon.com/codeguru/latest/profiler-
         api/API_Recommendation.html)_ objects that contain recommendations for a
         profiling group for a given time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_recommendations)
         """
+
     def list_findings_reports(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         dailyReportsOnly: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFindingsReportsResponseTypeDef:
         """
         List the available reports for a given profiling group and time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_findings_reports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_findings_reports)
         """
+
     def list_profile_times(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
         orderBy: OrderByType = ...
     ) -> ListProfileTimesResponseTypeDef:
         """
         Lists the start times of the available aggregated profiles of a profiling group
         for an aggregation period within the specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profile_times)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_profile_times)
         """
+
     def list_profiling_groups(
         self, *, includeDescription: bool = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListProfilingGroupsResponseTypeDef:
         """
         Returns a list of profiling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profiling_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_profiling_groups)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags that are assigned to a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_tags_for_resource)
         """
+
     def post_agent_profile(
         self,
         *,
-        agentProfile: Union[str, bytes, IO[Any], StreamingBody],
+        agentProfile: BlobTypeDef,
         contentType: str,
         profilingGroupName: str,
         profileToken: str = ...
     ) -> Dict[str, Any]:
         """
         Submits profiling data to an aggregated profile of a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.post_agent_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#post_agent_profile)
         """
+
     def put_permission(
         self,
         *,
         actionGroup: Literal["agentPermissions"],
         principals: Sequence[str],
         profilingGroupName: str,
         revisionId: str = ...
@@ -333,33 +352,36 @@
         """
         Adds permissions to a profiling group's resource-based policy that are provided
         using an action group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.put_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#put_permission)
         """
+
     def remove_notification_channel(
         self, *, channelId: str, profilingGroupName: str
     ) -> RemoveNotificationChannelResponseTypeDef:
         """
         Remove one anomaly notifications channel for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.remove_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#remove_notification_channel)
         """
+
     def remove_permission(
         self, *, actionGroup: Literal["agentPermissions"], profilingGroupName: str, revisionId: str
     ) -> RemovePermissionResponseTypeDef:
         """
         Removes permissions from a profiling group's resource-based policy that are
         provided using an action group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.remove_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#remove_permission)
         """
+
     def submit_feedback(
         self,
         *,
         anomalyInstanceId: str,
         profilingGroupName: str,
         type: FeedbackTypeType,
         comment: str = ...
@@ -367,37 +389,41 @@
         """
         Sends feedback to CodeGuru Profiler about whether the anomaly detected by the
         analysis is useful or not.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.submit_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#submit_feedback)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Use to assign one or more tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Use to remove one or more tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#untag_resource)
         """
+
     def update_profiling_group(
         self, *, agentOrchestrationConfig: AgentOrchestrationConfigTypeDef, profilingGroupName: str
     ) -> UpdateProfilingGroupResponseTypeDef:
         """
         Updates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.update_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#update_profiling_group)
         """
+
     def get_paginator(
         self, operation_name: Literal["list_profile_times"]
     ) -> ListProfileTimesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/literals.py` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/literals.pyi` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/paginator.py` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 
     session = Session()
     client: CodeGuruProfilerClient = session.client("codeguruprofiler")
 
     list_profile_times_paginator: ListProfileTimesPaginator = client.get_paginator("list_profile_times")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationPeriodType, OrderByType
-from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListProfileTimesPaginator",)
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
@@ -45,18 +44,18 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         orderBy: OrderByType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/paginator.pyi` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/paginator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 
     session = Session()
     client: CodeGuruProfilerClient = session.client("codeguruprofiler")
 
     list_profile_times_paginator: ListProfileTimesPaginator = client.get_paginator("list_profile_times")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationPeriodType, OrderByType
-from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListProfileTimesPaginator",)
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
@@ -42,18 +41,18 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         orderBy: OrderByType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/type_defs.py` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for codeguruprofiler service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_codeguruprofiler.type_defs import ChannelOutputTypeDef
+    from mypy_boto3_codeguruprofiler.type_defs import ResponseMetadataTypeDef
 
-    data: ChannelOutputTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -33,121 +33,85 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ChannelOutputTypeDef",
-    "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
-    "FrameMetricOutputTypeDef",
-    "FrameMetricTypeDef",
+    "TimestampTypeDef",
     "TimestampStructureTypeDef",
+    "BlobTypeDef",
+    "ChannelOutputTypeDef",
+    "ChannelTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
+    "FrameMetricOutputTypeDef",
+    "FrameMetricTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetProfileRequestRequestTypeDef",
-    "GetRecommendationsRequestRequestTypeDef",
-    "ListFindingsReportsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ListProfileTimesRequestRequestTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MatchTypeDef",
     "PatternTypeDef",
-    "PostAgentProfileRequestRequestTypeDef",
     "PutPermissionRequestRequestTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "NotificationConfigurationTypeDef",
-    "AddNotificationChannelsRequestRequestTypeDef",
     "GetPolicyResponseTypeDef",
     "GetProfileResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutPermissionResponseTypeDef",
     "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
-    "FrameMetricDatumTypeDef",
-    "BatchGetFrameMetricDataRequestRequestTypeDef",
+    "GetProfileRequestRequestTypeDef",
+    "GetRecommendationsRequestRequestTypeDef",
+    "ListFindingsReportsRequestRequestTypeDef",
+    "ListProfileTimesRequestRequestTypeDef",
+    "PostAgentProfileRequestRequestTypeDef",
+    "NotificationConfigurationTypeDef",
+    "ChannelUnionTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
+    "FrameMetricDatumTypeDef",
+    "FrameMetricUnionTypeDef",
     "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
+    "ProfilingGroupDescriptionTypeDef",
+    "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
-    "ProfilingGroupDescriptionTypeDef",
-    "AnomalyTypeDef",
+    "AddNotificationChannelsRequestRequestTypeDef",
     "BatchGetFrameMetricDataResponseTypeDef",
+    "BatchGetFrameMetricDataRequestRequestTypeDef",
     "CreateProfilingGroupResponseTypeDef",
     "DescribeProfilingGroupResponseTypeDef",
     "ListProfilingGroupsResponseTypeDef",
     "UpdateProfilingGroupResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
 )
 
-_RequiredChannelOutputTypeDef = TypedDict(
-    "_RequiredChannelOutputTypeDef",
-    {
-        "eventPublishers": List[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelOutputTypeDef = TypedDict(
-    "_OptionalChannelOutputTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-
-class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
-    pass
-
-
-_RequiredChannelTypeDef = TypedDict(
-    "_RequiredChannelTypeDef",
-    {
-        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelTypeDef = TypedDict(
-    "_OptionalChannelTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-
-class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
-    pass
-
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -205,39 +169,63 @@
     {
         "frameName": str,
         "threadStates": List[str],
         "type": Literal["AggregatedRelativeTotalTime"],
     },
 )
 
-FrameMetricOutputTypeDef = TypedDict(
-    "FrameMetricOutputTypeDef",
+TimestampTypeDef = Union[datetime, str]
+TimestampStructureTypeDef = TypedDict(
+    "TimestampStructureTypeDef",
     {
-        "frameName": str,
-        "threadStates": List[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
+        "value": datetime,
     },
 )
 
-FrameMetricTypeDef = TypedDict(
-    "FrameMetricTypeDef",
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredChannelOutputTypeDef = TypedDict(
+    "_RequiredChannelOutputTypeDef",
     {
-        "frameName": str,
-        "threadStates": Sequence[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
+        "eventPublishers": List[Literal["AnomalyDetection"]],
+        "uri": str,
     },
 )
+_OptionalChannelOutputTypeDef = TypedDict(
+    "_OptionalChannelOutputTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
 
-TimestampStructureTypeDef = TypedDict(
-    "TimestampStructureTypeDef",
+
+class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
+    pass
+
+
+_RequiredChannelTypeDef = TypedDict(
+    "_RequiredChannelTypeDef",
     {
-        "value": datetime,
+        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
+        "uri": str,
+    },
+)
+_OptionalChannelTypeDef = TypedDict(
+    "_OptionalChannelTypeDef",
+    {
+        "id": str,
     },
+    total=False,
 )
 
+
+class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
+    pass
+
+
 _RequiredConfigureAgentRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAgentRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalConfigureAgentRequestRequestTypeDef = TypedDict(
@@ -278,14 +266,32 @@
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "totalNumberOfFindings": int,
     },
     total=False,
 )
 
+FrameMetricOutputTypeDef = TypedDict(
+    "FrameMetricOutputTypeDef",
+    {
+        "frameName": str,
+        "threadStates": List[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
+    },
+)
+
+FrameMetricTypeDef = TypedDict(
+    "FrameMetricTypeDef",
+    {
+        "frameName": str,
+        "threadStates": Sequence[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
+    },
+)
+
 GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     {
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
@@ -302,125 +308,24 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
-_RequiredGetProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProfileRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-_OptionalGetProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProfileRequestRequestTypeDef",
-    {
-        "accept": str,
-        "endTime": Union[datetime, str],
-        "maxDepth": int,
-        "period": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GetProfileRequestRequestTypeDef(
-    _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRecommendationsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalGetRecommendationsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRecommendationsRequestRequestTypeDef",
-    {
-        "locale": str,
-    },
-    total=False,
-)
-
-
-class GetRecommendationsRequestRequestTypeDef(
-    _RequiredGetRecommendationsRequestRequestTypeDef,
-    _OptionalGetRecommendationsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsReportsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListFindingsReportsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsReportsRequestRequestTypeDef",
-    {
-        "dailyReportsOnly": bool,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListFindingsReportsRequestRequestTypeDef(
-    _RequiredListFindingsReportsRequestRequestTypeDef,
-    _OptionalListFindingsReportsRequestRequestTypeDef,
-):
-    pass
-
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListProfileTimesRequestRequestTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "orderBy": OrderByType,
-    },
-    total=False,
-)
-
-
-class ListProfileTimesRequestRequestTypeDef(
-    _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
-):
-    pass
-
-
 ProfileTimeTypeDef = TypedDict(
     "ProfileTimeTypeDef",
     {
         "start": datetime,
     },
     total=False,
 )
@@ -462,37 +367,14 @@
         "resolutionSteps": str,
         "targetFrames": List[List[str]],
         "thresholdPercent": float,
     },
     total=False,
 )
 
-_RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredPostAgentProfileRequestRequestTypeDef",
-    {
-        "agentProfile": Union[str, bytes, IO[Any], StreamingBody],
-        "contentType": str,
-        "profilingGroupName": str,
-    },
-)
-_OptionalPostAgentProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalPostAgentProfileRequestRequestTypeDef",
-    {
-        "profileToken": str,
-    },
-    total=False,
-)
-
-
-class PostAgentProfileRequestRequestTypeDef(
-    _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredPutPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredPutPermissionRequestRequestTypeDef",
     {
         "actionGroup": Literal["agentPermissions"],
         "principals": Sequence[str],
         "profilingGroupName": str,
     },
@@ -564,30 +446,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
-    {
-        "channels": List[ChannelOutputTypeDef],
-    },
-    total=False,
-)
-
-AddNotificationChannelsRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelsRequestRequestTypeDef",
-    {
-        "channels": Sequence[Union[ChannelTypeDef, ChannelOutputTypeDef]],
-        "profilingGroupName": str,
-    },
-)
-
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "policy": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -697,48 +563,147 @@
 )
 
 
 class AnomalyInstanceTypeDef(_RequiredAnomalyInstanceTypeDef, _OptionalAnomalyInstanceTypeDef):
     pass
 
 
-FrameMetricDatumTypeDef = TypedDict(
-    "FrameMetricDatumTypeDef",
+_RequiredGetProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProfileRequestRequestTypeDef",
     {
-        "frameMetric": FrameMetricOutputTypeDef,
-        "values": List[float],
+        "profilingGroupName": str,
     },
 )
+_OptionalGetProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProfileRequestRequestTypeDef",
+    {
+        "accept": str,
+        "endTime": TimestampTypeDef,
+        "maxDepth": int,
+        "period": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
 
-_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+
+class GetProfileRequestRequestTypeDef(
+    _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
+        "endTime": TimestampTypeDef,
         "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
     },
 )
-_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+_OptionalGetRecommendationsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRecommendationsRequestRequestTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "frameMetrics": Sequence[Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]],
-        "period": str,
-        "startTime": Union[datetime, str],
-        "targetResolution": AggregationPeriodType,
+        "locale": str,
     },
     total=False,
 )
 
 
-class BatchGetFrameMetricDataRequestRequestTypeDef(
-    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
-    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+class GetRecommendationsRequestRequestTypeDef(
+    _RequiredGetRecommendationsRequestRequestTypeDef,
+    _OptionalGetRecommendationsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsReportsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListFindingsReportsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsReportsRequestRequestTypeDef",
+    {
+        "dailyReportsOnly": bool,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListFindingsReportsRequestRequestTypeDef(
+    _RequiredListFindingsReportsRequestRequestTypeDef,
+    _OptionalListFindingsReportsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListProfileTimesRequestRequestTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "orderBy": OrderByType,
+    },
+    total=False,
+)
+
+
+class ListProfileTimesRequestRequestTypeDef(
+    _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredPostAgentProfileRequestRequestTypeDef",
+    {
+        "agentProfile": BlobTypeDef,
+        "contentType": str,
+        "profilingGroupName": str,
+    },
+)
+_OptionalPostAgentProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalPostAgentProfileRequestRequestTypeDef",
+    {
+        "profileToken": str,
+    },
+    total=False,
+)
+
+
+class PostAgentProfileRequestRequestTypeDef(
+    _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
+):
+    pass
+
+
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
+    {
+        "channels": List[ChannelOutputTypeDef],
+    },
+    total=False,
+)
+
+ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelOutputTypeDef]
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -749,21 +714,30 @@
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FrameMetricDatumTypeDef = TypedDict(
+    "FrameMetricDatumTypeDef",
+    {
+        "frameMetric": FrameMetricOutputTypeDef,
+        "values": List[float],
+    },
+)
+
+FrameMetricUnionTypeDef = Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]
 _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
         "period": AggregationPeriodType,
         "profilingGroupName": str,
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
     "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
     {
         "orderBy": OrderByType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -796,14 +770,38 @@
         "endTime": datetime,
         "pattern": PatternTypeDef,
         "startTime": datetime,
         "topMatches": List[MatchTypeDef],
     },
 )
 
+ProfilingGroupDescriptionTypeDef = TypedDict(
+    "ProfilingGroupDescriptionTypeDef",
+    {
+        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
+        "arn": str,
+        "computePlatform": ComputePlatformType,
+        "createdAt": datetime,
+        "name": str,
+        "profilingStatus": ProfilingStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "instances": List[AnomalyInstanceTypeDef],
+        "metric": MetricTypeDef,
+        "reason": str,
+    },
+)
+
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -820,35 +818,19 @@
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProfilingGroupDescriptionTypeDef = TypedDict(
-    "ProfilingGroupDescriptionTypeDef",
-    {
-        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
-        "arn": str,
-        "computePlatform": ComputePlatformType,
-        "createdAt": datetime,
-        "name": str,
-        "profilingStatus": ProfilingStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
+AddNotificationChannelsRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelsRequestRequestTypeDef",
     {
-        "instances": List[AnomalyInstanceTypeDef],
-        "metric": MetricTypeDef,
-        "reason": str,
+        "channels": Sequence[ChannelUnionTypeDef],
+        "profilingGroupName": str,
     },
 )
 
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
@@ -857,14 +839,40 @@
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "profilingGroupName": str,
+    },
+)
+_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "frameMetrics": Sequence[FrameMetricUnionTypeDef],
+        "period": str,
+        "startTime": TimestampTypeDef,
+        "targetResolution": AggregationPeriodType,
+    },
+    total=False,
+)
+
+
+class BatchGetFrameMetricDataRequestRequestTypeDef(
+    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
+    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+):
+    pass
+
+
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler/type_defs.pyi` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for codeguruprofiler service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_codeguruprofiler.type_defs import ChannelOutputTypeDef
+    from mypy_boto3_codeguruprofiler.type_defs import ResponseMetadataTypeDef
 
-    data: ChannelOutputTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -32,117 +32,85 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ChannelOutputTypeDef",
-    "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
-    "FrameMetricOutputTypeDef",
-    "FrameMetricTypeDef",
+    "TimestampTypeDef",
     "TimestampStructureTypeDef",
+    "BlobTypeDef",
+    "ChannelOutputTypeDef",
+    "ChannelTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
+    "FrameMetricOutputTypeDef",
+    "FrameMetricTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetProfileRequestRequestTypeDef",
-    "GetRecommendationsRequestRequestTypeDef",
-    "ListFindingsReportsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ListProfileTimesRequestRequestTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MatchTypeDef",
     "PatternTypeDef",
-    "PostAgentProfileRequestRequestTypeDef",
     "PutPermissionRequestRequestTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "NotificationConfigurationTypeDef",
-    "AddNotificationChannelsRequestRequestTypeDef",
     "GetPolicyResponseTypeDef",
     "GetProfileResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutPermissionResponseTypeDef",
     "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
-    "FrameMetricDatumTypeDef",
-    "BatchGetFrameMetricDataRequestRequestTypeDef",
+    "GetProfileRequestRequestTypeDef",
+    "GetRecommendationsRequestRequestTypeDef",
+    "ListFindingsReportsRequestRequestTypeDef",
+    "ListProfileTimesRequestRequestTypeDef",
+    "PostAgentProfileRequestRequestTypeDef",
+    "NotificationConfigurationTypeDef",
+    "ChannelUnionTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
+    "FrameMetricDatumTypeDef",
+    "FrameMetricUnionTypeDef",
     "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
+    "ProfilingGroupDescriptionTypeDef",
+    "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
-    "ProfilingGroupDescriptionTypeDef",
-    "AnomalyTypeDef",
+    "AddNotificationChannelsRequestRequestTypeDef",
     "BatchGetFrameMetricDataResponseTypeDef",
+    "BatchGetFrameMetricDataRequestRequestTypeDef",
     "CreateProfilingGroupResponseTypeDef",
     "DescribeProfilingGroupResponseTypeDef",
     "ListProfilingGroupsResponseTypeDef",
     "UpdateProfilingGroupResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
 )
 
-_RequiredChannelOutputTypeDef = TypedDict(
-    "_RequiredChannelOutputTypeDef",
-    {
-        "eventPublishers": List[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelOutputTypeDef = TypedDict(
-    "_OptionalChannelOutputTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
-    pass
-
-_RequiredChannelTypeDef = TypedDict(
-    "_RequiredChannelTypeDef",
-    {
-        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelTypeDef = TypedDict(
-    "_OptionalChannelTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
-    pass
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -198,38 +166,58 @@
     {
         "frameName": str,
         "threadStates": List[str],
         "type": Literal["AggregatedRelativeTotalTime"],
     },
 )
 
-FrameMetricOutputTypeDef = TypedDict(
-    "FrameMetricOutputTypeDef",
+TimestampTypeDef = Union[datetime, str]
+TimestampStructureTypeDef = TypedDict(
+    "TimestampStructureTypeDef",
     {
-        "frameName": str,
-        "threadStates": List[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
+        "value": datetime,
     },
 )
 
-FrameMetricTypeDef = TypedDict(
-    "FrameMetricTypeDef",
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredChannelOutputTypeDef = TypedDict(
+    "_RequiredChannelOutputTypeDef",
     {
-        "frameName": str,
-        "threadStates": Sequence[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
+        "eventPublishers": List[Literal["AnomalyDetection"]],
+        "uri": str,
+    },
+)
+_OptionalChannelOutputTypeDef = TypedDict(
+    "_OptionalChannelOutputTypeDef",
+    {
+        "id": str,
     },
+    total=False,
 )
 
-TimestampStructureTypeDef = TypedDict(
-    "TimestampStructureTypeDef",
+class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
+    pass
+
+_RequiredChannelTypeDef = TypedDict(
+    "_RequiredChannelTypeDef",
     {
-        "value": datetime,
+        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
+        "uri": str,
     },
 )
+_OptionalChannelTypeDef = TypedDict(
+    "_OptionalChannelTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
+    pass
 
 _RequiredConfigureAgentRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAgentRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
@@ -269,14 +257,32 @@
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "totalNumberOfFindings": int,
     },
     total=False,
 )
 
+FrameMetricOutputTypeDef = TypedDict(
+    "FrameMetricOutputTypeDef",
+    {
+        "frameName": str,
+        "threadStates": List[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
+    },
+)
+
+FrameMetricTypeDef = TypedDict(
+    "FrameMetricTypeDef",
+    {
+        "frameName": str,
+        "threadStates": Sequence[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
+    },
+)
+
 GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     {
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
@@ -293,117 +299,24 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
-_RequiredGetProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProfileRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-_OptionalGetProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProfileRequestRequestTypeDef",
-    {
-        "accept": str,
-        "endTime": Union[datetime, str],
-        "maxDepth": int,
-        "period": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GetProfileRequestRequestTypeDef(
-    _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
-):
-    pass
-
-_RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRecommendationsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalGetRecommendationsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRecommendationsRequestRequestTypeDef",
-    {
-        "locale": str,
-    },
-    total=False,
-)
-
-class GetRecommendationsRequestRequestTypeDef(
-    _RequiredGetRecommendationsRequestRequestTypeDef,
-    _OptionalGetRecommendationsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsReportsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListFindingsReportsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsReportsRequestRequestTypeDef",
-    {
-        "dailyReportsOnly": bool,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListFindingsReportsRequestRequestTypeDef(
-    _RequiredListFindingsReportsRequestRequestTypeDef,
-    _OptionalListFindingsReportsRequestRequestTypeDef,
-):
-    pass
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListProfileTimesRequestRequestTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "orderBy": OrderByType,
-    },
-    total=False,
-)
-
-class ListProfileTimesRequestRequestTypeDef(
-    _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
-):
-    pass
-
 ProfileTimeTypeDef = TypedDict(
     "ProfileTimeTypeDef",
     {
         "start": datetime,
     },
     total=False,
 )
@@ -445,35 +358,14 @@
         "resolutionSteps": str,
         "targetFrames": List[List[str]],
         "thresholdPercent": float,
     },
     total=False,
 )
 
-_RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredPostAgentProfileRequestRequestTypeDef",
-    {
-        "agentProfile": Union[str, bytes, IO[Any], StreamingBody],
-        "contentType": str,
-        "profilingGroupName": str,
-    },
-)
-_OptionalPostAgentProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalPostAgentProfileRequestRequestTypeDef",
-    {
-        "profileToken": str,
-    },
-    total=False,
-)
-
-class PostAgentProfileRequestRequestTypeDef(
-    _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
-):
-    pass
-
 _RequiredPutPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredPutPermissionRequestRequestTypeDef",
     {
         "actionGroup": Literal["agentPermissions"],
         "principals": Sequence[str],
         "profilingGroupName": str,
     },
@@ -541,30 +433,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
-    {
-        "channels": List[ChannelOutputTypeDef],
-    },
-    total=False,
-)
-
-AddNotificationChannelsRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelsRequestRequestTypeDef",
-    {
-        "channels": Sequence[Union[ChannelTypeDef, ChannelOutputTypeDef]],
-        "profilingGroupName": str,
-    },
-)
-
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "policy": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -670,46 +546,137 @@
     },
     total=False,
 )
 
 class AnomalyInstanceTypeDef(_RequiredAnomalyInstanceTypeDef, _OptionalAnomalyInstanceTypeDef):
     pass
 
-FrameMetricDatumTypeDef = TypedDict(
-    "FrameMetricDatumTypeDef",
+_RequiredGetProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProfileRequestRequestTypeDef",
     {
-        "frameMetric": FrameMetricOutputTypeDef,
-        "values": List[float],
+        "profilingGroupName": str,
     },
 )
+_OptionalGetProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProfileRequestRequestTypeDef",
+    {
+        "accept": str,
+        "endTime": TimestampTypeDef,
+        "maxDepth": int,
+        "period": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
 
-_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+class GetProfileRequestRequestTypeDef(
+    _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
+):
+    pass
+
+_RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
+        "endTime": TimestampTypeDef,
         "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
     },
 )
-_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+_OptionalGetRecommendationsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRecommendationsRequestRequestTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "frameMetrics": Sequence[Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]],
-        "period": str,
-        "startTime": Union[datetime, str],
-        "targetResolution": AggregationPeriodType,
+        "locale": str,
     },
     total=False,
 )
 
-class BatchGetFrameMetricDataRequestRequestTypeDef(
-    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
-    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+class GetRecommendationsRequestRequestTypeDef(
+    _RequiredGetRecommendationsRequestRequestTypeDef,
+    _OptionalGetRecommendationsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsReportsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListFindingsReportsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsReportsRequestRequestTypeDef",
+    {
+        "dailyReportsOnly": bool,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListFindingsReportsRequestRequestTypeDef(
+    _RequiredListFindingsReportsRequestRequestTypeDef,
+    _OptionalListFindingsReportsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListProfileTimesRequestRequestTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "orderBy": OrderByType,
+    },
+    total=False,
+)
+
+class ListProfileTimesRequestRequestTypeDef(
+    _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
+):
+    pass
+
+_RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredPostAgentProfileRequestRequestTypeDef",
+    {
+        "agentProfile": BlobTypeDef,
+        "contentType": str,
+        "profilingGroupName": str,
+    },
+)
+_OptionalPostAgentProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalPostAgentProfileRequestRequestTypeDef",
+    {
+        "profileToken": str,
+    },
+    total=False,
+)
+
+class PostAgentProfileRequestRequestTypeDef(
+    _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
+):
+    pass
+
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
+    {
+        "channels": List[ChannelOutputTypeDef],
+    },
+    total=False,
+)
+
+ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelOutputTypeDef]
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -720,21 +687,30 @@
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FrameMetricDatumTypeDef = TypedDict(
+    "FrameMetricDatumTypeDef",
+    {
+        "frameMetric": FrameMetricOutputTypeDef,
+        "values": List[float],
+    },
+)
+
+FrameMetricUnionTypeDef = Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]
 _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
         "period": AggregationPeriodType,
         "profilingGroupName": str,
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
     "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
     {
         "orderBy": OrderByType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -765,14 +741,38 @@
         "endTime": datetime,
         "pattern": PatternTypeDef,
         "startTime": datetime,
         "topMatches": List[MatchTypeDef],
     },
 )
 
+ProfilingGroupDescriptionTypeDef = TypedDict(
+    "ProfilingGroupDescriptionTypeDef",
+    {
+        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
+        "arn": str,
+        "computePlatform": ComputePlatformType,
+        "createdAt": datetime,
+        "name": str,
+        "profilingStatus": ProfilingStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "instances": List[AnomalyInstanceTypeDef],
+        "metric": MetricTypeDef,
+        "reason": str,
+    },
+)
+
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -789,35 +789,19 @@
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProfilingGroupDescriptionTypeDef = TypedDict(
-    "ProfilingGroupDescriptionTypeDef",
-    {
-        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
-        "arn": str,
-        "computePlatform": ComputePlatformType,
-        "createdAt": datetime,
-        "name": str,
-        "profilingStatus": ProfilingStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
+AddNotificationChannelsRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelsRequestRequestTypeDef",
     {
-        "instances": List[AnomalyInstanceTypeDef],
-        "metric": MetricTypeDef,
-        "reason": str,
+        "channels": Sequence[ChannelUnionTypeDef],
+        "profilingGroupName": str,
     },
 )
 
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
@@ -826,14 +810,38 @@
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "profilingGroupName": str,
+    },
+)
+_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "frameMetrics": Sequence[FrameMetricUnionTypeDef],
+        "period": str,
+        "startTime": TimestampTypeDef,
+        "targetResolution": AggregationPeriodType,
+    },
+    total=False,
+)
+
+class BatchGetFrameMetricDataRequestRequestTypeDef(
+    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
+    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+):
+    pass
+
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguruprofiler
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeGuruProfiler 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeGuruProfiler 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codeguruprofiler type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codeguruprofiler type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguruprofiler)](https://pepy.tech/project/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
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
@@ -319,92 +319,96 @@
 )
 
 
 def check_value(value: ActionGroupType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
-    ChannelOutputTypeDef,
-    ChannelTypeDef,
     ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
-    FrameMetricOutputTypeDef,
-    FrameMetricTypeDef,
+    TimestampTypeDef,
     TimestampStructureTypeDef,
+    BlobTypeDef,
+    ChannelOutputTypeDef,
+    ChannelTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
+    FrameMetricOutputTypeDef,
+    FrameMetricTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetProfileRequestRequestTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
-    ListFindingsReportsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListProfileTimesRequestRequestTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MatchTypeDef,
     PatternTypeDef,
-    PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
-    AddNotificationChannelsRequestRequestTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutPermissionResponseTypeDef,
     RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
-    FrameMetricDatumTypeDef,
-    BatchGetFrameMetricDataRequestRequestTypeDef,
+    GetProfileRequestRequestTypeDef,
+    GetRecommendationsRequestRequestTypeDef,
+    ListFindingsReportsRequestRequestTypeDef,
+    ListProfileTimesRequestRequestTypeDef,
+    PostAgentProfileRequestRequestTypeDef,
+    NotificationConfigurationTypeDef,
+    ChannelUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
+    FrameMetricDatumTypeDef,
+    FrameMetricUnionTypeDef,
     ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
+    ProfilingGroupDescriptionTypeDef,
+    AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
+    AddNotificationChannelsRequestRequestTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
+    BatchGetFrameMetricDataRequestRequestTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     UpdateProfilingGroupResponseTypeDef,
     GetRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> ChannelOutputTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt` & `mypy-boto3-codeguruprofiler-1.28.16/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.15.post1/setup.py` & `mypy-boto3-codeguruprofiler-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguruprofiler",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_codeguruprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruProfiler 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CodeGuruProfiler 1.28.16 service generated with"
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
-    keywords="boto3 codeguruprofiler type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 codeguruprofiler type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codeguruprofiler": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

