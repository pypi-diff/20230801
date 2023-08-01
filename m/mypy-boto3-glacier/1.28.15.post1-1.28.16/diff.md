# Comparing `tmp/mypy-boto3-glacier-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-glacier-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glacier-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:12 2023, max compression
+gzip compressed data, was "mypy-boto3-glacier-1.28.16.tar", last modified: Tue Aug  1 11:36:52 2023, max compression
```

## Comparing `mypy-boto3-glacier-1.28.15.post1.tar` & `mypy-boto3-glacier-1.28.16.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:12.445165 mypy-boto3-glacier-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19841 2023-07-29 10:03:12.445165 mypy-boto3-glacier-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:12.433165 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26791 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26745 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-29 09:46:03.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    39087 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39382 2023-07-29 09:46:04.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-07-29 09:46:03.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:12.445165 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19841 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:12.445165 mypy-boto3-glacier-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:46:01.000000 mypy-boto3-glacier-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.528881 mypy-boto3-glacier-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19926 2023-08-01 11:36:52.528881 mypy-boto3-glacier-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.528881 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26501 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26455 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38920 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39645 2023-08-01 11:18:42.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-08-01 11:18:42.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-01 11:18:39.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.528881 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19926 2023-08-01 11:36:52.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 11:36:52.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:52.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:52.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:52.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:36:52.000000 mypy-boto3-glacier-1.28.16/mypy_boto3_glacier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:52.528881 mypy-boto3-glacier-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:18:38.000000 mypy-boto3-glacier-1.28.16/setup.py
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/LICENSE` & `mypy-boto3-glacier-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/PKG-INFO` & `mypy-boto3-glacier-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glacier
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Glacier 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 glacier type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 glacier type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glacier)](https://pepy.tech/project/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +78,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -427,27 +427,28 @@
 )
 
 
 def check_value(value: ActionCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_glacier.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
@@ -486,31 +487,31 @@
     ListProvisionedCapacityInputRequestTypeDef,
     ProvisionedCapacityDescriptionTypeDef,
     ListTagsForVaultInputRequestTypeDef,
     ListVaultsInputRequestTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
     VaultNotificationConfigTypeDef,
-    UploadArchiveInputRequestTypeDef,
-    UploadArchiveInputVaultUploadArchiveTypeDef,
-    UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
-    UploadMultipartPartInputRequestTypeDef,
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
     DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultLockOutputTypeDef,
     InitiateJobOutputTypeDef,
     InitiateMultipartUploadOutputTypeDef,
     InitiateVaultLockOutputTypeDef,
     InventoryRetrievalJobDescriptionResponseTypeDef,
     ListTagsForVaultOutputTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
+    UploadArchiveInputRequestTypeDef,
+    UploadArchiveInputVaultUploadArchiveTypeDef,
+    UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
+    UploadMultipartPartInputRequestTypeDef,
     InputSerializationTypeDef,
     OutputSerializationTypeDef,
     DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
@@ -524,31 +525,33 @@
     ListPartsInputListPartsPaginateTypeDef,
     ListVaultsInputListVaultsPaginateTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
     SetVaultNotificationsInputNotificationSetTypeDef,
     SetVaultNotificationsInputRequestTypeDef,
+    VaultNotificationConfigUnionTypeDef,
     SelectParametersResponseTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
+    DataRetrievalPolicyUnionTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
     S3LocationOutputTypeDef,
     S3LocationTypeDef,
     OutputLocationOutputTypeDef,
     OutputLocationTypeDef,
     GlacierJobDescriptionResponseTypeDef,
     GlacierJobDescriptionTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     InitiateJobInputRequestTypeDef,
 )
 
 
