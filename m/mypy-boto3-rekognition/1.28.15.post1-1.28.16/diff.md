# Comparing `tmp/mypy-boto3-rekognition-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-rekognition-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rekognition-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:59 2023, max compression
+gzip compressed data, was "mypy-boto3-rekognition-1.28.16.tar", last modified: Tue Aug  1 11:37:39 2023, max compression
```

## Comparing `mypy-boto3-rekognition-1.28.15.post1.tar` & `mypy-boto3-rekognition-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.141358 mypy-boto3-rekognition-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26562 2023-07-29 10:03:59.141358 mypy-boto3-rekognition-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.125358 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57868 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57778 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-29 09:56:53.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98551 2023-07-29 09:56:55.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98430 2023-07-29 09:56:54.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.141358 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26562 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:59.141358 mypy-boto3-rekognition-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:56:51.000000 mypy-boto3-rekognition-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:39.060773 mypy-boto3-rekognition-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26703 2023-08-01 11:37:39.060773 mypy-boto3-rekognition-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25203 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:39.040773 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57536 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57446 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-08-01 11:30:15.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98968 2023-08-01 11:30:21.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98847 2023-08-01 11:30:16.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:39.060773 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26703 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:39.060773 mypy-boto3-rekognition-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/setup.py
```

### Comparing `mypy-boto3-rekognition-1.28.15.post1/LICENSE` & `mypy-boto3-rekognition-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/PKG-INFO` & `mypy-boto3-rekognition-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Rekognition 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rekognition type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 rekognition type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -416,33 +416,34 @@
 )
 
 
 def check_value(value: AttributeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rekognition.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
     ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
     BoundingBoxTypeDef,
     S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
+    BlobTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
@@ -453,15 +454,14 @@
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
     LivenessOutputConfigTypeDef,
     CreateProjectRequestRequestTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     CreateUserRequestRequestTypeDef,
-    DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
     UnsuccessfulFaceDeletionTypeDef,
@@ -575,26 +575,26 @@
     StartTextDetectionResponseTypeDef,
     StopProjectVersionResponseTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
     GroundTruthManifestTypeDef,
-    ImageTypeDef,
     SummaryTypeDef,
     VideoTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
+    DatasetChangesTypeDef,
+    ImageTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
     CreateFaceLivenessSessionRequestSettingsTypeDef,
-    UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
     DeleteFacesResponseTypeDef,
     DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
     DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     ListCollectionsRequestListCollectionsPaginateTypeDef,
@@ -630,29 +630,30 @@
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
     AssetTypeDef,
     DatasetSourceTypeDef,
+    EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
+    StartSegmentDetectionFiltersTypeDef,
+    UpdateDatasetEntriesRequestRequestTypeDef,
     CompareFacesRequestRequestTypeDef,
     DetectCustomLabelsRequestRequestTypeDef,
     DetectFacesRequestRequestTypeDef,
     DetectProtectiveEquipmentRequestRequestTypeDef,
     IndexFacesRequestRequestTypeDef,
     RecognizeCelebritiesRequestRequestTypeDef,
     SearchFacesByImageRequestRequestTypeDef,
     SearchUsersByImageRequestRequestTypeDef,
-    EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
-    StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
@@ -665,23 +666,23 @@
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
     DetectTextFiltersTypeDef,
+    RegionOfInterestUnionTypeDef,
     StartTextDetectionFiltersTypeDef,
-    UpdateStreamProcessorRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
     SearchUsersResponseTypeDef,
-    CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     TestingDataOutputTypeDef,
     TestingDataTypeDef,
     TrainingDataOutputTypeDef,
@@ -700,30 +701,34 @@
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
     DetectTextRequestRequestTypeDef,
+    CreateStreamProcessorRequestRequestTypeDef,
+    UpdateStreamProcessorRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
+    TestingDataUnionTypeDef,
     CreateProjectVersionRequestRequestTypeDef,
+    TrainingDataUnionTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
-def get_structure() -> AgeRangeTypeDef:
+def get_value() -> AgeRangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rekognition-1.28.15.post1/README.md` & `mypy-boto3-rekognition-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -384,33 +384,34 @@
 )
 
 
 def check_value(value: AttributeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rekognition.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
     ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
     BoundingBoxTypeDef,
     S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
+    BlobTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
@@ -421,15 +422,14 @@
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
     LivenessOutputConfigTypeDef,
     CreateProjectRequestRequestTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     CreateUserRequestRequestTypeDef,
-    DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
     UnsuccessfulFaceDeletionTypeDef,
@@ -543,26 +543,26 @@
     StartTextDetectionResponseTypeDef,
     StopProjectVersionResponseTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
     GroundTruthManifestTypeDef,
-    ImageTypeDef,
     SummaryTypeDef,
     VideoTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
+    DatasetChangesTypeDef,
+    ImageTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
     CreateFaceLivenessSessionRequestSettingsTypeDef,
-    UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
     DeleteFacesResponseTypeDef,
     DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
     DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     ListCollectionsRequestListCollectionsPaginateTypeDef,
@@ -598,29 +598,30 @@
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
     AssetTypeDef,
     DatasetSourceTypeDef,
+    EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
+    StartSegmentDetectionFiltersTypeDef,
+    UpdateDatasetEntriesRequestRequestTypeDef,
     CompareFacesRequestRequestTypeDef,
     DetectCustomLabelsRequestRequestTypeDef,
     DetectFacesRequestRequestTypeDef,
     DetectProtectiveEquipmentRequestRequestTypeDef,
     IndexFacesRequestRequestTypeDef,
     RecognizeCelebritiesRequestRequestTypeDef,
     SearchFacesByImageRequestRequestTypeDef,
     SearchUsersByImageRequestRequestTypeDef,
-    EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
-    StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
@@ -633,23 +634,23 @@
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
     DetectTextFiltersTypeDef,
+    RegionOfInterestUnionTypeDef,
     StartTextDetectionFiltersTypeDef,
-    UpdateStreamProcessorRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
     SearchUsersResponseTypeDef,
-    CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     TestingDataOutputTypeDef,
     TestingDataTypeDef,
     TrainingDataOutputTypeDef,
@@ -668,30 +669,34 @@
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
     DetectTextRequestRequestTypeDef,
+    CreateStreamProcessorRequestRequestTypeDef,
+    UpdateStreamProcessorRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
+    TestingDataUnionTypeDef,
     CreateProjectVersionRequestRequestTypeDef,
+    TrainingDataUnionTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
-def get_structure() -> AgeRangeTypeDef:
+def get_value() -> AgeRangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__init__.py` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__init__.pyi` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__main__.py` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Rekognition 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Rekognition 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
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

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/client.py` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_rekognition.client import RekognitionClient
 
     session = Session()
     client: RekognitionClient = session.client("rekognition")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AttributeType,
     CelebrityRecognitionSortByType,
     ContentModerationAggregateByType,
@@ -100,16 +100,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
-    RegionOfInterestOutputTypeDef,
-    RegionOfInterestTypeDef,
+    RegionOfInterestUnionTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
@@ -126,20 +125,17 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
-    StreamProcessorSettingsOutputTypeDef,
-    StreamProcessorSettingsTypeDef,
-    TestingDataOutputTypeDef,
-    TestingDataTypeDef,
-    TrainingDataOutputTypeDef,
-    TrainingDataTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
+    TestingDataUnionTypeDef,
+    TrainingDataUnionTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -315,16 +311,16 @@
 
     def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: Union[TrainingDataTypeDef, TrainingDataOutputTypeDef] = ...,
-        TestingData: Union[TestingDataTypeDef, TestingDataOutputTypeDef] = ...,
+        TrainingData: TrainingDataUnionTypeDef = ...,
+        TestingData: TestingDataUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -333,22 +329,20 @@
 
     def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: Union[StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef],
+        Settings: StreamProcessorSettingsUnionTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[
-            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
-        ] = ...,
+        RegionsOfInterest: Sequence[RegionOfInterestUnionTypeDef] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -1138,17 +1132,15 @@
         """
 
     def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[
-            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
-        ] = ...,
+        RegionsOfInterestForUpdate: Sequence[RegionOfInterestUnionTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
```

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/client.pyi` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_rekognition.client import RekognitionClient
 
     session = Session()
     client: RekognitionClient = session.client("rekognition")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AttributeType,
     CelebrityRecognitionSortByType,
     ContentModerationAggregateByType,
@@ -100,16 +100,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
-    RegionOfInterestOutputTypeDef,
-    RegionOfInterestTypeDef,
+    RegionOfInterestUnionTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
@@ -126,20 +125,17 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
-    StreamProcessorSettingsOutputTypeDef,
-    StreamProcessorSettingsTypeDef,
-    TestingDataOutputTypeDef,
-    TestingDataTypeDef,
-    TrainingDataOutputTypeDef,
-    TrainingDataTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
+    TestingDataUnionTypeDef,
+    TrainingDataUnionTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -301,16 +297,16 @@
         """
     def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: Union[TrainingDataTypeDef, TrainingDataOutputTypeDef] = ...,
-        TestingData: Union[TestingDataTypeDef, TestingDataOutputTypeDef] = ...,
+        TrainingData: TrainingDataUnionTypeDef = ...,
+        TestingData: TestingDataUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -318,22 +314,20 @@
         """
     def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: Union[StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef],
+        Settings: StreamProcessorSettingsUnionTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[
-            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
-        ] = ...,
+        RegionsOfInterest: Sequence[RegionOfInterestUnionTypeDef] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -1059,17 +1053,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#update_dataset_entries)
         """
     def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[
-            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
-        ] = ...,
+        RegionsOfInterestForUpdate: Sequence[RegionOfInterestUnionTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
```

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/literals.py` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/literals.pyi` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/paginator.py` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/paginator.pyi` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/type_defs.py` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_rekognition.type_defs import AgeRangeTypeDef
 
-    data: AgeRangeTypeDef = {...}
+    data: AgeRangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -75,14 +75,15 @@
     "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
     "BoundingBoxTypeDef",
     "S3ObjectTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
+    "BlobTypeDef",
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
@@ -93,15 +94,14 @@
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "LivenessOutputConfigTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "DatasetChangesTypeDef",
     "DatasetStatsTypeDef",
     "DatasetLabelStatsTypeDef",
     "DatasetMetadataTypeDef",
     "DeleteCollectionRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteFacesRequestRequestTypeDef",
     "UnsuccessfulFaceDeletionTypeDef",
@@ -215,26 +215,26 @@
     "StartTextDetectionResponseTypeDef",
     "StopProjectVersionResponseTypeDef",
     "AssociateFacesResponseTypeDef",
     "ComparedSourceImageFaceTypeDef",
     "FaceTypeDef",
     "AuditImageTypeDef",
     "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
     "SummaryTypeDef",
     "VideoTypeDef",
     "StartTechnicalCueDetectionFilterTypeDef",
+    "DatasetChangesTypeDef",
+    "ImageTypeDef",
     "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
     "CreateFaceLivenessSessionRequestSettingsTypeDef",
-    "UpdateDatasetEntriesRequestRequestTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetLabelDescriptionTypeDef",
     "ProjectDescriptionTypeDef",
     "DeleteFacesResponseTypeDef",
     "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
     "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     "ListCollectionsRequestListCollectionsPaginateTypeDef",
@@ -270,29 +270,30 @@
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
     "GetFaceLivenessSessionResultsResponseTypeDef",
     "AssetTypeDef",
     "DatasetSourceTypeDef",
+    "EvaluationResultTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
+    "StartSegmentDetectionFiltersTypeDef",
+    "UpdateDatasetEntriesRequestRequestTypeDef",
     "CompareFacesRequestRequestTypeDef",
     "DetectCustomLabelsRequestRequestTypeDef",
     "DetectFacesRequestRequestTypeDef",
     "DetectProtectiveEquipmentRequestRequestTypeDef",
     "IndexFacesRequestRequestTypeDef",
     "RecognizeCelebritiesRequestRequestTypeDef",
     "SearchFacesByImageRequestRequestTypeDef",
     "SearchUsersByImageRequestRequestTypeDef",
-    "EvaluationResultTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
-    "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
     "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
@@ -305,23 +306,23 @@
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
+    "StreamProcessorSettingsUnionTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
+    "RegionOfInterestUnionTypeDef",
     "StartTextDetectionFiltersTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
-    "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
     "TestingDataOutputTypeDef",
     "TestingDataTypeDef",
     "TrainingDataOutputTypeDef",
@@ -340,16 +341,20 @@
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
+    "CreateStreamProcessorRequestRequestTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
+    "TestingDataUnionTypeDef",
     "CreateProjectVersionRequestRequestTypeDef",
+    "TrainingDataUnionTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
@@ -467,14 +472,15 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
     },
     total=False,
 )
