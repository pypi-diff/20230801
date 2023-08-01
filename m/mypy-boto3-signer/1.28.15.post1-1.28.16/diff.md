# Comparing `tmp/mypy-boto3-signer-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-signer-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-signer-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:13 2023, max compression
+gzip compressed data, was "mypy-boto3-signer-1.28.16.tar", last modified: Tue Aug  1 11:37:52 2023, max compression
```

## Comparing `mypy-boto3-signer-1.28.15.post1.tar` & `mypy-boto3-signer-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:13.129408 mypy-boto3-signer-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15997 2023-07-29 10:04:13.125408 mypy-boto3-signer-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:13.117407 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21524 2023-07-29 09:59:43.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-07-29 09:59:43.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-29 09:59:42.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:13.125408 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15997 2023-07-29 10:04:12.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:04:12.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:12.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:04:12.000000 mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:13.129408 mypy-boto3-signer-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:59:41.000000 mypy-boto3-signer-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:52.492727 mypy-boto3-signer-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:14.000000 mypy-boto3-signer-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-08-01 11:37:52.488727 mypy-boto3-signer-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-08-01 11:33:14.000000 mypy-boto3-signer-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:52.488727 mypy-boto3-signer-1.28.16/mypy_boto3_signer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-01 11:33:14.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-01 11:33:14.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:33:14.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-08-01 11:33:15.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-08-01 11:33:15.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-08-01 11:33:15.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-08-01 11:33:15.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-01 11:33:15.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-01 11:33:15.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:14.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-08-01 11:33:16.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-08-01 11:33:15.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:14.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-01 11:33:15.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-01 11:33:15.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:52.488727 mypy-boto3-signer-1.28.16/mypy_boto3_signer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-08-01 11:37:52.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:52.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:52.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:52.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:52.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:37:52.000000 mypy-boto3-signer-1.28.16/mypy_boto3_signer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:52.492727 mypy-boto3-signer-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:33:14.000000 mypy-boto3-signer-1.28.16/setup.py
```

### Comparing `mypy-boto3-signer-1.28.15.post1/LICENSE` & `mypy-boto3-signer-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.15.post1/PKG-INFO` & `mypy-boto3-signer-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.signer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.signer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 signer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 signer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
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
@@ -352,65 +352,67 @@
 )
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
     SigningMaterialTypeDef,
     S3DestinationTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
-    GetRevocationStatusRequestRequestTypeDef,
+    TimestampTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     PaginatorConfigTypeDef,
-    ListSigningJobsRequestRequestTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
     RevokeSignatureRequestRequestTypeDef,
-    RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
     S3SourceTypeDef,
-    SignPayloadRequestRequestTypeDef,
     SigningConfigurationOverridesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddProfilePermissionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionResponseTypeDef,
     SignPayloadResponseTypeDef,
     StartSigningJobResponseTypeDef,
+    SignPayloadRequestRequestTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
+    GetRevocationStatusRequestRequestTypeDef,
+    ListSigningJobsRequestRequestTypeDef,
+    RevokeSigningProfileRequestRequestTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
     ListSigningJobsRequestListSigningJobsPaginateTypeDef,
     ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
@@ -425,15 +427,15 @@
     GetSigningProfileResponseTypeDef,
     PutSigningProfileRequestRequestTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningJobsResponseTypeDef,
 )
 
 
-def get_structure() -> AddProfilePermissionRequestRequestTypeDef:
+def get_value() -> AddProfilePermissionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-signer-1.28.15.post1/README.md` & `mypy-boto3-signer-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
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
@@ -320,65 +320,67 @@
 )
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
     SigningMaterialTypeDef,
     S3DestinationTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
-    GetRevocationStatusRequestRequestTypeDef,
+    TimestampTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     PaginatorConfigTypeDef,
-    ListSigningJobsRequestRequestTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
     RevokeSignatureRequestRequestTypeDef,
-    RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
     S3SourceTypeDef,
-    SignPayloadRequestRequestTypeDef,
     SigningConfigurationOverridesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddProfilePermissionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionResponseTypeDef,
     SignPayloadResponseTypeDef,
     StartSigningJobResponseTypeDef,
+    SignPayloadRequestRequestTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
+    GetRevocationStatusRequestRequestTypeDef,
+    ListSigningJobsRequestRequestTypeDef,
+    RevokeSigningProfileRequestRequestTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
     ListSigningJobsRequestListSigningJobsPaginateTypeDef,
     ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
