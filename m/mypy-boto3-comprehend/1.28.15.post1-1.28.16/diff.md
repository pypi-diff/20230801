# Comparing `tmp/mypy-boto3-comprehend-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-comprehend-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehend-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:50 2023, max compression
+gzip compressed data, was "mypy-boto3-comprehend-1.28.16.tar", last modified: Tue Aug  1 11:36:31 2023, max compression
```

## Comparing `mypy-boto3-comprehend-1.28.15.post1.tar` & `mypy-boto3-comprehend-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:50.581084 mypy-boto3-comprehend-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28048 2023-07-29 10:02:50.581084 mypy-boto3-comprehend-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:50.569084 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68388 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68287 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-07-29 09:41:10.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-07-29 09:41:10.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-07-29 09:41:10.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   104121 2023-07-29 09:41:14.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   104032 2023-07-29 09:41:11.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:50.581084 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28048 2023-07-29 10:02:50.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:02:50.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:50.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:50.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:50.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:50.000000 mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:50.581084 mypy-boto3-comprehend-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:41:09.000000 mypy-boto3-comprehend-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:31.712919 mypy-boto3-comprehend-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28372 2023-08-01 11:36:31.712919 mypy-boto3-comprehend-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:31.712919 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67151 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67050 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-08-01 11:13:42.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-08-01 11:13:42.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   105220 2023-08-01 11:13:46.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105131 2023-08-01 11:13:44.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:31.712919 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28372 2023-08-01 11:36:31.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:36:31.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:31.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:31.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:31.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:31.000000 mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:31.712919 mypy-boto3-comprehend-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:13:41.000000 mypy-boto3-comprehend-1.28.16/setup.py
```

### Comparing `mypy-boto3-comprehend-1.28.15.post1/LICENSE` & `mypy-boto3-comprehend-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.15.post1/PKG-INFO` & `mypy-boto3-comprehend-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehend
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Comprehend 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Comprehend 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 comprehend type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 comprehend type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehend)](https://pepy.tech/project/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
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
@@ -389,20 +389,20 @@
 )
 
 
 def check_value(value: AugmentedManifestsDocumentTypeFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_comprehend.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_comprehend.type_defs import (
     AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
@@ -411,14 +411,15 @@
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
+    BlobTypeDef,
     ChildBlockTypeDef,
     RelationshipsListItemTypeDef,
     BoundingBoxTypeDef,
     ClassifierEvaluationMetricsTypeDef,
     DocumentReaderConfigTypeDef,
     DocumentClassTypeDef,
     DocumentLabelTypeDef,
@@ -432,15 +433,15 @@
     VpcConfigTypeDef,
     VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
-    DatasetFilterTypeDef,
+    TimestampTypeDef,
     DatasetPropertiesTypeDef,
     DeleteDocumentClassifierRequestRequestTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEntityRecognizerRequestRequestTypeDef,
     DeleteFlywheelRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
@@ -465,48 +466,34 @@
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
     DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
-    DocumentClassificationJobFilterTypeDef,
     OutputDataConfigTypeDef,
     DocumentClassifierDocumentsTypeDef,
-    DocumentClassifierFilterTypeDef,
     DocumentReaderConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
-    DominantLanguageDetectionJobFilterTypeDef,
-    EndpointFilterTypeDef,
-    EntitiesDetectionJobFilterTypeDef,
     EntityTypesListItemTypeDef,
     EntityRecognizerAnnotationsTypeDef,
     EntityRecognizerDocumentsTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
-    EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
-    EventsDetectionJobFilterTypeDef,
-    FlywheelFilterTypeDef,
-    FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
-    KeyPhrasesDetectionJobFilterTypeDef,
     PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
-    PiiEntitiesDetectionJobFilterTypeDef,
-    SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TargetedSentimentDetectionJobFilterTypeDef,
-    TopicsDetectionJobFilterTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
     RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RedactionConfigTypeDef,
     StartFlywheelIterationRequestRequestTypeDef,
     StopDominantLanguageDetectionJobRequestRequestTypeDef,
@@ -562,60 +549,53 @@
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
     DataSecurityConfigOutputTypeDef,
+    VpcConfigUnionTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
-    ListDatasetsRequestRequestTypeDef,
+    DatasetFilterTypeDef,
+    DocumentClassificationJobFilterTypeDef,
+    DocumentClassifierFilterTypeDef,
+    DominantLanguageDetectionJobFilterTypeDef,
+    EndpointFilterTypeDef,
+    EntitiesDetectionJobFilterTypeDef,
+    EntityRecognizerFilterTypeDef,
+    EventsDetectionJobFilterTypeDef,
+    FlywheelFilterTypeDef,
+    FlywheelIterationFilterTypeDef,
+    KeyPhrasesDetectionJobFilterTypeDef,
+    PiiEntitiesDetectionJobFilterTypeDef,
+    SentimentDetectionJobFilterTypeDef,
+    TargetedSentimentDetectionJobFilterTypeDef,
+    TopicsDetectionJobFilterTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
-    ListDocumentClassificationJobsRequestRequestTypeDef,
     DocumentClassifierInputDataConfigTypeDef,
-    ListDocumentClassifiersRequestRequestTypeDef,
     DocumentClassifierInputDataConfigOutputTypeDef,
+    DocumentReaderConfigUnionTypeDef,
     InputDataConfigOutputTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
-    ListDominantLanguageDetectionJobsRequestRequestTypeDef,
-    ListEndpointsRequestRequestTypeDef,
-    ListEntitiesDetectionJobsRequestRequestTypeDef,
     EntityRecognitionConfigOutputTypeDef,
     EntityRecognitionConfigTypeDef,
     EntityRecognizerInputDataConfigOutputTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
-    ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
-    ListEventsDetectionJobsRequestRequestTypeDef,
-    ListFlywheelsRequestRequestTypeDef,
-    ListFlywheelIterationHistoryRequestRequestTypeDef,
     FlywheelIterationPropertiesTypeDef,
     ListFlywheelsResponseTypeDef,
     GeometryTypeDef,
-    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
-    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
-    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
-    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
-    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
-    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
-    ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
-    ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
-    ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
-    ListSentimentDetectionJobsRequestRequestTypeDef,
-    ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
-    ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
-    ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
+    RedactionConfigUnionTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     TargetedSentimentMentionTypeDef,
     EntityTypeDef,
     StartDocumentClassificationJobRequestRequestTypeDef,
     StartDominantLanguageDetectionJobRequestRequestTypeDef,
@@ -623,30 +603,59 @@
     StartEventsDetectionJobRequestRequestTypeDef,
     StartKeyPhrasesDetectionJobRequestRequestTypeDef,
     StartPiiEntitiesDetectionJobRequestRequestTypeDef,
     StartSentimentDetectionJobRequestRequestTypeDef,
     StartTargetedSentimentDetectionJobRequestRequestTypeDef,
     StartTopicsDetectionJobRequestRequestTypeDef,
     UpdateFlywheelRequestRequestTypeDef,
+    DataSecurityConfigUnionTypeDef,
     DatasetInputDataConfigTypeDef,
+    ListDatasetsRequestRequestTypeDef,
+    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
+    ListDocumentClassificationJobsRequestRequestTypeDef,
+    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
+    ListDocumentClassifiersRequestRequestTypeDef,
+    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
+    ListDominantLanguageDetectionJobsRequestRequestTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    ListEndpointsRequestRequestTypeDef,
+    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
+    ListEntitiesDetectionJobsRequestRequestTypeDef,
+    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
+    ListEntityRecognizersRequestRequestTypeDef,
+    ListEventsDetectionJobsRequestRequestTypeDef,
+    ListFlywheelsRequestRequestTypeDef,
+    ListFlywheelIterationHistoryRequestRequestTypeDef,
+    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
+    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
+    ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
+    ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
+    ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
+    ListSentimentDetectionJobsRequestRequestTypeDef,
+    ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
+    ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
+    ListTopicsDetectionJobsRequestRequestTypeDef,
     CreateDocumentClassifierRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
     DocumentClassifierPropertiesTypeDef,
     DocumentClassificationJobPropertiesTypeDef,
     DominantLanguageDetectionJobPropertiesTypeDef,
     EntitiesDetectionJobPropertiesTypeDef,
     EventsDetectionJobPropertiesTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobPropertiesTypeDef,
     PiiEntitiesDetectionJobPropertiesTypeDef,
     SentimentDetectionJobPropertiesTypeDef,
     TargetedSentimentDetectionJobPropertiesTypeDef,
     TopicsDetectionJobPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
     TaskConfigOutputTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
@@ -670,29 +679,30 @@
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     FlywheelPropertiesTypeDef,
     CreateFlywheelRequestRequestTypeDef,
+    TaskConfigUnionTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     DescribeFlywheelResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
     DescribeEntityRecognizerResponseTypeDef,
     ListEntityRecognizersResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
 )
 
 
-def get_structure() -> AugmentedManifestsListItemOutputTypeDef:
+def get_value() -> AugmentedManifestsListItemOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-comprehend-1.28.15.post1/README.md` & `mypy-boto3-comprehend-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehend)](https://pepy.tech/project/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
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
@@ -357,20 +357,20 @@
 )
 
 
 def check_value(value: AugmentedManifestsDocumentTypeFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_comprehend.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_comprehend.type_defs import (
     AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
@@ -379,14 +379,15 @@
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
+    BlobTypeDef,
     ChildBlockTypeDef,
     RelationshipsListItemTypeDef,
     BoundingBoxTypeDef,
     ClassifierEvaluationMetricsTypeDef,
     DocumentReaderConfigTypeDef,
     DocumentClassTypeDef,
     DocumentLabelTypeDef,
@@ -400,15 +401,15 @@
     VpcConfigTypeDef,
     VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
-    DatasetFilterTypeDef,
+    TimestampTypeDef,
     DatasetPropertiesTypeDef,
     DeleteDocumentClassifierRequestRequestTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEntityRecognizerRequestRequestTypeDef,
     DeleteFlywheelRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
@@ -433,48 +434,34 @@
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
     DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
-    DocumentClassificationJobFilterTypeDef,
     OutputDataConfigTypeDef,
     DocumentClassifierDocumentsTypeDef,
-    DocumentClassifierFilterTypeDef,
     DocumentReaderConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
-    DominantLanguageDetectionJobFilterTypeDef,
-    EndpointFilterTypeDef,
-    EntitiesDetectionJobFilterTypeDef,
     EntityTypesListItemTypeDef,
     EntityRecognizerAnnotationsTypeDef,
     EntityRecognizerDocumentsTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
-    EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
-    EventsDetectionJobFilterTypeDef,
-    FlywheelFilterTypeDef,
-    FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
-    KeyPhrasesDetectionJobFilterTypeDef,
     PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
-    PiiEntitiesDetectionJobFilterTypeDef,
-    SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TargetedSentimentDetectionJobFilterTypeDef,
-    TopicsDetectionJobFilterTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
     RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RedactionConfigTypeDef,
     StartFlywheelIterationRequestRequestTypeDef,
     StopDominantLanguageDetectionJobRequestRequestTypeDef,
@@ -530,60 +517,53 @@
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
     DataSecurityConfigOutputTypeDef,
+    VpcConfigUnionTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
-    ListDatasetsRequestRequestTypeDef,
+    DatasetFilterTypeDef,
+    DocumentClassificationJobFilterTypeDef,
+    DocumentClassifierFilterTypeDef,
+    DominantLanguageDetectionJobFilterTypeDef,
+    EndpointFilterTypeDef,
+    EntitiesDetectionJobFilterTypeDef,
+    EntityRecognizerFilterTypeDef,
+    EventsDetectionJobFilterTypeDef,
+    FlywheelFilterTypeDef,
+    FlywheelIterationFilterTypeDef,
+    KeyPhrasesDetectionJobFilterTypeDef,
+    PiiEntitiesDetectionJobFilterTypeDef,
+    SentimentDetectionJobFilterTypeDef,
+    TargetedSentimentDetectionJobFilterTypeDef,
+    TopicsDetectionJobFilterTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
-    ListDocumentClassificationJobsRequestRequestTypeDef,
     DocumentClassifierInputDataConfigTypeDef,
-    ListDocumentClassifiersRequestRequestTypeDef,
     DocumentClassifierInputDataConfigOutputTypeDef,
+    DocumentReaderConfigUnionTypeDef,
     InputDataConfigOutputTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
-    ListDominantLanguageDetectionJobsRequestRequestTypeDef,
-    ListEndpointsRequestRequestTypeDef,
-    ListEntitiesDetectionJobsRequestRequestTypeDef,
     EntityRecognitionConfigOutputTypeDef,
     EntityRecognitionConfigTypeDef,
     EntityRecognizerInputDataConfigOutputTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
-    ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
-    ListEventsDetectionJobsRequestRequestTypeDef,
-    ListFlywheelsRequestRequestTypeDef,
-    ListFlywheelIterationHistoryRequestRequestTypeDef,
     FlywheelIterationPropertiesTypeDef,
     ListFlywheelsResponseTypeDef,
     GeometryTypeDef,
-    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
-    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
-    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
-    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
-    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
-    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
-    ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
-    ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
-    ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
-    ListSentimentDetectionJobsRequestRequestTypeDef,
-    ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
-    ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
-    ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
+    RedactionConfigUnionTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     TargetedSentimentMentionTypeDef,
     EntityTypeDef,
     StartDocumentClassificationJobRequestRequestTypeDef,
     StartDominantLanguageDetectionJobRequestRequestTypeDef,
@@ -591,30 +571,59 @@
     StartEventsDetectionJobRequestRequestTypeDef,
     StartKeyPhrasesDetectionJobRequestRequestTypeDef,
     StartPiiEntitiesDetectionJobRequestRequestTypeDef,
     StartSentimentDetectionJobRequestRequestTypeDef,
     StartTargetedSentimentDetectionJobRequestRequestTypeDef,
     StartTopicsDetectionJobRequestRequestTypeDef,
     UpdateFlywheelRequestRequestTypeDef,
+    DataSecurityConfigUnionTypeDef,
     DatasetInputDataConfigTypeDef,
+    ListDatasetsRequestRequestTypeDef,
+    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
+    ListDocumentClassificationJobsRequestRequestTypeDef,
+    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
+    ListDocumentClassifiersRequestRequestTypeDef,
+    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
+    ListDominantLanguageDetectionJobsRequestRequestTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    ListEndpointsRequestRequestTypeDef,
+    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
+    ListEntitiesDetectionJobsRequestRequestTypeDef,
+    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
+    ListEntityRecognizersRequestRequestTypeDef,
+    ListEventsDetectionJobsRequestRequestTypeDef,
+    ListFlywheelsRequestRequestTypeDef,
+    ListFlywheelIterationHistoryRequestRequestTypeDef,
+    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
+    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
+    ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
+    ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
+    ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
+    ListSentimentDetectionJobsRequestRequestTypeDef,
+    ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
+    ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
+    ListTopicsDetectionJobsRequestRequestTypeDef,
     CreateDocumentClassifierRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
     DocumentClassifierPropertiesTypeDef,
     DocumentClassificationJobPropertiesTypeDef,
     DominantLanguageDetectionJobPropertiesTypeDef,
     EntitiesDetectionJobPropertiesTypeDef,
     EventsDetectionJobPropertiesTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobPropertiesTypeDef,
     PiiEntitiesDetectionJobPropertiesTypeDef,
     SentimentDetectionJobPropertiesTypeDef,
     TargetedSentimentDetectionJobPropertiesTypeDef,
     TopicsDetectionJobPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
     TaskConfigOutputTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
@@ -638,29 +647,30 @@
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     FlywheelPropertiesTypeDef,
     CreateFlywheelRequestRequestTypeDef,
+    TaskConfigUnionTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     DescribeFlywheelResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
     DescribeEntityRecognizerResponseTypeDef,
     ListEntityRecognizersResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
 )
 
 
-def get_structure() -> AugmentedManifestsListItemOutputTypeDef:
+def get_value() -> AugmentedManifestsListItemOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/__init__.py` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/__init__.pyi` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/__main__.py` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Comprehend 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Comprehend 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend\nOther"
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

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/client.py` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_comprehend.client import ComprehendClient
 
     session = Session()
     client: ComprehendClient = session.client("comprehend")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     DatasetTypeType,
     DocumentClassifierModeType,
     LanguageCodeType,
     ModelTypeType,
     PiiEntitiesDetectionModeType,
@@ -42,23 +41,23 @@
 from .type_defs import (
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
+    BlobTypeDef,
     ClassifyDocumentResponseTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDocumentClassifierResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEntityRecognizerResponseTypeDef,
     CreateFlywheelResponseTypeDef,
-    DataSecurityConfigOutputTypeDef,
-    DataSecurityConfigTypeDef,
+    DataSecurityConfigUnionTypeDef,
     DatasetFilterTypeDef,
     DatasetInputDataConfigTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     DescribeDocumentClassifierResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     DescribeEndpointResponseTypeDef,
@@ -78,31 +77,27 @@
     DetectKeyPhrasesResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
     DetectSentimentResponseTypeDef,
     DetectSyntaxResponseTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     DocumentClassificationJobFilterTypeDef,
     DocumentClassifierFilterTypeDef,
-    DocumentClassifierInputDataConfigOutputTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
-    DocumentReaderConfigOutputTypeDef,
-    DocumentReaderConfigTypeDef,
+    DocumentReaderConfigUnionTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
     EntityRecognizerFilterTypeDef,
-    EntityRecognizerInputDataConfigOutputTypeDef,
-    EntityRecognizerInputDataConfigTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     ImportModelResponseTypeDef,
-    InputDataConfigOutputTypeDef,
-    InputDataConfigTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
     ListDatasetsResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     ListDocumentClassifiersResponseTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     ListEndpointsResponseTypeDef,
@@ -117,16 +112,15 @@
     ListSentimentDetectionJobsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     OutputDataConfigTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     PutResourcePolicyResponseTypeDef,
-    RedactionConfigOutputTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigUnionTypeDef,
     SentimentDetectionJobFilterTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
@@ -139,22 +133,20 @@
     StopEventsDetectionJobResponseTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
     TagTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
-    TaskConfigOutputTypeDef,
-    TaskConfigTypeDef,
+    TaskConfigUnionTypeDef,
     TopicsDetectionJobFilterTypeDef,
     UpdateDataSecurityConfigTypeDef,
     UpdateEndpointResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -280,18 +272,16 @@
         """
 
     def classify_document(
         self,
         *,
         EndpointArn: str,
         Text: str = ...,
-        Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        DocumentReaderConfig: Union[
-            DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
-        ] = ...
+        Bytes: BlobTypeDef = ...,
+        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
     ) -> ClassifyDocumentResponseTypeDef:
         """
         Creates a new document classification request to analyze a single document in
         real-time, using a previously created and trained custom model and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.classify_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#classify_document)
@@ -337,24 +327,22 @@
         """
 
     def create_document_classifier(
         self,
         *,
         DocumentClassifierName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: Union[
-            DocumentClassifierInputDataConfigTypeDef, DocumentClassifierInputDataConfigOutputTypeDef
-        ],
+        InputDataConfig: DocumentClassifierInputDataConfigUnionTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OutputDataConfig: DocumentClassifierOutputDataConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Mode: DocumentClassifierModeType = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateDocumentClassifierResponseTypeDef:
         """
         Creates a new document classifier that you can use to categorize documents.
 
@@ -384,23 +372,21 @@
         """
 
     def create_entity_recognizer(
         self,
         *,
         RecognizerName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: Union[
-            EntityRecognizerInputDataConfigTypeDef, EntityRecognizerInputDataConfigOutputTypeDef
-        ],
+        InputDataConfig: EntityRecognizerInputDataConfigUnionTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateEntityRecognizerResponseTypeDef:
         """
         Creates an entity recognizer using submitted files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_entity_recognizer)
@@ -410,17 +396,17 @@
     def create_flywheel(
         self,
         *,
         FlywheelName: str,
         DataAccessRoleArn: str,
         DataLakeS3Uri: str,
         ActiveModelArn: str = ...,
-        TaskConfig: Union[TaskConfigTypeDef, TaskConfigOutputTypeDef] = ...,
+        TaskConfig: TaskConfigUnionTypeDef = ...,
         ModelType: ModelTypeType = ...,
-        DataSecurityConfig: Union[DataSecurityConfigTypeDef, DataSecurityConfigOutputTypeDef] = ...,
+        DataSecurityConfig: DataSecurityConfigUnionTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlywheelResponseTypeDef:
         """
         A flywheel is an Amazon Web Services resource that orchestrates the ongoing
         training of a model for custom classification or custom entity recognition.
 
@@ -637,18 +623,16 @@
 
     def detect_entities(
         self,
         *,
         Text: str = ...,
         LanguageCode: LanguageCodeType = ...,
         EndpointArn: str = ...,
-        Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        DocumentReaderConfig: Union[
-            DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
-        ] = ...
+        Bytes: BlobTypeDef = ...,
+        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
     ) -> DetectEntitiesResponseTypeDef:
         """
         Detects named entities in input text when you use the pre-trained model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#detect_entities)
         """
@@ -982,78 +966,78 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#put_resource_policy)
         """
 
     def start_document_classification_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         DocumentClassifierArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartDocumentClassificationJobResponseTypeDef:
         """
         Starts an asynchronous document classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_document_classification_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_document_classification_job)
         """
 
     def start_dominant_language_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartDominantLanguageDetectionJobResponseTypeDef:
         """
         Starts an asynchronous dominant language detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_dominant_language_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_dominant_language_detection_job)
         """
 
     def start_entities_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         EntityRecognizerArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_entities_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_entities_detection_job)
         """
 
     def start_events_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         TargetEventTypes: Sequence[str],
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
@@ -1075,103 +1059,103 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_flywheel_iteration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_flywheel_iteration)
         """
 
     def start_key_phrases_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartKeyPhrasesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous key phrase detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_key_phrases_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_key_phrases_detection_job)
         """
 
     def start_pii_entities_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         Mode: PiiEntitiesDetectionModeType,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
-        RedactionConfig: Union[RedactionConfigTypeDef, RedactionConfigOutputTypeDef] = ...,
+        RedactionConfig: RedactionConfigUnionTypeDef = ...,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartPiiEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous PII entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_pii_entities_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_pii_entities_detection_job)
         """
 
     def start_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous sentiment detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_sentiment_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_sentiment_detection_job)
         """
 
     def start_targeted_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTargetedSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous targeted sentiment detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_targeted_sentiment_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_targeted_sentiment_detection_job)
         """
 
     def start_topics_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         NumberOfTopics: int = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTopicsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_topics_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_topics_detection_job)