-def get_structure() -> AbortMultipartUploadInputRequestTypeDef:
+def get_value() -> AbortMultipartUploadInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/README.md` & `mypy-boto3-glacier-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glacier)](https://pepy.tech/project/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -46,15 +46,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -395,27 +395,28 @@
 )
 
 
 def check_value(value: ActionCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_glacier.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
@@ -454,31 +455,31 @@
     ListProvisionedCapacityInputRequestTypeDef,
     ProvisionedCapacityDescriptionTypeDef,
     ListTagsForVaultInputRequestTypeDef,
     ListVaultsInputRequestTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
     VaultNotificationConfigTypeDef,
-    UploadArchiveInputRequestTypeDef,
-    UploadArchiveInputVaultUploadArchiveTypeDef,
-    UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
-    UploadMultipartPartInputRequestTypeDef,
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
     DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultLockOutputTypeDef,
     InitiateJobOutputTypeDef,
     InitiateMultipartUploadOutputTypeDef,
     InitiateVaultLockOutputTypeDef,
     InventoryRetrievalJobDescriptionResponseTypeDef,
     ListTagsForVaultOutputTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
+    UploadArchiveInputRequestTypeDef,
+    UploadArchiveInputVaultUploadArchiveTypeDef,
+    UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
+    UploadMultipartPartInputRequestTypeDef,
     InputSerializationTypeDef,
     OutputSerializationTypeDef,
     DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
@@ -492,31 +493,33 @@
     ListPartsInputListPartsPaginateTypeDef,
     ListVaultsInputListVaultsPaginateTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
     SetVaultNotificationsInputNotificationSetTypeDef,
     SetVaultNotificationsInputRequestTypeDef,
+    VaultNotificationConfigUnionTypeDef,
     SelectParametersResponseTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
+    DataRetrievalPolicyUnionTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
     S3LocationOutputTypeDef,
     S3LocationTypeDef,
     OutputLocationOutputTypeDef,
     OutputLocationTypeDef,
     GlacierJobDescriptionResponseTypeDef,
     GlacierJobDescriptionTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     InitiateJobInputRequestTypeDef,
 )
 
 
-def get_structure() -> AbortMultipartUploadInputRequestTypeDef:
+def get_value() -> AbortMultipartUploadInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__init__.py` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__init__.pyi` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__main__.py` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glacier 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Glacier 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier\nOther"
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

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/client.py` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,29 @@
     from mypy_boto3_glacier.client import GlacierClient
 
     session = Session()
     client: GlacierClient = session.client("glacier")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     ListJobsPaginator,
     ListMultipartUploadsPaginator,
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
+    BlobTypeDef,
     CreateVaultOutputTypeDef,
-    DataRetrievalPolicyOutputTypeDef,
-    DataRetrievalPolicyTypeDef,
+    DataRetrievalPolicyUnionTypeDef,
     DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsOutputTypeDef,
@@ -48,16 +47,15 @@
     ListProvisionedCapacityOutputTypeDef,
     ListTagsForVaultOutputTypeDef,
     ListVaultsOutputTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
     VaultAccessPolicyTypeDef,
     VaultLockPolicyTypeDef,
-    VaultNotificationConfigOutputTypeDef,
-    VaultNotificationConfigTypeDef,
+    VaultNotificationConfigUnionTypeDef,
 )
 from .waiter import VaultExistsWaiter, VaultNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -451,18 +449,15 @@
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.remove_tags_from_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#remove_tags_from_vault)
         """
 
     def set_data_retrieval_policy(
-        self,
-        *,
-        accountId: str = "-",
-        Policy: Union[DataRetrievalPolicyTypeDef, DataRetrievalPolicyOutputTypeDef] = ...
+        self, *, accountId: str = "-", Policy: DataRetrievalPolicyUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation sets and then enacts a data retrieval policy in the region
         specified in the PUT request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_data_retrieval_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_data_retrieval_policy)
@@ -480,17 +475,15 @@
         """
 
     def set_vault_notifications(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
-        vaultNotificationConfig: Union[
-            VaultNotificationConfigTypeDef, VaultNotificationConfigOutputTypeDef
-        ] = ...
+        vaultNotificationConfig: VaultNotificationConfigUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation configures notifications that will be sent when specific events
         happen to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_vault_notifications)
@@ -499,15 +492,15 @@
     def upload_archive(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
         archiveDescription: str = ...,
         checksum: str = ...,
-        body: Union[str, bytes, IO[Any], StreamingBody] = ...
+        body: BlobTypeDef = ...
     ) -> ArchiveCreationOutputTypeDef:
         """
         This operation adds an archive to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_archive)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#upload_archive)
         """
@@ -516,15 +509,15 @@
         self,
         *,
         vaultName: str,
         uploadId: str,
         accountId: str = "-",
         checksum: str = ...,
         range: str = ...,