@@ -393,15 +395,15 @@
     GetSigningProfileResponseTypeDef,
     PutSigningProfileRequestRequestTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningJobsResponseTypeDef,
 )
 
 
-def get_structure() -> AddProfilePermissionRequestRequestTypeDef:
+def get_value() -> AddProfilePermissionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/__init__.py` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/__init__.pyi` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/__main__.py` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.signer 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.signer 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer\nOther"
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

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/client.py` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,27 @@
     from mypy_boto3_signer.client import signerClient
 
     session = Session()
     client: signerClient = session.client("signer")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 from .type_defs import (
     AddProfilePermissionResponseTypeDef,
+    BlobTypeDef,
     DescribeSigningJobResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     GetSigningProfileResponseTypeDef,
     ListProfilePermissionsResponseTypeDef,
@@ -43,48 +42,45 @@
     RemoveProfilePermissionResponseTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningMaterialTypeDef,
     SigningPlatformOverridesTypeDef,
     SignPayloadResponseTypeDef,
     SourceTypeDef,
     StartSigningJobResponseTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import SuccessfulSigningJobWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("signerClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServiceErrorException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class signerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/)
     """
 
     meta: ClientMeta
@@ -93,15 +89,14 @@
     def exceptions(self) -> Exceptions:
         """
         signerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#exceptions)
         """
-
     def add_profile_permission(
         self,
         *,
         profileName: str,
         action: str,
         principal: str,
         statementId: str,
@@ -110,126 +105,115 @@
     ) -> AddProfilePermissionResponseTypeDef:
         """
         Adds cross-account permissions to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.add_profile_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#add_profile_permission)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#can_paginate)
         """
-
     def cancel_signing_profile(self, *, profileName: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of an `ACTIVE` signing profile to `CANCELED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.cancel_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#cancel_signing_profile)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#close)
         """
-
     def describe_signing_job(self, *, jobId: str) -> DescribeSigningJobResponseTypeDef:
         """
         Returns information about a specific code signing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.describe_signing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#describe_signing_job)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#generate_presigned_url)
         """
-
     def get_revocation_status(
         self,
         *,
-        signatureTimestamp: Union[datetime, str],
+        signatureTimestamp: TimestampTypeDef,
         platformId: str,
         profileVersionArn: str,
         jobArn: str,
         certificateHashes: Sequence[str]
     ) -> GetRevocationStatusResponseTypeDef:
         """
         Retrieves the revocation status of one or more of the signing profile, signing
         job, and signing certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_revocation_status)
         """
-
     def get_signing_platform(self, *, platformId: str) -> GetSigningPlatformResponseTypeDef:
         """
         Returns information on a specific signing platform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_platform)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_platform)
         """
-
     def get_signing_profile(
         self, *, profileName: str, profileOwner: str = ...
     ) -> GetSigningProfileResponseTypeDef:
         """
         Returns information on a specific signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_profile)
         """
-
     def list_profile_permissions(
         self, *, profileName: str, nextToken: str = ...
     ) -> ListProfilePermissionsResponseTypeDef:
         """
         Lists the cross-account permissions associated with a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_profile_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_profile_permissions)
         """
-
     def list_signing_jobs(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         isRevoked: bool = ...,
-        signatureExpiresBefore: Union[datetime, str] = ...,
-        signatureExpiresAfter: Union[datetime, str] = ...,
+        signatureExpiresBefore: TimestampTypeDef = ...,
+        signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...
     ) -> ListSigningJobsResponseTypeDef:
         """
         Lists all your signing jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_jobs)
         """
-
     def list_signing_platforms(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
         maxResults: int = ...,
@@ -238,15 +222,14 @@
         """
         Lists all signing platforms available in code signing that match the request
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_platforms)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_platforms)
         """
-
     def list_signing_profiles(
         self,
         *,
         includeCanceled: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         platformId: str = ...,
@@ -254,23 +237,21 @@
     ) -> ListSigningProfilesResponseTypeDef:
         """
         Lists all available signing profiles in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_profiles)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags associated with a signing profile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_tags_for_resource)
         """
-
     def put_signing_profile(
         self,
         *,
         profileName: str,
         platformId: str,
         signingMaterial: SigningMaterialTypeDef = ...,
         signatureValidityPeriod: SignatureValidityPeriodTypeDef = ...,
@@ -280,65 +261,50 @@
     ) -> PutSigningProfileResponseTypeDef:
         """
         Creates a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.put_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#put_signing_profile)
         """
-
     def remove_profile_permission(
         self, *, profileName: str, revisionId: str, statementId: str
     ) -> RemoveProfilePermissionResponseTypeDef:
         """
         Removes cross-account permissions from a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.remove_profile_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#remove_profile_permission)
         """
-
     def revoke_signature(
         self, *, jobId: str, reason: str, jobOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing job to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signature)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signature)
         """
-
     def revoke_signing_profile(
-        self,
-        *,
-        profileName: str,
-        profileVersion: str,
-        reason: str,
-        effectiveTime: Union[datetime, str]
+        self, *, profileName: str, profileVersion: str, reason: str, effectiveTime: TimestampTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing profile to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signing_profile)
         """
-
     def sign_payload(
-        self,
-        *,
-        profileName: str,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
-        payloadFormat: str,
-        profileOwner: str = ...
+        self, *, profileName: str, payload: BlobTypeDef, payloadFormat: str, profileOwner: str = ...
     ) -> SignPayloadResponseTypeDef:
         """
         Signs a binary payload and returns a signature envelope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.sign_payload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#sign_payload)
         """
-
     def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
@@ -346,58 +312,52 @@
     ) -> StartSigningJobResponseTypeDef:
         """
         Initiates a signing job to be performed on the code provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.start_signing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#start_signing_job)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more tags to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#untag_resource)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_jobs"]
     ) -> ListSigningJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_platforms"]
     ) -> ListSigningPlatformsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_profiles"]
     ) -> ListSigningProfilesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
-
     def get_waiter(
         self, waiter_name: Literal["successful_signing_job"]
     ) -> SuccessfulSigningJobWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/client.pyi` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,27 @@
     from mypy_boto3_signer.client import signerClient
 
     session = Session()
     client: signerClient = session.client("signer")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 from .type_defs import (
     AddProfilePermissionResponseTypeDef,
+    BlobTypeDef,
     DescribeSigningJobResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     GetSigningProfileResponseTypeDef,
     ListProfilePermissionsResponseTypeDef,
@@ -43,44 +42,49 @@
     RemoveProfilePermissionResponseTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningMaterialTypeDef,
     SigningPlatformOverridesTypeDef,
     SignPayloadResponseTypeDef,
     SourceTypeDef,
     StartSigningJobResponseTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import SuccessfulSigningJobWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("signerClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServiceErrorException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class signerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/)
     """
 
     meta: ClientMeta
@@ -89,14 +93,15 @@
     def exceptions(self) -> Exceptions:
         """
         signerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#exceptions)
         """
+
     def add_profile_permission(
         self,
         *,
         profileName: str,
         action: str,
         principal: str,
         statementId: str,
@@ -105,115 +110,126 @@
     ) -> AddProfilePermissionResponseTypeDef:
         """
         Adds cross-account permissions to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.add_profile_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#add_profile_permission)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#can_paginate)
         """
+
     def cancel_signing_profile(self, *, profileName: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of an `ACTIVE` signing profile to `CANCELED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.cancel_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#cancel_signing_profile)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#close)
         """
+
     def describe_signing_job(self, *, jobId: str) -> DescribeSigningJobResponseTypeDef:
         """
         Returns information about a specific code signing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.describe_signing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#describe_signing_job)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#generate_presigned_url)
         """
+
     def get_revocation_status(
         self,
         *,
-        signatureTimestamp: Union[datetime, str],
+        signatureTimestamp: TimestampTypeDef,
         platformId: str,
         profileVersionArn: str,
         jobArn: str,
         certificateHashes: Sequence[str]
     ) -> GetRevocationStatusResponseTypeDef:
         """
         Retrieves the revocation status of one or more of the signing profile, signing
         job, and signing certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_revocation_status)
         """
+
     def get_signing_platform(self, *, platformId: str) -> GetSigningPlatformResponseTypeDef:
         """
         Returns information on a specific signing platform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_platform)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_platform)
         """
+
     def get_signing_profile(
         self, *, profileName: str, profileOwner: str = ...
     ) -> GetSigningProfileResponseTypeDef:
         """
         Returns information on a specific signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_profile)
         """
+
     def list_profile_permissions(
         self, *, profileName: str, nextToken: str = ...
     ) -> ListProfilePermissionsResponseTypeDef:
         """
         Lists the cross-account permissions associated with a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_profile_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_profile_permissions)
         """
+
     def list_signing_jobs(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         isRevoked: bool = ...,
-        signatureExpiresBefore: Union[datetime, str] = ...,
-        signatureExpiresAfter: Union[datetime, str] = ...,
+        signatureExpiresBefore: TimestampTypeDef = ...,
+        signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...
     ) -> ListSigningJobsResponseTypeDef:
         """
         Lists all your signing jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_jobs)
         """
+
     def list_signing_platforms(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
         maxResults: int = ...,
@@ -222,14 +238,15 @@
         """
         Lists all signing platforms available in code signing that match the request
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_platforms)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_platforms)
         """
+
     def list_signing_profiles(
         self,
         *,
         includeCanceled: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         platformId: str = ...,
@@ -237,21 +254,23 @@
     ) -> ListSigningProfilesResponseTypeDef:
         """
         Lists all available signing profiles in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_profiles)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags associated with a signing profile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_tags_for_resource)
         """
+
     def put_signing_profile(
         self,
         *,
         profileName: str,
         platformId: str,
         signingMaterial: SigningMaterialTypeDef = ...,
         signatureValidityPeriod: SignatureValidityPeriodTypeDef = ...,
@@ -261,60 +280,55 @@
     ) -> PutSigningProfileResponseTypeDef:
         """
         Creates a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.put_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#put_signing_profile)
         """
+
     def remove_profile_permission(
         self, *, profileName: str, revisionId: str, statementId: str
     ) -> RemoveProfilePermissionResponseTypeDef:
         """
         Removes cross-account permissions from a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.remove_profile_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#remove_profile_permission)
         """
+
     def revoke_signature(
         self, *, jobId: str, reason: str, jobOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing job to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signature)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signature)
         """
+
     def revoke_signing_profile(
-        self,
-        *,
-        profileName: str,
-        profileVersion: str,
-        reason: str,
-        effectiveTime: Union[datetime, str]
+        self, *, profileName: str, profileVersion: str, reason: str, effectiveTime: TimestampTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing profile to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signing_profile)
         """
+
     def sign_payload(
-        self,
-        *,
-        profileName: str,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
-        payloadFormat: str,
-        profileOwner: str = ...
+        self, *, profileName: str, payload: BlobTypeDef, payloadFormat: str, profileOwner: str = ...
     ) -> SignPayloadResponseTypeDef:
         """
         Signs a binary payload and returns a signature envelope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.sign_payload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#sign_payload)
         """
+
     def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
@@ -322,52 +336,58 @@
     ) -> StartSigningJobResponseTypeDef:
         """
         Initiates a signing job to be performed on the code provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.start_signing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#start_signing_job)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more tags to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#untag_resource)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_jobs"]
     ) -> ListSigningJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_platforms"]
     ) -> ListSigningPlatformsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_profiles"]
     ) -> ListSigningProfilesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
+
     def get_waiter(
         self, waiter_name: Literal["successful_signing_job"]
     ) -> SuccessfulSigningJobWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/literals.py` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/literals.pyi` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/paginator.py` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,25 @@
     client: signerClient = session.client("signer")
 
     list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
     list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")
     list_signing_profiles_paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .type_defs import (
     ListSigningJobsResponseTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningProfilesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
 )
@@ -62,16 +62,16 @@
     def paginate(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
-        signatureExpiresBefore: Union[datetime, str] = ...,
-        signatureExpiresAfter: Union[datetime, str] = ...,
+        signatureExpiresBefore: TimestampTypeDef = ...,
+        signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
         """
```

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/paginator.pyi` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,25 @@
     client: signerClient = session.client("signer")
 
     list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
     list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")
     list_signing_profiles_paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .type_defs import (
     ListSigningJobsResponseTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningProfilesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
 )
@@ -59,16 +59,16 @@
     def paginate(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
-        signatureExpiresBefore: Union[datetime, str] = ...,
-        signatureExpiresAfter: Union[datetime, str] = ...,
+        signatureExpiresBefore: TimestampTypeDef = ...,
+        signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
         """
```

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/type_defs.py` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
-    data: AddProfilePermissionRequestRequestTypeDef = {...}
+    data: AddProfilePermissionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -35,54 +35,56 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
     "SigningMaterialTypeDef",
     "S3DestinationTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
-    "GetRevocationStatusRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
     "SignatureValidityPeriodTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "PaginatorConfigTypeDef",
-    "ListSigningJobsRequestRequestTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
-    "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
     "S3SourceTypeDef",
-    "SignPayloadRequestRequestTypeDef",
     "SigningConfigurationOverridesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddProfilePermissionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetRevocationStatusResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutSigningProfileResponseTypeDef",
     "RemoveProfilePermissionResponseTypeDef",
     "SignPayloadResponseTypeDef",
     "StartSigningJobResponseTypeDef",
+    "SignPayloadRequestRequestTypeDef",
     "DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     "DestinationTypeDef",
+    "GetRevocationStatusRequestRequestTypeDef",
+    "ListSigningJobsRequestRequestTypeDef",
+    "RevokeSigningProfileRequestRequestTypeDef",
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
     "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
     "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
@@ -133,14 +135,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
     },
 )
 
@@ -190,25 +193,15 @@
     "EncryptionAlgorithmOptionsTypeDef",
     {
         "allowedValues": List[EncryptionAlgorithmType],
         "defaultValue": EncryptionAlgorithmType,
     },
 )
 