```

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/client.pyi` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_comprehend.client import ComprehendClient
 
     session = Session()
     client: ComprehendClient = session.client("comprehend")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     DatasetTypeType,
     DocumentClassifierModeType,
     LanguageCodeType,
     ModelTypeType,
     PiiEntitiesDetectionModeType,
@@ -42,23 +41,23 @@
 from .type_defs import (
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
+    BlobTypeDef,
     ClassifyDocumentResponseTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDocumentClassifierResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEntityRecognizerResponseTypeDef,
     CreateFlywheelResponseTypeDef,
-    DataSecurityConfigOutputTypeDef,
-    DataSecurityConfigTypeDef,
+    DataSecurityConfigUnionTypeDef,
     DatasetFilterTypeDef,
     DatasetInputDataConfigTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     DescribeDocumentClassifierResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     DescribeEndpointResponseTypeDef,
@@ -78,31 +77,27 @@
     DetectKeyPhrasesResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
     DetectSentimentResponseTypeDef,
     DetectSyntaxResponseTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     DocumentClassificationJobFilterTypeDef,
     DocumentClassifierFilterTypeDef,
-    DocumentClassifierInputDataConfigOutputTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
-    DocumentReaderConfigOutputTypeDef,
-    DocumentReaderConfigTypeDef,
+    DocumentReaderConfigUnionTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
     EntityRecognizerFilterTypeDef,
-    EntityRecognizerInputDataConfigOutputTypeDef,
-    EntityRecognizerInputDataConfigTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     ImportModelResponseTypeDef,
-    InputDataConfigOutputTypeDef,
-    InputDataConfigTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
     ListDatasetsResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     ListDocumentClassifiersResponseTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     ListEndpointsResponseTypeDef,
@@ -117,16 +112,15 @@
     ListSentimentDetectionJobsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     OutputDataConfigTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     PutResourcePolicyResponseTypeDef,
-    RedactionConfigOutputTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigUnionTypeDef,
     SentimentDetectionJobFilterTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
@@ -139,22 +133,20 @@
     StopEventsDetectionJobResponseTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
     TagTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
-    TaskConfigOutputTypeDef,
-    TaskConfigTypeDef,
+    TaskConfigUnionTypeDef,
     TopicsDetectionJobFilterTypeDef,
     UpdateDataSecurityConfigTypeDef,
     UpdateEndpointResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -268,18 +260,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#can_paginate)
         """
     def classify_document(
         self,
         *,
         EndpointArn: str,
         Text: str = ...,
-        Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        DocumentReaderConfig: Union[
-            DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
-        ] = ...
+        Bytes: BlobTypeDef = ...,
+        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
     ) -> ClassifyDocumentResponseTypeDef:
         """
         Creates a new document classification request to analyze a single document in
         real-time, using a previously created and trained custom model and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.classify_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#classify_document)
@@ -321,24 +311,22 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#create_dataset)
         """
     def create_document_classifier(
         self,
         *,
         DocumentClassifierName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: Union[
-            DocumentClassifierInputDataConfigTypeDef, DocumentClassifierInputDataConfigOutputTypeDef
-        ],
+        InputDataConfig: DocumentClassifierInputDataConfigUnionTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OutputDataConfig: DocumentClassifierOutputDataConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Mode: DocumentClassifierModeType = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateDocumentClassifierResponseTypeDef:
         """
         Creates a new document classifier that you can use to categorize documents.
 
@@ -366,23 +354,21 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#create_endpoint)
         """
     def create_entity_recognizer(
         self,
         *,
         RecognizerName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: Union[
-            EntityRecognizerInputDataConfigTypeDef, EntityRecognizerInputDataConfigOutputTypeDef
-        ],
+        InputDataConfig: EntityRecognizerInputDataConfigUnionTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateEntityRecognizerResponseTypeDef:
         """
         Creates an entity recognizer using submitted files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_entity_recognizer)