@@ -686,21 +692,14 @@
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
 
-DatasetChangesTypeDef = TypedDict(
-    "DatasetChangesTypeDef",
-    {
-        "GroundTruth": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 DatasetStatsTypeDef = TypedDict(
     "DatasetStatsTypeDef",
     {
         "LabeledEntries": int,
         "TotalEntries": int,
         "TotalLabels": int,
         "ErrorEntries": int,
@@ -2057,23 +2056,14 @@
     "GroundTruthManifestTypeDef",
     {
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
 SummaryTypeDef = TypedDict(
     "SummaryTypeDef",
     {
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
@@ -2091,14 +2081,30 @@
     {
         "MinSegmentConfidence": float,
         "BlackFrame": BlackFrameTypeDef,
     },
     total=False,
 )
 
+DatasetChangesTypeDef = TypedDict(
+    "DatasetChangesTypeDef",
+    {
+        "GroundTruth": BlobTypeDef,
+    },
+)
+
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
+    {
+        "Bytes": BlobTypeDef,
+        "S3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
 GetCelebrityInfoResponseTypeDef = TypedDict(
     "GetCelebrityInfoResponseTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "KnownGender": KnownGenderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2182,22 +2188,14 @@
     {
         "OutputConfig": LivenessOutputConfigTypeDef,
         "AuditImagesLimit": int,
     },
     total=False,
 )
 
-UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
-    "UpdateDatasetEntriesRequestRequestTypeDef",
-    {
-        "DatasetArn": str,
-        "Changes": DatasetChangesTypeDef,
-    },
-)
-
 DatasetDescriptionTypeDef = TypedDict(
     "DatasetDescriptionTypeDef",
     {
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
@@ -2735,14 +2733,163 @@
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
         "DatasetArn": str,
     },
     total=False,
 )
 
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
+    {
+        "F1Score": float,
+        "Summary": SummaryTypeDef,
+    },
+    total=False,
+)
+
+_RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCelebrityRecognitionRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartCelebrityRecognitionRequestRequestTypeDef(
+    _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
+    _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartContentModerationRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartContentModerationRequestRequestTypeDef",
+    {
+        "MinConfidence": float,
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartContentModerationRequestRequestTypeDef(
+    _RequiredStartContentModerationRequestRequestTypeDef,
+    _OptionalStartContentModerationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFaceDetectionRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFaceDetectionRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "FaceAttributes": FaceAttributesType,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartFaceDetectionRequestRequestTypeDef(
+    _RequiredStartFaceDetectionRequestRequestTypeDef,
+    _OptionalStartFaceDetectionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFaceSearchRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+        "CollectionId": str,
+    },
+)
+_OptionalStartFaceSearchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFaceSearchRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "FaceMatchThreshold": float,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartFaceSearchRequestRequestTypeDef(
+    _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
+):
+    pass
+
+
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
+    "UpdateDatasetEntriesRequestRequestTypeDef",
+    {
+        "DatasetArn": str,
+        "Changes": DatasetChangesTypeDef,
+    },
+)
+
 _RequiredCompareFacesRequestRequestTypeDef = TypedDict(
     "_RequiredCompareFacesRequestRequestTypeDef",
     {
         "SourceImage": ImageTypeDef,
         "TargetImage": ImageTypeDef,
     },
 )
@@ -2907,155 +3054,14 @@
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
 
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
-    {
-        "F1Score": float,
-        "Summary": SummaryTypeDef,
-    },
-    total=False,
-)
-
-_RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartCelebrityRecognitionRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartCelebrityRecognitionRequestRequestTypeDef(
-    _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
-    _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartContentModerationRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartContentModerationRequestRequestTypeDef",
-    {
-        "MinConfidence": float,
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartContentModerationRequestRequestTypeDef(
-    _RequiredStartContentModerationRequestRequestTypeDef,
-    _OptionalStartContentModerationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFaceDetectionRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFaceDetectionRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "FaceAttributes": FaceAttributesType,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartFaceDetectionRequestRequestTypeDef(
-    _RequiredStartFaceDetectionRequestRequestTypeDef,
-    _OptionalStartFaceDetectionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFaceSearchRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-        "CollectionId": str,
-    },
-)
-_OptionalStartFaceSearchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFaceSearchRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "FaceMatchThreshold": float,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartFaceSearchRequestRequestTypeDef(
-    _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
-):
-    pass
-
-
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
 CelebrityTypeDef = TypedDict(
     "CelebrityTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "Id": str,
         "Face": ComparedFaceTypeDef,
@@ -3285,14 +3291,17 @@
     {
         "FaceDetails": FaceDetailTypeDef,
         "Reasons": List[UnsearchedFaceReasonType],
     },
     total=False,
 )
 
+StreamProcessorSettingsUnionTypeDef = Union[
+    StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef
+]
 CustomLabelTypeDef = TypedDict(
     "CustomLabelTypeDef",
     {
         "Name": str,
         "Confidence": float,
         "Geometry": GeometryTypeDef,
     },
@@ -3317,50 +3326,24 @@
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
+RegionOfInterestUnionTypeDef = Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
 StartTextDetectionFiltersTypeDef = TypedDict(
     "StartTextDetectionFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[
-            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
-        ],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
-    },
-    total=False,
-)
-
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -3410,46 +3393,14 @@
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceTypeDef,
         "SearchedUser": SearchedUserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Input": StreamProcessorInputTypeDef,
-        "Output": StreamProcessorOutputTypeDef,
-        "Name": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
-        "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[
-            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
-        ],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateStreamProcessorRequestRequestTypeDef(
-    _RequiredCreateStreamProcessorRequestRequestTypeDef,
-    _OptionalCreateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
@@ -3759,14 +3710,69 @@
 
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Input": StreamProcessorInputTypeDef,
+        "Output": StreamProcessorOutputTypeDef,
+        "Name": str,
+        "Settings": StreamProcessorSettingsTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "KmsKeyId": str,
+        "RegionsOfInterest": Sequence[RegionOfInterestUnionTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateStreamProcessorRequestRequestTypeDef(
+    _RequiredCreateStreamProcessorRequestRequestTypeDef,
+    _OptionalCreateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestUnionTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartTextDetectionRequestRequestTypeDef = TypedDict(
@@ -3784,14 +3790,15 @@
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
 
+TestingDataUnionTypeDef = Union[TestingDataTypeDef, TestingDataOutputTypeDef]
 _RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "VersionName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
@@ -3811,14 +3818,15 @@
 class CreateProjectVersionRequestRequestTypeDef(
     _RequiredCreateProjectVersionRequestRequestTypeDef,
     _OptionalCreateProjectVersionRequestRequestTypeDef,
 ):
     pass
 
 
+TrainingDataUnionTypeDef = Union[TrainingDataTypeDef, TrainingDataOutputTypeDef]
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
         "Input": TestingDataOutputTypeDef,
         "Output": TestingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
```

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/type_defs.pyi` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_rekognition.type_defs import AgeRangeTypeDef
 
-    data: AgeRangeTypeDef = {...}
+    data: AgeRangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -74,14 +74,15 @@
     "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
     "BoundingBoxTypeDef",
     "S3ObjectTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
+    "BlobTypeDef",
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
@@ -92,15 +93,14 @@
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "LivenessOutputConfigTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "DatasetChangesTypeDef",
     "DatasetStatsTypeDef",
     "DatasetLabelStatsTypeDef",
     "DatasetMetadataTypeDef",
     "DeleteCollectionRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteFacesRequestRequestTypeDef",
     "UnsuccessfulFaceDeletionTypeDef",
@@ -214,26 +214,26 @@
     "StartTextDetectionResponseTypeDef",
     "StopProjectVersionResponseTypeDef",
     "AssociateFacesResponseTypeDef",
     "ComparedSourceImageFaceTypeDef",
     "FaceTypeDef",
     "AuditImageTypeDef",
     "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
     "SummaryTypeDef",
     "VideoTypeDef",
     "StartTechnicalCueDetectionFilterTypeDef",
+    "DatasetChangesTypeDef",
+    "ImageTypeDef",
     "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
     "CreateFaceLivenessSessionRequestSettingsTypeDef",
-    "UpdateDatasetEntriesRequestRequestTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetLabelDescriptionTypeDef",
     "ProjectDescriptionTypeDef",
     "DeleteFacesResponseTypeDef",
     "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
     "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     "ListCollectionsRequestListCollectionsPaginateTypeDef",
@@ -269,29 +269,30 @@
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
     "GetFaceLivenessSessionResultsResponseTypeDef",
     "AssetTypeDef",
     "DatasetSourceTypeDef",
+    "EvaluationResultTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
+    "StartSegmentDetectionFiltersTypeDef",
+    "UpdateDatasetEntriesRequestRequestTypeDef",
     "CompareFacesRequestRequestTypeDef",
     "DetectCustomLabelsRequestRequestTypeDef",
     "DetectFacesRequestRequestTypeDef",
     "DetectProtectiveEquipmentRequestRequestTypeDef",
     "IndexFacesRequestRequestTypeDef",
     "RecognizeCelebritiesRequestRequestTypeDef",
     "SearchFacesByImageRequestRequestTypeDef",
     "SearchUsersByImageRequestRequestTypeDef",
-    "EvaluationResultTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
-    "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
     "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
@@ -304,23 +305,23 @@
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
+    "StreamProcessorSettingsUnionTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
+    "RegionOfInterestUnionTypeDef",
     "StartTextDetectionFiltersTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
-    "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
     "TestingDataOutputTypeDef",
     "TestingDataTypeDef",
     "TrainingDataOutputTypeDef",
@@ -339,16 +340,20 @@
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
+    "CreateStreamProcessorRequestRequestTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
+    "TestingDataUnionTypeDef",
     "CreateProjectVersionRequestRequestTypeDef",
+    "TrainingDataUnionTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
@@ -464,14 +469,15 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
     },
     total=False,
 )
@@ -673,21 +679,14 @@
 )
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-DatasetChangesTypeDef = TypedDict(
-    "DatasetChangesTypeDef",
-    {
-        "GroundTruth": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 DatasetStatsTypeDef = TypedDict(
     "DatasetStatsTypeDef",
     {
         "LabeledEntries": int,
         "TotalEntries": int,
         "TotalLabels": int,
         "ErrorEntries": int,
@@ -2002,23 +2001,14 @@
     "GroundTruthManifestTypeDef",
     {
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
 SummaryTypeDef = TypedDict(
     "SummaryTypeDef",
     {
         "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
@@ -2036,14 +2026,30 @@
     {
         "MinSegmentConfidence": float,
         "BlackFrame": BlackFrameTypeDef,
     },
     total=False,
 )
 
+DatasetChangesTypeDef = TypedDict(
+    "DatasetChangesTypeDef",
+    {
+        "GroundTruth": BlobTypeDef,
+    },
+)
+
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
+    {
+        "Bytes": BlobTypeDef,
+        "S3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
 GetCelebrityInfoResponseTypeDef = TypedDict(
     "GetCelebrityInfoResponseTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "KnownGender": KnownGenderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2125,22 +2131,14 @@
     {
         "OutputConfig": LivenessOutputConfigTypeDef,
         "AuditImagesLimit": int,
     },
     total=False,
 )
 
-UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
-    "UpdateDatasetEntriesRequestRequestTypeDef",
-    {
-        "DatasetArn": str,
-        "Changes": DatasetChangesTypeDef,
-    },
-)
-
 DatasetDescriptionTypeDef = TypedDict(
     "DatasetDescriptionTypeDef",
     {
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
@@ -2660,14 +2658,153 @@
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
         "DatasetArn": str,
     },
     total=False,
 )
 
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
+    {
+        "F1Score": float,
+        "Summary": SummaryTypeDef,
+    },
+    total=False,
+)
+
+_RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCelebrityRecognitionRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartCelebrityRecognitionRequestRequestTypeDef(
+    _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
+    _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartContentModerationRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartContentModerationRequestRequestTypeDef",
+    {
+        "MinConfidence": float,
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartContentModerationRequestRequestTypeDef(
+    _RequiredStartContentModerationRequestRequestTypeDef,
+    _OptionalStartContentModerationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFaceDetectionRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFaceDetectionRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "FaceAttributes": FaceAttributesType,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartFaceDetectionRequestRequestTypeDef(
+    _RequiredStartFaceDetectionRequestRequestTypeDef,
+    _OptionalStartFaceDetectionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFaceSearchRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+        "CollectionId": str,
+    },
+)
+_OptionalStartFaceSearchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFaceSearchRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "FaceMatchThreshold": float,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartFaceSearchRequestRequestTypeDef(
+    _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
+):
+    pass
+
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
+):
+    pass
+
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
+    "UpdateDatasetEntriesRequestRequestTypeDef",
+    {
+        "DatasetArn": str,
+        "Changes": DatasetChangesTypeDef,
+    },
+)
+
 _RequiredCompareFacesRequestRequestTypeDef = TypedDict(
     "_RequiredCompareFacesRequestRequestTypeDef",
     {
         "SourceImage": ImageTypeDef,
         "TargetImage": ImageTypeDef,
     },
 )
@@ -2818,145 +2955,14 @@
 
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
-    {
-        "F1Score": float,
-        "Summary": SummaryTypeDef,
-    },
-    total=False,
-)
-
-_RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartCelebrityRecognitionRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartCelebrityRecognitionRequestRequestTypeDef(
-    _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
-    _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartContentModerationRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartContentModerationRequestRequestTypeDef",
-    {
-        "MinConfidence": float,
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartContentModerationRequestRequestTypeDef(
-    _RequiredStartContentModerationRequestRequestTypeDef,
-    _OptionalStartContentModerationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFaceDetectionRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFaceDetectionRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "FaceAttributes": FaceAttributesType,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartFaceDetectionRequestRequestTypeDef(
-    _RequiredStartFaceDetectionRequestRequestTypeDef,
-    _OptionalStartFaceDetectionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFaceSearchRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-        "CollectionId": str,
-    },
-)
-_OptionalStartFaceSearchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFaceSearchRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "FaceMatchThreshold": float,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartFaceSearchRequestRequestTypeDef(
-    _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
-):
-    pass
-
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
-):
-    pass
-
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
 CelebrityTypeDef = TypedDict(
     "CelebrityTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "Id": str,
         "Face": ComparedFaceTypeDef,
@@ -3182,14 +3188,17 @@
     {
         "FaceDetails": FaceDetailTypeDef,
         "Reasons": List[UnsearchedFaceReasonType],
     },
     total=False,
 )
 
+StreamProcessorSettingsUnionTypeDef = Union[
+    StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef
+]
 CustomLabelTypeDef = TypedDict(
     "CustomLabelTypeDef",
     {
         "Name": str,
         "Confidence": float,
         "Geometry": GeometryTypeDef,
     },
@@ -3214,48 +3223,24 @@
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
+RegionOfInterestUnionTypeDef = Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
 StartTextDetectionFiltersTypeDef = TypedDict(
     "StartTextDetectionFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[
-            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
-        ],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
-    },
-    total=False,
-)
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -3301,44 +3286,14 @@
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceTypeDef,
         "SearchedUser": SearchedUserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Input": StreamProcessorInputTypeDef,
-        "Output": StreamProcessorOutputTypeDef,
-        "Name": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
-        "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[
-            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
-        ],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-    },
-    total=False,
-)
-
-class CreateStreamProcessorRequestRequestTypeDef(
-    _RequiredCreateStreamProcessorRequestRequestTypeDef,
-    _OptionalCreateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
@@ -3642,14 +3597,65 @@
 )
 
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Input": StreamProcessorInputTypeDef,
+        "Output": StreamProcessorOutputTypeDef,
+        "Name": str,
+        "Settings": StreamProcessorSettingsTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "KmsKeyId": str,
+        "RegionsOfInterest": Sequence[RegionOfInterestUnionTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
+    },
+    total=False,
+)
+
+class CreateStreamProcessorRequestRequestTypeDef(
+    _RequiredCreateStreamProcessorRequestRequestTypeDef,
+    _OptionalCreateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestUnionTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartTextDetectionRequestRequestTypeDef = TypedDict(
@@ -3665,14 +3671,15 @@
 
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
+TestingDataUnionTypeDef = Union[TestingDataTypeDef, TestingDataOutputTypeDef]
 _RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "VersionName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
@@ -3690,14 +3697,15 @@
 
 class CreateProjectVersionRequestRequestTypeDef(
     _RequiredCreateProjectVersionRequestRequestTypeDef,
     _OptionalCreateProjectVersionRequestRequestTypeDef,
 ):
     pass
 
+TrainingDataUnionTypeDef = Union[TrainingDataTypeDef, TrainingDataOutputTypeDef]
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
         "Input": TestingDataOutputTypeDef,
         "Output": TestingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
```

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/waiter.py` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/waiter.pyi` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/PKG-INFO` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Rekognition 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rekognition type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 rekognition type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -416,33 +416,34 @@
 )
 
 
 def check_value(value: AttributeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rekognition.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
     ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
     BoundingBoxTypeDef,
     S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
+    BlobTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
@@ -453,15 +454,14 @@
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
     LivenessOutputConfigTypeDef,
     CreateProjectRequestRequestTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     CreateUserRequestRequestTypeDef,
-    DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
     UnsuccessfulFaceDeletionTypeDef,
@@ -575,26 +575,26 @@
     StartTextDetectionResponseTypeDef,
     StopProjectVersionResponseTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
     GroundTruthManifestTypeDef,
-    ImageTypeDef,
     SummaryTypeDef,
     VideoTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
+    DatasetChangesTypeDef,
+    ImageTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
     CreateFaceLivenessSessionRequestSettingsTypeDef,
-    UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
     DeleteFacesResponseTypeDef,
     DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
     DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     ListCollectionsRequestListCollectionsPaginateTypeDef,
@@ -630,29 +630,30 @@
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
     AssetTypeDef,
     DatasetSourceTypeDef,
+    EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
+    StartSegmentDetectionFiltersTypeDef,
+    UpdateDatasetEntriesRequestRequestTypeDef,
     CompareFacesRequestRequestTypeDef,
     DetectCustomLabelsRequestRequestTypeDef,
     DetectFacesRequestRequestTypeDef,
     DetectProtectiveEquipmentRequestRequestTypeDef,
     IndexFacesRequestRequestTypeDef,
     RecognizeCelebritiesRequestRequestTypeDef,
     SearchFacesByImageRequestRequestTypeDef,
     SearchUsersByImageRequestRequestTypeDef,
-    EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
-    StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
@@ -665,23 +666,23 @@
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
+    StreamProcessorSettingsUnionTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
     DetectTextFiltersTypeDef,
+    RegionOfInterestUnionTypeDef,
     StartTextDetectionFiltersTypeDef,
-    UpdateStreamProcessorRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
     SearchUsersResponseTypeDef,
-    CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     TestingDataOutputTypeDef,
     TestingDataTypeDef,
     TrainingDataOutputTypeDef,
@@ -700,30 +701,34 @@
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
     DetectTextRequestRequestTypeDef,
+    CreateStreamProcessorRequestRequestTypeDef,
+    UpdateStreamProcessorRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
+    TestingDataUnionTypeDef,
     CreateProjectVersionRequestRequestTypeDef,
+    TrainingDataUnionTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
-def get_structure() -> AgeRangeTypeDef:
+def get_value() -> AgeRangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/SOURCES.txt` & `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15.post1/setup.py` & `mypy-boto3-rekognition-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rekognition",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Rekognition 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 rekognition type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 rekognition type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_rekognition": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