-GetRevocationStatusRequestRequestTypeDef = TypedDict(
-    "GetRevocationStatusRequestRequestTypeDef",
-    {
-        "signatureTimestamp": Union[datetime, str],
-        "platformId": str,
-        "profileVersionArn": str,
-        "jobArn": str,
-        "certificateHashes": Sequence[str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 GetSigningPlatformRequestRequestTypeDef = TypedDict(
     "GetSigningPlatformRequestRequestTypeDef",
     {
         "platformId": str,
     },
 )
 
@@ -307,30 +300,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListSigningJobsRequestRequestTypeDef = TypedDict(
-    "ListSigningJobsRequestRequestTypeDef",
-    {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "maxResults": int,
-        "nextToken": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-    },
-    total=False,
-)
-
 ListSigningPlatformsRequestRequestTypeDef = TypedDict(
     "ListSigningPlatformsRequestRequestTypeDef",
     {
         "category": str,
         "partner": str,
         "target": str,
         "maxResults": int,
@@ -385,24 +362,14 @@
 
 class RevokeSignatureRequestRequestTypeDef(
     _RequiredRevokeSignatureRequestRequestTypeDef, _OptionalRevokeSignatureRequestRequestTypeDef
 ):
     pass
 
 
-RevokeSigningProfileRequestRequestTypeDef = TypedDict(
-    "RevokeSigningProfileRequestRequestTypeDef",
-    {
-        "profileName": str,
-        "profileVersion": str,
-        "reason": str,
-        "effectiveTime": Union[datetime, str],
-    },
-)
-
 S3SignedObjectTypeDef = TypedDict(
     "S3SignedObjectTypeDef",
     {
         "bucketName": str,
         "key": str,
     },
     total=False,
@@ -413,37 +380,14 @@
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
 )
 
-_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
-    "_RequiredSignPayloadRequestRequestTypeDef",
-    {
-        "profileName": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
-        "payloadFormat": str,
-    },
-)
-_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
-    "_OptionalSignPayloadRequestRequestTypeDef",
-    {
-        "profileOwner": str,
-    },
-    total=False,
-)
-
-
-class SignPayloadRequestRequestTypeDef(
-    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
-):
-    pass
-
-
 SigningConfigurationOverridesTypeDef = TypedDict(
     "SigningConfigurationOverridesTypeDef",
     {
         "encryptionAlgorithm": EncryptionAlgorithmType,
         "hashAlgorithm": HashAlgorithmType,
     },
     total=False,
@@ -530,14 +474,37 @@
     {
         "jobId": str,
         "jobOwner": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
+    "_RequiredSignPayloadRequestRequestTypeDef",
+    {
+        "profileName": str,
+        "payload": BlobTypeDef,
+        "payloadFormat": str,
+    },
+)
+_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
+    "_OptionalSignPayloadRequestRequestTypeDef",
+    {
+        "profileOwner": str,
+    },
+    total=False,
+)
+
+
+class SignPayloadRequestRequestTypeDef(
+    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
@@ -560,14 +527,51 @@
     "DestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
     },
     total=False,
 )
 
+GetRevocationStatusRequestRequestTypeDef = TypedDict(
+    "GetRevocationStatusRequestRequestTypeDef",
+    {
+        "signatureTimestamp": TimestampTypeDef,
+        "platformId": str,
+        "profileVersionArn": str,
+        "jobArn": str,
+        "certificateHashes": Sequence[str],
+    },
+)
+
+ListSigningJobsRequestRequestTypeDef = TypedDict(
+    "ListSigningJobsRequestRequestTypeDef",
+    {
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "maxResults": int,
+        "nextToken": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": TimestampTypeDef,
+        "signatureExpiresAfter": TimestampTypeDef,
+        "jobInvoker": str,
+    },
+    total=False,
+)
+
+RevokeSigningProfileRequestRequestTypeDef = TypedDict(
+    "RevokeSigningProfileRequestRequestTypeDef",
+    {
+        "profileName": str,
+        "profileVersion": str,
+        "reason": str,
+        "effectiveTime": TimestampTypeDef,
+    },
+)
+
 SigningProfileTypeDef = TypedDict(
     "SigningProfileTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
         "signingMaterial": SigningMaterialTypeDef,
@@ -604,16 +608,16 @@
 ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
     "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     {
         "status": SigningStatusType,
         "platformId": str,
         "requestedBy": str,
         "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
+        "signatureExpiresBefore": TimestampTypeDef,
+        "signatureExpiresAfter": TimestampTypeDef,
         "jobInvoker": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
```

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/type_defs.pyi` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
-    data: AddProfilePermissionRequestRequestTypeDef = {...}
+    data: AddProfilePermissionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -34,54 +34,56 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
     "SigningMaterialTypeDef",
     "S3DestinationTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
-    "GetRevocationStatusRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
     "SignatureValidityPeriodTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "PaginatorConfigTypeDef",
-    "ListSigningJobsRequestRequestTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
-    "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
     "S3SourceTypeDef",
-    "SignPayloadRequestRequestTypeDef",
     "SigningConfigurationOverridesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddProfilePermissionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetRevocationStatusResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutSigningProfileResponseTypeDef",
     "RemoveProfilePermissionResponseTypeDef",
     "SignPayloadResponseTypeDef",
     "StartSigningJobResponseTypeDef",
+    "SignPayloadRequestRequestTypeDef",
     "DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     "DestinationTypeDef",
+    "GetRevocationStatusRequestRequestTypeDef",
+    "ListSigningJobsRequestRequestTypeDef",
+    "RevokeSigningProfileRequestRequestTypeDef",
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
     "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
     "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
@@ -130,14 +132,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
     },
 )
 
@@ -187,25 +190,15 @@
     "EncryptionAlgorithmOptionsTypeDef",
     {
         "allowedValues": List[EncryptionAlgorithmType],
         "defaultValue": EncryptionAlgorithmType,
     },
 )
 