-        body: Union[str, bytes, IO[Any], StreamingBody] = ...
+        body: BlobTypeDef = ...
     ) -> UploadMultipartPartOutputTypeDef:
         """
         This operation uploads a part of an archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_multipart_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#upload_multipart_part)
         """
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/client.pyi` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,29 @@
     from mypy_boto3_glacier.client import GlacierClient
 
     session = Session()
     client: GlacierClient = session.client("glacier")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     ListJobsPaginator,
     ListMultipartUploadsPaginator,
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
+    BlobTypeDef,
     CreateVaultOutputTypeDef,
-    DataRetrievalPolicyOutputTypeDef,
-    DataRetrievalPolicyTypeDef,
+    DataRetrievalPolicyUnionTypeDef,
     DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsOutputTypeDef,
@@ -48,16 +47,15 @@
     ListProvisionedCapacityOutputTypeDef,
     ListTagsForVaultOutputTypeDef,
     ListVaultsOutputTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
     VaultAccessPolicyTypeDef,
     VaultLockPolicyTypeDef,
-    VaultNotificationConfigOutputTypeDef,
-    VaultNotificationConfigTypeDef,
+    VaultNotificationConfigUnionTypeDef,
 )
 from .waiter import VaultExistsWaiter, VaultNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -415,18 +413,15 @@
         This operation removes one or more tags from the set of tags attached to a
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.remove_tags_from_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#remove_tags_from_vault)
         """
     def set_data_retrieval_policy(
-        self,
-        *,
-        accountId: str = "-",
-        Policy: Union[DataRetrievalPolicyTypeDef, DataRetrievalPolicyOutputTypeDef] = ...
+        self, *, accountId: str = "-", Policy: DataRetrievalPolicyUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation sets and then enacts a data retrieval policy in the region
         specified in the PUT request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_data_retrieval_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_data_retrieval_policy)
@@ -442,17 +437,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_vault_access_policy)
         """
     def set_vault_notifications(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
-        vaultNotificationConfig: Union[
-            VaultNotificationConfigTypeDef, VaultNotificationConfigOutputTypeDef
-        ] = ...
+        vaultNotificationConfig: VaultNotificationConfigUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation configures notifications that will be sent when specific events
         happen to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_vault_notifications)
@@ -460,15 +453,15 @@
     def upload_archive(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
         archiveDescription: str = ...,
         checksum: str = ...,
-        body: Union[str, bytes, IO[Any], StreamingBody] = ...
+        body: BlobTypeDef = ...
     ) -> ArchiveCreationOutputTypeDef:
         """
         This operation adds an archive to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_archive)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#upload_archive)
         """
@@ -476,15 +469,15 @@
         self,
         *,
         vaultName: str,
         uploadId: str,
         accountId: str = "-",
         checksum: str = ...,
         range: str = ...,
-        body: Union[str, bytes, IO[Any], StreamingBody] = ...
+        body: BlobTypeDef = ...
     ) -> UploadMultipartPartOutputTypeDef:
         """
         This operation uploads a part of an archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_multipart_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#upload_multipart_part)
         """
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/literals.py` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/literals.pyi` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/paginator.py` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/paginator.pyi` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/service_resource.py` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     my_archive: glacier_resources.Archive = resource.Archive(...)
     my_job: glacier_resources.Job = resource.Job(...)
     my_multipart_upload: glacier_resources.MultipartUpload = resource.MultipartUpload(...)
     my_notification: glacier_resources.Notification = resource.Notification(...)
     my_vault: glacier_resources.Vault = resource.Vault(...)
 ```
 """
-from typing import IO, Any, Iterator, List, Sequence, Union
+from typing import Iterator, List, Sequence
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
-from botocore.response import StreamingBody
 
 from .client import GlacierClient
 from .literals import ActionCodeType, StatusCodeType
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
+    BlobTypeDef,
     CreateVaultOutputTypeDef,
     GetJobOutputOutputTypeDef,
     InventoryRetrievalJobDescriptionResponseTypeDef,
     ListPartsOutputTypeDef,
     OutputLocationTypeDef,
     SelectParametersResponseTypeDef,
     UploadMultipartPartOutputTypeDef,
@@ -525,19 +525,15 @@
         specific multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.MultipartUpload.parts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/service_resource/#multipartuploadparts-method)
         """
 
     def upload_part(
-        self,
-        *,
-        checksum: str = ...,
-        range: str = ...,
-        body: Union[str, bytes, IO[Any], StreamingBody] = ...
+        self, *, checksum: str = ..., range: str = ..., body: BlobTypeDef = ...
     ) -> UploadMultipartPartOutputTypeDef:
         """
         This operation uploads a part of an archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.MultipartUpload.upload_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/service_resource/#multipartuploadupload_part-method)
         """
@@ -816,19 +812,15 @@
         Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/service_resource/#vaultreload-method)
         """
 
     def upload_archive(
-        self,
-        *,
-        archiveDescription: str = ...,
-        checksum: str = ...,
-        body: Union[str, bytes, IO[Any], StreamingBody] = ...
+        self, *, archiveDescription: str = ..., checksum: str = ..., body: BlobTypeDef = ...
     ) -> _Archive:
         """
         This operation adds an archive to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.upload_archive)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/service_resource/#vaultupload_archive-method)
         """
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/service_resource.pyi` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     my_archive: glacier_resources.Archive = resource.Archive(...)
     my_job: glacier_resources.Job = resource.Job(...)
     my_multipart_upload: glacier_resources.MultipartUpload = resource.MultipartUpload(...)
     my_notification: glacier_resources.Notification = resource.Notification(...)
     my_vault: glacier_resources.Vault = resource.Vault(...)
 ```
 """
-from typing import IO, Any, Iterator, List, Sequence, Union
+from typing import Iterator, List, Sequence
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
-from botocore.response import StreamingBody
 
 from .client import GlacierClient
 from .literals import ActionCodeType, StatusCodeType
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
+    BlobTypeDef,
     CreateVaultOutputTypeDef,
     GetJobOutputOutputTypeDef,
     InventoryRetrievalJobDescriptionResponseTypeDef,
     ListPartsOutputTypeDef,
     OutputLocationTypeDef,
     SelectParametersResponseTypeDef,
     UploadMultipartPartOutputTypeDef,
@@ -492,19 +492,15 @@
         This operation lists the parts of an archive that have been uploaded in a
         specific multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.MultipartUpload.parts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/service_resource/#multipartuploadparts-method)
         """
     def upload_part(
-        self,
-        *,
-        checksum: str = ...,
-        range: str = ...,
-        body: Union[str, bytes, IO[Any], StreamingBody] = ...
+        self, *, checksum: str = ..., range: str = ..., body: BlobTypeDef = ...
     ) -> UploadMultipartPartOutputTypeDef:
         """
         This operation uploads a part of an archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.MultipartUpload.upload_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/service_resource/#multipartuploadupload_part-method)
         """
@@ -720,19 +716,15 @@
         Calls :py:meth:`Glacier.Client.describe_vault` to update the attributes of the
         Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/service_resource/#vaultreload-method)
         """
     def upload_archive(
-        self,
-        *,
-        archiveDescription: str = ...,
-        checksum: str = ...,
-        body: Union[str, bytes, IO[Any], StreamingBody] = ...
+        self, *, archiveDescription: str = ..., checksum: str = ..., body: BlobTypeDef = ...
     ) -> _Archive:
         """
         This operation adds an archive to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.upload_archive)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/service_resource/#vaultupload_archive-method)
         """
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/type_defs.py` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_glacier.type_defs import AbortMultipartUploadInputRequestTypeDef
 