@@ -391,17 +377,17 @@
     def create_flywheel(
         self,
         *,
         FlywheelName: str,
         DataAccessRoleArn: str,
         DataLakeS3Uri: str,
         ActiveModelArn: str = ...,
-        TaskConfig: Union[TaskConfigTypeDef, TaskConfigOutputTypeDef] = ...,
+        TaskConfig: TaskConfigUnionTypeDef = ...,
         ModelType: ModelTypeType = ...,
-        DataSecurityConfig: Union[DataSecurityConfigTypeDef, DataSecurityConfigOutputTypeDef] = ...,
+        DataSecurityConfig: DataSecurityConfigUnionTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlywheelResponseTypeDef:
         """
         A flywheel is an Amazon Web Services resource that orchestrates the ongoing
         training of a model for custom classification or custom entity recognition.
 
@@ -595,18 +581,16 @@
         """
     def detect_entities(
         self,
         *,
         Text: str = ...,
         LanguageCode: LanguageCodeType = ...,
         EndpointArn: str = ...,
-        Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        DocumentReaderConfig: Union[
-            DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
-        ] = ...
+        Bytes: BlobTypeDef = ...,
+        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
     ) -> DetectEntitiesResponseTypeDef:
         """
         Detects named entities in input text when you use the pre-trained model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#detect_entities)
         """
@@ -913,75 +897,75 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#put_resource_policy)
         """
     def start_document_classification_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         DocumentClassifierArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartDocumentClassificationJobResponseTypeDef:
         """
         Starts an asynchronous document classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_document_classification_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_document_classification_job)
         """
     def start_dominant_language_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartDominantLanguageDetectionJobResponseTypeDef:
         """
         Starts an asynchronous dominant language detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_dominant_language_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_dominant_language_detection_job)
         """
     def start_entities_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         EntityRecognizerArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_entities_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_entities_detection_job)
         """
     def start_events_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         TargetEventTypes: Sequence[str],
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
@@ -1001,99 +985,99 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_flywheel_iteration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_flywheel_iteration)
         """
     def start_key_phrases_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartKeyPhrasesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous key phrase detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_key_phrases_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_key_phrases_detection_job)
         """
     def start_pii_entities_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         Mode: PiiEntitiesDetectionModeType,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
