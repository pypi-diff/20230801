# Comparing `tmp/mypy-boto3-ecr-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ecr-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-1.28.16.tar", last modified: Tue Aug  1 11:36:42 2023, max compression
```

## Comparing `mypy-boto3-ecr-1.28.15.post1.tar` & `mypy-boto3-ecr-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.097126 mypy-boto3-ecr-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-07-29 10:03:02.097126 mypy-boto3-ecr-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.093126 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33909 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33853 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52949 2023-07-29 09:44:15.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52874 2023-07-29 09:44:14.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.097126 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.097126 mypy-boto3-ecr-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.232901 mypy-boto3-ecr-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-08-01 11:36:42.232901 mypy-boto3-ecr-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.212901 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33653 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33597 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-08-01 11:16:48.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53273 2023-08-01 11:16:49.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53198 2023-08-01 11:16:48.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.232901 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-08-01 11:36:41.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:36:42.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:41.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:41.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:41.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:41.000000 mypy-boto3-ecr-1.28.16/mypy_boto3_ecr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:42.232901 mypy-boto3-ecr-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:16:47.000000 mypy-boto3-ecr-1.28.16/setup.py
```

### Comparing `mypy-boto3-ecr-1.28.15.post1/LICENSE` & `mypy-boto3-ecr-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/PKG-INFO` & `mypy-boto3-ecr-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ECR 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ecr type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ecr type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
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
@@ -375,33 +375,34 @@
 )
 
 
 def check_value(value: DescribeImageScanFindingsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ecr.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
@@ -436,15 +437,14 @@
     RecommendationTypeDef,
     ScanningRepositoryFilterTypeDef,
     ReplicationDestinationTypeDef,
     RepositoryFilterTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
     ImageScanFindingTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleResponseTypeDef,
@@ -466,14 +466,15 @@
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
     StartImageScanRequestRequestTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
@@ -507,30 +508,32 @@
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
     ScoreDetailsTypeDef,
     DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
     RegistryScanningConfigurationTypeDef,
-    PutRegistryScanningConfigurationRequestRequestTypeDef,
+    RegistryScanningRuleUnionTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
+    PutRegistryScanningConfigurationRequestRequestTypeDef,
     DescribeRegistryResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
     PutReplicationConfigurationRequestRequestTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     ImageScanFindingsTypeDef,
     DescribeImageScanFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ecr-1.28.15.post1/README.md` & `mypy-boto3-ecr-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
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
@@ -343,33 +343,34 @@
 )
 
 
 def check_value(value: DescribeImageScanFindingsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ecr.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
@@ -404,15 +405,14 @@
     RecommendationTypeDef,
     ScanningRepositoryFilterTypeDef,
     ReplicationDestinationTypeDef,
     RepositoryFilterTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
     ImageScanFindingTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleResponseTypeDef,
@@ -434,14 +434,15 @@
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
     StartImageScanRequestRequestTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
@@ -475,30 +476,32 @@
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
     ScoreDetailsTypeDef,
     DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
     RegistryScanningConfigurationTypeDef,
-    PutRegistryScanningConfigurationRequestRequestTypeDef,
+    RegistryScanningRuleUnionTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
+    PutRegistryScanningConfigurationRequestRequestTypeDef,
     DescribeRegistryResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
     PutReplicationConfigurationRequestRequestTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     ImageScanFindingsTypeDef,
     DescribeImageScanFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__init__.py` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__init__.pyi` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__main__.py` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECR 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.ECR 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
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

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/client.py` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_ecr.client import ECRClient
 
     session = Session()
     client: ECRClient = session.client("ecr")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import ImageTagMutabilityType, ScanTypeType
 from .paginator import (
     DescribeImageScanFindingsPaginator,
     DescribeImagesPaginator,
     DescribePullThroughCacheRulesPaginator,
     DescribeRepositoriesPaginator,
@@ -29,14 +28,15 @@
     ListImagesPaginator,
 )
 from .type_defs import (
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleResponseTypeDef,
     DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
@@ -66,18 +66,16 @@
     PutImageResponseTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
-    RegistryScanningRuleOutputTypeDef,
-    RegistryScanningRuleTypeDef,
-    ReplicationConfigurationOutputTypeDef,
-    ReplicationConfigurationTypeDef,
+    RegistryScanningRuleUnionTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartImageScanResponseTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     TagTypeDef,
     UploadLayerPartResponseTypeDef,
 )
 from .waiter import ImageScanCompleteWaiter, LifecyclePolicyPreviewCompleteWaiter
@@ -577,29 +575,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_registry_policy)
         """
 
     def put_registry_scanning_configuration(
         self,
         *,
         scanType: ScanTypeType = ...,
-        rules: Sequence[Union[RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef]] = ...
+        rules: Sequence[RegistryScanningRuleUnionTypeDef] = ...
     ) -> PutRegistryScanningConfigurationResponseTypeDef:
         """
         Creates or updates the scanning configuration for your private registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_scanning_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_registry_scanning_configuration)
         """
 
     def put_replication_configuration(
-        self,
-        *,
-        replicationConfiguration: Union[
-            ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-        ]
+        self, *, replicationConfiguration: ReplicationConfigurationUnionTypeDef
     ) -> PutReplicationConfigurationResponseTypeDef:
         """
         Creates or updates the replication configuration for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_replication_configuration)
         """
@@ -654,15 +648,15 @@
     def upload_layer_part(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
-        layerPartBlob: Union[str, bytes, IO[Any], StreamingBody],
+        layerPartBlob: BlobTypeDef,
         registryId: str = ...
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.upload_layer_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#upload_layer_part)
```

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/client.pyi` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_ecr.client import ECRClient
 
     session = Session()
     client: ECRClient = session.client("ecr")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import ImageTagMutabilityType, ScanTypeType
 from .paginator import (
     DescribeImageScanFindingsPaginator,
     DescribeImagesPaginator,
     DescribePullThroughCacheRulesPaginator,
     DescribeRepositoriesPaginator,
@@ -29,14 +28,15 @@
     ListImagesPaginator,
 )
 from .type_defs import (
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleResponseTypeDef,
     DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
@@ -66,18 +66,16 @@
     PutImageResponseTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
-    RegistryScanningRuleOutputTypeDef,
-    RegistryScanningRuleTypeDef,
-    ReplicationConfigurationOutputTypeDef,
-    ReplicationConfigurationTypeDef,
+    RegistryScanningRuleUnionTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartImageScanResponseTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     TagTypeDef,
     UploadLayerPartResponseTypeDef,
 )
 from .waiter import ImageScanCompleteWaiter, LifecyclePolicyPreviewCompleteWaiter
@@ -536,28 +534,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_registry_policy)
         """
     def put_registry_scanning_configuration(
         self,
         *,
         scanType: ScanTypeType = ...,
-        rules: Sequence[Union[RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef]] = ...
+        rules: Sequence[RegistryScanningRuleUnionTypeDef] = ...
     ) -> PutRegistryScanningConfigurationResponseTypeDef:
         """
         Creates or updates the scanning configuration for your private registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_scanning_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_registry_scanning_configuration)
         """
     def put_replication_configuration(
-        self,
-        *,
-        replicationConfiguration: Union[
-            ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-        ]
+        self, *, replicationConfiguration: ReplicationConfigurationUnionTypeDef
     ) -> PutReplicationConfigurationResponseTypeDef:
         """
         Creates or updates the replication configuration for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_replication_configuration)
         """