-    data: AbortMultipartUploadInputRequestTypeDef = {...}
+    data: AbortMultipartUploadInputRequestTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -39,14 +39,15 @@
 
 
 __all__ = (
     "AbortMultipartUploadInputRequestTypeDef",
     "AbortVaultLockInputRequestTypeDef",
     "AddTagsToVaultInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "CompleteMultipartUploadInputMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadInputRequestTypeDef",
     "CompleteVaultLockInputRequestTypeDef",
     "CreateVaultInputAccountCreateVaultTypeDef",
     "CreateVaultInputRequestTypeDef",
@@ -85,31 +86,31 @@
     "ListProvisionedCapacityInputRequestTypeDef",
     "ProvisionedCapacityDescriptionTypeDef",
     "ListTagsForVaultInputRequestTypeDef",
     "ListVaultsInputRequestTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
     "VaultNotificationConfigTypeDef",
-    "UploadArchiveInputRequestTypeDef",
-    "UploadArchiveInputVaultUploadArchiveTypeDef",
-    "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
-    "UploadMultipartPartInputRequestTypeDef",
     "ArchiveCreationOutputTypeDef",
     "CreateVaultOutputTypeDef",
     "DescribeVaultResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetJobOutputOutputTypeDef",
     "GetVaultLockOutputTypeDef",
     "InitiateJobOutputTypeDef",
     "InitiateMultipartUploadOutputTypeDef",
     "InitiateVaultLockOutputTypeDef",
     "InventoryRetrievalJobDescriptionResponseTypeDef",
     "ListTagsForVaultOutputTypeDef",
     "PurchaseProvisionedCapacityOutputTypeDef",
     "UploadMultipartPartOutputTypeDef",
+    "UploadArchiveInputRequestTypeDef",
+    "UploadArchiveInputVaultUploadArchiveTypeDef",
+    "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
+    "UploadMultipartPartInputRequestTypeDef",
     "InputSerializationTypeDef",
     "OutputSerializationTypeDef",
     "DataRetrievalPolicyOutputTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
@@ -123,17 +124,19 @@
     "ListPartsInputListPartsPaginateTypeDef",
     "ListVaultsInputListVaultsPaginateTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
     "SetVaultNotificationsInputNotificationSetTypeDef",
     "SetVaultNotificationsInputRequestTypeDef",
+    "VaultNotificationConfigUnionTypeDef",
     "SelectParametersResponseTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
+    "DataRetrievalPolicyUnionTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
     "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "OutputLocationOutputTypeDef",
     "OutputLocationTypeDef",
     "GlacierJobDescriptionResponseTypeDef",
     "GlacierJobDescriptionTypeDef",
@@ -215,14 +218,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
         "Comments": str,
         "QuoteEscapeCharacter": str,
         "RecordDelimiter": str,
@@ -925,83 +929,14 @@
     {
         "SNSTopic": str,
         "Events": Sequence[str],
     },
     total=False,
 )
 
