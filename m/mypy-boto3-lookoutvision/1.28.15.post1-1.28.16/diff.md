# Comparing `tmp/mypy-boto3-lookoutvision-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-lookoutvision-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutvision-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:34 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutvision-1.28.16.tar", last modified: Tue Aug  1 11:37:14 2023, max compression
```

## Comparing `mypy-boto3-lookoutvision-1.28.15.post1.tar` & `mypy-boto3-lookoutvision-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.569256 mypy-boto3-lookoutvision-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-07-29 10:03:34.565256 mypy-boto3-lookoutvision-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.557256 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19116 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19083 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-29 09:50:15.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-29 09:50:15.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27131 2023-07-29 09:50:15.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.565256 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:34.569256 mypy-boto3-lookoutvision-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:14.412835 mypy-boto3-lookoutvision-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16390 2023-08-01 11:37:14.404835 mypy-boto3-lookoutvision-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14879 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:14.404835 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18815 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27414 2023-08-01 11:23:07.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27371 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:06.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:14.404835 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16390 2023-08-01 11:37:14.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-01 11:37:14.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:14.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:14.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:14.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:37:14.000000 mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:14.412835 mypy-boto3-lookoutvision-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-01 11:23:05.000000 mypy-boto3-lookoutvision-1.28.16/setup.py
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/LICENSE` & `mypy-boto3-lookoutvision-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/PKG-INFO` & `mypy-boto3-lookoutvision-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LookoutforVision 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LookoutforVision 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lookoutvision type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lookoutvision type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutvision)](https://pepy.tech/project/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
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
@@ -334,57 +334,58 @@
 )
 
 
 def check_value(value: DatasetStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lookoutvision.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lookoutvision.type_defs import (
     PixelAnomalyTypeDef,
+    BlobTypeDef,
     DatasetMetadataTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectMetadataTypeDef,
     DatasetImageStatsTypeDef,
     InputS3ObjectTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
-    DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
     PaginatorConfigTypeDef,
-    ListDatasetEntriesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListModelPackagingJobsRequestRequestTypeDef,
     ModelPackagingJobMetadataTypeDef,
     ListModelsRequestRequestTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModelPerformanceTypeDef,
     OutputS3ObjectTypeDef,
     StartModelRequestRequestTypeDef,
     StopModelRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateDatasetEntriesRequestRequestTypeDef,
     AnomalyTypeDef,
+    DetectAnomaliesRequestRequestTypeDef,
+    UpdateDatasetEntriesRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
     CreateDatasetResponseTypeDef,
     DeleteModelResponseTypeDef,
     DeleteProjectResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     StartModelPackagingJobResponseTypeDef,
     StartModelResponseTypeDef,
@@ -396,18 +397,19 @@
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
     OutputConfigTypeDef,
     GreengrassConfigurationOutputTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     ListModelsRequestListModelsPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListDatasetEntriesRequestRequestTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
     CreateModelRequestRequestTypeDef,
@@ -416,20 +418,21 @@
     ModelPackagingConfigurationTypeDef,
     CreateModelResponseTypeDef,
     ListModelsResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
     ModelPackagingDescriptionTypeDef,
+    ModelPackagingConfigurationUnionTypeDef,
     StartModelPackagingJobRequestRequestTypeDef,
     DescribeModelPackagingJobResponseTypeDef,
 )
 
 
-def get_structure() -> PixelAnomalyTypeDef:
+def get_value() -> PixelAnomalyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/README.md` & `mypy-boto3-lookoutvision-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutvision)](https://pepy.tech/project/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
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
@@ -302,57 +302,58 @@
 )
 
 
 def check_value(value: DatasetStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lookoutvision.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lookoutvision.type_defs import (
     PixelAnomalyTypeDef,
+    BlobTypeDef,
     DatasetMetadataTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectMetadataTypeDef,
     DatasetImageStatsTypeDef,
     InputS3ObjectTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
-    DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
     PaginatorConfigTypeDef,
-    ListDatasetEntriesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListModelPackagingJobsRequestRequestTypeDef,
     ModelPackagingJobMetadataTypeDef,
     ListModelsRequestRequestTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModelPerformanceTypeDef,
     OutputS3ObjectTypeDef,
     StartModelRequestRequestTypeDef,
     StopModelRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateDatasetEntriesRequestRequestTypeDef,
     AnomalyTypeDef,
+    DetectAnomaliesRequestRequestTypeDef,
+    UpdateDatasetEntriesRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
     CreateDatasetResponseTypeDef,
     DeleteModelResponseTypeDef,
     DeleteProjectResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     StartModelPackagingJobResponseTypeDef,
     StartModelResponseTypeDef,
@@ -364,18 +365,19 @@
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
     OutputConfigTypeDef,
     GreengrassConfigurationOutputTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     ListModelsRequestListModelsPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListDatasetEntriesRequestRequestTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
     CreateModelRequestRequestTypeDef,
@@ -384,20 +386,21 @@
     ModelPackagingConfigurationTypeDef,
     CreateModelResponseTypeDef,
     ListModelsResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
     ModelPackagingDescriptionTypeDef,
+    ModelPackagingConfigurationUnionTypeDef,
     StartModelPackagingJobRequestRequestTypeDef,
     DescribeModelPackagingJobResponseTypeDef,
 )
 
 
-def get_structure() -> PixelAnomalyTypeDef:
+def get_value() -> PixelAnomalyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__init__.py` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__init__.pyi` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__main__.py` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutforVision 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LookoutforVision 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision\nOther"
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

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/client.py` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,26 @@
     from mypy_boto3_lookoutvision.client import LookoutforVisionClient
 
     session = Session()
     client: LookoutforVisionClient = session.client("lookoutvision")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     ListDatasetEntriesPaginator,
     ListModelPackagingJobsPaginator,
     ListModelsPaginator,
     ListProjectsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CreateDatasetResponseTypeDef,
     CreateModelResponseTypeDef,
     CreateProjectResponseTypeDef,
     DatasetSourceTypeDef,
     DeleteModelResponseTypeDef,
     DeleteProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
@@ -39,21 +38,21 @@
     DescribeProjectResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ListModelsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ModelPackagingConfigurationOutputTypeDef,
-    ModelPackagingConfigurationTypeDef,
+    ModelPackagingConfigurationUnionTypeDef,
     OutputConfigTypeDef,
     StartModelPackagingJobResponseTypeDef,
     StartModelResponseTypeDef,
     StopModelResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateDatasetEntriesResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -221,20 +220,15 @@
         Describes an Amazon Lookout for Vision project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.describe_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#describe_project)
         """
 
     def detect_anomalies(
-        self,
-        *,
-        ProjectName: str,
-        ModelVersion: str,
-        Body: Union[str, bytes, IO[Any], StreamingBody],
-        ContentType: str
+        self, *, ProjectName: str, ModelVersion: str, Body: BlobTypeDef, ContentType: str
     ) -> DetectAnomaliesResponseTypeDef:
         """
         Detects anomalies in an image that you supply.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.detect_anomalies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#detect_anomalies)
         """
@@ -256,16 +250,16 @@
     def list_dataset_entries(
         self,
         *,
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
-        BeforeCreationDate: Union[datetime, str] = ...,
-        AfterCreationDate: Union[datetime, str] = ...,
+        BeforeCreationDate: TimestampTypeDef = ...,
+        AfterCreationDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SourceRefContains: str = ...
     ) -> ListDatasetEntriesResponseTypeDef:
         """
         Lists the JSON Lines within a dataset.
 
@@ -330,17 +324,15 @@
         """
 
     def start_model_packaging_job(
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
-        Configuration: Union[
-            ModelPackagingConfigurationTypeDef, ModelPackagingConfigurationOutputTypeDef
-        ],
+        Configuration: ModelPackagingConfigurationUnionTypeDef,
         JobName: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> StartModelPackagingJobResponseTypeDef:
         """
         Starts an Amazon Lookout for Vision model packaging job.
 
@@ -371,20 +363,15 @@
         Removes one or more tags from an Amazon Lookout for Vision model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#untag_resource)
         """
 
     def update_dataset_entries(
-        self,
-        *,
-        ProjectName: str,
-        DatasetType: str,
-        Changes: Union[str, bytes, IO[Any], StreamingBody],
-        ClientToken: str = ...
+        self, *, ProjectName: str, DatasetType: str, Changes: BlobTypeDef, ClientToken: str = ...
     ) -> UpdateDatasetEntriesResponseTypeDef:
         """
         Adds or updates one or more JSON Line entries in a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.update_dataset_entries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#update_dataset_entries)
         """
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/client.pyi` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,26 @@
     from mypy_boto3_lookoutvision.client import LookoutforVisionClient
 
     session = Session()
     client: LookoutforVisionClient = session.client("lookoutvision")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     ListDatasetEntriesPaginator,
     ListModelPackagingJobsPaginator,
     ListModelsPaginator,
     ListProjectsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CreateDatasetResponseTypeDef,
     CreateModelResponseTypeDef,
     CreateProjectResponseTypeDef,
     DatasetSourceTypeDef,
     DeleteModelResponseTypeDef,
     DeleteProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
@@ -39,21 +38,21 @@
     DescribeProjectResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ListModelsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ModelPackagingConfigurationOutputTypeDef,
-    ModelPackagingConfigurationTypeDef,
+    ModelPackagingConfigurationUnionTypeDef,
     OutputConfigTypeDef,
     StartModelPackagingJobResponseTypeDef,
     StartModelResponseTypeDef,
     StopModelResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateDatasetEntriesResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -204,20 +203,15 @@
         """
         Describes an Amazon Lookout for Vision project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.describe_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#describe_project)
         """
     def detect_anomalies(
-        self,
-        *,
-        ProjectName: str,
-        ModelVersion: str,
-        Body: Union[str, bytes, IO[Any], StreamingBody],
-        ContentType: str
+        self, *, ProjectName: str, ModelVersion: str, Body: BlobTypeDef, ContentType: str
     ) -> DetectAnomaliesResponseTypeDef:
         """
         Detects anomalies in an image that you supply.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.detect_anomalies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#detect_anomalies)
         """
@@ -237,16 +231,16 @@
     def list_dataset_entries(
         self,
         *,
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
-        BeforeCreationDate: Union[datetime, str] = ...,
-        AfterCreationDate: Union[datetime, str] = ...,
+        BeforeCreationDate: TimestampTypeDef = ...,
+        AfterCreationDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SourceRefContains: str = ...
     ) -> ListDatasetEntriesResponseTypeDef:
         """
         Lists the JSON Lines within a dataset.
 
@@ -305,17 +299,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#start_model)
         """
     def start_model_packaging_job(
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
-        Configuration: Union[
-            ModelPackagingConfigurationTypeDef, ModelPackagingConfigurationOutputTypeDef
-        ],
+        Configuration: ModelPackagingConfigurationUnionTypeDef,
         JobName: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> StartModelPackagingJobResponseTypeDef:
         """
         Starts an Amazon Lookout for Vision model packaging job.
 
@@ -342,20 +334,15 @@
         """
         Removes one or more tags from an Amazon Lookout for Vision model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#untag_resource)
         """
     def update_dataset_entries(
-        self,
-        *,
-        ProjectName: str,
-        DatasetType: str,
-        Changes: Union[str, bytes, IO[Any], StreamingBody],
-        ClientToken: str = ...
+        self, *, ProjectName: str, DatasetType: str, Changes: BlobTypeDef, ClientToken: str = ...
     ) -> UpdateDatasetEntriesResponseTypeDef:
         """
         Adds or updates one or more JSON Line entries in a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.update_dataset_entries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#update_dataset_entries)
         """
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/literals.py` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/literals.pyi` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/paginator.py` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
     list_dataset_entries_paginator: ListDatasetEntriesPaginator = client.get_paginator("list_dataset_entries")
     list_model_packaging_jobs_paginator: ListModelPackagingJobsPaginator = client.get_paginator("list_model_packaging_jobs")
     list_models_paginator: ListModelsPaginator = client.get_paginator("list_models")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ListModelsResponseTypeDef,
     ListProjectsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListDatasetEntriesPaginator",
     "ListModelPackagingJobsPaginator",
     "ListModelsPaginator",
     "ListProjectsPaginator",
@@ -65,16 +65,16 @@
     def paginate(
         self,
         *,
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
-        BeforeCreationDate: Union[datetime, str] = ...,
-        AfterCreationDate: Union[datetime, str] = ...,
+        BeforeCreationDate: TimestampTypeDef = ...,
+        AfterCreationDate: TimestampTypeDef = ...,
         SourceRefContains: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listdatasetentriespaginator)
         """
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/paginator.pyi` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
     list_dataset_entries_paginator: ListDatasetEntriesPaginator = client.get_paginator("list_dataset_entries")
     list_model_packaging_jobs_paginator: ListModelPackagingJobsPaginator = client.get_paginator("list_model_packaging_jobs")
     list_models_paginator: ListModelsPaginator = client.get_paginator("list_models")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ListModelsResponseTypeDef,
     ListProjectsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListDatasetEntriesPaginator",
     "ListModelPackagingJobsPaginator",
     "ListModelsPaginator",
     "ListProjectsPaginator",
@@ -62,16 +62,16 @@
     def paginate(
         self,
         *,
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
-        BeforeCreationDate: Union[datetime, str] = ...,
-        AfterCreationDate: Union[datetime, str] = ...,
+        BeforeCreationDate: TimestampTypeDef = ...,
+        AfterCreationDate: TimestampTypeDef = ...,
         SourceRefContains: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listdatasetentriespaginator)
         """
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/type_defs.py` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lookoutvision.type_defs import PixelAnomalyTypeDef
 
-    data: PixelAnomalyTypeDef = {...}
+    data: PixelAnomalyTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -33,47 +33,48 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "PixelAnomalyTypeDef",
+    "BlobTypeDef",
     "DatasetMetadataTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectMetadataTypeDef",
     "DatasetImageStatsTypeDef",
     "InputS3ObjectTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeModelPackagingJobRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
-    "DetectAnomaliesRequestRequestTypeDef",
     "ImageSourceTypeDef",
     "S3LocationTypeDef",
     "TargetPlatformTypeDef",
     "GreengrassOutputDetailsTypeDef",
     "PaginatorConfigTypeDef",
-    "ListDatasetEntriesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListModelPackagingJobsRequestRequestTypeDef",
     "ModelPackagingJobMetadataTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModelPerformanceTypeDef",
     "OutputS3ObjectTypeDef",
     "StartModelRequestRequestTypeDef",
     "StopModelRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateDatasetEntriesRequestRequestTypeDef",
     "AnomalyTypeDef",
+    "DetectAnomaliesRequestRequestTypeDef",
+    "UpdateDatasetEntriesRequestRequestTypeDef",
     "ProjectDescriptionTypeDef",
     "CreateDatasetResponseTypeDef",
     "DeleteModelResponseTypeDef",
     "DeleteProjectResponseTypeDef",
     "ListDatasetEntriesResponseTypeDef",
     "StartModelPackagingJobResponseTypeDef",
     "StartModelResponseTypeDef",
@@ -85,18 +86,19 @@
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
     "OutputConfigTypeDef",
     "GreengrassConfigurationOutputTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     "ListModelsRequestListModelsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "ListDatasetEntriesRequestRequestTypeDef",
     "ListModelPackagingJobsResponseTypeDef",
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
     "CreateModelRequestRequestTypeDef",
@@ -105,27 +107,29 @@
     "ModelPackagingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
     "ListModelsResponseTypeDef",
     "DetectAnomaliesResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
     "ModelPackagingDescriptionTypeDef",
+    "ModelPackagingConfigurationUnionTypeDef",
     "StartModelPackagingJobRequestRequestTypeDef",
     "DescribeModelPackagingJobResponseTypeDef",
 )
 
 PixelAnomalyTypeDef = TypedDict(
     "PixelAnomalyTypeDef",
     {
         "TotalPercentageArea": float,
         "Color": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 DatasetMetadataTypeDef = TypedDict(
     "DatasetMetadataTypeDef",
     {
         "DatasetType": str,
         "CreationTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
@@ -306,24 +310,14 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
-DetectAnomaliesRequestRequestTypeDef = TypedDict(
-    "DetectAnomaliesRequestRequestTypeDef",
-    {
-        "ProjectName": str,
-        "ModelVersion": str,
-        "Body": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-
 ImageSourceTypeDef = TypedDict(
     "ImageSourceTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
@@ -383,43 +377,15 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestRequestTypeDef",
-    {
-        "ProjectName": str,
-        "DatasetType": str,
-    },
-)
-_OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestRequestTypeDef",
-    {
-        "Labeled": bool,
-        "AnomalyClass": str,
-        "BeforeCreationDate": Union[datetime, str],
-        "AfterCreationDate": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-        "SourceRefContains": str,
-    },
-    total=False,
-)
-
-
-class ListDatasetEntriesRequestRequestTypeDef(
-    _RequiredListDatasetEntriesRequestRequestTypeDef,
-    _OptionalListDatasetEntriesRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListModelPackagingJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelPackagingJobsRequestRequestTypeDef = TypedDict(
@@ -561,20 +527,39 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "Name": str,
+        "PixelAnomaly": PixelAnomalyTypeDef,
+    },
+    total=False,
+)
+
+DetectAnomaliesRequestRequestTypeDef = TypedDict(
+    "DetectAnomaliesRequestRequestTypeDef",
+    {
+        "ProjectName": str,
+        "ModelVersion": str,
+        "Body": BlobTypeDef,
+        "ContentType": str,
+    },
+)
+
 _RequiredUpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
-        "Changes": Union[str, bytes, IO[Any], StreamingBody],
+        "Changes": BlobTypeDef,
     },
 )
 _OptionalUpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
@@ -585,23 +570,14 @@
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
 
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
-    {
-        "Name": str,
-        "PixelAnomaly": PixelAnomalyTypeDef,
-    },
-    total=False,
-)
-
 ProjectDescriptionTypeDef = TypedDict(
     "ProjectDescriptionTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
         "Datasets": List[DatasetMetadataTypeDef],
@@ -794,42 +770,14 @@
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ProjectName": str,
-        "DatasetType": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "Labeled": bool,
-        "AnomalyClass": str,
-        "BeforeCreationDate": Union[datetime, str],
-        "AfterCreationDate": Union[datetime, str],
-        "SourceRefContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
@@ -874,14 +822,71 @@
     "ListProjectsRequestListProjectsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ProjectName": str,
+        "DatasetType": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "Labeled": bool,
+        "AnomalyClass": str,
+        "BeforeCreationDate": TimestampTypeDef,
+        "AfterCreationDate": TimestampTypeDef,
+        "SourceRefContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestRequestTypeDef",
+    {
+        "ProjectName": str,
+        "DatasetType": str,
+    },
+)
+_OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestRequestTypeDef",
+    {
+        "Labeled": bool,
+        "AnomalyClass": str,
+        "BeforeCreationDate": TimestampTypeDef,
+        "AfterCreationDate": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "SourceRefContains": str,
+    },
+    total=False,
+)
+
+
+class ListDatasetEntriesRequestRequestTypeDef(
+    _RequiredListDatasetEntriesRequestRequestTypeDef,
+    _OptionalListDatasetEntriesRequestRequestTypeDef,
+):
+    pass
+
+
 ListModelPackagingJobsResponseTypeDef = TypedDict(
     "ListModelPackagingJobsResponseTypeDef",
     {
         "ModelPackagingJobs": List[ModelPackagingJobMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1067,14 +1072,17 @@
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+ModelPackagingConfigurationUnionTypeDef = Union[
+    ModelPackagingConfigurationTypeDef, ModelPackagingConfigurationOutputTypeDef
+]
 _RequiredStartModelPackagingJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartModelPackagingJobRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
         "Configuration": ModelPackagingConfigurationTypeDef,
     },
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/type_defs.pyi` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lookoutvision.type_defs import PixelAnomalyTypeDef
 
-    data: PixelAnomalyTypeDef = {...}
+    data: PixelAnomalyTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -32,47 +32,48 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "PixelAnomalyTypeDef",
+    "BlobTypeDef",
     "DatasetMetadataTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectMetadataTypeDef",
     "DatasetImageStatsTypeDef",
     "InputS3ObjectTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeModelPackagingJobRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
-    "DetectAnomaliesRequestRequestTypeDef",
     "ImageSourceTypeDef",
     "S3LocationTypeDef",
     "TargetPlatformTypeDef",
     "GreengrassOutputDetailsTypeDef",
     "PaginatorConfigTypeDef",
-    "ListDatasetEntriesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListModelPackagingJobsRequestRequestTypeDef",
     "ModelPackagingJobMetadataTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModelPerformanceTypeDef",
     "OutputS3ObjectTypeDef",
     "StartModelRequestRequestTypeDef",
     "StopModelRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateDatasetEntriesRequestRequestTypeDef",
     "AnomalyTypeDef",
+    "DetectAnomaliesRequestRequestTypeDef",
+    "UpdateDatasetEntriesRequestRequestTypeDef",
     "ProjectDescriptionTypeDef",
     "CreateDatasetResponseTypeDef",
     "DeleteModelResponseTypeDef",
     "DeleteProjectResponseTypeDef",
     "ListDatasetEntriesResponseTypeDef",
     "StartModelPackagingJobResponseTypeDef",
     "StartModelResponseTypeDef",
@@ -84,18 +85,19 @@
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
     "OutputConfigTypeDef",
     "GreengrassConfigurationOutputTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     "ListModelsRequestListModelsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "ListDatasetEntriesRequestRequestTypeDef",
     "ListModelPackagingJobsResponseTypeDef",
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
     "CreateModelRequestRequestTypeDef",
@@ -104,27 +106,29 @@
     "ModelPackagingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
     "ListModelsResponseTypeDef",
     "DetectAnomaliesResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
     "ModelPackagingDescriptionTypeDef",
+    "ModelPackagingConfigurationUnionTypeDef",
     "StartModelPackagingJobRequestRequestTypeDef",
     "DescribeModelPackagingJobResponseTypeDef",
 )
 
 PixelAnomalyTypeDef = TypedDict(
     "PixelAnomalyTypeDef",
     {
         "TotalPercentageArea": float,
         "Color": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 DatasetMetadataTypeDef = TypedDict(
     "DatasetMetadataTypeDef",
     {
         "DatasetType": str,
         "CreationTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
@@ -295,24 +299,14 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
-DetectAnomaliesRequestRequestTypeDef = TypedDict(
-    "DetectAnomaliesRequestRequestTypeDef",
-    {
-        "ProjectName": str,
-        "ModelVersion": str,
-        "Body": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-
 ImageSourceTypeDef = TypedDict(
     "ImageSourceTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
@@ -368,41 +362,15 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestRequestTypeDef",
-    {
-        "ProjectName": str,
-        "DatasetType": str,
-    },
-)
-_OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestRequestTypeDef",
-    {
-        "Labeled": bool,
-        "AnomalyClass": str,
-        "BeforeCreationDate": Union[datetime, str],
-        "AfterCreationDate": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-        "SourceRefContains": str,
-    },
-    total=False,
-)
-
-class ListDatasetEntriesRequestRequestTypeDef(
-    _RequiredListDatasetEntriesRequestRequestTypeDef,
-    _OptionalListDatasetEntriesRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListModelPackagingJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelPackagingJobsRequestRequestTypeDef = TypedDict(
@@ -536,20 +504,39 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "Name": str,
+        "PixelAnomaly": PixelAnomalyTypeDef,
+    },
+    total=False,
+)
+
+DetectAnomaliesRequestRequestTypeDef = TypedDict(
+    "DetectAnomaliesRequestRequestTypeDef",
+    {
+        "ProjectName": str,
+        "ModelVersion": str,
+        "Body": BlobTypeDef,
+        "ContentType": str,
+    },
+)
+
 _RequiredUpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
-        "Changes": Union[str, bytes, IO[Any], StreamingBody],
+        "Changes": BlobTypeDef,
     },
 )
 _OptionalUpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
@@ -558,23 +545,14 @@
 
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
-    {
-        "Name": str,
-        "PixelAnomaly": PixelAnomalyTypeDef,
-    },
-    total=False,
-)
-
 ProjectDescriptionTypeDef = TypedDict(
     "ProjectDescriptionTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
         "Datasets": List[DatasetMetadataTypeDef],
@@ -763,40 +741,14 @@
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ProjectName": str,
-        "DatasetType": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "Labeled": bool,
-        "AnomalyClass": str,
-        "BeforeCreationDate": Union[datetime, str],
-        "AfterCreationDate": Union[datetime, str],
-        "SourceRefContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
 _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
@@ -837,14 +789,67 @@
     "ListProjectsRequestListProjectsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ProjectName": str,
+        "DatasetType": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "Labeled": bool,
+        "AnomalyClass": str,
+        "BeforeCreationDate": TimestampTypeDef,
+        "AfterCreationDate": TimestampTypeDef,
+        "SourceRefContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+_RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestRequestTypeDef",
+    {
+        "ProjectName": str,
+        "DatasetType": str,
+    },
+)
+_OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestRequestTypeDef",
+    {
+        "Labeled": bool,
+        "AnomalyClass": str,
+        "BeforeCreationDate": TimestampTypeDef,
+        "AfterCreationDate": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "SourceRefContains": str,
+    },
+    total=False,
+)
+
+class ListDatasetEntriesRequestRequestTypeDef(
+    _RequiredListDatasetEntriesRequestRequestTypeDef,
+    _OptionalListDatasetEntriesRequestRequestTypeDef,
+):
+    pass
+
 ListModelPackagingJobsResponseTypeDef = TypedDict(
     "ListModelPackagingJobsResponseTypeDef",
     {
         "ModelPackagingJobs": List[ModelPackagingJobMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1026,14 +1031,17 @@
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+ModelPackagingConfigurationUnionTypeDef = Union[
+    ModelPackagingConfigurationTypeDef, ModelPackagingConfigurationOutputTypeDef
+]
 _RequiredStartModelPackagingJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartModelPackagingJobRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
         "Configuration": ModelPackagingConfigurationTypeDef,
     },
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/PKG-INFO` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LookoutforVision 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LookoutforVision 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lookoutvision type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lookoutvision type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutvision)](https://pepy.tech/project/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
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
@@ -334,57 +334,58 @@
 )
 
 
 def check_value(value: DatasetStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lookoutvision.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lookoutvision.type_defs import (
     PixelAnomalyTypeDef,
+    BlobTypeDef,
     DatasetMetadataTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectMetadataTypeDef,
     DatasetImageStatsTypeDef,
     InputS3ObjectTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
-    DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
     PaginatorConfigTypeDef,
-    ListDatasetEntriesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListModelPackagingJobsRequestRequestTypeDef,
     ModelPackagingJobMetadataTypeDef,
     ListModelsRequestRequestTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModelPerformanceTypeDef,
     OutputS3ObjectTypeDef,
     StartModelRequestRequestTypeDef,
     StopModelRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateDatasetEntriesRequestRequestTypeDef,
     AnomalyTypeDef,
+    DetectAnomaliesRequestRequestTypeDef,
+    UpdateDatasetEntriesRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
     CreateDatasetResponseTypeDef,
     DeleteModelResponseTypeDef,
     DeleteProjectResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     StartModelPackagingJobResponseTypeDef,
     StartModelResponseTypeDef,
@@ -396,18 +397,19 @@
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
     OutputConfigTypeDef,
     GreengrassConfigurationOutputTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     ListModelsRequestListModelsPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListDatasetEntriesRequestRequestTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
     CreateModelRequestRequestTypeDef,
@@ -416,20 +418,21 @@
     ModelPackagingConfigurationTypeDef,
     CreateModelResponseTypeDef,
     ListModelsResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
     ModelPackagingDescriptionTypeDef,
+    ModelPackagingConfigurationUnionTypeDef,
     StartModelPackagingJobRequestRequestTypeDef,
     DescribeModelPackagingJobResponseTypeDef,
 )
 
 
-def get_structure() -> PixelAnomalyTypeDef:
+def get_value() -> PixelAnomalyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/SOURCES.txt` & `mypy-boto3-lookoutvision-1.28.16/mypy_boto3_lookoutvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15.post1/setup.py` & `mypy-boto3-lookoutvision-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutvision",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_lookoutvision"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutforVision 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.LookoutforVision 1.28.16 service generated with"
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
-    keywords="boto3 lookoutvision type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 lookoutvision type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_lookoutvision": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