-GetRevocationStatusRequestRequestTypeDef = TypedDict(
-    "GetRevocationStatusRequestRequestTypeDef",
-    {
-        "signatureTimestamp": Union[datetime, str],
-        "platformId": str,
-        "profileVersionArn": str,
-        "jobArn": str,
-        "certificateHashes": Sequence[str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 GetSigningPlatformRequestRequestTypeDef = TypedDict(
     "GetSigningPlatformRequestRequestTypeDef",
     {
         "platformId": str,
     },
 )
 
@@ -300,30 +293,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListSigningJobsRequestRequestTypeDef = TypedDict(
-    "ListSigningJobsRequestRequestTypeDef",
-    {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "maxResults": int,
-        "nextToken": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-    },
-    total=False,
-)
-
 ListSigningPlatformsRequestRequestTypeDef = TypedDict(
     "ListSigningPlatformsRequestRequestTypeDef",
     {
         "category": str,
         "partner": str,
         "target": str,
         "maxResults": int,
@@ -376,24 +353,14 @@
 )
 
 class RevokeSignatureRequestRequestTypeDef(
     _RequiredRevokeSignatureRequestRequestTypeDef, _OptionalRevokeSignatureRequestRequestTypeDef
 ):
     pass
 
-RevokeSigningProfileRequestRequestTypeDef = TypedDict(
-    "RevokeSigningProfileRequestRequestTypeDef",
-    {
-        "profileName": str,
-        "profileVersion": str,
-        "reason": str,
-        "effectiveTime": Union[datetime, str],
-    },
-)
-
 S3SignedObjectTypeDef = TypedDict(
     "S3SignedObjectTypeDef",
     {
         "bucketName": str,
         "key": str,
     },
     total=False,
@@ -404,35 +371,14 @@
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
 )
 
-_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
-    "_RequiredSignPayloadRequestRequestTypeDef",
-    {
-        "profileName": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
-        "payloadFormat": str,
-    },
-)
-_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
-    "_OptionalSignPayloadRequestRequestTypeDef",
-    {
-        "profileOwner": str,
-    },
-    total=False,
-)
-
-class SignPayloadRequestRequestTypeDef(
-    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
-):
-    pass
-
 SigningConfigurationOverridesTypeDef = TypedDict(
     "SigningConfigurationOverridesTypeDef",
     {
         "encryptionAlgorithm": EncryptionAlgorithmType,
         "hashAlgorithm": HashAlgorithmType,
     },
     total=False,
@@ -519,14 +465,35 @@
     {
         "jobId": str,
         "jobOwner": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
+    "_RequiredSignPayloadRequestRequestTypeDef",
+    {
+        "profileName": str,
+        "payload": BlobTypeDef,
+        "payloadFormat": str,
+    },
+)
+_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
+    "_OptionalSignPayloadRequestRequestTypeDef",
+    {
+        "profileOwner": str,
+    },
+    total=False,
+)
+
+class SignPayloadRequestRequestTypeDef(
+    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
+):
+    pass
+
 _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
@@ -547,14 +514,51 @@
     "DestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
     },
     total=False,
 )
 