@@ -606,15 +600,15 @@
     def upload_layer_part(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
-        layerPartBlob: Union[str, bytes, IO[Any], StreamingBody],
+        layerPartBlob: BlobTypeDef,
         registryId: str = ...
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.upload_layer_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#upload_layer_part)
```

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/literals.py` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/literals.pyi` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/paginator.py` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/paginator.pyi` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/type_defs.py` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ecr.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -49,14 +49,15 @@
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
     "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
+    "BlobTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
     "EncryptionConfigurationTypeDef",
     "ImageScanningConfigurationTypeDef",
     "TagTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
@@ -91,15 +92,14 @@
     "RecommendationTypeDef",
     "ScanningRepositoryFilterTypeDef",
     "ReplicationDestinationTypeDef",
     "RepositoryFilterTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadLayerPartRequestRequestTypeDef",
     "ImageScanFindingTypeDef",
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
     "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleResponseTypeDef",
     "DeleteLifecyclePolicyResponseTypeDef",
     "DeletePullThroughCacheRuleResponseTypeDef",
@@ -121,14 +121,15 @@
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
     "StartImageScanRequestRequestTypeDef",
+    "UploadLayerPartRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
     "PutImageScanningConfigurationResponseTypeDef",
     "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
@@ -162,24 +163,26 @@
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
     "ScoreDetailsTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
     "RegistryScanningConfigurationTypeDef",
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    "RegistryScanningRuleUnionTypeDef",
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "DescribeRegistryResponseTypeDef",
     "PutReplicationConfigurationResponseTypeDef",
     "PutReplicationConfigurationRequestRequestTypeDef",
+    "ReplicationConfigurationUnionTypeDef",
     "ImageScanFindingsTypeDef",
     "DescribeImageScanFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -301,14 +304,15 @@
         "repositoryName": str,
         "failureCode": Literal["REPOSITORY_NOT_FOUND"],
         "failureReason": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCompleteLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCompleteLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
         "uploadId": str,
         "layerDigests": Sequence[str],
     },