-_RequiredUploadArchiveInputRequestTypeDef = TypedDict(
-    "_RequiredUploadArchiveInputRequestTypeDef",
-    {
-        "vaultName": str,
-    },
-)
-_OptionalUploadArchiveInputRequestTypeDef = TypedDict(
-    "_OptionalUploadArchiveInputRequestTypeDef",
-    {
-        "accountId": str,
-        "archiveDescription": str,
-        "checksum": str,
-        "body": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class UploadArchiveInputRequestTypeDef(
-    _RequiredUploadArchiveInputRequestTypeDef, _OptionalUploadArchiveInputRequestTypeDef
-):
-    pass
-
-
-UploadArchiveInputVaultUploadArchiveTypeDef = TypedDict(
-    "UploadArchiveInputVaultUploadArchiveTypeDef",
-    {
-        "archiveDescription": str,
-        "checksum": str,
-        "body": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-UploadMultipartPartInputMultipartUploadUploadPartTypeDef = TypedDict(
-    "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
-    {
-        "checksum": str,
-        "range": str,
-        "body": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-_RequiredUploadMultipartPartInputRequestTypeDef = TypedDict(
-    "_RequiredUploadMultipartPartInputRequestTypeDef",
-    {
-        "vaultName": str,
-        "uploadId": str,
-    },
-)
-_OptionalUploadMultipartPartInputRequestTypeDef = TypedDict(
-    "_OptionalUploadMultipartPartInputRequestTypeDef",
-    {
-        "accountId": str,
-        "checksum": str,
-        "range": str,
-        "body": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class UploadMultipartPartInputRequestTypeDef(
-    _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
-):
-    pass
-
-
 ArchiveCreationOutputTypeDef = TypedDict(
     "ArchiveCreationOutputTypeDef",
     {
         "location": str,
         "checksum": str,
         "archiveId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1120,14 +1055,83 @@
     "UploadMultipartPartOutputTypeDef",
     {
         "checksum": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUploadArchiveInputRequestTypeDef = TypedDict(
+    "_RequiredUploadArchiveInputRequestTypeDef",
+    {
+        "vaultName": str,
+    },
+)
+_OptionalUploadArchiveInputRequestTypeDef = TypedDict(
+    "_OptionalUploadArchiveInputRequestTypeDef",
+    {
+        "accountId": str,
+        "archiveDescription": str,
+        "checksum": str,
+        "body": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class UploadArchiveInputRequestTypeDef(
+    _RequiredUploadArchiveInputRequestTypeDef, _OptionalUploadArchiveInputRequestTypeDef
+):
+    pass
+
+
+UploadArchiveInputVaultUploadArchiveTypeDef = TypedDict(
+    "UploadArchiveInputVaultUploadArchiveTypeDef",
+    {
+        "archiveDescription": str,
+        "checksum": str,
+        "body": BlobTypeDef,
+    },
+    total=False,
+)
+
+UploadMultipartPartInputMultipartUploadUploadPartTypeDef = TypedDict(
+    "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
+    {
+        "checksum": str,
+        "range": str,
+        "body": BlobTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUploadMultipartPartInputRequestTypeDef = TypedDict(
+    "_RequiredUploadMultipartPartInputRequestTypeDef",
+    {
+        "vaultName": str,
+        "uploadId": str,
+    },
+)
+_OptionalUploadMultipartPartInputRequestTypeDef = TypedDict(
+    "_OptionalUploadMultipartPartInputRequestTypeDef",
+    {
+        "accountId": str,
+        "checksum": str,
+        "range": str,
+        "body": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class UploadMultipartPartInputRequestTypeDef(
+    _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
+):
+    pass
+
+
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "csv": CSVInputTypeDef,
     },
     total=False,
 )
@@ -1431,14 +1435,17 @@
 class SetVaultNotificationsInputRequestTypeDef(
     _RequiredSetVaultNotificationsInputRequestTypeDef,
     _OptionalSetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
 
+VaultNotificationConfigUnionTypeDef = Union[
+    VaultNotificationConfigTypeDef, VaultNotificationConfigOutputTypeDef
+]
 SelectParametersResponseTypeDef = TypedDict(
     "SelectParametersResponseTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
@@ -1461,14 +1468,17 @@
     "GetDataRetrievalPolicyOutputTypeDef",
     {
         "Policy": DataRetrievalPolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataRetrievalPolicyUnionTypeDef = Union[
+    DataRetrievalPolicyTypeDef, DataRetrievalPolicyOutputTypeDef
+]
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
         "Policy": DataRetrievalPolicyTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/type_defs.pyi` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_glacier.type_defs import AbortMultipartUploadInputRequestTypeDef
 
-    data: AbortMultipartUploadInputRequestTypeDef = {...}
+    data: AbortMultipartUploadInputRequestTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -38,14 +38,15 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortMultipartUploadInputRequestTypeDef",
     "AbortVaultLockInputRequestTypeDef",
     "AddTagsToVaultInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "CompleteMultipartUploadInputMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadInputRequestTypeDef",
     "CompleteVaultLockInputRequestTypeDef",
     "CreateVaultInputAccountCreateVaultTypeDef",
     "CreateVaultInputRequestTypeDef",
@@ -84,31 +85,31 @@
     "ListProvisionedCapacityInputRequestTypeDef",
     "ProvisionedCapacityDescriptionTypeDef",
     "ListTagsForVaultInputRequestTypeDef",
     "ListVaultsInputRequestTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
     "VaultNotificationConfigTypeDef",
-    "UploadArchiveInputRequestTypeDef",
-    "UploadArchiveInputVaultUploadArchiveTypeDef",
-    "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
-    "UploadMultipartPartInputRequestTypeDef",
     "ArchiveCreationOutputTypeDef",
     "CreateVaultOutputTypeDef",
     "DescribeVaultResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetJobOutputOutputTypeDef",
     "GetVaultLockOutputTypeDef",
     "InitiateJobOutputTypeDef",
     "InitiateMultipartUploadOutputTypeDef",
     "InitiateVaultLockOutputTypeDef",
     "InventoryRetrievalJobDescriptionResponseTypeDef",
     "ListTagsForVaultOutputTypeDef",
     "PurchaseProvisionedCapacityOutputTypeDef",
     "UploadMultipartPartOutputTypeDef",
+    "UploadArchiveInputRequestTypeDef",
+    "UploadArchiveInputVaultUploadArchiveTypeDef",
+    "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
+    "UploadMultipartPartInputRequestTypeDef",
     "InputSerializationTypeDef",
     "OutputSerializationTypeDef",
     "DataRetrievalPolicyOutputTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
@@ -122,17 +123,19 @@
     "ListPartsInputListPartsPaginateTypeDef",
     "ListVaultsInputListVaultsPaginateTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
     "SetVaultNotificationsInputNotificationSetTypeDef",
     "SetVaultNotificationsInputRequestTypeDef",
+    "VaultNotificationConfigUnionTypeDef",
     "SelectParametersResponseTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
+    "DataRetrievalPolicyUnionTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
     "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "OutputLocationOutputTypeDef",
     "OutputLocationTypeDef",
     "GlacierJobDescriptionResponseTypeDef",
     "GlacierJobDescriptionTypeDef",
@@ -208,14 +211,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
         "Comments": str,
         "QuoteEscapeCharacter": str,
         "RecordDelimiter": str,
@@ -876,79 +880,14 @@
     {
         "SNSTopic": str,
         "Events": Sequence[str],
     },
     total=False,
 )
 
-_RequiredUploadArchiveInputRequestTypeDef = TypedDict(
-    "_RequiredUploadArchiveInputRequestTypeDef",
-    {
-        "vaultName": str,
-    },
-)
-_OptionalUploadArchiveInputRequestTypeDef = TypedDict(
-    "_OptionalUploadArchiveInputRequestTypeDef",
-    {
-        "accountId": str,
-        "archiveDescription": str,
-        "checksum": str,
-        "body": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class UploadArchiveInputRequestTypeDef(
-    _RequiredUploadArchiveInputRequestTypeDef, _OptionalUploadArchiveInputRequestTypeDef
-):
-    pass
-
-UploadArchiveInputVaultUploadArchiveTypeDef = TypedDict(
-    "UploadArchiveInputVaultUploadArchiveTypeDef",
-    {
-        "archiveDescription": str,
-        "checksum": str,
-        "body": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-UploadMultipartPartInputMultipartUploadUploadPartTypeDef = TypedDict(
-    "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
-    {
-        "checksum": str,
-        "range": str,
-        "body": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-_RequiredUploadMultipartPartInputRequestTypeDef = TypedDict(
-    "_RequiredUploadMultipartPartInputRequestTypeDef",
-    {
-        "vaultName": str,
-        "uploadId": str,
-    },
-)
-_OptionalUploadMultipartPartInputRequestTypeDef = TypedDict(
-    "_OptionalUploadMultipartPartInputRequestTypeDef",
-    {
-        "accountId": str,
-        "checksum": str,
-        "range": str,
-        "body": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class UploadMultipartPartInputRequestTypeDef(
-    _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
-):
-    pass
-
 ArchiveCreationOutputTypeDef = TypedDict(
     "ArchiveCreationOutputTypeDef",
     {
         "location": str,
         "checksum": str,
         "archiveId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1067,14 +1006,79 @@
     "UploadMultipartPartOutputTypeDef",
     {
         "checksum": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUploadArchiveInputRequestTypeDef = TypedDict(
+    "_RequiredUploadArchiveInputRequestTypeDef",
+    {
+        "vaultName": str,
+    },
+)
+_OptionalUploadArchiveInputRequestTypeDef = TypedDict(
+    "_OptionalUploadArchiveInputRequestTypeDef",
+    {
+        "accountId": str,
+        "archiveDescription": str,
+        "checksum": str,
+        "body": BlobTypeDef,
+    },
+    total=False,
+)
+
+class UploadArchiveInputRequestTypeDef(
+    _RequiredUploadArchiveInputRequestTypeDef, _OptionalUploadArchiveInputRequestTypeDef
+):
+    pass
+
+UploadArchiveInputVaultUploadArchiveTypeDef = TypedDict(
+    "UploadArchiveInputVaultUploadArchiveTypeDef",
+    {
+        "archiveDescription": str,
+        "checksum": str,
+        "body": BlobTypeDef,
+    },
+    total=False,
+)
+
+UploadMultipartPartInputMultipartUploadUploadPartTypeDef = TypedDict(
+    "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
+    {
+        "checksum": str,
+        "range": str,
+        "body": BlobTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUploadMultipartPartInputRequestTypeDef = TypedDict(
+    "_RequiredUploadMultipartPartInputRequestTypeDef",
+    {
+        "vaultName": str,
+        "uploadId": str,
+    },
+)
+_OptionalUploadMultipartPartInputRequestTypeDef = TypedDict(
+    "_OptionalUploadMultipartPartInputRequestTypeDef",
+    {
+        "accountId": str,
+        "checksum": str,
+        "range": str,
+        "body": BlobTypeDef,
+    },
+    total=False,
+)
+
+class UploadMultipartPartInputRequestTypeDef(
+    _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
+):
+    pass
+
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "csv": CSVInputTypeDef,
     },
     total=False,
 )
@@ -1360,14 +1364,17 @@
 
 class SetVaultNotificationsInputRequestTypeDef(
     _RequiredSetVaultNotificationsInputRequestTypeDef,
     _OptionalSetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
+VaultNotificationConfigUnionTypeDef = Union[
+    VaultNotificationConfigTypeDef, VaultNotificationConfigOutputTypeDef
+]
 SelectParametersResponseTypeDef = TypedDict(
     "SelectParametersResponseTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
@@ -1390,14 +1397,17 @@
     "GetDataRetrievalPolicyOutputTypeDef",
     {
         "Policy": DataRetrievalPolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataRetrievalPolicyUnionTypeDef = Union[
+    DataRetrievalPolicyTypeDef, DataRetrievalPolicyOutputTypeDef
+]
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
         "Policy": DataRetrievalPolicyTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/waiter.py` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/waiter.pyi` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/PKG-INFO` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glacier
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Glacier 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 glacier type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 glacier type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glacier)](https://pepy.tech/project/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +78,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -427,27 +427,28 @@
 )
 
 
 def check_value(value: ActionCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_glacier.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
@@ -486,31 +487,31 @@
     ListProvisionedCapacityInputRequestTypeDef,
     ProvisionedCapacityDescriptionTypeDef,
     ListTagsForVaultInputRequestTypeDef,
     ListVaultsInputRequestTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
     VaultNotificationConfigTypeDef,
-    UploadArchiveInputRequestTypeDef,
-    UploadArchiveInputVaultUploadArchiveTypeDef,
-    UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
-    UploadMultipartPartInputRequestTypeDef,
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
     DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultLockOutputTypeDef,
     InitiateJobOutputTypeDef,
     InitiateMultipartUploadOutputTypeDef,
     InitiateVaultLockOutputTypeDef,
     InventoryRetrievalJobDescriptionResponseTypeDef,
     ListTagsForVaultOutputTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
+    UploadArchiveInputRequestTypeDef,
+    UploadArchiveInputVaultUploadArchiveTypeDef,
+    UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
+    UploadMultipartPartInputRequestTypeDef,
     InputSerializationTypeDef,
     OutputSerializationTypeDef,
     DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
@@ -524,31 +525,33 @@
     ListPartsInputListPartsPaginateTypeDef,
     ListVaultsInputListVaultsPaginateTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
     SetVaultNotificationsInputNotificationSetTypeDef,
     SetVaultNotificationsInputRequestTypeDef,
+    VaultNotificationConfigUnionTypeDef,
     SelectParametersResponseTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
+    DataRetrievalPolicyUnionTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
     S3LocationOutputTypeDef,
     S3LocationTypeDef,
     OutputLocationOutputTypeDef,
     OutputLocationTypeDef,
     GlacierJobDescriptionResponseTypeDef,
     GlacierJobDescriptionTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     InitiateJobInputRequestTypeDef,
 )
 
 
-def get_structure() -> AbortMultipartUploadInputRequestTypeDef:
+def get_value() -> AbortMultipartUploadInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/SOURCES.txt` & `mypy-boto3-glacier-1.28.16/mypy_boto3_glacier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15.post1/setup.py` & `mypy-boto3-glacier-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glacier",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_glacier"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Glacier 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 glacier type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 glacier type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_glacier": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