+GetRevocationStatusRequestRequestTypeDef = TypedDict(
+    "GetRevocationStatusRequestRequestTypeDef",
+    {
+        "signatureTimestamp": TimestampTypeDef,
+        "platformId": str,
+        "profileVersionArn": str,
+        "jobArn": str,
+        "certificateHashes": Sequence[str],
+    },
+)
+
+ListSigningJobsRequestRequestTypeDef = TypedDict(
+    "ListSigningJobsRequestRequestTypeDef",
+    {
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "maxResults": int,
+        "nextToken": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": TimestampTypeDef,
+        "signatureExpiresAfter": TimestampTypeDef,
+        "jobInvoker": str,
+    },
+    total=False,
+)
+
+RevokeSigningProfileRequestRequestTypeDef = TypedDict(
+    "RevokeSigningProfileRequestRequestTypeDef",
+    {
+        "profileName": str,
+        "profileVersion": str,
+        "reason": str,
+        "effectiveTime": TimestampTypeDef,
+    },
+)
+
 SigningProfileTypeDef = TypedDict(
     "SigningProfileTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
         "signingMaterial": SigningMaterialTypeDef,
@@ -591,16 +595,16 @@
 ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
     "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     {
         "status": SigningStatusType,
         "platformId": str,
         "requestedBy": str,
         "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
+        "signatureExpiresBefore": TimestampTypeDef,
+        "signatureExpiresAfter": TimestampTypeDef,
         "jobInvoker": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
```

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/waiter.py` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer/waiter.pyi` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer.egg-info/PKG-INFO` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.signer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.signer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 signer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 signer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
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
@@ -352,65 +352,67 @@
 )
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
     SigningMaterialTypeDef,
     S3DestinationTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
