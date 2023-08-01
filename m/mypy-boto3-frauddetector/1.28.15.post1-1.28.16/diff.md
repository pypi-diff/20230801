# Comparing `tmp/mypy-boto3-frauddetector-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-frauddetector-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-frauddetector-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:10 2023, max compression
+gzip compressed data, was "mypy-boto3-frauddetector-1.28.16.tar", last modified: Tue Aug  1 11:36:50 2023, max compression
```

## Comparing `mypy-boto3-frauddetector-1.28.15.post1.tar` & `mypy-boto3-frauddetector-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:10.113157 mypy-boto3-frauddetector-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-07-29 10:03:10.113157 mypy-boto3-frauddetector-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:10.105157 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46531 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46451 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-29 09:45:41.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60744 2023-07-29 09:45:43.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60673 2023-07-29 09:45:42.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:10.113157 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:10.113157 mypy-boto3-frauddetector-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:50.016886 mypy-boto3-frauddetector-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:18:17.000000 mypy-boto3-frauddetector-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-08-01 11:36:50.008886 mypy-boto3-frauddetector-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-08-01 11:18:17.000000 mypy-boto3-frauddetector-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:50.000886 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-01 11:18:17.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 11:18:17.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 11:18:17.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46356 2023-08-01 11:18:18.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46276 2023-08-01 11:18:17.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-08-01 11:18:18.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-08-01 11:18:18.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:18:17.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61091 2023-08-01 11:18:20.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61020 2023-08-01 11:18:19.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:18:17.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:50.008886 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-08-01 11:36:49.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 11:36:49.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:49.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:49.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:49.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:36:49.000000 mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:50.016886 mypy-boto3-frauddetector-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 11:18:17.000000 mypy-boto3-frauddetector-1.28.16/setup.py
```

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/LICENSE` & `mypy-boto3-frauddetector-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/PKG-INFO` & `mypy-boto3-frauddetector-1.28.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.FraudDetector 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 frauddetector type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 frauddetector type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-frauddetector)](https://pepy.tech/project/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -303,20 +303,20 @@
 )
 
 
 def check_value(value: AsyncJobStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_frauddetector.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_frauddetector.type_defs import (
     ATIMetricDataPointTypeDef,
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
@@ -326,14 +326,15 @@
     VariableEntryTypeDef,
     ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
     BatchImportTypeDef,
     BatchPredictionTypeDef,
+    BlobTypeDef,
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
     ExternalEventsDetailTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
@@ -371,15 +372,14 @@
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
-    ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
@@ -437,14 +437,15 @@
     GetListsMetadataResultTypeDef,
     ListTagsForResourceResultTypeDef,
     UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
+    ModelEndpointDataBlobTypeDef,
     ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
     CreateRuleResultTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetDetectorVersionResultTypeDef,
     UpdateDetectorVersionRequestRequestTypeDef,
     UpdateRuleMetadataRequestRequestTypeDef,
@@ -457,51 +458,53 @@
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
     PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
-    GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
     GetModelsResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
     IngestedEventsDetailTypeDef,
     TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     ListEventPredictionsRequestRequestTypeDef,
     VariableImportanceMetricsTypeDef,
     TrainingMetricsTypeDef,
+    ModelOutputConfigurationUnionTypeDef,
     PutExternalModelRequestRequestTypeDef,
     OFIModelPerformanceTypeDef,
     TFIModelPerformanceTypeDef,
     PredictionExplanationsTypeDef,
+    GetEventPredictionRequestRequestTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
     GetEventPredictionResultTypeDef,
     GetExternalModelsResultTypeDef,
     UpdateModelVersionRequestRequestTypeDef,
     GetModelVersionResultTypeDef,
     CreateModelVersionRequestRequestTypeDef,
+    TrainingDataSchemaUnionTypeDef,
     TrainingResultTypeDef,
     OFITrainingMetricsValueTypeDef,
     TFITrainingMetricsValueTypeDef,
     ModelVersionEvaluationTypeDef,
     TrainingMetricsV2TypeDef,
     EvaluatedModelVersionTypeDef,
     TrainingResultV2TypeDef,
     GetEventPredictionMetadataResultTypeDef,
     ModelVersionDetailTypeDef,
     DescribeModelVersionsResultTypeDef,
 )
 
 
-def get_structure() -> ATIMetricDataPointTypeDef:
+def get_value() -> ATIMetricDataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/README.md` & `mypy-boto3-frauddetector-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-frauddetector)](https://pepy.tech/project/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -271,20 +271,20 @@
 )
 
 
 def check_value(value: AsyncJobStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_frauddetector.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_frauddetector.type_defs import (
     ATIMetricDataPointTypeDef,
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
@@ -294,14 +294,15 @@
     VariableEntryTypeDef,
     ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
     BatchImportTypeDef,
     BatchPredictionTypeDef,
+    BlobTypeDef,
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
     ExternalEventsDetailTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
@@ -339,15 +340,14 @@
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
-    ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
@@ -405,14 +405,15 @@
     GetListsMetadataResultTypeDef,
     ListTagsForResourceResultTypeDef,
     UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
+    ModelEndpointDataBlobTypeDef,
     ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
     CreateRuleResultTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetDetectorVersionResultTypeDef,
     UpdateDetectorVersionRequestRequestTypeDef,
     UpdateRuleMetadataRequestRequestTypeDef,
@@ -425,51 +426,53 @@
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
     PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
-    GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
     GetModelsResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
     IngestedEventsDetailTypeDef,
     TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     ListEventPredictionsRequestRequestTypeDef,
     VariableImportanceMetricsTypeDef,
     TrainingMetricsTypeDef,
+    ModelOutputConfigurationUnionTypeDef,
     PutExternalModelRequestRequestTypeDef,
     OFIModelPerformanceTypeDef,
     TFIModelPerformanceTypeDef,
     PredictionExplanationsTypeDef,
+    GetEventPredictionRequestRequestTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
     GetEventPredictionResultTypeDef,
     GetExternalModelsResultTypeDef,
     UpdateModelVersionRequestRequestTypeDef,
     GetModelVersionResultTypeDef,
     CreateModelVersionRequestRequestTypeDef,
+    TrainingDataSchemaUnionTypeDef,
     TrainingResultTypeDef,
     OFITrainingMetricsValueTypeDef,
     TFITrainingMetricsValueTypeDef,
     ModelVersionEvaluationTypeDef,
     TrainingMetricsV2TypeDef,
     EvaluatedModelVersionTypeDef,
     TrainingResultV2TypeDef,
     GetEventPredictionMetadataResultTypeDef,
     ModelVersionDetailTypeDef,
     DescribeModelVersionsResultTypeDef,
 )
 
 
-def get_structure() -> ATIMetricDataPointTypeDef:
+def get_value() -> ATIMetricDataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/__main__.py` & `mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FraudDetector 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.FraudDetector 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector\nOther"
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

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/client.py` & `mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_frauddetector.client import FraudDetectorClient
 
     session = Session()
     client: FraudDetectorClient = session.client("frauddetector")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
@@ -64,22 +64,20 @@
     GetRulesResultTypeDef,
     GetVariablesResultTypeDef,
     IngestedEventsDetailTypeDef,
     ListEventPredictionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     ModelEndpointDataBlobTypeDef,
     ModelInputConfigurationTypeDef,
-    ModelOutputConfigurationOutputTypeDef,
-    ModelOutputConfigurationTypeDef,
+    ModelOutputConfigurationUnionTypeDef,
     ModelVersionTypeDef,
     PredictionTimeRangeTypeDef,
     RuleTypeDef,
     TagTypeDef,
-    TrainingDataSchemaOutputTypeDef,
-    TrainingDataSchemaTypeDef,
+    TrainingDataSchemaUnionTypeDef,
     UpdateModelVersionResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     VariableEntryTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -264,15 +262,15 @@
 
     def create_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
-        trainingDataSchema: Union[TrainingDataSchemaTypeDef, TrainingDataSchemaOutputTypeDef],
+        trainingDataSchema: TrainingDataSchemaUnionTypeDef,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
@@ -794,17 +792,15 @@
     def put_external_model(
         self,
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
-        outputConfiguration: Union[
-            ModelOutputConfigurationTypeDef, ModelOutputConfigurationOutputTypeDef
-        ],
+        outputConfiguration: ModelOutputConfigurationUnionTypeDef,
         modelEndpointStatus: ModelEndpointStatusType,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
```

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/client.pyi` & `mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_frauddetector.client import FraudDetectorClient
 
     session = Session()
     client: FraudDetectorClient = session.client("frauddetector")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