@@ -901,39 +905,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_RequiredUploadLayerPartRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "uploadId": str,
-        "partFirstByte": int,
-        "partLastByte": int,
-        "layerPartBlob": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_OptionalUploadLayerPartRequestRequestTypeDef",
-    {
-        "registryId": str,
-    },
-    total=False,
-)
-
-
-class UploadLayerPartRequestRequestTypeDef(
-    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
-):
-    pass
-
-
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "name": str,
         "description": str,
         "uri": str,
         "severity": FindingSeverityType,
@@ -1281,14 +1260,39 @@
 
 class StartImageScanRequestRequestTypeDef(
     _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_RequiredUploadLayerPartRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "uploadId": str,
+        "partFirstByte": int,
+        "partLastByte": int,
+        "layerPartBlob": BlobTypeDef,
+    },
+)
+_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_OptionalUploadLayerPartRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+
+class UploadLayerPartRequestRequestTypeDef(
+    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredPutImageScanningConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
 )
@@ -1883,23 +1887,17 @@
     {
         "scanType": ScanTypeType,
         "rules": List[RegistryScanningRuleOutputTypeDef],
     },
     total=False,
 )
 
-PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
-    {
-        "scanType": ScanTypeType,
-        "rules": Sequence[Union[RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef]],
-    },
-    total=False,
-)
-
+RegistryScanningRuleUnionTypeDef = Union[
+    RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef
+]
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1954,14 +1952,23 @@
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    {
+        "scanType": ScanTypeType,
+        "rules": Sequence[RegistryScanningRuleUnionTypeDef],
+    },
+    total=False,
+)
+
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
         "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1978,14 +1985,17 @@
 PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
+ReplicationConfigurationUnionTypeDef = Union[
+    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+]
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
         "findings": List[ImageScanFindingTypeDef],
```

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/type_defs.pyi` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ecr.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -48,14 +48,15 @@
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
     "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
+    "BlobTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
     "EncryptionConfigurationTypeDef",
     "ImageScanningConfigurationTypeDef",
     "TagTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
@@ -90,15 +91,14 @@
     "RecommendationTypeDef",
     "ScanningRepositoryFilterTypeDef",
     "ReplicationDestinationTypeDef",
     "RepositoryFilterTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadLayerPartRequestRequestTypeDef",
     "ImageScanFindingTypeDef",
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
     "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleResponseTypeDef",
     "DeleteLifecyclePolicyResponseTypeDef",
     "DeletePullThroughCacheRuleResponseTypeDef",
@@ -120,14 +120,15 @@
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
     "StartImageScanRequestRequestTypeDef",
