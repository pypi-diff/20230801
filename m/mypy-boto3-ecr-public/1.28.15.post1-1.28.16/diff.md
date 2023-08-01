# Comparing `tmp/mypy-boto3-ecr-public-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ecr-public-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-public-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-public-1.28.16.tar", last modified: Tue Aug  1 11:36:42 2023, max compression
```

## Comparing `mypy-boto3-ecr-public-1.28.15.post1.tar` & `mypy-boto3-ecr-public-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.349127 mypy-boto3-ecr-public-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-07-29 10:03:02.345127 mypy-boto3-ecr-public-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.341127 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-29 09:44:16.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23708 2023-07-29 09:44:16.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-07-29 09:44:16.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.345127 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.349127 mypy-boto3-ecr-public-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.272901 mypy-boto3-ecr-public-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:16:49.000000 mypy-boto3-ecr-public-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-08-01 11:36:42.272901 mypy-boto3-ecr-public-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-08-01 11:16:49.000000 mypy-boto3-ecr-public-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.260901 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-01 11:16:49.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-01 11:16:49.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-01 11:16:49.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-08-01 11:16:50.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-08-01 11:16:50.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-08-01 11:16:50.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-08-01 11:16:50.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-01 11:16:50.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-08-01 11:16:50.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:16:49.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23721 2023-08-01 11:16:51.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-08-01 11:16:50.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:16:49.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.272901 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-08-01 11:36:42.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:36:42.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:42.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:42.000000 mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:42.272901 mypy-boto3-ecr-public-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-01 11:16:49.000000 mypy-boto3-ecr-public-1.28.16/setup.py
```

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/LICENSE` & `mypy-boto3-ecr-public-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/PKG-INFO` & `mypy-boto3-ecr-public-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ECRPublic 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ecr-public type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ecr-public type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr-public)](https://pepy.tech/project/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
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
@@ -330,31 +330,31 @@
 )
 
 
 def check_value(value: DescribeImageTagsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ecr_public.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
@@ -368,29 +368,28 @@
     InitiateLayerUploadRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
     CompleteLayerUploadResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
     GetAuthorizationTokenResponseTypeDef,
     GetRepositoryPolicyResponseTypeDef,
     InitiateLayerUploadResponseTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
-    PutRepositoryCatalogDataRequestRequestTypeDef,
-    CreateRepositoryRequestRequestTypeDef,
+    RepositoryCatalogDataInputTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
@@ -401,20 +400,22 @@
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
+    CreateRepositoryRequestRequestTypeDef,
+    PutRepositoryCatalogDataRequestRequestTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationDataTypeDef:
+def get_value() -> AuthorizationDataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/README.md` & `mypy-boto3-ecr-public-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr-public)](https://pepy.tech/project/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
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
@@ -298,31 +298,31 @@
 )
 
 
 def check_value(value: DescribeImageTagsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ecr_public.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
@@ -336,29 +336,28 @@
     InitiateLayerUploadRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
     CompleteLayerUploadResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
     GetAuthorizationTokenResponseTypeDef,
     GetRepositoryPolicyResponseTypeDef,
     InitiateLayerUploadResponseTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
-    PutRepositoryCatalogDataRequestRequestTypeDef,
-    CreateRepositoryRequestRequestTypeDef,
+    RepositoryCatalogDataInputTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
@@ -369,20 +368,22 @@
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
+    CreateRepositoryRequestRequestTypeDef,
+    PutRepositoryCatalogDataRequestRequestTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationDataTypeDef:
+def get_value() -> AuthorizationDataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__init__.py` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__init__.pyi` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__main__.py` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECRPublic 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ECRPublic 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
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

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/client.py` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     from mypy_boto3_ecr_public.client import ECRPublicClient
 
     session = Session()
     client: ECRPublicClient = session.client("ecr-public")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     DescribeImagesPaginator,
     DescribeImageTagsPaginator,
     DescribeRegistriesPaginator,
     DescribeRepositoriesPaginator,
 )
 from .type_defs import (
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageResponseTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeImagesResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
@@ -403,15 +403,15 @@
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.upload_layer_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/client/#upload_layer_part)
```

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/client.pyi` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     from mypy_boto3_ecr_public.client import ECRPublicClient
 
     session = Session()
     client: ECRPublicClient = session.client("ecr-public")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     DescribeImagesPaginator,
     DescribeImageTagsPaginator,
     DescribeRegistriesPaginator,
     DescribeRepositoriesPaginator,
 )
 from .type_defs import (
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageResponseTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeImagesResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
@@ -373,15 +373,15 @@
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.upload_layer_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/client/#upload_layer_part)
```

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/literals.py` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/literals.pyi` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/paginator.py` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/paginator.pyi` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/type_defs.py` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ecr_public.type_defs import AuthorizationDataTypeDef
 
-    data: AuthorizationDataTypeDef = {...}
+    data: AuthorizationDataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -33,16 +33,16 @@
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
     "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
+    "BlobTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeImageTagsRequestRequestTypeDef",
@@ -56,29 +56,28 @@
     "InitiateLayerUploadRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadLayerPartRequestRequestTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
     "CompleteLayerUploadResponseTypeDef",
     "DeleteRepositoryPolicyResponseTypeDef",
     "GetAuthorizationTokenResponseTypeDef",
     "GetRepositoryPolicyResponseTypeDef",
     "InitiateLayerUploadResponseTypeDef",
     "SetRepositoryPolicyResponseTypeDef",
     "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
-    "PutRepositoryCatalogDataRequestRequestTypeDef",
-    "CreateRepositoryRequestRequestTypeDef",
+    "RepositoryCatalogDataInputTypeDef",
+    "UploadLayerPartRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
@@ -89,14 +88,16 @@
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
+    "CreateRepositoryRequestRequestTypeDef",
+    "PutRepositoryCatalogDataRequestRequestTypeDef",
     "DescribeImageTagsResponseTypeDef",
     "DescribeRegistriesResponseTypeDef",
 )
 
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
@@ -166,14 +167,15 @@
     {
         "imageDigest": str,
         "imageTag": str,
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
@@ -190,27 +192,14 @@
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
 
-RepositoryCatalogDataInputTypeDef = TypedDict(
-    "RepositoryCatalogDataInputTypeDef",
-    {
-        "description": str,
-        "architectures": Sequence[str],
-        "operatingSystems": Sequence[str],
-        "logoImageBlob": Union[str, bytes, IO[Any], StreamingBody],
-        "aboutText": str,
-        "usageText": str,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -518,39 +507,14 @@
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
 BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
     "BatchCheckLayerAvailabilityResponseTypeDef",
     {
         "layers": List[LayerTypeDef],
         "failures": List[LayerFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -689,55 +653,48 @@
         "imageId": ImageIdentifierTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
-_RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRepositoryCatalogDataRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "catalogData": RepositoryCatalogDataInputTypeDef,
-    },
-)
-_OptionalPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
+RepositoryCatalogDataInputTypeDef = TypedDict(
+    "RepositoryCatalogDataInputTypeDef",
     {
-        "registryId": str,
+        "description": str,
+        "architectures": Sequence[str],
+        "operatingSystems": Sequence[str],
+        "logoImageBlob": BlobTypeDef,
+        "aboutText": str,
+        "usageText": str,
     },
     total=False,
 )
 
-
-class PutRepositoryCatalogDataRequestRequestTypeDef(
-    _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
-    _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRepositoryRequestRequestTypeDef",
+_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_RequiredUploadLayerPartRequestRequestTypeDef",
     {
         "repositoryName": str,
+        "uploadId": str,
+        "partFirstByte": int,
+        "partLastByte": int,
+        "layerPartBlob": BlobTypeDef,
     },
 )
-_OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRepositoryRequestRequestTypeDef",
+_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
-        "catalogData": RepositoryCatalogDataInputTypeDef,
-        "tags": Sequence[TagTypeDef],
+        "registryId": str,
     },
     total=False,
 )
 
 
-class CreateRepositoryRequestRequestTypeDef(
-    _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
+class UploadLayerPartRequestRequestTypeDef(
+    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
@@ -920,14 +877,59 @@
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRepositoryRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRepositoryRequestRequestTypeDef",
+    {
+        "catalogData": RepositoryCatalogDataInputTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateRepositoryRequestRequestTypeDef(
+    _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRepositoryCatalogDataRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "catalogData": RepositoryCatalogDataInputTypeDef,
+    },
+)
+_OptionalPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+
+class PutRepositoryCatalogDataRequestRequestTypeDef(
+    _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
+    _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeImageTagsResponseTypeDef = TypedDict(
     "DescribeImageTagsResponseTypeDef",
     {
         "imageTagDetails": List[ImageTagDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/type_defs.pyi` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ecr_public.type_defs import AuthorizationDataTypeDef
 