-    GetRevocationStatusRequestRequestTypeDef,
+    TimestampTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     PaginatorConfigTypeDef,
-    ListSigningJobsRequestRequestTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
     RevokeSignatureRequestRequestTypeDef,
-    RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
     S3SourceTypeDef,
-    SignPayloadRequestRequestTypeDef,
     SigningConfigurationOverridesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddProfilePermissionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionResponseTypeDef,
     SignPayloadResponseTypeDef,
     StartSigningJobResponseTypeDef,
+    SignPayloadRequestRequestTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
+    GetRevocationStatusRequestRequestTypeDef,
+    ListSigningJobsRequestRequestTypeDef,
+    RevokeSigningProfileRequestRequestTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
     ListSigningJobsRequestListSigningJobsPaginateTypeDef,
     ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
@@ -425,15 +427,15 @@
     GetSigningProfileResponseTypeDef,
     PutSigningProfileRequestRequestTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningJobsResponseTypeDef,
 )
 
 
-def get_structure() -> AddProfilePermissionRequestRequestTypeDef:
+def get_value() -> AddProfilePermissionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-signer-1.28.15.post1/mypy_boto3_signer.egg-info/SOURCES.txt` & `mypy-boto3-signer-1.28.16/mypy_boto3_signer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.15.post1/setup.py` & `mypy-boto3-signer-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-signer",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_signer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.signer 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.signer 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 signer type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 signer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_signer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