-        RedactionConfig: Union[RedactionConfigTypeDef, RedactionConfigOutputTypeDef] = ...,
+        RedactionConfig: RedactionConfigUnionTypeDef = ...,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartPiiEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous PII entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_pii_entities_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_pii_entities_detection_job)
         """
     def start_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous sentiment detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_sentiment_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_sentiment_detection_job)
         """
     def start_targeted_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTargetedSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous targeted sentiment detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_targeted_sentiment_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_targeted_sentiment_detection_job)
         """
     def start_topics_detection_job(
         self,
         *,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         NumberOfTopics: int = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTopicsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_topics_detection_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#start_topics_detection_job)
```

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/literals.py` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/literals.pyi` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/paginator.py` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/paginator.pyi` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/type_defs.py` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_comprehend.type_defs import AugmentedManifestsListItemOutputTypeDef
 
-    data: AugmentedManifestsListItemOutputTypeDef = {...}
+    data: AugmentedManifestsListItemOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -57,29 +57,29 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
     "SentimentScoreTypeDef",
     "BatchDetectSentimentRequestRequestTypeDef",
     "BatchDetectSyntaxRequestRequestTypeDef",
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
+    "BlobTypeDef",
     "ChildBlockTypeDef",
     "RelationshipsListItemTypeDef",
     "BoundingBoxTypeDef",
     "ClassifierEvaluationMetricsTypeDef",
     "DocumentReaderConfigTypeDef",
     "DocumentClassTypeDef",
     "DocumentLabelTypeDef",
@@ -93,15 +93,15 @@
     "VpcConfigTypeDef",
     "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
-    "DatasetFilterTypeDef",
+    "TimestampTypeDef",
     "DatasetPropertiesTypeDef",
     "DeleteDocumentClassifierRequestRequestTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEntityRecognizerRequestRequestTypeDef",
     "DeleteFlywheelRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
@@ -126,48 +126,34 @@
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
     "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
-    "DocumentClassificationJobFilterTypeDef",
     "OutputDataConfigTypeDef",
     "DocumentClassifierDocumentsTypeDef",
-    "DocumentClassifierFilterTypeDef",
     "DocumentReaderConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
-    "DominantLanguageDetectionJobFilterTypeDef",
-    "EndpointFilterTypeDef",
-    "EntitiesDetectionJobFilterTypeDef",
     "EntityTypesListItemTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
     "EntityRecognizerDocumentsTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
-    "EntityRecognizerFilterTypeDef",
     "EntityTypesEvaluationMetricsTypeDef",
     "EntityRecognizerOutputDataConfigTypeDef",
     "EntityRecognizerSummaryTypeDef",
-    "EventsDetectionJobFilterTypeDef",
-    "FlywheelFilterTypeDef",
-    "FlywheelIterationFilterTypeDef",
     "FlywheelModelEvaluationMetricsTypeDef",
     "FlywheelSummaryTypeDef",
     "PointTypeDef",
-    "KeyPhrasesDetectionJobFilterTypeDef",
     "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
-    "PiiEntitiesDetectionJobFilterTypeDef",
-    "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TargetedSentimentDetectionJobFilterTypeDef",
-    "TopicsDetectionJobFilterTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
     "RedactionConfigOutputTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RedactionConfigTypeDef",
     "StartFlywheelIterationRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobRequestRequestTypeDef",
@@ -223,60 +209,53 @@
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
     "DataSecurityConfigOutputTypeDef",
+    "VpcConfigUnionTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
-    "ListDatasetsRequestRequestTypeDef",
+    "DatasetFilterTypeDef",
+    "DocumentClassificationJobFilterTypeDef",
+    "DocumentClassifierFilterTypeDef",
+    "DominantLanguageDetectionJobFilterTypeDef",
+    "EndpointFilterTypeDef",
+    "EntitiesDetectionJobFilterTypeDef",
+    "EntityRecognizerFilterTypeDef",
+    "EventsDetectionJobFilterTypeDef",
+    "FlywheelFilterTypeDef",
+    "FlywheelIterationFilterTypeDef",
+    "KeyPhrasesDetectionJobFilterTypeDef",
+    "PiiEntitiesDetectionJobFilterTypeDef",
+    "SentimentDetectionJobFilterTypeDef",
+    "TargetedSentimentDetectionJobFilterTypeDef",
+    "TopicsDetectionJobFilterTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
-    "ListDocumentClassificationJobsRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigTypeDef",
-    "ListDocumentClassifiersRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigOutputTypeDef",
+    "DocumentReaderConfigUnionTypeDef",
     "InputDataConfigOutputTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
-    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
-    "ListEndpointsRequestRequestTypeDef",
-    "ListEntitiesDetectionJobsRequestRequestTypeDef",
     "EntityRecognitionConfigOutputTypeDef",
     "EntityRecognitionConfigTypeDef",
     "EntityRecognizerInputDataConfigOutputTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
-    "ListEntityRecognizersRequestRequestTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
-    "ListEventsDetectionJobsRequestRequestTypeDef",
-    "ListFlywheelsRequestRequestTypeDef",
-    "ListFlywheelIterationHistoryRequestRequestTypeDef",
     "FlywheelIterationPropertiesTypeDef",
     "ListFlywheelsResponseTypeDef",
     "GeometryTypeDef",
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
-    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
-    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
-    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
-    "ListSentimentDetectionJobsRequestRequestTypeDef",
-    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
-    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
-    "ListTopicsDetectionJobsRequestRequestTypeDef",
     "SyntaxTokenTypeDef",
+    "RedactionConfigUnionTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
     "TargetedSentimentMentionTypeDef",
     "EntityTypeDef",
     "StartDocumentClassificationJobRequestRequestTypeDef",
     "StartDominantLanguageDetectionJobRequestRequestTypeDef",
@@ -284,30 +263,59 @@
     "StartEventsDetectionJobRequestRequestTypeDef",
     "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StartSentimentDetectionJobRequestRequestTypeDef",
     "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StartTopicsDetectionJobRequestRequestTypeDef",
     "UpdateFlywheelRequestRequestTypeDef",
+    "DataSecurityConfigUnionTypeDef",
     "DatasetInputDataConfigTypeDef",
+    "ListDatasetsRequestRequestTypeDef",
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    "ListDocumentClassificationJobsRequestRequestTypeDef",
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    "ListDocumentClassifiersRequestRequestTypeDef",
+    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    "ListEndpointsRequestRequestTypeDef",
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    "ListEntitiesDetectionJobsRequestRequestTypeDef",
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    "ListEntityRecognizersRequestRequestTypeDef",
+    "ListEventsDetectionJobsRequestRequestTypeDef",
+    "ListFlywheelsRequestRequestTypeDef",
+    "ListFlywheelIterationHistoryRequestRequestTypeDef",
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
+    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
+    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
+    "ListSentimentDetectionJobsRequestRequestTypeDef",
+    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
+    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
+    "ListTopicsDetectionJobsRequestRequestTypeDef",
     "CreateDocumentClassifierRequestRequestTypeDef",
+    "DocumentClassifierInputDataConfigUnionTypeDef",
     "DocumentClassifierPropertiesTypeDef",
     "DocumentClassificationJobPropertiesTypeDef",
     "DominantLanguageDetectionJobPropertiesTypeDef",
     "EntitiesDetectionJobPropertiesTypeDef",
     "EventsDetectionJobPropertiesTypeDef",
+    "InputDataConfigUnionTypeDef",
     "KeyPhrasesDetectionJobPropertiesTypeDef",
     "PiiEntitiesDetectionJobPropertiesTypeDef",
     "SentimentDetectionJobPropertiesTypeDef",
     "TargetedSentimentDetectionJobPropertiesTypeDef",
     "TopicsDetectionJobPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
     "TaskConfigOutputTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
+    "EntityRecognizerInputDataConfigUnionTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
@@ -331,14 +339,15 @@
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
     "FlywheelPropertiesTypeDef",
     "CreateFlywheelRequestRequestTypeDef",
+    "TaskConfigUnionTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
     "BatchDetectEntitiesResponseTypeDef",
     "DescribeFlywheelResponseTypeDef",
@@ -362,22 +371,20 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
-
 class AugmentedManifestsListItemOutputTypeDef(
     _RequiredAugmentedManifestsListItemOutputTypeDef,
     _OptionalAugmentedManifestsListItemOutputTypeDef,
 ):
     pass
 
-
 _RequiredAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredAugmentedManifestsListItemTypeDef",
     {
         "S3Uri": str,
         "AttributeNames": Sequence[str],
     },
 )
@@ -388,21 +395,19 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
-
 class AugmentedManifestsListItemTypeDef(
     _RequiredAugmentedManifestsListItemTypeDef, _OptionalAugmentedManifestsListItemTypeDef
 ):
     pass
 
-
 DominantLanguageTypeDef = TypedDict(
     "DominantLanguageTypeDef",
     {
         "LanguageCode": str,
         "Score": float,
     },
     total=False,
@@ -494,14 +499,15 @@
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChildBlockTypeDef = TypedDict(
     "ChildBlockTypeDef",
     {
         "ChildBlockId": str,
         "BeginOffset": int,
         "EndOffset": int,
     },
@@ -554,21 +560,19 @@
     {
         "DocumentReadMode": DocumentReadModeType,
         "FeatureTypes": Sequence[DocumentReadFeatureTypesType],
     },
     total=False,
 )
 
-
 class DocumentReaderConfigTypeDef(
     _RequiredDocumentReaderConfigTypeDef, _OptionalDocumentReaderConfigTypeDef
 ):
     pass
 
-
 DocumentClassTypeDef = TypedDict(
     "DocumentClassTypeDef",
     {
         "Name": str,
         "Score": float,
         "Page": int,
     },
@@ -641,19 +645,17 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 DocumentClassifierOutputDataConfigTypeDef = TypedDict(
     "DocumentClassifierOutputDataConfigTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
         "FlywheelStatsS3Prefix": str,
     },
@@ -689,44 +691,40 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
-
 class DatasetAugmentedManifestsListItemTypeDef(
     _RequiredDatasetAugmentedManifestsListItemTypeDef,
     _OptionalDatasetAugmentedManifestsListItemTypeDef,
 ):
     pass
 
-
 _RequiredDatasetDocumentClassifierInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetDocumentClassifierInputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalDatasetDocumentClassifierInputDataConfigTypeDef = TypedDict(
     "_OptionalDatasetDocumentClassifierInputDataConfigTypeDef",
     {
         "LabelDelimiter": str,
     },
     total=False,
 )
 
-
 class DatasetDocumentClassifierInputDataConfigTypeDef(
     _RequiredDatasetDocumentClassifierInputDataConfigTypeDef,
     _OptionalDatasetDocumentClassifierInputDataConfigTypeDef,
 ):
     pass
 
-
 DatasetEntityRecognizerAnnotationsTypeDef = TypedDict(
     "DatasetEntityRecognizerAnnotationsTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -740,40 +738,28 @@
     "_OptionalDatasetEntityRecognizerDocumentsTypeDef",
     {
         "InputFormat": InputFormatType,
     },
     total=False,
 )
 
-
 class DatasetEntityRecognizerDocumentsTypeDef(
     _RequiredDatasetEntityRecognizerDocumentsTypeDef,
     _OptionalDatasetEntityRecognizerDocumentsTypeDef,
 ):
     pass
 
-
 DatasetEntityRecognizerEntityListTypeDef = TypedDict(
     "DatasetEntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
-DatasetFilterTypeDef = TypedDict(
-    "DatasetFilterTypeDef",
-    {
-        "Status": DatasetStatusType,
-        "DatasetType": DatasetTypeType,
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DatasetPropertiesTypeDef = TypedDict(
     "DatasetPropertiesTypeDef",
     {
         "DatasetArn": str,
         "DatasetName": str,
         "DatasetType": DatasetTypeType,
         "DatasetS3Uri": str,
@@ -825,22 +811,20 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -1037,105 +1021,75 @@
     "_OptionalDocumentClassificationConfigOutputTypeDef",
     {
         "Labels": List[str],
     },
     total=False,
 )
 
-
 class DocumentClassificationConfigOutputTypeDef(
     _RequiredDocumentClassificationConfigOutputTypeDef,
     _OptionalDocumentClassificationConfigOutputTypeDef,
 ):
     pass
 
-
 _RequiredDocumentClassificationConfigTypeDef = TypedDict(
     "_RequiredDocumentClassificationConfigTypeDef",
     {
         "Mode": DocumentClassifierModeType,
     },
 )
 _OptionalDocumentClassificationConfigTypeDef = TypedDict(
     "_OptionalDocumentClassificationConfigTypeDef",
     {
         "Labels": Sequence[str],
     },
     total=False,
 )
 
-
 class DocumentClassificationConfigTypeDef(
     _RequiredDocumentClassificationConfigTypeDef, _OptionalDocumentClassificationConfigTypeDef
 ):
     pass
 
-
-DocumentClassificationJobFilterTypeDef = TypedDict(
-    "DocumentClassificationJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalOutputDataConfigTypeDef = TypedDict(
     "_OptionalOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-
 _RequiredDocumentClassifierDocumentsTypeDef = TypedDict(
     "_RequiredDocumentClassifierDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalDocumentClassifierDocumentsTypeDef = TypedDict(
     "_OptionalDocumentClassifierDocumentsTypeDef",
     {
         "TestS3Uri": str,
     },
     total=False,
 )
 
-
 class DocumentClassifierDocumentsTypeDef(
     _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
 ):
     pass
 
-
-DocumentClassifierFilterTypeDef = TypedDict(
-    "DocumentClassifierFilterTypeDef",
-    {
-        "Status": ModelStatusType,
-        "DocumentClassifierName": str,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredDocumentReaderConfigOutputTypeDef = TypedDict(
     "_RequiredDocumentReaderConfigOutputTypeDef",
     {
         "DocumentReadAction": DocumentReadActionType,
     },
 )
 _OptionalDocumentReaderConfigOutputTypeDef = TypedDict(
@@ -1143,21 +1097,19 @@
     {
         "DocumentReadMode": DocumentReadModeType,
         "FeatureTypes": List[DocumentReadFeatureTypesType],
     },
     total=False,
 )
 
-
 class DocumentReaderConfigOutputTypeDef(
     _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
 ):
     pass
 
-
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1171,47 +1123,14 @@
     {
         "Page": int,
         "Count": int,
     },
     total=False,
 )
 
-DominantLanguageDetectionJobFilterTypeDef = TypedDict(
-    "DominantLanguageDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-EndpointFilterTypeDef = TypedDict(
-    "EndpointFilterTypeDef",
-    {
-        "ModelArn": str,
-        "Status": EndpointStatusType,
-        "CreationTimeBefore": Union[datetime, str],
-        "CreationTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-EntitiesDetectionJobFilterTypeDef = TypedDict(
-    "EntitiesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 EntityTypesListItemTypeDef = TypedDict(
     "EntityTypesListItemTypeDef",
     {
         "Type": str,
     },
 )
 
@@ -1225,21 +1144,19 @@
     "_OptionalEntityRecognizerAnnotationsTypeDef",
     {
         "TestS3Uri": str,
     },
     total=False,
 )
 
-
 class EntityRecognizerAnnotationsTypeDef(
     _RequiredEntityRecognizerAnnotationsTypeDef, _OptionalEntityRecognizerAnnotationsTypeDef
 ):
     pass
 
-
 _RequiredEntityRecognizerDocumentsTypeDef = TypedDict(
     "_RequiredEntityRecognizerDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalEntityRecognizerDocumentsTypeDef = TypedDict(
@@ -1247,21 +1164,19 @@
     {
         "TestS3Uri": str,
         "InputFormat": InputFormatType,
     },
     total=False,
 )
 
-
 class EntityRecognizerDocumentsTypeDef(
     _RequiredEntityRecognizerDocumentsTypeDef, _OptionalEntityRecognizerDocumentsTypeDef
 ):
     pass
 
-
 EntityRecognizerEntityListTypeDef = TypedDict(
     "EntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -1271,25 +1186,14 @@
         "Precision": float,
         "Recall": float,
         "F1Score": float,
     },
     total=False,
 )
 
-EntityRecognizerFilterTypeDef = TypedDict(
-    "EntityRecognizerFilterTypeDef",
-    {
-        "Status": ModelStatusType,
-        "RecognizerName": str,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 EntityTypesEvaluationMetricsTypeDef = TypedDict(
     "EntityTypesEvaluationMetricsTypeDef",
     {
         "Precision": float,
         "Recall": float,
         "F1Score": float,
     },
@@ -1312,44 +1216,14 @@
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
         "LatestVersionStatus": ModelStatusType,
     },
     total=False,
 )
 
-EventsDetectionJobFilterTypeDef = TypedDict(
-    "EventsDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-FlywheelFilterTypeDef = TypedDict(
-    "FlywheelFilterTypeDef",
-    {
-        "Status": FlywheelStatusType,
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-FlywheelIterationFilterTypeDef = TypedDict(
-    "FlywheelIterationFilterTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 FlywheelModelEvaluationMetricsTypeDef = TypedDict(
     "FlywheelModelEvaluationMetricsTypeDef",
     {
         "AverageF1Score": float,
         "AveragePrecision": float,
         "AverageRecall": float,
         "AverageAccuracy": float,
@@ -1378,25 +1252,14 @@
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
-KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1417,65 +1280,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PiiEntitiesDetectionJobFilterTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-SentimentDetectionJobFilterTypeDef = TypedDict(
-    "SentimentDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-TopicsDetectionJobFilterTypeDef = TypedDict(
-    "TopicsDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 PartOfSpeechTagTypeDef = TypedDict(
     "PartOfSpeechTagTypeDef",
     {
         "Tag": PartOfSpeechTagTypeType,
         "Score": float,
     },
     total=False,
@@ -1491,21 +1310,19 @@
     "_OptionalPiiOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class PiiOutputDataConfigTypeDef(
     _RequiredPiiOutputDataConfigTypeDef, _OptionalPiiOutputDataConfigTypeDef
 ):
     pass
 
-
 RedactionConfigOutputTypeDef = TypedDict(
     "RedactionConfigOutputTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
@@ -1523,21 +1340,19 @@
     "_OptionalPutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
 RedactionConfigTypeDef = TypedDict(
     "RedactionConfigTypeDef",
     {
         "PiiEntityTypes": Sequence[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
@@ -1554,22 +1369,20 @@
     "_OptionalStartFlywheelIterationRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class StartFlywheelIterationRequestRequestTypeDef(
     _RequiredStartFlywheelIterationRequestRequestTypeDef,
     _OptionalStartFlywheelIterationRequestRequestTypeDef,
 ):
     pass
 
-
 StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
     "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -1650,21 +1463,19 @@
         "DesiredInferenceUnits": int,
         "DesiredDataAccessRoleArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
-
 class UpdateEndpointRequestRequestTypeDef(
     _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
-
 BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
     "BatchDetectDominantLanguageItemResultTypeDef",
     {
         "Index": int,
         "Languages": List[DominantLanguageTypeDef],
     },
     total=False,
@@ -1992,34 +1803,32 @@
         "EndpointArn": str,
     },
 )
 _OptionalClassifyDocumentRequestRequestTypeDef = TypedDict(
     "_OptionalClassifyDocumentRequestRequestTypeDef",
     {
         "Text": str,
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-
 class ClassifyDocumentRequestRequestTypeDef(
     _RequiredClassifyDocumentRequestRequestTypeDef, _OptionalClassifyDocumentRequestRequestTypeDef
 ):
     pass
 
-
 DetectEntitiesRequestRequestTypeDef = TypedDict(
     "DetectEntitiesRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
         "EndpointArn": str,
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
@@ -2032,19 +1841,17 @@
     {
         "InputFormat": InputFormatType,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
-
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2064,21 +1871,19 @@
         "Tags": Sequence[TagTypeDef],
         "DataAccessRoleArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
-
 class CreateEndpointRequestRequestTypeDef(
     _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredImportModelRequestRequestTypeDef = TypedDict(
     "_RequiredImportModelRequestRequestTypeDef",
     {
         "SourceModelArn": str,
     },
 )
 _OptionalImportModelRequestRequestTypeDef = TypedDict(
@@ -2089,21 +1894,19 @@
         "ModelKmsKeyId": str,
         "DataAccessRoleArn": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportModelRequestRequestTypeDef(
     _RequiredImportModelRequestRequestTypeDef, _OptionalImportModelRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2145,14 +1948,15 @@
         "VolumeKmsKeyId": str,
         "DataLakeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetEntityRecognizerInputDataConfigTypeDef",
     {
         "Documents": DatasetEntityRecognizerDocumentsTypeDef,
     },
 )
 _OptionalDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2160,29 +1964,178 @@
     {
         "Annotations": DatasetEntityRecognizerAnnotationsTypeDef,
         "EntityList": DatasetEntityRecognizerEntityListTypeDef,
     },
     total=False,
 )
 
-
 class DatasetEntityRecognizerInputDataConfigTypeDef(
     _RequiredDatasetEntityRecognizerInputDataConfigTypeDef,
     _OptionalDatasetEntityRecognizerInputDataConfigTypeDef,
 ):
     pass
 
+DatasetFilterTypeDef = TypedDict(
+    "DatasetFilterTypeDef",
+    {
+        "Status": DatasetStatusType,
+        "DatasetType": DatasetTypeType,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
 
-ListDatasetsRequestRequestTypeDef = TypedDict(
-    "ListDatasetsRequestRequestTypeDef",
+DocumentClassificationJobFilterTypeDef = TypedDict(
+    "DocumentClassificationJobFilterTypeDef",
     {
-        "FlywheelArn": str,
-        "Filter": DatasetFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DocumentClassifierFilterTypeDef = TypedDict(
+    "DocumentClassifierFilterTypeDef",
+    {
+        "Status": ModelStatusType,
+        "DocumentClassifierName": str,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobFilterTypeDef = TypedDict(
+    "DominantLanguageDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EndpointFilterTypeDef = TypedDict(
+    "EndpointFilterTypeDef",
+    {
+        "ModelArn": str,
+        "Status": EndpointStatusType,
+        "CreationTimeBefore": TimestampTypeDef,
+        "CreationTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobFilterTypeDef = TypedDict(
+    "EntitiesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EntityRecognizerFilterTypeDef = TypedDict(
+    "EntityRecognizerFilterTypeDef",
+    {
+        "Status": ModelStatusType,
+        "RecognizerName": str,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EventsDetectionJobFilterTypeDef = TypedDict(
+    "EventsDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+FlywheelFilterTypeDef = TypedDict(
+    "FlywheelFilterTypeDef",
+    {
+        "Status": FlywheelStatusType,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+FlywheelIterationFilterTypeDef = TypedDict(
+    "FlywheelIterationFilterTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobFilterTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+SentimentDetectionJobFilterTypeDef = TypedDict(
+    "SentimentDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobFilterTypeDef = TypedDict(
+    "TopicsDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
@@ -2221,24 +2174,14 @@
     "DetectPiiEntitiesResponseTypeDef",
     {
         "Entities": List[PiiEntityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestRequestTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 DocumentClassifierInputDataConfigTypeDef = TypedDict(
     "DocumentClassifierInputDataConfigTypeDef",
     {
         "DataFormat": DocumentClassifierDataFormatType,
         "S3Uri": str,
         "TestS3Uri": str,
         "LabelDelimiter": str,
@@ -2246,24 +2189,14 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestRequestTypeDef",
-    {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 DocumentClassifierInputDataConfigOutputTypeDef = TypedDict(
     "DocumentClassifierInputDataConfigOutputTypeDef",
     {
         "DataFormat": DocumentClassifierDataFormatType,
         "S3Uri": str,
         "TestS3Uri": str,
         "LabelDelimiter": str,
@@ -2271,14 +2204,17 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
+DocumentReaderConfigUnionTypeDef = Union[
+    DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
+]
 _RequiredInputDataConfigOutputTypeDef = TypedDict(
     "_RequiredInputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalInputDataConfigOutputTypeDef = TypedDict(
@@ -2286,21 +2222,19 @@
     {
         "InputFormat": InputFormatType,
         "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
-
 class InputDataConfigOutputTypeDef(
     _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
 ):
     pass
 
-
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2311,44 +2245,14 @@
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
-ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": DominantLanguageDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListEndpointsRequestRequestTypeDef = TypedDict(
-    "ListEndpointsRequestRequestTypeDef",
-    {
-        "Filter": EndpointFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 EntityRecognitionConfigOutputTypeDef = TypedDict(
     "EntityRecognitionConfigOutputTypeDef",
     {
         "EntityTypes": List[EntityTypesListItemTypeDef],
     },
 )
 
@@ -2373,22 +2277,20 @@
         "Annotations": EntityRecognizerAnnotationsTypeDef,
         "EntityList": EntityRecognizerEntityListTypeDef,
         "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
     },
     total=False,
 )
 
-
 class EntityRecognizerInputDataConfigOutputTypeDef(
     _RequiredEntityRecognizerInputDataConfigOutputTypeDef,
     _OptionalEntityRecognizerInputDataConfigOutputTypeDef,
 ):
     pass
 
-
 _RequiredEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 _OptionalEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2399,31 +2301,19 @@
         "Annotations": EntityRecognizerAnnotationsTypeDef,
         "EntityList": EntityRecognizerEntityListTypeDef,
         "AugmentedManifests": Sequence[AugmentedManifestsListItemTypeDef],
     },
     total=False,
 )
 
-
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
-
-ListEntityRecognizersRequestRequestTypeDef = TypedDict(
-    "ListEntityRecognizersRequestRequestTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 EntityRecognizerMetadataEntityTypesListItemTypeDef = TypedDict(
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     {
         "Type": str,
         "EvaluationMetrics": EntityTypesEvaluationMetricsTypeDef,
         "NumberOfTrainMentions": int,
     },
@@ -2435,58 +2325,14 @@
     {
         "EntityRecognizerSummariesList": List[EntityRecognizerSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListEventsDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": EventsDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListFlywheelsRequestRequestTypeDef = TypedDict(
-    "ListFlywheelsRequestRequestTypeDef",
-    {
-        "Filter": FlywheelFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-_RequiredListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredListFlywheelIterationHistoryRequestRequestTypeDef",
-    {
-        "FlywheelArn": str,
-    },
-)
-_OptionalListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalListFlywheelIterationHistoryRequestRequestTypeDef",
-    {
-        "Filter": FlywheelIterationFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListFlywheelIterationHistoryRequestRequestTypeDef(
-    _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
-    _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
-):
-    pass
-
-
 FlywheelIterationPropertiesTypeDef = TypedDict(
     "FlywheelIterationPropertiesTypeDef",
     {
         "FlywheelArn": str,
         "FlywheelIterationId": str,
         "CreationTime": datetime,
         "EndTime": datetime,
@@ -2515,168 +2361,27 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
-    TypedDict(
-        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-        {
-            "Filter": DominantLanguageDetectionJobFilterTypeDef,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    {
-        "Filter": EndpointFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
-    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
-    {
-        "Filter": SentimentDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListSentimentDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": SentimentDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": TargetedSentimentDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
-    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
-    {
-        "Filter": TopicsDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListTopicsDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": TopicsDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 SyntaxTokenTypeDef = TypedDict(
     "SyntaxTokenTypeDef",
     {
         "TokenId": int,
         "Text": str,
         "BeginOffset": int,
         "EndOffset": int,
         "PartOfSpeech": PartOfSpeechTagTypeDef,
     },
     total=False,
 )
 
+RedactionConfigUnionTypeDef = Union[RedactionConfigTypeDef, RedactionConfigOutputTypeDef]
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2745,22 +2450,20 @@
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "FlywheelArn": str,
     },
     total=False,
 )
 
-
 class StartDocumentClassificationJobRequestRequestTypeDef(
     _RequiredStartDocumentClassificationJobRequestRequestTypeDef,
     _OptionalStartDocumentClassificationJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2773,22 +2476,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartDominantLanguageDetectionJobRequestRequestTypeDef(
     _RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef,
     _OptionalStartDominantLanguageDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEntitiesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2804,22 +2505,20 @@
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "FlywheelArn": str,
     },
     total=False,
 )
 
-
 class StartEntitiesDetectionJobRequestRequestTypeDef(
     _RequiredStartEntitiesDetectionJobRequestRequestTypeDef,
     _OptionalStartEntitiesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartEventsDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEventsDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2832,22 +2531,20 @@
         "JobName": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartEventsDetectionJobRequestRequestTypeDef(
     _RequiredStartEventsDetectionJobRequestRequestTypeDef,
     _OptionalStartEventsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2861,22 +2558,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartKeyPhrasesDetectionJobRequestRequestTypeDef(
     _RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef,
     _OptionalStartKeyPhrasesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "Mode": PiiEntitiesDetectionModeType,
         "DataAccessRoleArn": str,
@@ -2890,22 +2585,20 @@
         "JobName": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartPiiEntitiesDetectionJobRequestRequestTypeDef(
     _RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef,
     _OptionalStartPiiEntitiesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSentimentDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2919,22 +2612,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartSentimentDetectionJobRequestRequestTypeDef(
     _RequiredStartSentimentDetectionJobRequestRequestTypeDef,
     _OptionalStartSentimentDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2948,22 +2639,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartTargetedSentimentDetectionJobRequestRequestTypeDef(
     _RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef,
     _OptionalStartTargetedSentimentDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartTopicsDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTopicsDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2977,22 +2666,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartTopicsDetectionJobRequestRequestTypeDef(
     _RequiredStartTopicsDetectionJobRequestRequestTypeDef,
     _OptionalStartTopicsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlywheelRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
 _OptionalUpdateFlywheelRequestRequestTypeDef = TypedDict(
@@ -3001,32 +2688,286 @@
         "ActiveModelArn": str,
         "DataAccessRoleArn": str,
         "DataSecurityConfig": UpdateDataSecurityConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFlywheelRequestRequestTypeDef(
     _RequiredUpdateFlywheelRequestRequestTypeDef, _OptionalUpdateFlywheelRequestRequestTypeDef
 ):
     pass
 
-
+DataSecurityConfigUnionTypeDef = Union[DataSecurityConfigTypeDef, DataSecurityConfigOutputTypeDef]
 DatasetInputDataConfigTypeDef = TypedDict(
     "DatasetInputDataConfigTypeDef",
     {
         "AugmentedManifests": Sequence[DatasetAugmentedManifestsListItemTypeDef],
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
     },
     total=False,
 )
 
+ListDatasetsRequestRequestTypeDef = TypedDict(
+    "ListDatasetsRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+        "Filter": DatasetFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestRequestTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestRequestTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
+    TypedDict(
+        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+        {
+            "Filter": DominantLanguageDetectionJobFilterTypeDef,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": DominantLanguageDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEndpointsRequestRequestTypeDef = TypedDict(
+    "ListEndpointsRequestRequestTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestRequestTypeDef = TypedDict(
+    "ListEntityRecognizersRequestRequestTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListEventsDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": EventsDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListFlywheelsRequestRequestTypeDef = TypedDict(
+    "ListFlywheelsRequestRequestTypeDef",
+    {
+        "Filter": FlywheelFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+_RequiredListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredListFlywheelIterationHistoryRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+    },
+)
+_OptionalListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalListFlywheelIterationHistoryRequestRequestTypeDef",
+    {
+        "Filter": FlywheelIterationFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListFlywheelIterationHistoryRequestRequestTypeDef(
+    _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
+    _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
+):
+    pass
+
+ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
+    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
+    {
+        "Filter": SentimentDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListSentimentDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": SentimentDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": TargetedSentimentDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
+    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
+    {
+        "Filter": TopicsDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListTopicsDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": TopicsDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentClassifierRequestRequestTypeDef",
     {
         "DocumentClassifierName": str,
         "DataAccessRoleArn": str,
         "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
@@ -3044,22 +2985,23 @@
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "ModelPolicy": str,
     },
     total=False,
 )
 
-
 class CreateDocumentClassifierRequestRequestTypeDef(
     _RequiredCreateDocumentClassifierRequestRequestTypeDef,
     _OptionalCreateDocumentClassifierRequestRequestTypeDef,
 ):
     pass
 
-
+DocumentClassifierInputDataConfigUnionTypeDef = Union[
+    DocumentClassifierInputDataConfigTypeDef, DocumentClassifierInputDataConfigOutputTypeDef
+]
 DocumentClassifierPropertiesTypeDef = TypedDict(
     "DocumentClassifierPropertiesTypeDef",
     {
         "DocumentClassifierArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
@@ -3159,14 +3101,15 @@
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "TargetEventTypes": List[str],
     },
     total=False,
 )
 
+InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
 KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
     "KeyPhrasesDetectionJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
@@ -3287,19 +3230,17 @@
     {
         "DocumentClassificationConfig": DocumentClassificationConfigOutputTypeDef,
         "EntityRecognitionConfig": EntityRecognitionConfigOutputTypeDef,
     },
     total=False,
 )
 
-
 class TaskConfigOutputTypeDef(_RequiredTaskConfigOutputTypeDef, _OptionalTaskConfigOutputTypeDef):
     pass
 
-
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
     },
 )
 _OptionalTaskConfigTypeDef = TypedDict(
@@ -3307,19 +3248,17 @@
     {
         "DocumentClassificationConfig": DocumentClassificationConfigTypeDef,
         "EntityRecognitionConfig": EntityRecognitionConfigTypeDef,
     },
     total=False,
 )
 
-
 class TaskConfigTypeDef(_RequiredTaskConfigTypeDef, _OptionalTaskConfigTypeDef):
     pass
 
-
 _RequiredCreateEntityRecognizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRecognizerRequestRequestTypeDef",
     {
         "RecognizerName": str,
         "DataAccessRoleArn": str,
         "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
@@ -3335,22 +3274,23 @@
         "VpcConfig": VpcConfigTypeDef,
         "ModelKmsKeyId": str,
         "ModelPolicy": str,
     },
     total=False,
 )
 
-
 class CreateEntityRecognizerRequestRequestTypeDef(
     _RequiredCreateEntityRecognizerRequestRequestTypeDef,
     _OptionalCreateEntityRecognizerRequestRequestTypeDef,
 ):
     pass
 
-
+EntityRecognizerInputDataConfigUnionTypeDef = Union[
+    EntityRecognizerInputDataConfigTypeDef, EntityRecognizerInputDataConfigOutputTypeDef
+]
 EntityRecognizerMetadataTypeDef = TypedDict(
     "EntityRecognizerMetadataTypeDef",
     {
         "NumberOfTrainedDocuments": int,
         "NumberOfTestDocuments": int,
         "EvaluationMetrics": EntityRecognizerEvaluationMetricsTypeDef,
         "EntityTypes": List[EntityRecognizerMetadataEntityTypesListItemTypeDef],
@@ -3438,21 +3378,19 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 DescribeDocumentClassifierResponseTypeDef = TypedDict(
     "DescribeDocumentClassifierResponseTypeDef",
     {
         "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3659,21 +3597,20 @@
         "DataSecurityConfig": DataSecurityConfigTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFlywheelRequestRequestTypeDef(
     _RequiredCreateFlywheelRequestRequestTypeDef, _OptionalCreateFlywheelRequestRequestTypeDef
 ):
     pass
 
-
+TaskConfigUnionTypeDef = Union[TaskConfigTypeDef, TaskConfigOutputTypeDef]
 EntityRecognizerPropertiesTypeDef = TypedDict(
     "EntityRecognizerPropertiesTypeDef",
     {
         "EntityRecognizerArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
```

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend/type_defs.pyi` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_comprehend.type_defs import AugmentedManifestsListItemOutputTypeDef
 
-    data: AugmentedManifestsListItemOutputTypeDef = {...}
+    data: AugmentedManifestsListItemOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -57,28 +57,30 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
     "SentimentScoreTypeDef",
     "BatchDetectSentimentRequestRequestTypeDef",
     "BatchDetectSyntaxRequestRequestTypeDef",
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
+    "BlobTypeDef",
     "ChildBlockTypeDef",
     "RelationshipsListItemTypeDef",
     "BoundingBoxTypeDef",
     "ClassifierEvaluationMetricsTypeDef",
     "DocumentReaderConfigTypeDef",
     "DocumentClassTypeDef",
     "DocumentLabelTypeDef",
@@ -92,15 +94,15 @@
     "VpcConfigTypeDef",
     "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
-    "DatasetFilterTypeDef",
+    "TimestampTypeDef",
     "DatasetPropertiesTypeDef",
     "DeleteDocumentClassifierRequestRequestTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEntityRecognizerRequestRequestTypeDef",
     "DeleteFlywheelRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
@@ -125,48 +127,34 @@
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
     "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
-    "DocumentClassificationJobFilterTypeDef",
     "OutputDataConfigTypeDef",
     "DocumentClassifierDocumentsTypeDef",
-    "DocumentClassifierFilterTypeDef",
     "DocumentReaderConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
-    "DominantLanguageDetectionJobFilterTypeDef",
-    "EndpointFilterTypeDef",
-    "EntitiesDetectionJobFilterTypeDef",
     "EntityTypesListItemTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
     "EntityRecognizerDocumentsTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
-    "EntityRecognizerFilterTypeDef",
     "EntityTypesEvaluationMetricsTypeDef",
     "EntityRecognizerOutputDataConfigTypeDef",
     "EntityRecognizerSummaryTypeDef",
-    "EventsDetectionJobFilterTypeDef",
-    "FlywheelFilterTypeDef",
-    "FlywheelIterationFilterTypeDef",
     "FlywheelModelEvaluationMetricsTypeDef",
     "FlywheelSummaryTypeDef",
     "PointTypeDef",
-    "KeyPhrasesDetectionJobFilterTypeDef",
     "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
-    "PiiEntitiesDetectionJobFilterTypeDef",
-    "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TargetedSentimentDetectionJobFilterTypeDef",
-    "TopicsDetectionJobFilterTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
     "RedactionConfigOutputTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RedactionConfigTypeDef",
     "StartFlywheelIterationRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobRequestRequestTypeDef",
@@ -222,60 +210,53 @@
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
     "DataSecurityConfigOutputTypeDef",
+    "VpcConfigUnionTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
-    "ListDatasetsRequestRequestTypeDef",
+    "DatasetFilterTypeDef",
+    "DocumentClassificationJobFilterTypeDef",
+    "DocumentClassifierFilterTypeDef",
+    "DominantLanguageDetectionJobFilterTypeDef",
+    "EndpointFilterTypeDef",
+    "EntitiesDetectionJobFilterTypeDef",
+    "EntityRecognizerFilterTypeDef",
+    "EventsDetectionJobFilterTypeDef",
+    "FlywheelFilterTypeDef",
+    "FlywheelIterationFilterTypeDef",
+    "KeyPhrasesDetectionJobFilterTypeDef",
+    "PiiEntitiesDetectionJobFilterTypeDef",
+    "SentimentDetectionJobFilterTypeDef",
+    "TargetedSentimentDetectionJobFilterTypeDef",
+    "TopicsDetectionJobFilterTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
-    "ListDocumentClassificationJobsRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigTypeDef",
-    "ListDocumentClassifiersRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigOutputTypeDef",
+    "DocumentReaderConfigUnionTypeDef",
     "InputDataConfigOutputTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
-    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
-    "ListEndpointsRequestRequestTypeDef",
-    "ListEntitiesDetectionJobsRequestRequestTypeDef",
     "EntityRecognitionConfigOutputTypeDef",
     "EntityRecognitionConfigTypeDef",
     "EntityRecognizerInputDataConfigOutputTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
-    "ListEntityRecognizersRequestRequestTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
-    "ListEventsDetectionJobsRequestRequestTypeDef",
-    "ListFlywheelsRequestRequestTypeDef",
-    "ListFlywheelIterationHistoryRequestRequestTypeDef",
     "FlywheelIterationPropertiesTypeDef",
     "ListFlywheelsResponseTypeDef",
     "GeometryTypeDef",
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
-    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
-    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
-    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
-    "ListSentimentDetectionJobsRequestRequestTypeDef",
-    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
-    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
-    "ListTopicsDetectionJobsRequestRequestTypeDef",
     "SyntaxTokenTypeDef",
+    "RedactionConfigUnionTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
     "TargetedSentimentMentionTypeDef",
     "EntityTypeDef",
     "StartDocumentClassificationJobRequestRequestTypeDef",
     "StartDominantLanguageDetectionJobRequestRequestTypeDef",
@@ -283,30 +264,59 @@
     "StartEventsDetectionJobRequestRequestTypeDef",
     "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StartSentimentDetectionJobRequestRequestTypeDef",
     "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StartTopicsDetectionJobRequestRequestTypeDef",
     "UpdateFlywheelRequestRequestTypeDef",
+    "DataSecurityConfigUnionTypeDef",
     "DatasetInputDataConfigTypeDef",
+    "ListDatasetsRequestRequestTypeDef",
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    "ListDocumentClassificationJobsRequestRequestTypeDef",
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    "ListDocumentClassifiersRequestRequestTypeDef",
+    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    "ListEndpointsRequestRequestTypeDef",
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    "ListEntitiesDetectionJobsRequestRequestTypeDef",
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    "ListEntityRecognizersRequestRequestTypeDef",
+    "ListEventsDetectionJobsRequestRequestTypeDef",
+    "ListFlywheelsRequestRequestTypeDef",
+    "ListFlywheelIterationHistoryRequestRequestTypeDef",
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
+    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
+    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
+    "ListSentimentDetectionJobsRequestRequestTypeDef",
+    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
+    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
+    "ListTopicsDetectionJobsRequestRequestTypeDef",
     "CreateDocumentClassifierRequestRequestTypeDef",
+    "DocumentClassifierInputDataConfigUnionTypeDef",
     "DocumentClassifierPropertiesTypeDef",
     "DocumentClassificationJobPropertiesTypeDef",
     "DominantLanguageDetectionJobPropertiesTypeDef",
     "EntitiesDetectionJobPropertiesTypeDef",
     "EventsDetectionJobPropertiesTypeDef",
+    "InputDataConfigUnionTypeDef",
     "KeyPhrasesDetectionJobPropertiesTypeDef",
     "PiiEntitiesDetectionJobPropertiesTypeDef",
     "SentimentDetectionJobPropertiesTypeDef",
     "TargetedSentimentDetectionJobPropertiesTypeDef",
     "TopicsDetectionJobPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
     "TaskConfigOutputTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
+    "EntityRecognizerInputDataConfigUnionTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
@@ -330,14 +340,15 @@
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
     "FlywheelPropertiesTypeDef",
     "CreateFlywheelRequestRequestTypeDef",
+    "TaskConfigUnionTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
     "BatchDetectEntitiesResponseTypeDef",
     "DescribeFlywheelResponseTypeDef",
@@ -361,20 +372,22 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
+
 class AugmentedManifestsListItemOutputTypeDef(
     _RequiredAugmentedManifestsListItemOutputTypeDef,
     _OptionalAugmentedManifestsListItemOutputTypeDef,
 ):
     pass
 
+
 _RequiredAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredAugmentedManifestsListItemTypeDef",
     {
         "S3Uri": str,
         "AttributeNames": Sequence[str],
     },
 )
@@ -385,19 +398,21 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
+
 class AugmentedManifestsListItemTypeDef(
     _RequiredAugmentedManifestsListItemTypeDef, _OptionalAugmentedManifestsListItemTypeDef
 ):
     pass
 
+
 DominantLanguageTypeDef = TypedDict(
     "DominantLanguageTypeDef",
     {
         "LanguageCode": str,
         "Score": float,
     },
     total=False,
@@ -489,14 +504,15 @@
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChildBlockTypeDef = TypedDict(
     "ChildBlockTypeDef",
     {
         "ChildBlockId": str,
         "BeginOffset": int,
         "EndOffset": int,
     },
@@ -549,19 +565,21 @@
     {
         "DocumentReadMode": DocumentReadModeType,
         "FeatureTypes": Sequence[DocumentReadFeatureTypesType],
     },
     total=False,
 )
 
+
 class DocumentReaderConfigTypeDef(
     _RequiredDocumentReaderConfigTypeDef, _OptionalDocumentReaderConfigTypeDef
 ):
     pass
 
+
 DocumentClassTypeDef = TypedDict(
     "DocumentClassTypeDef",
     {
         "Name": str,
         "Score": float,
         "Page": int,
     },
@@ -634,17 +652,19 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 DocumentClassifierOutputDataConfigTypeDef = TypedDict(
     "DocumentClassifierOutputDataConfigTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
         "FlywheelStatsS3Prefix": str,
     },
@@ -680,40 +700,44 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
+
 class DatasetAugmentedManifestsListItemTypeDef(
     _RequiredDatasetAugmentedManifestsListItemTypeDef,
     _OptionalDatasetAugmentedManifestsListItemTypeDef,
 ):
     pass
 
+
 _RequiredDatasetDocumentClassifierInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetDocumentClassifierInputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalDatasetDocumentClassifierInputDataConfigTypeDef = TypedDict(
     "_OptionalDatasetDocumentClassifierInputDataConfigTypeDef",
     {
         "LabelDelimiter": str,
     },
     total=False,
 )
 
+
 class DatasetDocumentClassifierInputDataConfigTypeDef(
     _RequiredDatasetDocumentClassifierInputDataConfigTypeDef,
     _OptionalDatasetDocumentClassifierInputDataConfigTypeDef,
 ):
     pass
 
+
 DatasetEntityRecognizerAnnotationsTypeDef = TypedDict(
     "DatasetEntityRecognizerAnnotationsTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -727,38 +751,30 @@
     "_OptionalDatasetEntityRecognizerDocumentsTypeDef",
     {
         "InputFormat": InputFormatType,
     },
     total=False,
 )
 
+
 class DatasetEntityRecognizerDocumentsTypeDef(
     _RequiredDatasetEntityRecognizerDocumentsTypeDef,
     _OptionalDatasetEntityRecognizerDocumentsTypeDef,
 ):
     pass
 
+
 DatasetEntityRecognizerEntityListTypeDef = TypedDict(
     "DatasetEntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
-DatasetFilterTypeDef = TypedDict(
-    "DatasetFilterTypeDef",
-    {
-        "Status": DatasetStatusType,
-        "DatasetType": DatasetTypeType,
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DatasetPropertiesTypeDef = TypedDict(
     "DatasetPropertiesTypeDef",
     {
         "DatasetArn": str,
         "DatasetName": str,
         "DatasetType": DatasetTypeType,
         "DatasetS3Uri": str,
@@ -810,20 +826,22 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -1020,49 +1038,42 @@
     "_OptionalDocumentClassificationConfigOutputTypeDef",
     {
         "Labels": List[str],
     },
     total=False,
 )
 
+
 class DocumentClassificationConfigOutputTypeDef(
     _RequiredDocumentClassificationConfigOutputTypeDef,
     _OptionalDocumentClassificationConfigOutputTypeDef,
 ):
     pass
 
+
 _RequiredDocumentClassificationConfigTypeDef = TypedDict(
     "_RequiredDocumentClassificationConfigTypeDef",
     {
         "Mode": DocumentClassifierModeType,
     },
 )
 _OptionalDocumentClassificationConfigTypeDef = TypedDict(
     "_OptionalDocumentClassificationConfigTypeDef",
     {
         "Labels": Sequence[str],
     },
     total=False,
 )
 
+
 class DocumentClassificationConfigTypeDef(
     _RequiredDocumentClassificationConfigTypeDef, _OptionalDocumentClassificationConfigTypeDef
 ):
     pass
 
-DocumentClassificationJobFilterTypeDef = TypedDict(
-    "DocumentClassificationJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
 
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
@@ -1070,46 +1081,39 @@
     "_OptionalOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
+
 _RequiredDocumentClassifierDocumentsTypeDef = TypedDict(
     "_RequiredDocumentClassifierDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalDocumentClassifierDocumentsTypeDef = TypedDict(
     "_OptionalDocumentClassifierDocumentsTypeDef",
     {
         "TestS3Uri": str,
     },
     total=False,
 )
 
+
 class DocumentClassifierDocumentsTypeDef(
     _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
 ):
     pass
 
-DocumentClassifierFilterTypeDef = TypedDict(
-    "DocumentClassifierFilterTypeDef",
-    {
-        "Status": ModelStatusType,
-        "DocumentClassifierName": str,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
 
 _RequiredDocumentReaderConfigOutputTypeDef = TypedDict(
     "_RequiredDocumentReaderConfigOutputTypeDef",
     {
         "DocumentReadAction": DocumentReadActionType,
     },
 )
@@ -1118,19 +1122,21 @@
     {
         "DocumentReadMode": DocumentReadModeType,
         "FeatureTypes": List[DocumentReadFeatureTypesType],
     },
     total=False,
 )
 
+
 class DocumentReaderConfigOutputTypeDef(
     _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
 ):
     pass
 
+
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1144,47 +1150,14 @@
     {
         "Page": int,
         "Count": int,
     },
     total=False,
 )
 
-DominantLanguageDetectionJobFilterTypeDef = TypedDict(
-    "DominantLanguageDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-EndpointFilterTypeDef = TypedDict(
-    "EndpointFilterTypeDef",
-    {
-        "ModelArn": str,
-        "Status": EndpointStatusType,
-        "CreationTimeBefore": Union[datetime, str],
-        "CreationTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-EntitiesDetectionJobFilterTypeDef = TypedDict(
-    "EntitiesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 EntityTypesListItemTypeDef = TypedDict(
     "EntityTypesListItemTypeDef",
     {
         "Type": str,
     },
 )
 
@@ -1198,19 +1171,21 @@
     "_OptionalEntityRecognizerAnnotationsTypeDef",
     {
         "TestS3Uri": str,
     },
     total=False,
 )
 
+
 class EntityRecognizerAnnotationsTypeDef(
     _RequiredEntityRecognizerAnnotationsTypeDef, _OptionalEntityRecognizerAnnotationsTypeDef
 ):
     pass
 
+
 _RequiredEntityRecognizerDocumentsTypeDef = TypedDict(
     "_RequiredEntityRecognizerDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalEntityRecognizerDocumentsTypeDef = TypedDict(
@@ -1218,19 +1193,21 @@
     {
         "TestS3Uri": str,
         "InputFormat": InputFormatType,
     },
     total=False,
 )
 
+
 class EntityRecognizerDocumentsTypeDef(
     _RequiredEntityRecognizerDocumentsTypeDef, _OptionalEntityRecognizerDocumentsTypeDef
 ):
     pass
 
+
 EntityRecognizerEntityListTypeDef = TypedDict(
     "EntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -1240,25 +1217,14 @@
         "Precision": float,
         "Recall": float,
         "F1Score": float,
     },
     total=False,
 )
 
-EntityRecognizerFilterTypeDef = TypedDict(
-    "EntityRecognizerFilterTypeDef",
-    {
-        "Status": ModelStatusType,
-        "RecognizerName": str,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 EntityTypesEvaluationMetricsTypeDef = TypedDict(
     "EntityTypesEvaluationMetricsTypeDef",
     {
         "Precision": float,
         "Recall": float,
         "F1Score": float,
     },
@@ -1281,44 +1247,14 @@
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
         "LatestVersionStatus": ModelStatusType,
     },
     total=False,
 )
 
-EventsDetectionJobFilterTypeDef = TypedDict(
-    "EventsDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-FlywheelFilterTypeDef = TypedDict(
-    "FlywheelFilterTypeDef",
-    {
-        "Status": FlywheelStatusType,
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-FlywheelIterationFilterTypeDef = TypedDict(
-    "FlywheelIterationFilterTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 FlywheelModelEvaluationMetricsTypeDef = TypedDict(
     "FlywheelModelEvaluationMetricsTypeDef",
     {
         "AverageF1Score": float,
         "AveragePrecision": float,
         "AverageRecall": float,
         "AverageAccuracy": float,
@@ -1347,25 +1283,14 @@
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
-KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1386,65 +1311,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PiiEntitiesDetectionJobFilterTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-SentimentDetectionJobFilterTypeDef = TypedDict(
-    "SentimentDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-TopicsDetectionJobFilterTypeDef = TypedDict(
-    "TopicsDetectionJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 PartOfSpeechTagTypeDef = TypedDict(
     "PartOfSpeechTagTypeDef",
     {
         "Tag": PartOfSpeechTagTypeType,
         "Score": float,
     },
     total=False,
@@ -1460,19 +1341,21 @@
     "_OptionalPiiOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class PiiOutputDataConfigTypeDef(
     _RequiredPiiOutputDataConfigTypeDef, _OptionalPiiOutputDataConfigTypeDef
 ):
     pass
 
+
 RedactionConfigOutputTypeDef = TypedDict(
     "RedactionConfigOutputTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
@@ -1490,19 +1373,21 @@
     "_OptionalPutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+
 RedactionConfigTypeDef = TypedDict(
     "RedactionConfigTypeDef",
     {
         "PiiEntityTypes": Sequence[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
@@ -1519,20 +1404,22 @@
     "_OptionalStartFlywheelIterationRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class StartFlywheelIterationRequestRequestTypeDef(
     _RequiredStartFlywheelIterationRequestRequestTypeDef,
     _OptionalStartFlywheelIterationRequestRequestTypeDef,
 ):
     pass
 
+
 StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
     "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -1613,19 +1500,21 @@
         "DesiredInferenceUnits": int,
         "DesiredDataAccessRoleArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
+
 class UpdateEndpointRequestRequestTypeDef(
     _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
+
 BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
     "BatchDetectDominantLanguageItemResultTypeDef",
     {
         "Index": int,
         "Languages": List[DominantLanguageTypeDef],
     },
     total=False,
@@ -1953,32 +1842,34 @@
         "EndpointArn": str,
     },
 )
 _OptionalClassifyDocumentRequestRequestTypeDef = TypedDict(
     "_OptionalClassifyDocumentRequestRequestTypeDef",
     {
         "Text": str,
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
+
 class ClassifyDocumentRequestRequestTypeDef(
     _RequiredClassifyDocumentRequestRequestTypeDef, _OptionalClassifyDocumentRequestRequestTypeDef
 ):
     pass
 
+
 DetectEntitiesRequestRequestTypeDef = TypedDict(
     "DetectEntitiesRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
         "EndpointArn": str,
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "Bytes": BlobTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
@@ -1991,17 +1882,19 @@
     {
         "InputFormat": InputFormatType,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
+
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
+
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2021,19 +1914,21 @@
         "Tags": Sequence[TagTypeDef],
         "DataAccessRoleArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
+
 class CreateEndpointRequestRequestTypeDef(
     _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredImportModelRequestRequestTypeDef = TypedDict(
     "_RequiredImportModelRequestRequestTypeDef",
     {
         "SourceModelArn": str,
     },
 )
 _OptionalImportModelRequestRequestTypeDef = TypedDict(
@@ -2044,19 +1939,21 @@
         "ModelKmsKeyId": str,
         "DataAccessRoleArn": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportModelRequestRequestTypeDef(
     _RequiredImportModelRequestRequestTypeDef, _OptionalImportModelRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2098,14 +1995,15 @@
         "VolumeKmsKeyId": str,
         "DataLakeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetEntityRecognizerInputDataConfigTypeDef",
     {
         "Documents": DatasetEntityRecognizerDocumentsTypeDef,
     },
 )
 _OptionalDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2113,27 +2011,180 @@
     {
         "Annotations": DatasetEntityRecognizerAnnotationsTypeDef,
         "EntityList": DatasetEntityRecognizerEntityListTypeDef,
     },
     total=False,
 )
 
+
 class DatasetEntityRecognizerInputDataConfigTypeDef(
     _RequiredDatasetEntityRecognizerInputDataConfigTypeDef,
     _OptionalDatasetEntityRecognizerInputDataConfigTypeDef,
 ):
     pass
 
-ListDatasetsRequestRequestTypeDef = TypedDict(
-    "ListDatasetsRequestRequestTypeDef",
+
+DatasetFilterTypeDef = TypedDict(
+    "DatasetFilterTypeDef",
     {
-        "FlywheelArn": str,
-        "Filter": DatasetFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "Status": DatasetStatusType,
+        "DatasetType": DatasetTypeType,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DocumentClassificationJobFilterTypeDef = TypedDict(
+    "DocumentClassificationJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DocumentClassifierFilterTypeDef = TypedDict(
+    "DocumentClassifierFilterTypeDef",
+    {
+        "Status": ModelStatusType,
+        "DocumentClassifierName": str,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobFilterTypeDef = TypedDict(
+    "DominantLanguageDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EndpointFilterTypeDef = TypedDict(
+    "EndpointFilterTypeDef",
+    {
+        "ModelArn": str,
+        "Status": EndpointStatusType,
+        "CreationTimeBefore": TimestampTypeDef,
+        "CreationTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobFilterTypeDef = TypedDict(
+    "EntitiesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EntityRecognizerFilterTypeDef = TypedDict(
+    "EntityRecognizerFilterTypeDef",
+    {
+        "Status": ModelStatusType,
+        "RecognizerName": str,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EventsDetectionJobFilterTypeDef = TypedDict(
+    "EventsDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+FlywheelFilterTypeDef = TypedDict(
+    "FlywheelFilterTypeDef",
+    {
+        "Status": FlywheelStatusType,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+FlywheelIterationFilterTypeDef = TypedDict(
+    "FlywheelIterationFilterTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobFilterTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+SentimentDetectionJobFilterTypeDef = TypedDict(
+    "SentimentDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobFilterTypeDef = TypedDict(
+    "TopicsDetectionJobFilterTypeDef",
+    {
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
@@ -2172,24 +2223,14 @@
     "DetectPiiEntitiesResponseTypeDef",
     {
         "Entities": List[PiiEntityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestRequestTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 DocumentClassifierInputDataConfigTypeDef = TypedDict(
     "DocumentClassifierInputDataConfigTypeDef",
     {
         "DataFormat": DocumentClassifierDataFormatType,
         "S3Uri": str,
         "TestS3Uri": str,
         "LabelDelimiter": str,
@@ -2197,24 +2238,14 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestRequestTypeDef",
-    {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 DocumentClassifierInputDataConfigOutputTypeDef = TypedDict(
     "DocumentClassifierInputDataConfigOutputTypeDef",
     {
         "DataFormat": DocumentClassifierDataFormatType,
         "S3Uri": str,
         "TestS3Uri": str,
         "LabelDelimiter": str,
@@ -2222,14 +2253,17 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
+DocumentReaderConfigUnionTypeDef = Union[
+    DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
+]
 _RequiredInputDataConfigOutputTypeDef = TypedDict(
     "_RequiredInputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalInputDataConfigOutputTypeDef = TypedDict(
@@ -2237,19 +2271,21 @@
     {
         "InputFormat": InputFormatType,
         "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
+
 class InputDataConfigOutputTypeDef(
     _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
 ):
     pass
 
+
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2260,44 +2296,14 @@
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
-ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": DominantLanguageDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListEndpointsRequestRequestTypeDef = TypedDict(
-    "ListEndpointsRequestRequestTypeDef",
-    {
-        "Filter": EndpointFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 EntityRecognitionConfigOutputTypeDef = TypedDict(
     "EntityRecognitionConfigOutputTypeDef",
     {
         "EntityTypes": List[EntityTypesListItemTypeDef],
     },
 )
 
@@ -2322,20 +2328,22 @@
         "Annotations": EntityRecognizerAnnotationsTypeDef,
         "EntityList": EntityRecognizerEntityListTypeDef,
         "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
     },
     total=False,
 )
 
+
 class EntityRecognizerInputDataConfigOutputTypeDef(
     _RequiredEntityRecognizerInputDataConfigOutputTypeDef,
     _OptionalEntityRecognizerInputDataConfigOutputTypeDef,
 ):
     pass
 
+
 _RequiredEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 _OptionalEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2346,28 +2354,20 @@
         "Annotations": EntityRecognizerAnnotationsTypeDef,
         "EntityList": EntityRecognizerEntityListTypeDef,
         "AugmentedManifests": Sequence[AugmentedManifestsListItemTypeDef],
     },
     total=False,
 )
 
+
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
-ListEntityRecognizersRequestRequestTypeDef = TypedDict(
-    "ListEntityRecognizersRequestRequestTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
 
 EntityRecognizerMetadataEntityTypesListItemTypeDef = TypedDict(
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     {
         "Type": str,
         "EvaluationMetrics": EntityTypesEvaluationMetricsTypeDef,
         "NumberOfTrainMentions": int,
@@ -2380,56 +2380,14 @@
     {
         "EntityRecognizerSummariesList": List[EntityRecognizerSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListEventsDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": EventsDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListFlywheelsRequestRequestTypeDef = TypedDict(
-    "ListFlywheelsRequestRequestTypeDef",
-    {
-        "Filter": FlywheelFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-_RequiredListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredListFlywheelIterationHistoryRequestRequestTypeDef",
-    {
-        "FlywheelArn": str,
-    },
-)
-_OptionalListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalListFlywheelIterationHistoryRequestRequestTypeDef",
-    {
-        "Filter": FlywheelIterationFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListFlywheelIterationHistoryRequestRequestTypeDef(
-    _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
-    _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
-):
-    pass
-
 FlywheelIterationPropertiesTypeDef = TypedDict(
     "FlywheelIterationPropertiesTypeDef",
     {
         "FlywheelArn": str,
         "FlywheelIterationId": str,
         "CreationTime": datetime,
         "EndTime": datetime,
@@ -2458,168 +2416,27 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
-    TypedDict(
-        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-        {
-            "Filter": DominantLanguageDetectionJobFilterTypeDef,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    {
-        "Filter": EndpointFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
-    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
-    {
-        "Filter": SentimentDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListSentimentDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": SentimentDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": TargetedSentimentDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
-    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
-    {
-        "Filter": TopicsDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListTopicsDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": TopicsDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 SyntaxTokenTypeDef = TypedDict(
     "SyntaxTokenTypeDef",
     {
         "TokenId": int,
         "Text": str,
         "BeginOffset": int,
         "EndOffset": int,
         "PartOfSpeech": PartOfSpeechTagTypeDef,
     },
     total=False,
 )
 
+RedactionConfigUnionTypeDef = Union[RedactionConfigTypeDef, RedactionConfigOutputTypeDef]
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2688,20 +2505,22 @@
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "FlywheelArn": str,
     },
     total=False,
 )
 
+
 class StartDocumentClassificationJobRequestRequestTypeDef(
     _RequiredStartDocumentClassificationJobRequestRequestTypeDef,
     _OptionalStartDocumentClassificationJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2714,20 +2533,22 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartDominantLanguageDetectionJobRequestRequestTypeDef(
     _RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef,
     _OptionalStartDominantLanguageDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEntitiesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2743,20 +2564,22 @@
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "FlywheelArn": str,
     },
     total=False,
 )
 
+
 class StartEntitiesDetectionJobRequestRequestTypeDef(
     _RequiredStartEntitiesDetectionJobRequestRequestTypeDef,
     _OptionalStartEntitiesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartEventsDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEventsDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2769,20 +2592,22 @@
         "JobName": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartEventsDetectionJobRequestRequestTypeDef(
     _RequiredStartEventsDetectionJobRequestRequestTypeDef,
     _OptionalStartEventsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2796,20 +2621,22 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartKeyPhrasesDetectionJobRequestRequestTypeDef(
     _RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef,
     _OptionalStartKeyPhrasesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "Mode": PiiEntitiesDetectionModeType,
         "DataAccessRoleArn": str,
@@ -2823,20 +2650,22 @@
         "JobName": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartPiiEntitiesDetectionJobRequestRequestTypeDef(
     _RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef,
     _OptionalStartPiiEntitiesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSentimentDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2850,20 +2679,22 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartSentimentDetectionJobRequestRequestTypeDef(
     _RequiredStartSentimentDetectionJobRequestRequestTypeDef,
     _OptionalStartSentimentDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2877,20 +2708,22 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartTargetedSentimentDetectionJobRequestRequestTypeDef(
     _RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef,
     _OptionalStartTargetedSentimentDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartTopicsDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTopicsDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2904,20 +2737,22 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartTopicsDetectionJobRequestRequestTypeDef(
     _RequiredStartTopicsDetectionJobRequestRequestTypeDef,
     _OptionalStartTopicsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlywheelRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
 _OptionalUpdateFlywheelRequestRequestTypeDef = TypedDict(
@@ -2926,30 +2761,290 @@
         "ActiveModelArn": str,
         "DataAccessRoleArn": str,
         "DataSecurityConfig": UpdateDataSecurityConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFlywheelRequestRequestTypeDef(
     _RequiredUpdateFlywheelRequestRequestTypeDef, _OptionalUpdateFlywheelRequestRequestTypeDef
 ):
     pass
 
+
+DataSecurityConfigUnionTypeDef = Union[DataSecurityConfigTypeDef, DataSecurityConfigOutputTypeDef]
 DatasetInputDataConfigTypeDef = TypedDict(
     "DatasetInputDataConfigTypeDef",
     {
         "AugmentedManifests": Sequence[DatasetAugmentedManifestsListItemTypeDef],
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
     },
     total=False,
 )
 
+ListDatasetsRequestRequestTypeDef = TypedDict(
+    "ListDatasetsRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+        "Filter": DatasetFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestRequestTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestRequestTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
+    TypedDict(
+        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+        {
+            "Filter": DominantLanguageDetectionJobFilterTypeDef,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": DominantLanguageDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEndpointsRequestRequestTypeDef = TypedDict(
+    "ListEndpointsRequestRequestTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestRequestTypeDef = TypedDict(
+    "ListEntityRecognizersRequestRequestTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListEventsDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": EventsDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListFlywheelsRequestRequestTypeDef = TypedDict(
+    "ListFlywheelsRequestRequestTypeDef",
+    {
+        "Filter": FlywheelFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+_RequiredListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredListFlywheelIterationHistoryRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+    },
+)
+_OptionalListFlywheelIterationHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalListFlywheelIterationHistoryRequestRequestTypeDef",
+    {
+        "Filter": FlywheelIterationFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListFlywheelIterationHistoryRequestRequestTypeDef(
+    _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
+    _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
+):
+    pass
+
+
+ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": KeyPhrasesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": PiiEntitiesDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
+    "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
+    {
+        "Filter": SentimentDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListSentimentDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": SentimentDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": TargetedSentimentDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
+    "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
+    {
+        "Filter": TopicsDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListTopicsDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": TopicsDetectionJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentClassifierRequestRequestTypeDef",
     {
         "DocumentClassifierName": str,
         "DataAccessRoleArn": str,
         "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
@@ -2967,20 +3062,25 @@
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "ModelPolicy": str,
     },
     total=False,
 )
 
+
 class CreateDocumentClassifierRequestRequestTypeDef(
     _RequiredCreateDocumentClassifierRequestRequestTypeDef,
     _OptionalCreateDocumentClassifierRequestRequestTypeDef,
 ):
     pass
 
+
+DocumentClassifierInputDataConfigUnionTypeDef = Union[
+    DocumentClassifierInputDataConfigTypeDef, DocumentClassifierInputDataConfigOutputTypeDef
+]
 DocumentClassifierPropertiesTypeDef = TypedDict(
     "DocumentClassifierPropertiesTypeDef",
     {
         "DocumentClassifierArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
@@ -3080,14 +3180,15 @@
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "TargetEventTypes": List[str],
     },
     total=False,
 )
 
+InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
 KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
     "KeyPhrasesDetectionJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
@@ -3208,17 +3309,19 @@
     {
         "DocumentClassificationConfig": DocumentClassificationConfigOutputTypeDef,
         "EntityRecognitionConfig": EntityRecognitionConfigOutputTypeDef,
     },
     total=False,
 )
 
+
 class TaskConfigOutputTypeDef(_RequiredTaskConfigOutputTypeDef, _OptionalTaskConfigOutputTypeDef):
     pass
 
+
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
     },
 )
 _OptionalTaskConfigTypeDef = TypedDict(
@@ -3226,17 +3329,19 @@
     {
         "DocumentClassificationConfig": DocumentClassificationConfigTypeDef,
         "EntityRecognitionConfig": EntityRecognitionConfigTypeDef,
     },
     total=False,
 )
 
+
 class TaskConfigTypeDef(_RequiredTaskConfigTypeDef, _OptionalTaskConfigTypeDef):
     pass
 
+
 _RequiredCreateEntityRecognizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRecognizerRequestRequestTypeDef",
     {
         "RecognizerName": str,
         "DataAccessRoleArn": str,
         "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
@@ -3252,20 +3357,25 @@
         "VpcConfig": VpcConfigTypeDef,
         "ModelKmsKeyId": str,
         "ModelPolicy": str,
     },
     total=False,
 )
 
+
 class CreateEntityRecognizerRequestRequestTypeDef(
     _RequiredCreateEntityRecognizerRequestRequestTypeDef,
     _OptionalCreateEntityRecognizerRequestRequestTypeDef,
 ):
     pass
 
+
+EntityRecognizerInputDataConfigUnionTypeDef = Union[
+    EntityRecognizerInputDataConfigTypeDef, EntityRecognizerInputDataConfigOutputTypeDef
+]
 EntityRecognizerMetadataTypeDef = TypedDict(
     "EntityRecognizerMetadataTypeDef",
     {
         "NumberOfTrainedDocuments": int,
         "NumberOfTestDocuments": int,
         "EvaluationMetrics": EntityRecognizerEvaluationMetricsTypeDef,
         "EntityTypes": List[EntityRecognizerMetadataEntityTypesListItemTypeDef],
@@ -3353,19 +3463,21 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 DescribeDocumentClassifierResponseTypeDef = TypedDict(
     "DescribeDocumentClassifierResponseTypeDef",
     {
         "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3572,19 +3684,22 @@
         "DataSecurityConfig": DataSecurityConfigTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateFlywheelRequestRequestTypeDef(
     _RequiredCreateFlywheelRequestRequestTypeDef, _OptionalCreateFlywheelRequestRequestTypeDef
 ):
     pass
 
+
+TaskConfigUnionTypeDef = Union[TaskConfigTypeDef, TaskConfigOutputTypeDef]
 EntityRecognizerPropertiesTypeDef = TypedDict(
     "EntityRecognizerPropertiesTypeDef",
     {
         "EntityRecognizerArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
```

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend.egg-info/PKG-INFO` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehend
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Comprehend 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Comprehend 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 comprehend type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 comprehend type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehend)](https://pepy.tech/project/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
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
@@ -389,20 +389,20 @@
 )
 
 
 def check_value(value: AugmentedManifestsDocumentTypeFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_comprehend.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_comprehend.type_defs import (
     AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
@@ -411,14 +411,15 @@
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
+    BlobTypeDef,
     ChildBlockTypeDef,
     RelationshipsListItemTypeDef,
     BoundingBoxTypeDef,
     ClassifierEvaluationMetricsTypeDef,
     DocumentReaderConfigTypeDef,
     DocumentClassTypeDef,
     DocumentLabelTypeDef,
@@ -432,15 +433,15 @@
     VpcConfigTypeDef,
     VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
-    DatasetFilterTypeDef,
+    TimestampTypeDef,
     DatasetPropertiesTypeDef,
     DeleteDocumentClassifierRequestRequestTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEntityRecognizerRequestRequestTypeDef,
     DeleteFlywheelRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
@@ -465,48 +466,34 @@
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
     DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
-    DocumentClassificationJobFilterTypeDef,
     OutputDataConfigTypeDef,
     DocumentClassifierDocumentsTypeDef,
-    DocumentClassifierFilterTypeDef,
     DocumentReaderConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
-    DominantLanguageDetectionJobFilterTypeDef,
-    EndpointFilterTypeDef,
-    EntitiesDetectionJobFilterTypeDef,
     EntityTypesListItemTypeDef,
     EntityRecognizerAnnotationsTypeDef,
     EntityRecognizerDocumentsTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
-    EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
-    EventsDetectionJobFilterTypeDef,
-    FlywheelFilterTypeDef,
-    FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
-    KeyPhrasesDetectionJobFilterTypeDef,
     PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
-    PiiEntitiesDetectionJobFilterTypeDef,
-    SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TargetedSentimentDetectionJobFilterTypeDef,
-    TopicsDetectionJobFilterTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
     RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RedactionConfigTypeDef,
     StartFlywheelIterationRequestRequestTypeDef,
     StopDominantLanguageDetectionJobRequestRequestTypeDef,
@@ -562,60 +549,53 @@
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
     DataSecurityConfigOutputTypeDef,
+    VpcConfigUnionTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
-    ListDatasetsRequestRequestTypeDef,
+    DatasetFilterTypeDef,
+    DocumentClassificationJobFilterTypeDef,
+    DocumentClassifierFilterTypeDef,
+    DominantLanguageDetectionJobFilterTypeDef,
+    EndpointFilterTypeDef,
+    EntitiesDetectionJobFilterTypeDef,
+    EntityRecognizerFilterTypeDef,
+    EventsDetectionJobFilterTypeDef,
+    FlywheelFilterTypeDef,
+    FlywheelIterationFilterTypeDef,
+    KeyPhrasesDetectionJobFilterTypeDef,
+    PiiEntitiesDetectionJobFilterTypeDef,
+    SentimentDetectionJobFilterTypeDef,
+    TargetedSentimentDetectionJobFilterTypeDef,
+    TopicsDetectionJobFilterTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
-    ListDocumentClassificationJobsRequestRequestTypeDef,
     DocumentClassifierInputDataConfigTypeDef,
-    ListDocumentClassifiersRequestRequestTypeDef,
     DocumentClassifierInputDataConfigOutputTypeDef,
+    DocumentReaderConfigUnionTypeDef,
     InputDataConfigOutputTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
-    ListDominantLanguageDetectionJobsRequestRequestTypeDef,
-    ListEndpointsRequestRequestTypeDef,
-    ListEntitiesDetectionJobsRequestRequestTypeDef,
     EntityRecognitionConfigOutputTypeDef,
     EntityRecognitionConfigTypeDef,
     EntityRecognizerInputDataConfigOutputTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
-    ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
-    ListEventsDetectionJobsRequestRequestTypeDef,
-    ListFlywheelsRequestRequestTypeDef,
-    ListFlywheelIterationHistoryRequestRequestTypeDef,
     FlywheelIterationPropertiesTypeDef,
     ListFlywheelsResponseTypeDef,
     GeometryTypeDef,
-    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
-    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
-    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
-    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
-    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
-    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
-    ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
-    ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
-    ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
-    ListSentimentDetectionJobsRequestRequestTypeDef,
-    ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
-    ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
-    ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
+    RedactionConfigUnionTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     TargetedSentimentMentionTypeDef,
     EntityTypeDef,
     StartDocumentClassificationJobRequestRequestTypeDef,
     StartDominantLanguageDetectionJobRequestRequestTypeDef,
@@ -623,30 +603,59 @@
     StartEventsDetectionJobRequestRequestTypeDef,
     StartKeyPhrasesDetectionJobRequestRequestTypeDef,
     StartPiiEntitiesDetectionJobRequestRequestTypeDef,
     StartSentimentDetectionJobRequestRequestTypeDef,
     StartTargetedSentimentDetectionJobRequestRequestTypeDef,
     StartTopicsDetectionJobRequestRequestTypeDef,
     UpdateFlywheelRequestRequestTypeDef,
+    DataSecurityConfigUnionTypeDef,
     DatasetInputDataConfigTypeDef,
+    ListDatasetsRequestRequestTypeDef,
+    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
+    ListDocumentClassificationJobsRequestRequestTypeDef,
+    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
+    ListDocumentClassifiersRequestRequestTypeDef,
+    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
+    ListDominantLanguageDetectionJobsRequestRequestTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    ListEndpointsRequestRequestTypeDef,
+    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
+    ListEntitiesDetectionJobsRequestRequestTypeDef,
+    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
+    ListEntityRecognizersRequestRequestTypeDef,
+    ListEventsDetectionJobsRequestRequestTypeDef,
+    ListFlywheelsRequestRequestTypeDef,
+    ListFlywheelIterationHistoryRequestRequestTypeDef,
+    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
+    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
+    ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
+    ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
+    ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
+    ListSentimentDetectionJobsRequestRequestTypeDef,
+    ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
+    ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
+    ListTopicsDetectionJobsRequestRequestTypeDef,
     CreateDocumentClassifierRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigUnionTypeDef,
     DocumentClassifierPropertiesTypeDef,
     DocumentClassificationJobPropertiesTypeDef,
     DominantLanguageDetectionJobPropertiesTypeDef,
     EntitiesDetectionJobPropertiesTypeDef,
     EventsDetectionJobPropertiesTypeDef,
+    InputDataConfigUnionTypeDef,
     KeyPhrasesDetectionJobPropertiesTypeDef,
     PiiEntitiesDetectionJobPropertiesTypeDef,
     SentimentDetectionJobPropertiesTypeDef,
     TargetedSentimentDetectionJobPropertiesTypeDef,
     TopicsDetectionJobPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
     TaskConfigOutputTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
+    EntityRecognizerInputDataConfigUnionTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
@@ -670,29 +679,30 @@
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     FlywheelPropertiesTypeDef,
     CreateFlywheelRequestRequestTypeDef,
+    TaskConfigUnionTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     DescribeFlywheelResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
     DescribeEntityRecognizerResponseTypeDef,
     ListEntityRecognizersResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
 )
 
 
-def get_structure() -> AugmentedManifestsListItemOutputTypeDef:
+def get_value() -> AugmentedManifestsListItemOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-comprehend-1.28.15.post1/mypy_boto3_comprehend.egg-info/SOURCES.txt` & `mypy-boto3-comprehend-1.28.16/mypy_boto3_comprehend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.15.post1/setup.py` & `mypy-boto3-comprehend-1.28.16/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehend",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_comprehend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Comprehend 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Comprehend 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 comprehend type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 comprehend type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_comprehend": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