+    "UploadLayerPartRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
     "PutImageScanningConfigurationResponseTypeDef",
     "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
@@ -161,24 +162,26 @@
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
     "ScoreDetailsTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
     "RegistryScanningConfigurationTypeDef",
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    "RegistryScanningRuleUnionTypeDef",
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "DescribeRegistryResponseTypeDef",
     "PutReplicationConfigurationResponseTypeDef",
     "PutReplicationConfigurationRequestRequestTypeDef",
+    "ReplicationConfigurationUnionTypeDef",
     "ImageScanFindingsTypeDef",
     "DescribeImageScanFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -296,14 +299,15 @@
         "repositoryName": str,
         "failureCode": Literal["REPOSITORY_NOT_FOUND"],
         "failureReason": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCompleteLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCompleteLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
         "uploadId": str,
         "layerDigests": Sequence[str],
     },
@@ -864,37 +868,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_RequiredUploadLayerPartRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "uploadId": str,
-        "partFirstByte": int,
-        "partLastByte": int,
-        "layerPartBlob": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_OptionalUploadLayerPartRequestRequestTypeDef",
-    {
-        "registryId": str,
-    },
-    total=False,
-)
-
-class UploadLayerPartRequestRequestTypeDef(
-    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
-):
-    pass
-
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "name": str,
         "description": str,
         "uri": str,
         "severity": FindingSeverityType,
@@ -1232,14 +1213,37 @@
 )
 
 class StartImageScanRequestRequestTypeDef(
     _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
 ):
     pass
 
+_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_RequiredUploadLayerPartRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "uploadId": str,
+        "partFirstByte": int,
+        "partLastByte": int,
+        "layerPartBlob": BlobTypeDef,
+    },
+)
+_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_OptionalUploadLayerPartRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+class UploadLayerPartRequestRequestTypeDef(
+    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
+):
+    pass
+
 _RequiredPutImageScanningConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
 )
@@ -1808,23 +1812,17 @@
     {
         "scanType": ScanTypeType,
         "rules": List[RegistryScanningRuleOutputTypeDef],
     },
     total=False,
 )
 
-PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
-    {
-        "scanType": ScanTypeType,
-        "rules": Sequence[Union[RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef]],
-    },
-    total=False,
-)
-
+RegistryScanningRuleUnionTypeDef = Union[
+    RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef
+]
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1879,14 +1877,23 @@
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    {
+        "scanType": ScanTypeType,
+        "rules": Sequence[RegistryScanningRuleUnionTypeDef],
+    },
+    total=False,
+)
+
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
         "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1903,14 +1910,17 @@
 PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
+ReplicationConfigurationUnionTypeDef = Union[
+    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+]
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
         "findings": List[ImageScanFindingTypeDef],
```

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/waiter.py` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/waiter.pyi` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/PKG-INFO` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ECR 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ecr type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ecr type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
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
@@ -375,33 +375,34 @@
 )
 
 
 def check_value(value: DescribeImageScanFindingsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ecr.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
@@ -436,15 +437,14 @@
     RecommendationTypeDef,
     ScanningRepositoryFilterTypeDef,
     ReplicationDestinationTypeDef,
     RepositoryFilterTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
     ImageScanFindingTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleResponseTypeDef,
@@ -466,14 +466,15 @@
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
     StartImageScanRequestRequestTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
@@ -507,30 +508,32 @@
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
     ScoreDetailsTypeDef,
     DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
     RegistryScanningConfigurationTypeDef,
-    PutRegistryScanningConfigurationRequestRequestTypeDef,
+    RegistryScanningRuleUnionTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
+    PutRegistryScanningConfigurationRequestRequestTypeDef,
     DescribeRegistryResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
     PutReplicationConfigurationRequestRequestTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     ImageScanFindingsTypeDef,
     DescribeImageScanFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/SOURCES.txt` & `mypy-boto3-ecr-1.28.16/mypy_boto3_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15.post1/setup.py` & `mypy-boto3-ecr-1.28.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ECR 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 ecr type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ecr type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ecr": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

