# Comparing `tmp/mypy-boto3-storagegateway-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-storagegateway-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-storagegateway-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:19 2023, max compression
+gzip compressed data, was "mypy-boto3-storagegateway-1.28.16.tar", last modified: Tue Aug  1 11:37:58 2023, max compression
```

## Comparing `mypy-boto3-storagegateway-1.28.15.post1.tar` & `mypy-boto3-storagegateway-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.085431 mypy-boto3-storagegateway-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-29 10:04:19.081431 mypy-boto3-storagegateway-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.077431 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68554 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68446 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-29 10:00:32.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-29 10:00:32.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    77993 2023-07-29 10:00:34.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77914 2023-07-29 10:00:33.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.081431 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:19.085431 mypy-boto3-storagegateway-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:58.408712 mypy-boto3-storagegateway-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:06.000000 mypy-boto3-storagegateway-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24255 2023-08-01 11:37:58.404712 mypy-boto3-storagegateway-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22743 2023-08-01 11:34:06.000000 mypy-boto3-storagegateway-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:58.404712 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-08-01 11:34:06.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-01 11:34:06.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:34:07.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68250 2023-08-01 11:34:07.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68142 2023-08-01 11:34:07.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-08-01 11:34:07.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-08-01 11:34:07.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-08-01 11:34:07.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-08-01 11:34:07.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:07.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    78405 2023-08-01 11:34:10.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78326 2023-08-01 11:34:09.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:06.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:58.404712 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24255 2023-08-01 11:37:58.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:37:58.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:58.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:58.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:58.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:37:58.000000 mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:58.408712 mypy-boto3-storagegateway-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:34:06.000000 mypy-boto3-storagegateway-1.28.16/setup.py
```

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/LICENSE` & `mypy-boto3-storagegateway-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/PKG-INFO` & `mypy-boto3-storagegateway-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.StorageGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.StorageGateway 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 storagegateway type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 storagegateway type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
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
@@ -364,20 +364,20 @@
 )
 
 
 def check_value(value: ActiveDirectoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_storagegateway.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_storagegateway.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
     AddCacheInputRequestTypeDef,
     AddUploadBufferInputRequestTypeDef,
@@ -558,15 +558,15 @@
     SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
     NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
@@ -583,34 +583,37 @@
     ListTapesInputListTapesPaginateTypeDef,
     ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
+    SMBLocalGroupsUnionTypeDef,
     UpdateSMBLocalGroupsInputRequestTypeDef,
     DescribeSMBFileSharesOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
     DescribeNFSFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/README.md` & `mypy-boto3-storagegateway-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
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
@@ -332,20 +332,20 @@
 )
 
 
 def check_value(value: ActiveDirectoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_storagegateway.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_storagegateway.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
     AddCacheInputRequestTypeDef,
     AddUploadBufferInputRequestTypeDef,
@@ -526,15 +526,15 @@
     SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
     NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
@@ -551,34 +551,37 @@
     ListTapesInputListTapesPaginateTypeDef,
     ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
+    SMBLocalGroupsUnionTypeDef,
     UpdateSMBLocalGroupsInputRequestTypeDef,
     DescribeSMBFileSharesOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
     DescribeNFSFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__init__.py` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__init__.pyi` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__main__.py` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.StorageGateway 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.StorageGateway 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway\nOther"
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

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/client.py` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_storagegateway.client import StorageGatewayClient
 
     session = Session()
     client: StorageGatewayClient = session.client("storagegateway")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CaseSensitivityType,
     GatewayCapacityType,
     ObjectACLType,
@@ -45,16 +45,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
-    BandwidthRateLimitIntervalOutputTypeDef,
-    BandwidthRateLimitIntervalTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
     CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
@@ -92,16 +91,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
-    EndpointNetworkConfigurationOutputTypeDef,
-    EndpointNetworkConfigurationTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -116,16 +114,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
-    SMBLocalGroupsOutputTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsUnionTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsOutputTypeDef,
@@ -258,17 +255,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: Union[
-            EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
-        ] = ...
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationUnionTypeDef = ...
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#associate_file_system)
         """
@@ -1112,17 +1107,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit)
         """
 
     def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[
-            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
-        ]
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef]
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1266,18 +1259,15 @@
         browse list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_file_share_visibility)
         """
 
     def update_smb_local_groups(
-        self,
-        *,
-        GatewayARN: str,
-        SMBLocalGroups: Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
+        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsUnionTypeDef
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_local_groups)
```

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/client.pyi` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_storagegateway.client import StorageGatewayClient
 
     session = Session()
     client: StorageGatewayClient = session.client("storagegateway")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CaseSensitivityType,
     GatewayCapacityType,
     ObjectACLType,
@@ -45,16 +45,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
-    BandwidthRateLimitIntervalOutputTypeDef,
-    BandwidthRateLimitIntervalTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
     CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
@@ -92,16 +91,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
-    EndpointNetworkConfigurationOutputTypeDef,
-    EndpointNetworkConfigurationTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -116,16 +114,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
-    SMBLocalGroupsOutputTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsUnionTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsOutputTypeDef,
@@ -247,17 +244,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: Union[
-            EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
-        ] = ...
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationUnionTypeDef = ...
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#associate_file_system)
         """
@@ -1027,17 +1022,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit)
         """
     def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[
-            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
-        ]
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef]
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1172,18 +1165,15 @@
         Controls whether the shares on an S3 File Gateway are visible in a net view or
         browse list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_file_share_visibility)
         """
     def update_smb_local_groups(
-        self,
-        *,
-        GatewayARN: str,
-        SMBLocalGroups: Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
+        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsUnionTypeDef
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_local_groups)
```

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/literals.py` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/literals.pyi` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/paginator.py` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/paginator.pyi` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/type_defs.py` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_storagegateway.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -217,15 +217,15 @@
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    "BandwidthRateLimitIntervalUnionTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
@@ -242,25 +242,28 @@
     "ListTapesInputListTapesPaginateTypeDef",
     "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
+    "EndpointNetworkConfigurationUnionTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
+    "SMBLocalGroupsUnionTypeDef",
     "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
     "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
 )
 
@@ -2458,24 +2461,17 @@
     {
         "GatewayARN": str,
         "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[
-            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
-        ],
-    },
-)
-
+BandwidthRateLimitIntervalUnionTypeDef = Union[
+    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
+]
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": str,
         "VolumeId": str,
         "VolumeType": str,
         "VolumeStatus": str,
@@ -2866,14 +2862,17 @@
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EndpointNetworkConfigurationUnionTypeDef = Union[
+    EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
+]
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2948,14 +2947,15 @@
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SMBLocalGroupsUnionTypeDef = Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
 UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
     "UpdateSMBLocalGroupsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
@@ -2972,14 +2972,22 @@
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+    },
+)
+
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/type_defs.pyi` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_storagegateway.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -216,15 +216,15 @@
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    "BandwidthRateLimitIntervalUnionTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
@@ -241,25 +241,28 @@
     "ListTapesInputListTapesPaginateTypeDef",
     "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
+    "EndpointNetworkConfigurationUnionTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
+    "SMBLocalGroupsUnionTypeDef",
     "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
     "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
 )
 
@@ -2391,24 +2394,17 @@
     {
         "GatewayARN": str,
         "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[
-            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
-        ],
-    },
-)
-
+BandwidthRateLimitIntervalUnionTypeDef = Union[
+    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
+]
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": str,
         "VolumeId": str,
         "VolumeType": str,
         "VolumeStatus": str,
@@ -2787,14 +2783,17 @@
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EndpointNetworkConfigurationUnionTypeDef = Union[
+    EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
+]
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2869,14 +2868,15 @@
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SMBLocalGroupsUnionTypeDef = Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
 UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
     "UpdateSMBLocalGroupsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
@@ -2893,14 +2893,22 @@
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+    },
+)
+
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/PKG-INFO` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.StorageGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.StorageGateway 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 storagegateway type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 storagegateway type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
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
@@ -364,20 +364,20 @@
 )
 
 
 def check_value(value: ActiveDirectoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_storagegateway.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_storagegateway.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
     AddCacheInputRequestTypeDef,
     AddUploadBufferInputRequestTypeDef,
@@ -558,15 +558,15 @@
     SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
     NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
@@ -583,34 +583,37 @@
     ListTapesInputListTapesPaginateTypeDef,
     ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
+    SMBLocalGroupsUnionTypeDef,
     UpdateSMBLocalGroupsInputRequestTypeDef,
     DescribeSMBFileSharesOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
     DescribeNFSFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/SOURCES.txt` & `mypy-boto3-storagegateway-1.28.16/mypy_boto3_storagegateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15.post1/setup.py` & `mypy-boto3-storagegateway-1.28.16/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-storagegateway",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_storagegateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.StorageGateway 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.StorageGateway 1.28.16 service generated with"
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
-    keywords="boto3 storagegateway type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 storagegateway type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_storagegateway": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

