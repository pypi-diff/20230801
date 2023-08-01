# Comparing `tmp/mypy-boto3-evidently-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-evidently-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-evidently-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:07 2023, max compression
+gzip compressed data, was "mypy-boto3-evidently-1.28.16.tar", last modified: Tue Aug  1 11:36:48 2023, max compression
```

## Comparing `mypy-boto3-evidently-1.28.15.post1.tar` & `mypy-boto3-evidently-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:07.901149 mypy-boto3-evidently-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:15.000000 mypy-boto3-evidently-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18390 2023-07-29 10:03:07.893149 mypy-boto3-evidently-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-07-29 09:45:15.000000 mypy-boto3-evidently-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:07.889149 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-29 09:45:15.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-29 09:45:15.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:45:15.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30404 2023-07-29 09:45:16.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-29 09:45:15.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-29 09:45:16.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-29 09:45:16.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-29 09:45:16.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-29 09:45:16.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:15.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45680 2023-07-29 09:45:17.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45595 2023-07-29 09:45:17.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:15.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:07.893149 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18390 2023-07-29 10:03:07.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:07.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:07.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:07.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:07.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:07.000000 mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:07.901149 mypy-boto3-evidently-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-29 09:45:15.000000 mypy-boto3-evidently-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:48.452889 mypy-boto3-evidently-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-08-01 11:36:48.444889 mypy-boto3-evidently-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16900 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:48.444889 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30377 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30326 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45722 2023-08-01 11:17:54.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45637 2023-08-01 11:17:53.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:48.444889 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-08-01 11:36:48.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:36:48.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:48.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:36:48.000000 mypy-boto3-evidently-1.28.16/mypy_boto3_evidently.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:48.452889 mypy-boto3-evidently-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-01 11:17:52.000000 mypy-boto3-evidently-1.28.16/setup.py
```

### Comparing `mypy-boto3-evidently-1.28.15.post1/LICENSE` & `mypy-boto3-evidently-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.15.post1/PKG-INFO` & `mypy-boto3-evidently-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-evidently
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatchEvidently 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatchEvidently 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 evidently type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 evidently type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-evidently)](https://pepy.tech/project/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
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
@@ -346,20 +346,20 @@
 )
 
 
 def check_value(value: ChangeDirectionEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_evidently.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_evidently.type_defs import (
     EvaluationRequestTypeDef,
     ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
@@ -373,23 +373,22 @@
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
     VariableValueTypeDef,
     EvaluationRuleTypeDef,
-    EventTypeDef,
+    TimestampTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
     TreatmentTypeDef,
     GetExperimentRequestRequestTypeDef,
-    GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
     PaginatorConfigTypeDef,
@@ -406,15 +405,14 @@
     MetricDefinitionTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
     SegmentOverrideTypeDef,
     SegmentOverrideOutputTypeDef,
-    StartExperimentRequestRequestTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     StopLaunchRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
@@ -428,15 +426,17 @@
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
     VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
-    PutProjectEventsRequestRequestTypeDef,
+    EventTypeDef,
+    GetExperimentResultsRequestRequestTypeDef,
+    StartExperimentRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
     ListExperimentsRequestListExperimentsPaginateTypeDef,
     ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentsRequestListSegmentsPaginateTypeDef,
@@ -453,14 +453,15 @@
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
     CreateFeatureRequestRequestTypeDef,
     UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
+    PutProjectEventsRequestRequestTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
@@ -482,15 +483,15 @@
     GetLaunchResponseTypeDef,
     ListLaunchesResponseTypeDef,
     StartLaunchResponseTypeDef,
     UpdateLaunchResponseTypeDef,
 )
 
 
-def get_structure() -> EvaluationRequestTypeDef:
+def get_value() -> EvaluationRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-evidently-1.28.15.post1/README.md` & `mypy-boto3-evidently-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-evidently)](https://pepy.tech/project/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: ChangeDirectionEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_evidently.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_evidently.type_defs import (
     EvaluationRequestTypeDef,
     ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
@@ -341,23 +341,22 @@
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
     VariableValueTypeDef,
     EvaluationRuleTypeDef,
-    EventTypeDef,
+    TimestampTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
     TreatmentTypeDef,
     GetExperimentRequestRequestTypeDef,
-    GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
     PaginatorConfigTypeDef,
@@ -374,15 +373,14 @@
     MetricDefinitionTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
     SegmentOverrideTypeDef,
     SegmentOverrideOutputTypeDef,
-    StartExperimentRequestRequestTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     StopLaunchRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
@@ -396,15 +394,17 @@
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
     VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
-    PutProjectEventsRequestRequestTypeDef,
+    EventTypeDef,
+    GetExperimentResultsRequestRequestTypeDef,
+    StartExperimentRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
     ListExperimentsRequestListExperimentsPaginateTypeDef,
     ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentsRequestListSegmentsPaginateTypeDef,
@@ -421,14 +421,15 @@
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
     CreateFeatureRequestRequestTypeDef,
     UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
+    PutProjectEventsRequestRequestTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
@@ -450,15 +451,15 @@
     GetLaunchResponseTypeDef,
     ListLaunchesResponseTypeDef,
     StartLaunchResponseTypeDef,
     UpdateLaunchResponseTypeDef,
 )
 
 