-    data: AuthorizationDataTypeDef = {...}
+    data: AuthorizationDataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -32,16 +32,16 @@
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
     "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
+    "BlobTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeImageTagsRequestRequestTypeDef",
@@ -55,29 +55,28 @@
     "InitiateLayerUploadRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadLayerPartRequestRequestTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
     "CompleteLayerUploadResponseTypeDef",
     "DeleteRepositoryPolicyResponseTypeDef",
     "GetAuthorizationTokenResponseTypeDef",
     "GetRepositoryPolicyResponseTypeDef",
     "InitiateLayerUploadResponseTypeDef",
     "SetRepositoryPolicyResponseTypeDef",
     "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
-    "PutRepositoryCatalogDataRequestRequestTypeDef",
-    "CreateRepositoryRequestRequestTypeDef",
+    "RepositoryCatalogDataInputTypeDef",
+    "UploadLayerPartRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
@@ -88,14 +87,16 @@
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
+    "CreateRepositoryRequestRequestTypeDef",
+    "PutRepositoryCatalogDataRequestRequestTypeDef",
     "DescribeImageTagsResponseTypeDef",
     "DescribeRegistriesResponseTypeDef",
 )
 
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
@@ -163,14 +164,15 @@
     {
         "imageDigest": str,
         "imageTag": str,
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
@@ -185,27 +187,14 @@
 
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-RepositoryCatalogDataInputTypeDef = TypedDict(
-    "RepositoryCatalogDataInputTypeDef",
-    {
-        "description": str,
-        "architectures": Sequence[str],
-        "operatingSystems": Sequence[str],
-        "logoImageBlob": Union[str, bytes, IO[Any], StreamingBody],
-        "aboutText": str,
-        "usageText": str,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -497,37 +486,14 @@
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
 BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
     "BatchCheckLayerAvailabilityResponseTypeDef",
     {
         "layers": List[LayerTypeDef],
         "failures": List[LayerFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -662,52 +628,47 @@
         "imageId": ImageIdentifierTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
-_RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRepositoryCatalogDataRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "catalogData": RepositoryCatalogDataInputTypeDef,
-    },
-)
-_OptionalPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
+RepositoryCatalogDataInputTypeDef = TypedDict(
+    "RepositoryCatalogDataInputTypeDef",
     {
-        "registryId": str,
+        "description": str,
+        "architectures": Sequence[str],
+        "operatingSystems": Sequence[str],
+        "logoImageBlob": BlobTypeDef,
+        "aboutText": str,
+        "usageText": str,
     },
     total=False,
 )
 
-class PutRepositoryCatalogDataRequestRequestTypeDef(
-    _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
-    _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRepositoryRequestRequestTypeDef",
+_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_RequiredUploadLayerPartRequestRequestTypeDef",
     {
         "repositoryName": str,
+        "uploadId": str,
+        "partFirstByte": int,
+        "partLastByte": int,
+        "layerPartBlob": BlobTypeDef,
     },
 )
-_OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRepositoryRequestRequestTypeDef",
+_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
-        "catalogData": RepositoryCatalogDataInputTypeDef,
-        "tags": Sequence[TagTypeDef],
+        "registryId": str,
     },
     total=False,
 )
 
-class CreateRepositoryRequestRequestTypeDef(
-    _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
+class UploadLayerPartRequestRequestTypeDef(
+    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
@@ -885,14 +846,55 @@
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRepositoryRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRepositoryRequestRequestTypeDef",
+    {
+        "catalogData": RepositoryCatalogDataInputTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateRepositoryRequestRequestTypeDef(
+    _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
+):
+    pass
+
+_RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRepositoryCatalogDataRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "catalogData": RepositoryCatalogDataInputTypeDef,
+    },
+)
+_OptionalPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+class PutRepositoryCatalogDataRequestRequestTypeDef(
+    _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
+    _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
+):
+    pass
+
 DescribeImageTagsResponseTypeDef = TypedDict(
     "DescribeImageTagsResponseTypeDef",
     {
         "imageTagDetails": List[ImageTagDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/PKG-INFO` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ECRPublic 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ecr-public type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ecr-public type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr-public)](https://pepy.tech/project/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
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
@@ -330,31 +330,31 @@
 )
 
 
 def check_value(value: DescribeImageTagsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ecr_public.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
@@ -368,29 +368,28 @@
     InitiateLayerUploadRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
     CompleteLayerUploadResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
     GetAuthorizationTokenResponseTypeDef,
     GetRepositoryPolicyResponseTypeDef,
     InitiateLayerUploadResponseTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
-    PutRepositoryCatalogDataRequestRequestTypeDef,
-    CreateRepositoryRequestRequestTypeDef,
+    RepositoryCatalogDataInputTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
@@ -401,20 +400,22 @@
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
+    CreateRepositoryRequestRequestTypeDef,
+    PutRepositoryCatalogDataRequestRequestTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationDataTypeDef:
+def get_value() -> AuthorizationDataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/SOURCES.txt` & `mypy-boto3-ecr-public-1.28.16/mypy_boto3_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15.post1/setup.py` & `mypy-boto3-ecr-public-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr-public",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.ECRPublic 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 ecr-public type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ecr-public type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ecr_public": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