@@ -64,22 +64,20 @@
     GetRulesResultTypeDef,
     GetVariablesResultTypeDef,
     IngestedEventsDetailTypeDef,
     ListEventPredictionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     ModelEndpointDataBlobTypeDef,
     ModelInputConfigurationTypeDef,
-    ModelOutputConfigurationOutputTypeDef,
-    ModelOutputConfigurationTypeDef,
+    ModelOutputConfigurationUnionTypeDef,
     ModelVersionTypeDef,
     PredictionTimeRangeTypeDef,
     RuleTypeDef,
     TagTypeDef,
-    TrainingDataSchemaOutputTypeDef,
-    TrainingDataSchemaTypeDef,
+    TrainingDataSchemaUnionTypeDef,
     UpdateModelVersionResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     VariableEntryTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -248,15 +246,15 @@
         """
     def create_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
-        trainingDataSchema: Union[TrainingDataSchemaTypeDef, TrainingDataSchemaOutputTypeDef],
+        trainingDataSchema: TrainingDataSchemaUnionTypeDef,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
@@ -731,17 +729,15 @@
     def put_external_model(
         self,
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
-        outputConfiguration: Union[
-            ModelOutputConfigurationTypeDef, ModelOutputConfigurationOutputTypeDef
-        ],
+        outputConfiguration: ModelOutputConfigurationUnionTypeDef,
         modelEndpointStatus: ModelEndpointStatusType,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
```

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/literals.py` & `mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/literals.pyi` & `mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/type_defs.py` & `mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_frauddetector.type_defs import ATIMetricDataPointTypeDef
 
-    data: ATIMetricDataPointTypeDef = {...}
+    data: ATIMetricDataPointTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -54,14 +54,15 @@
     "VariableEntryTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetVariableErrorTypeDef",
     "BatchGetVariableRequestRequestTypeDef",
     "VariableTypeDef",
     "BatchImportTypeDef",
     "BatchPredictionTypeDef",
+    "BlobTypeDef",
     "CancelBatchImportJobRequestRequestTypeDef",
     "CancelBatchPredictionJobRequestRequestTypeDef",
     "ModelVersionTypeDef",
     "RuleTypeDef",
     "ExternalEventsDetailTypeDef",
     "FieldValidationMessageTypeDef",
     "FileValidationMessageTypeDef",
@@ -99,15 +100,14 @@
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
     "GetEventPredictionMetadataRequestRequestTypeDef",
-    "ModelEndpointDataBlobTypeDef",
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
     "GetExternalModelsRequestRequestTypeDef",
     "KMSKeyTypeDef",
     "GetLabelsRequestRequestTypeDef",
     "LabelTypeDef",
@@ -165,14 +165,15 @@
     "GetListsMetadataResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "UpdateModelVersionResultTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
+    "ModelEndpointDataBlobTypeDef",
     "ModelScoresTypeDef",
     "CreateDetectorVersionRequestRequestTypeDef",
     "CreateRuleResultTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "GetDetectorVersionResultTypeDef",
     "UpdateDetectorVersionRequestRequestTypeDef",
     "UpdateRuleMetadataRequestRequestTypeDef",
@@ -185,37 +186,39 @@
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
-    "GetEventPredictionRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
     "GetLabelsResultTypeDef",
     "GetModelsResultTypeDef",
     "GetOutcomesResultTypeDef",
     "GetRulesResultTypeDef",
     "IngestedEventsDetailTypeDef",
     "TrainingDataSchemaOutputTypeDef",
     "TrainingDataSchemaTypeDef",
     "ListEventPredictionsRequestRequestTypeDef",
     "VariableImportanceMetricsTypeDef",
     "TrainingMetricsTypeDef",
+    "ModelOutputConfigurationUnionTypeDef",
     "PutExternalModelRequestRequestTypeDef",
     "OFIModelPerformanceTypeDef",
     "TFIModelPerformanceTypeDef",
     "PredictionExplanationsTypeDef",
+    "GetEventPredictionRequestRequestTypeDef",
     "GetEventResultTypeDef",
     "GetEventTypesResultTypeDef",
     "GetEventPredictionResultTypeDef",
     "GetExternalModelsResultTypeDef",
     "UpdateModelVersionRequestRequestTypeDef",
     "GetModelVersionResultTypeDef",
     "CreateModelVersionRequestRequestTypeDef",
+    "TrainingDataSchemaUnionTypeDef",
     "TrainingResultTypeDef",
     "OFITrainingMetricsValueTypeDef",
     "TFITrainingMetricsValueTypeDef",
     "ModelVersionEvaluationTypeDef",
     "TrainingMetricsV2TypeDef",
     "EvaluatedModelVersionTypeDef",
     "TrainingResultV2TypeDef",
@@ -397,14 +400,15 @@
         "arn": str,
         "processedRecordsCount": int,
         "totalRecordsCount": int,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelBatchImportJobRequestRequestTypeDef = TypedDict(
     "CancelBatchImportJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -869,23 +873,14 @@
         "eventTypeName": str,
         "detectorId": str,
         "detectorVersionId": str,
         "predictionTimestamp": str,
     },
 )
 
-ModelEndpointDataBlobTypeDef = TypedDict(
-    "ModelEndpointDataBlobTypeDef",
-    {
-        "byteBuffer": Union[str, bytes, IO[Any], StreamingBody],
-        "contentType": str,
-    },
-    total=False,
-)
-
 RuleResultTypeDef = TypedDict(
     "RuleResultTypeDef",
     {
         "ruleId": str,
         "outcomes": List[str],
     },
     total=False,
@@ -1756,14 +1751,23 @@
     {
         "batchPredictions": List[BatchPredictionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ModelEndpointDataBlobTypeDef = TypedDict(
+    "ModelEndpointDataBlobTypeDef",
+    {
+        "byteBuffer": BlobTypeDef,
+        "contentType": str,
+    },
+    total=False,
+)
+
 ModelScoresTypeDef = TypedDict(
     "ModelScoresTypeDef",
     {
         "modelVersion": ModelVersionTypeDef,
         "scores": Dict[str, float],
     },
     total=False,
@@ -2050,42 +2054,14 @@
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
-_RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
-    "_RequiredGetEventPredictionRequestRequestTypeDef",
-    {
-        "detectorId": str,
-        "eventId": str,
-        "eventTypeName": str,
-        "entities": Sequence[EntityTypeDef],
-        "eventTimestamp": str,
-        "eventVariables": Mapping[str, str],
-    },
-)
-_OptionalGetEventPredictionRequestRequestTypeDef = TypedDict(
-    "_OptionalGetEventPredictionRequestRequestTypeDef",
-    {
-        "detectorVersionId": str,
-        "externalModelEndpointDataBlobs": Mapping[str, ModelEndpointDataBlobTypeDef],
-    },
-    total=False,
-)
-
-
-class GetEventPredictionRequestRequestTypeDef(
-    _RequiredGetEventPredictionRequestRequestTypeDef,
-    _OptionalGetEventPredictionRequestRequestTypeDef,
-):
-    pass
-
-
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2202,14 +2178,17 @@
     {
         "auc": float,
         "metricDataPoints": List[MetricDataPointTypeDef],
     },
     total=False,
 )
 
+ModelOutputConfigurationUnionTypeDef = Union[
+    ModelOutputConfigurationTypeDef, ModelOutputConfigurationOutputTypeDef
+]
 _RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
     "_RequiredPutExternalModelRequestRequestTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
         "invokeModelEndpointRoleArn": str,
         "inputConfiguration": ModelInputConfigurationTypeDef,
@@ -2255,14 +2234,42 @@
     {
         "variableImpactExplanations": List[VariableImpactExplanationTypeDef],
         "aggregatedVariablesImpactExplanations": List[AggregatedVariablesImpactExplanationTypeDef],
     },
     total=False,
 )
 
+_RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
+    "_RequiredGetEventPredictionRequestRequestTypeDef",
+    {
+        "detectorId": str,
+        "eventId": str,
+        "eventTypeName": str,
+        "entities": Sequence[EntityTypeDef],
+        "eventTimestamp": str,
+        "eventVariables": Mapping[str, str],
+    },
+)
+_OptionalGetEventPredictionRequestRequestTypeDef = TypedDict(
+    "_OptionalGetEventPredictionRequestRequestTypeDef",
+    {
+        "detectorVersionId": str,
+        "externalModelEndpointDataBlobs": Mapping[str, ModelEndpointDataBlobTypeDef],
+    },
+    total=False,
+)
+
+
+class GetEventPredictionRequestRequestTypeDef(
+    _RequiredGetEventPredictionRequestRequestTypeDef,
+    _OptionalGetEventPredictionRequestRequestTypeDef,
+):
+    pass
+
+
 GetEventResultTypeDef = TypedDict(
     "GetEventResultTypeDef",
     {
         "event": EventTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2360,14 +2367,15 @@
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
 
+TrainingDataSchemaUnionTypeDef = Union[TrainingDataSchemaTypeDef, TrainingDataSchemaOutputTypeDef]
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
         "trainingMetrics": TrainingMetricsTypeDef,
         "variableImportanceMetrics": VariableImportanceMetricsTypeDef,
     },
```

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/type_defs.pyi` & `mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_frauddetector.type_defs import ATIMetricDataPointTypeDef
 
-    data: ATIMetricDataPointTypeDef = {...}
+    data: ATIMetricDataPointTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -53,14 +53,15 @@
     "VariableEntryTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetVariableErrorTypeDef",
     "BatchGetVariableRequestRequestTypeDef",
     "VariableTypeDef",
     "BatchImportTypeDef",
     "BatchPredictionTypeDef",
+    "BlobTypeDef",
     "CancelBatchImportJobRequestRequestTypeDef",
     "CancelBatchPredictionJobRequestRequestTypeDef",
     "ModelVersionTypeDef",
     "RuleTypeDef",
     "ExternalEventsDetailTypeDef",
     "FieldValidationMessageTypeDef",
     "FileValidationMessageTypeDef",
@@ -98,15 +99,14 @@
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
     "GetEventPredictionMetadataRequestRequestTypeDef",
-    "ModelEndpointDataBlobTypeDef",
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
     "GetExternalModelsRequestRequestTypeDef",
     "KMSKeyTypeDef",
     "GetLabelsRequestRequestTypeDef",
     "LabelTypeDef",
@@ -164,14 +164,15 @@
     "GetListsMetadataResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "UpdateModelVersionResultTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
+    "ModelEndpointDataBlobTypeDef",
     "ModelScoresTypeDef",
     "CreateDetectorVersionRequestRequestTypeDef",
     "CreateRuleResultTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "GetDetectorVersionResultTypeDef",
     "UpdateDetectorVersionRequestRequestTypeDef",
     "UpdateRuleMetadataRequestRequestTypeDef",
@@ -184,37 +185,39 @@
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
-    "GetEventPredictionRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
     "GetLabelsResultTypeDef",
     "GetModelsResultTypeDef",
     "GetOutcomesResultTypeDef",
     "GetRulesResultTypeDef",
     "IngestedEventsDetailTypeDef",
     "TrainingDataSchemaOutputTypeDef",
     "TrainingDataSchemaTypeDef",
     "ListEventPredictionsRequestRequestTypeDef",
     "VariableImportanceMetricsTypeDef",
     "TrainingMetricsTypeDef",
+    "ModelOutputConfigurationUnionTypeDef",
     "PutExternalModelRequestRequestTypeDef",
     "OFIModelPerformanceTypeDef",
     "TFIModelPerformanceTypeDef",
     "PredictionExplanationsTypeDef",
+    "GetEventPredictionRequestRequestTypeDef",
     "GetEventResultTypeDef",
     "GetEventTypesResultTypeDef",
     "GetEventPredictionResultTypeDef",
     "GetExternalModelsResultTypeDef",
     "UpdateModelVersionRequestRequestTypeDef",
     "GetModelVersionResultTypeDef",
     "CreateModelVersionRequestRequestTypeDef",
+    "TrainingDataSchemaUnionTypeDef",
     "TrainingResultTypeDef",
     "OFITrainingMetricsValueTypeDef",
     "TFITrainingMetricsValueTypeDef",
     "ModelVersionEvaluationTypeDef",
     "TrainingMetricsV2TypeDef",
     "EvaluatedModelVersionTypeDef",
     "TrainingResultV2TypeDef",
@@ -394,14 +397,15 @@
         "arn": str,
         "processedRecordsCount": int,
         "totalRecordsCount": int,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelBatchImportJobRequestRequestTypeDef = TypedDict(
     "CancelBatchImportJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -856,23 +860,14 @@
         "eventTypeName": str,
         "detectorId": str,
         "detectorVersionId": str,
         "predictionTimestamp": str,
     },
 )
 
-ModelEndpointDataBlobTypeDef = TypedDict(
-    "ModelEndpointDataBlobTypeDef",
-    {
-        "byteBuffer": Union[str, bytes, IO[Any], StreamingBody],
-        "contentType": str,
-    },
-    total=False,
-)
-
 RuleResultTypeDef = TypedDict(
     "RuleResultTypeDef",
     {
         "ruleId": str,
         "outcomes": List[str],
     },
     total=False,
@@ -1707,14 +1702,23 @@
     {
         "batchPredictions": List[BatchPredictionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ModelEndpointDataBlobTypeDef = TypedDict(
+    "ModelEndpointDataBlobTypeDef",
+    {
+        "byteBuffer": BlobTypeDef,
+        "contentType": str,
+    },
+    total=False,
+)
+
 ModelScoresTypeDef = TypedDict(
     "ModelScoresTypeDef",
     {
         "modelVersion": ModelVersionTypeDef,
         "scores": Dict[str, float],
     },
     total=False,
@@ -1991,40 +1995,14 @@
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
-_RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
-    "_RequiredGetEventPredictionRequestRequestTypeDef",
-    {
-        "detectorId": str,
-        "eventId": str,
-        "eventTypeName": str,
-        "entities": Sequence[EntityTypeDef],
-        "eventTimestamp": str,
-        "eventVariables": Mapping[str, str],
-    },
-)
-_OptionalGetEventPredictionRequestRequestTypeDef = TypedDict(
-    "_OptionalGetEventPredictionRequestRequestTypeDef",
-    {
-        "detectorVersionId": str,
-        "externalModelEndpointDataBlobs": Mapping[str, ModelEndpointDataBlobTypeDef],
-    },
-    total=False,
-)
-
-class GetEventPredictionRequestRequestTypeDef(
-    _RequiredGetEventPredictionRequestRequestTypeDef,
-    _OptionalGetEventPredictionRequestRequestTypeDef,
-):
-    pass
-
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2137,14 +2115,17 @@
     {
         "auc": float,
         "metricDataPoints": List[MetricDataPointTypeDef],
     },
     total=False,
 )
 
+ModelOutputConfigurationUnionTypeDef = Union[
+    ModelOutputConfigurationTypeDef, ModelOutputConfigurationOutputTypeDef
+]
 _RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
     "_RequiredPutExternalModelRequestRequestTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
         "invokeModelEndpointRoleArn": str,
         "inputConfiguration": ModelInputConfigurationTypeDef,
@@ -2188,14 +2169,40 @@
     {
         "variableImpactExplanations": List[VariableImpactExplanationTypeDef],
         "aggregatedVariablesImpactExplanations": List[AggregatedVariablesImpactExplanationTypeDef],
     },
     total=False,
 )
 
+_RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
+    "_RequiredGetEventPredictionRequestRequestTypeDef",
+    {
+        "detectorId": str,
+        "eventId": str,
+        "eventTypeName": str,
+        "entities": Sequence[EntityTypeDef],
+        "eventTimestamp": str,
+        "eventVariables": Mapping[str, str],
+    },
+)
+_OptionalGetEventPredictionRequestRequestTypeDef = TypedDict(
+    "_OptionalGetEventPredictionRequestRequestTypeDef",
+    {
+        "detectorVersionId": str,
+        "externalModelEndpointDataBlobs": Mapping[str, ModelEndpointDataBlobTypeDef],
+    },
+    total=False,
+)
+
+class GetEventPredictionRequestRequestTypeDef(
+    _RequiredGetEventPredictionRequestRequestTypeDef,
+    _OptionalGetEventPredictionRequestRequestTypeDef,
+):
+    pass
+
 GetEventResultTypeDef = TypedDict(
     "GetEventResultTypeDef",
     {
         "event": EventTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2289,14 +2296,15 @@
 
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
+TrainingDataSchemaUnionTypeDef = Union[TrainingDataSchemaTypeDef, TrainingDataSchemaOutputTypeDef]
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
         "trainingMetrics": TrainingMetricsTypeDef,
         "variableImportanceMetrics": VariableImportanceMetricsTypeDef,
     },
```

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/PKG-INFO` & `mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.FraudDetector 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 frauddetector type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 frauddetector type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-frauddetector)](https://pepy.tech/project/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -303,20 +303,20 @@
 )
 
 
 def check_value(value: AsyncJobStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_frauddetector.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_frauddetector.type_defs import (
     ATIMetricDataPointTypeDef,
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
@@ -326,14 +326,15 @@
     VariableEntryTypeDef,
     ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
     BatchImportTypeDef,
     BatchPredictionTypeDef,
+    BlobTypeDef,
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
     ExternalEventsDetailTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
@@ -371,15 +372,14 @@
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
-    ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
@@ -437,14 +437,15 @@
     GetListsMetadataResultTypeDef,
     ListTagsForResourceResultTypeDef,
     UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
+    ModelEndpointDataBlobTypeDef,
     ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
     CreateRuleResultTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetDetectorVersionResultTypeDef,
     UpdateDetectorVersionRequestRequestTypeDef,
     UpdateRuleMetadataRequestRequestTypeDef,
@@ -457,51 +458,53 @@
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
     PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
-    GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
     GetModelsResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
     IngestedEventsDetailTypeDef,
     TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     ListEventPredictionsRequestRequestTypeDef,
     VariableImportanceMetricsTypeDef,
     TrainingMetricsTypeDef,
+    ModelOutputConfigurationUnionTypeDef,
     PutExternalModelRequestRequestTypeDef,
     OFIModelPerformanceTypeDef,
     TFIModelPerformanceTypeDef,
     PredictionExplanationsTypeDef,
+    GetEventPredictionRequestRequestTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
     GetEventPredictionResultTypeDef,
     GetExternalModelsResultTypeDef,
     UpdateModelVersionRequestRequestTypeDef,
     GetModelVersionResultTypeDef,
     CreateModelVersionRequestRequestTypeDef,
+    TrainingDataSchemaUnionTypeDef,
     TrainingResultTypeDef,
     OFITrainingMetricsValueTypeDef,
     TFITrainingMetricsValueTypeDef,
     ModelVersionEvaluationTypeDef,
     TrainingMetricsV2TypeDef,
     EvaluatedModelVersionTypeDef,
     TrainingResultV2TypeDef,
     GetEventPredictionMetadataResultTypeDef,
     ModelVersionDetailTypeDef,
     DescribeModelVersionsResultTypeDef,
 )
 
 
-def get_structure() -> ATIMetricDataPointTypeDef:
+def get_value() -> ATIMetricDataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/SOURCES.txt` & `mypy-boto3-frauddetector-1.28.16/mypy_boto3_frauddetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15.post1/setup.py` & `mypy-boto3-frauddetector-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-frauddetector",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_frauddetector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.FraudDetector 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 frauddetector type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 frauddetector type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_frauddetector": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