-def get_structure() -> EvaluationRequestTypeDef:
+def get_value() -> EvaluationRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/__init__.py` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/__init__.pyi` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/client.py` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_evidently.client import CloudWatchEvidentlyClient
 
     session = Session()
     client: CloudWatchEvidentlyClient = session.client("evidently")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ExperimentResultRequestTypeType,
     ExperimentStatusType,
     ExperimentStopDesiredStateType,
@@ -70,14 +69,15 @@
     S3DestinationConfigTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     StartExperimentResponseTypeDef,
     StartLaunchResponseTypeDef,
     StopExperimentResponseTypeDef,
     StopLaunchResponseTypeDef,
     TestSegmentPatternResponseTypeDef,
+    TimestampTypeDef,
     TreatmentConfigTypeDef,
     UpdateExperimentResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     UpdateLaunchResponseTypeDef,
     UpdateProjectDataDeliveryResponseTypeDef,
     UpdateProjectResponseTypeDef,
     VariationConfigTypeDef,
@@ -317,19 +317,19 @@
         self,
         *,
         experiment: str,
         metricNames: Sequence[str],
         project: str,
         treatmentNames: Sequence[str],
         baseStat: Literal["Mean"] = ...,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         period: int = ...,
         reportNames: Sequence[Literal["BayesianInference"]] = ...,
         resultStats: Sequence[ExperimentResultRequestTypeType] = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> GetExperimentResultsResponseTypeDef:
         """
         Retrieves the results of a running or completed experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.get_experiment_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/client/#get_experiment_results)
         """
@@ -460,15 +460,15 @@
         Sends performance events to Evidently.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.put_project_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/client/#put_project_events)
         """
 
     def start_experiment(
-        self, *, analysisCompleteTime: Union[datetime, str], experiment: str, project: str
+        self, *, analysisCompleteTime: TimestampTypeDef, experiment: str, project: str
     ) -> StartExperimentResponseTypeDef:
         """
         Starts an existing experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.start_experiment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/client/#start_experiment)
         """
```

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/client.pyi` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_evidently.client import CloudWatchEvidentlyClient
 
     session = Session()
     client: CloudWatchEvidentlyClient = session.client("evidently")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ExperimentResultRequestTypeType,
     ExperimentStatusType,
     ExperimentStopDesiredStateType,
@@ -70,14 +69,15 @@
     S3DestinationConfigTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     StartExperimentResponseTypeDef,
     StartLaunchResponseTypeDef,
     StopExperimentResponseTypeDef,
     StopLaunchResponseTypeDef,
     TestSegmentPatternResponseTypeDef,
+    TimestampTypeDef,
     TreatmentConfigTypeDef,
     UpdateExperimentResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     UpdateLaunchResponseTypeDef,
     UpdateProjectDataDeliveryResponseTypeDef,
     UpdateProjectResponseTypeDef,
     VariationConfigTypeDef,
@@ -296,19 +296,19 @@
         self,
         *,
         experiment: str,
         metricNames: Sequence[str],
         project: str,
         treatmentNames: Sequence[str],
         baseStat: Literal["Mean"] = ...,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         period: int = ...,
         reportNames: Sequence[Literal["BayesianInference"]] = ...,
         resultStats: Sequence[ExperimentResultRequestTypeType] = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> GetExperimentResultsResponseTypeDef:
         """
         Retrieves the results of a running or completed experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.get_experiment_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/client/#get_experiment_results)
         """
@@ -426,15 +426,15 @@
         """
         Sends performance events to Evidently.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.put_project_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/client/#put_project_events)
         """
     def start_experiment(
-        self, *, analysisCompleteTime: Union[datetime, str], experiment: str, project: str
+        self, *, analysisCompleteTime: TimestampTypeDef, experiment: str, project: str
     ) -> StartExperimentResponseTypeDef:
         """
         Starts an existing experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.start_experiment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/client/#start_experiment)
         """
```

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/literals.py` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/literals.pyi` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/paginator.py` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/paginator.pyi` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/type_defs.py` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_evidently.type_defs import EvaluationRequestTypeDef
 
-    data: EvaluationRequestTypeDef = {...}
+    data: EvaluationRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -56,23 +56,22 @@
     "DeleteFeatureRequestRequestTypeDef",
     "DeleteLaunchRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteSegmentRequestRequestTypeDef",
     "EvaluateFeatureRequestRequestTypeDef",
     "VariableValueTypeDef",
     "EvaluationRuleTypeDef",
-    "EventTypeDef",
+    "TimestampTypeDef",
     "ExperimentExecutionTypeDef",
     "ExperimentReportTypeDef",
     "ExperimentResultsDataTypeDef",
     "ExperimentScheduleTypeDef",
     "OnlineAbDefinitionTypeDef",
     "TreatmentTypeDef",
     "GetExperimentRequestRequestTypeDef",
-    "GetExperimentResultsRequestRequestTypeDef",
     "GetFeatureRequestRequestTypeDef",
     "GetLaunchRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "LaunchExecutionTypeDef",
     "LaunchGroupTypeDef",
     "PaginatorConfigTypeDef",
@@ -89,15 +88,14 @@
     "MetricDefinitionTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
     "SegmentOverrideTypeDef",
     "SegmentOverrideOutputTypeDef",
-    "StartExperimentRequestRequestTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "StopLaunchRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
@@ -111,15 +109,17 @@
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
     "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
-    "PutProjectEventsRequestRequestTypeDef",
+    "EventTypeDef",
+    "GetExperimentResultsRequestRequestTypeDef",
+    "StartExperimentRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
     "ListExperimentsRequestListExperimentsPaginateTypeDef",
     "ListFeaturesRequestListFeaturesPaginateTypeDef",
     "ListLaunchesRequestListLaunchesPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
     "ListSegmentsRequestListSegmentsPaginateTypeDef",
@@ -136,14 +136,15 @@
     "ScheduledSplitConfigTypeDef",
     "ScheduledSplitTypeDef",
     "BatchEvaluateFeatureResponseTypeDef",
     "CreateFeatureRequestRequestTypeDef",
     "UpdateFeatureRequestRequestTypeDef",
     "FeatureTypeDef",
     "ListFeaturesResponseTypeDef",
+    "PutProjectEventsRequestRequestTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
     "ExperimentTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectTypeDef",
     "ScheduledSplitsLaunchConfigTypeDef",
     "ScheduledSplitsLaunchDefinitionTypeDef",
@@ -415,23 +416,15 @@
 )
 
 
 class EvaluationRuleTypeDef(_RequiredEvaluationRuleTypeDef, _OptionalEvaluationRuleTypeDef):
     pass
 
 
-EventTypeDef = TypedDict(
-    "EventTypeDef",
-    {
-        "data": str,
-        "timestamp": Union[datetime, str],
-        "type": EventTypeType,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ExperimentExecutionTypeDef = TypedDict(
     "ExperimentExecutionTypeDef",
     {
         "endedTime": datetime,
         "startedTime": datetime,
     },
     total=False,
@@ -500,44 +493,14 @@
     "GetExperimentRequestRequestTypeDef",
     {
         "experiment": str,
         "project": str,
     },
 )
 
-_RequiredGetExperimentResultsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetExperimentResultsRequestRequestTypeDef",
-    {
-        "experiment": str,
-        "metricNames": Sequence[str],
-        "project": str,
-        "treatmentNames": Sequence[str],
-    },
-)
-_OptionalGetExperimentResultsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetExperimentResultsRequestRequestTypeDef",
-    {
-        "baseStat": Literal["Mean"],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "reportNames": Sequence[Literal["BayesianInference"]],
-        "resultStats": Sequence[ExperimentResultRequestTypeType],
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GetExperimentResultsRequestRequestTypeDef(
-    _RequiredGetExperimentResultsRequestRequestTypeDef,
-    _OptionalGetExperimentResultsRequestRequestTypeDef,
-):
-    pass
-
-
 GetFeatureRequestRequestTypeDef = TypedDict(
     "GetFeatureRequestRequestTypeDef",
     {
         "feature": str,
         "project": str,
     },
 )
@@ -860,23 +823,14 @@
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Dict[str, int],
     },
 )
 
-StartExperimentRequestRequestTypeDef = TypedDict(
-    "StartExperimentRequestRequestTypeDef",
-    {
-        "analysisCompleteTime": Union[datetime, str],
-        "experiment": str,
-        "project": str,
-    },
-)
-
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -1121,18 +1075,58 @@
 )
 
 
 class FeatureSummaryTypeDef(_RequiredFeatureSummaryTypeDef, _OptionalFeatureSummaryTypeDef):
     pass
 
 
-PutProjectEventsRequestRequestTypeDef = TypedDict(
-    "PutProjectEventsRequestRequestTypeDef",
+EventTypeDef = TypedDict(
+    "EventTypeDef",
     {
-        "events": Sequence[EventTypeDef],
+        "data": str,
+        "timestamp": TimestampTypeDef,
+        "type": EventTypeType,
+    },
+)
+
+_RequiredGetExperimentResultsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetExperimentResultsRequestRequestTypeDef",
+    {
+        "experiment": str,
+        "metricNames": Sequence[str],
+        "project": str,
+        "treatmentNames": Sequence[str],
+    },
+)
+_OptionalGetExperimentResultsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetExperimentResultsRequestRequestTypeDef",
+    {
+        "baseStat": Literal["Mean"],
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "reportNames": Sequence[Literal["BayesianInference"]],
+        "resultStats": Sequence[ExperimentResultRequestTypeType],
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GetExperimentResultsRequestRequestTypeDef(
+    _RequiredGetExperimentResultsRequestRequestTypeDef,
+    _OptionalGetExperimentResultsRequestRequestTypeDef,
+):
+    pass
+
+
+StartExperimentRequestRequestTypeDef = TypedDict(
+    "StartExperimentRequestRequestTypeDef",
+    {
+        "analysisCompleteTime": TimestampTypeDef,
+        "experiment": str,
         "project": str,
     },
 )
 
 GetExperimentResultsResponseTypeDef = TypedDict(
     "GetExperimentResultsResponseTypeDef",
     {
@@ -1371,15 +1365,15 @@
     },
 )
 
 _RequiredScheduledSplitConfigTypeDef = TypedDict(
     "_RequiredScheduledSplitConfigTypeDef",
     {
         "groupWeights": Mapping[str, int],
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalScheduledSplitConfigTypeDef = TypedDict(
     "_OptionalScheduledSplitConfigTypeDef",
     {
         "segmentOverrides": Sequence[SegmentOverrideTypeDef],
     },
@@ -1511,14 +1505,22 @@
     {
         "features": List[FeatureSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutProjectEventsRequestRequestTypeDef = TypedDict(
+    "PutProjectEventsRequestRequestTypeDef",
+    {
+        "events": Sequence[EventTypeDef],
+        "project": str,
+    },
+)
+
 _RequiredCreateExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentRequestRequestTypeDef",
     {
         "metricGoals": Sequence[MetricGoalConfigTypeDef],
         "name": str,
         "project": str,
         "treatments": Sequence[TreatmentConfigTypeDef],
```

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently/type_defs.pyi` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_evidently.type_defs import EvaluationRequestTypeDef
 
-    data: EvaluationRequestTypeDef = {...}
+    data: EvaluationRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -55,23 +55,22 @@
     "DeleteFeatureRequestRequestTypeDef",
     "DeleteLaunchRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteSegmentRequestRequestTypeDef",
     "EvaluateFeatureRequestRequestTypeDef",
     "VariableValueTypeDef",
     "EvaluationRuleTypeDef",
-    "EventTypeDef",
+    "TimestampTypeDef",
     "ExperimentExecutionTypeDef",
     "ExperimentReportTypeDef",
     "ExperimentResultsDataTypeDef",
     "ExperimentScheduleTypeDef",
     "OnlineAbDefinitionTypeDef",
     "TreatmentTypeDef",
     "GetExperimentRequestRequestTypeDef",
-    "GetExperimentResultsRequestRequestTypeDef",
     "GetFeatureRequestRequestTypeDef",
     "GetLaunchRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "LaunchExecutionTypeDef",
     "LaunchGroupTypeDef",
     "PaginatorConfigTypeDef",
@@ -88,15 +87,14 @@
     "MetricDefinitionTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
     "SegmentOverrideTypeDef",
     "SegmentOverrideOutputTypeDef",
-    "StartExperimentRequestRequestTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "StopLaunchRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
@@ -110,15 +108,17 @@
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
     "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
-    "PutProjectEventsRequestRequestTypeDef",
+    "EventTypeDef",
+    "GetExperimentResultsRequestRequestTypeDef",
+    "StartExperimentRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
     "ListExperimentsRequestListExperimentsPaginateTypeDef",
     "ListFeaturesRequestListFeaturesPaginateTypeDef",
     "ListLaunchesRequestListLaunchesPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
     "ListSegmentsRequestListSegmentsPaginateTypeDef",
@@ -135,14 +135,15 @@
     "ScheduledSplitConfigTypeDef",
     "ScheduledSplitTypeDef",
     "BatchEvaluateFeatureResponseTypeDef",
     "CreateFeatureRequestRequestTypeDef",
     "UpdateFeatureRequestRequestTypeDef",
     "FeatureTypeDef",
     "ListFeaturesResponseTypeDef",
+    "PutProjectEventsRequestRequestTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
     "ExperimentTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectTypeDef",
     "ScheduledSplitsLaunchConfigTypeDef",
     "ScheduledSplitsLaunchDefinitionTypeDef",
@@ -400,23 +401,15 @@
     },
     total=False,
 )
 
 class EvaluationRuleTypeDef(_RequiredEvaluationRuleTypeDef, _OptionalEvaluationRuleTypeDef):
     pass
 
-EventTypeDef = TypedDict(
-    "EventTypeDef",
-    {
-        "data": str,
-        "timestamp": Union[datetime, str],
-        "type": EventTypeType,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ExperimentExecutionTypeDef = TypedDict(
     "ExperimentExecutionTypeDef",
     {
         "endedTime": datetime,
         "startedTime": datetime,
     },
     total=False,
@@ -483,42 +476,14 @@
     "GetExperimentRequestRequestTypeDef",
     {
         "experiment": str,
         "project": str,
     },
 )
 
-_RequiredGetExperimentResultsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetExperimentResultsRequestRequestTypeDef",
-    {
-        "experiment": str,
-        "metricNames": Sequence[str],
-        "project": str,
-        "treatmentNames": Sequence[str],
-    },
-)
-_OptionalGetExperimentResultsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetExperimentResultsRequestRequestTypeDef",
-    {
-        "baseStat": Literal["Mean"],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "reportNames": Sequence[Literal["BayesianInference"]],
-        "resultStats": Sequence[ExperimentResultRequestTypeType],
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GetExperimentResultsRequestRequestTypeDef(
-    _RequiredGetExperimentResultsRequestRequestTypeDef,
-    _OptionalGetExperimentResultsRequestRequestTypeDef,
-):
-    pass
-
 GetFeatureRequestRequestTypeDef = TypedDict(
     "GetFeatureRequestRequestTypeDef",
     {
         "feature": str,
         "project": str,
     },
 )
@@ -825,23 +790,14 @@
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Dict[str, int],
     },
 )
 
-StartExperimentRequestRequestTypeDef = TypedDict(
-    "StartExperimentRequestRequestTypeDef",
-    {
-        "analysisCompleteTime": Union[datetime, str],
-        "experiment": str,
-        "project": str,
-    },
-)
-
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -1076,18 +1032,56 @@
     },
     total=False,
 )
 
 class FeatureSummaryTypeDef(_RequiredFeatureSummaryTypeDef, _OptionalFeatureSummaryTypeDef):
     pass
 
-PutProjectEventsRequestRequestTypeDef = TypedDict(
-    "PutProjectEventsRequestRequestTypeDef",
+EventTypeDef = TypedDict(
+    "EventTypeDef",
     {
-        "events": Sequence[EventTypeDef],
+        "data": str,
+        "timestamp": TimestampTypeDef,
+        "type": EventTypeType,
+    },
+)
+
+_RequiredGetExperimentResultsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetExperimentResultsRequestRequestTypeDef",
+    {
+        "experiment": str,
+        "metricNames": Sequence[str],
+        "project": str,
+        "treatmentNames": Sequence[str],
+    },
+)
+_OptionalGetExperimentResultsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetExperimentResultsRequestRequestTypeDef",
+    {
+        "baseStat": Literal["Mean"],
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "reportNames": Sequence[Literal["BayesianInference"]],
+        "resultStats": Sequence[ExperimentResultRequestTypeType],
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class GetExperimentResultsRequestRequestTypeDef(
+    _RequiredGetExperimentResultsRequestRequestTypeDef,
+    _OptionalGetExperimentResultsRequestRequestTypeDef,
+):
+    pass
+
+StartExperimentRequestRequestTypeDef = TypedDict(
+    "StartExperimentRequestRequestTypeDef",
+    {
+        "analysisCompleteTime": TimestampTypeDef,
+        "experiment": str,
         "project": str,
     },
 )
 
 GetExperimentResultsResponseTypeDef = TypedDict(
     "GetExperimentResultsResponseTypeDef",
     {
@@ -1312,15 +1306,15 @@
     },
 )
 
 _RequiredScheduledSplitConfigTypeDef = TypedDict(
     "_RequiredScheduledSplitConfigTypeDef",
     {
         "groupWeights": Mapping[str, int],
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalScheduledSplitConfigTypeDef = TypedDict(
     "_OptionalScheduledSplitConfigTypeDef",
     {
         "segmentOverrides": Sequence[SegmentOverrideTypeDef],
     },
@@ -1442,14 +1436,22 @@
     {
         "features": List[FeatureSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutProjectEventsRequestRequestTypeDef = TypedDict(
+    "PutProjectEventsRequestRequestTypeDef",
+    {
+        "events": Sequence[EventTypeDef],
+        "project": str,
+    },
+)
+
 _RequiredCreateExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentRequestRequestTypeDef",
     {
         "metricGoals": Sequence[MetricGoalConfigTypeDef],
         "name": str,
         "project": str,
         "treatments": Sequence[TreatmentConfigTypeDef],
```

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently.egg-info/PKG-INFO` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-evidently
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatchEvidently 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatchEvidently 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 evidently type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 evidently type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-evidently)](https://pepy.tech/project/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
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
@@ -346,20 +346,20 @@
 )
 
 
 def check_value(value: ChangeDirectionEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_evidently.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_evidently.type_defs import (
     EvaluationRequestTypeDef,
     ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
@@ -373,23 +373,22 @@
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
     VariableValueTypeDef,
     EvaluationRuleTypeDef,
-    EventTypeDef,
+    TimestampTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
     TreatmentTypeDef,
     GetExperimentRequestRequestTypeDef,
-    GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
     PaginatorConfigTypeDef,
@@ -406,15 +405,14 @@
     MetricDefinitionTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
     SegmentOverrideTypeDef,
     SegmentOverrideOutputTypeDef,
-    StartExperimentRequestRequestTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     StopLaunchRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
@@ -428,15 +426,17 @@
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
     VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
-    PutProjectEventsRequestRequestTypeDef,
+    EventTypeDef,
+    GetExperimentResultsRequestRequestTypeDef,
+    StartExperimentRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
     ListExperimentsRequestListExperimentsPaginateTypeDef,
     ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentsRequestListSegmentsPaginateTypeDef,
@@ -453,14 +453,15 @@
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
     CreateFeatureRequestRequestTypeDef,
     UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
+    PutProjectEventsRequestRequestTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
@@ -482,15 +483,15 @@
     GetLaunchResponseTypeDef,
     ListLaunchesResponseTypeDef,
     StartLaunchResponseTypeDef,
     UpdateLaunchResponseTypeDef,
 )
 
 
-def get_structure() -> EvaluationRequestTypeDef:
+def get_value() -> EvaluationRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-evidently-1.28.15.post1/mypy_boto3_evidently.egg-info/SOURCES.txt` & `mypy-boto3-evidently-1.28.16/mypy_boto3_evidently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.15.post1/setup.py` & `mypy-boto3-evidently-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-evidently",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_evidently"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchEvidently 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CloudWatchEvidently 1.28.16 service generated with"
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
-    keywords="boto3 evidently type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 evidently type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_evidently": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

