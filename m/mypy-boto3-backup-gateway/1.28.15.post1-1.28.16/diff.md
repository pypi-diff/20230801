# Comparing `tmp/mypy-boto3-backup-gateway-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-backup-gateway-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-gateway-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
+gzip compressed data, was "mypy-boto3-backup-gateway-1.28.16.tar", last modified: Tue Aug  1 11:36:15 2023, max compression
```

## Comparing `mypy-boto3-backup-gateway-1.28.15.post1.tar` & `mypy-boto3-backup-gateway-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.749022 mypy-boto3-backup-gateway-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-07-29 10:02:34.745022 mypy-boto3-backup-gateway-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.745022 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20095 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-29 09:38:59.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-29 09:38:59.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20415 2023-07-29 09:38:59.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.745022 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.749022 mypy-boto3-backup-gateway-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.380945 mypy-boto3-backup-gateway-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-08-01 11:36:15.380945 mypy-boto3-backup-gateway-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.380945 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-08-01 11:11:32.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-08-01 11:11:32.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-08-01 11:11:32.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-08-01 11:11:32.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.380945 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-08-01 11:36:15.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:36:15.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:15.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:36:15.000000 mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:15.380945 mypy-boto3-backup-gateway-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-01 11:11:31.000000 mypy-boto3-backup-gateway-1.28.16/setup.py
```

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/LICENSE` & `mypy-boto3-backup-gateway-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/PKG-INFO` & `mypy-boto3-backup-gateway-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup-gateway
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.BackupGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.BackupGateway 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 backup-gateway type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 backup-gateway type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup-gateway)](https://pepy.tech/project/mypy-boto3-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupGateway 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[boto3.BackupGateway 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [mypy-boto3-backup-gateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/).
 
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
@@ -324,20 +324,20 @@
 )
 
 
 def check_value(value: GatewayTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_backup_gateway.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_backup_gateway.type_defs import (
     AssociateGatewayToServerInputRequestTypeDef,
     ResponseMetadataTypeDef,
     BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
@@ -381,15 +381,15 @@
     StartVirtualMachinesMetadataSyncOutputTypeDef,
     TagResourceOutputTypeDef,
     UntagResourceOutputTypeDef,
     UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateHypervisorOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
-    PutBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayInputRequestTypeDef,
     ImportHypervisorConfigurationInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     GatewayDetailsTypeDef,
     ListGatewaysOutputTypeDef,
     GetHypervisorOutputTypeDef,
@@ -397,20 +397,21 @@
     PutHypervisorPropertyMappingsInputRequestTypeDef,
     ListHypervisorsOutputTypeDef,
     ListGatewaysInputListGatewaysPaginateTypeDef,
     ListHypervisorsInputListHypervisorsPaginateTypeDef,
     ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesOutputTypeDef,
     VirtualMachineDetailsTypeDef,
+    PutBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayOutputTypeDef,
     GetVirtualMachineOutputTypeDef,
 )
 
 
-def get_structure() -> AssociateGatewayToServerInputRequestTypeDef:
+def get_value() -> AssociateGatewayToServerInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/README.md` & `mypy-boto3-backup-gateway-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup-gateway)](https://pepy.tech/project/mypy-boto3-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupGateway 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[boto3.BackupGateway 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [mypy-boto3-backup-gateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/).
 
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
@@ -292,20 +292,20 @@
 )
 
 
 def check_value(value: GatewayTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_backup_gateway.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_backup_gateway.type_defs import (
     AssociateGatewayToServerInputRequestTypeDef,
     ResponseMetadataTypeDef,
     BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
@@ -349,15 +349,15 @@
     StartVirtualMachinesMetadataSyncOutputTypeDef,
     TagResourceOutputTypeDef,
     UntagResourceOutputTypeDef,
     UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateHypervisorOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
-    PutBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayInputRequestTypeDef,
     ImportHypervisorConfigurationInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     GatewayDetailsTypeDef,
     ListGatewaysOutputTypeDef,
     GetHypervisorOutputTypeDef,
@@ -365,20 +365,21 @@
     PutHypervisorPropertyMappingsInputRequestTypeDef,
     ListHypervisorsOutputTypeDef,
     ListGatewaysInputListGatewaysPaginateTypeDef,
     ListHypervisorsInputListHypervisorsPaginateTypeDef,
     ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesOutputTypeDef,
     VirtualMachineDetailsTypeDef,
+    PutBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayOutputTypeDef,
     GetVirtualMachineOutputTypeDef,
 )
 
 
-def get_structure() -> AssociateGatewayToServerInputRequestTypeDef:
+def get_value() -> AssociateGatewayToServerInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__init__.py` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__init__.pyi` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__main__.py` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BackupGateway 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.BackupGateway 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway\nOther"
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

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/client.py` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,22 @@
     from mypy_boto3_backup_gateway.client import BackupGatewayClient
 
     session = Session()
     client: BackupGatewayClient = session.client("backup-gateway")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListGatewaysPaginator, ListHypervisorsPaginator, ListVirtualMachinesPaginator
 from .type_defs import (
     AssociateGatewayToServerOutputTypeDef,
-    BandwidthRateLimitIntervalOutputTypeDef,
-    BandwidthRateLimitIntervalTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayOutputTypeDef,
     DeleteGatewayOutputTypeDef,
     DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     GetGatewayOutputTypeDef,
     GetHypervisorOutputTypeDef,
@@ -277,17 +276,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_virtual_machines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/client/#list_virtual_machines)
         """
 
     def put_bandwidth_rate_limit_schedule(
         self,
         *,
-        BandwidthRateLimitIntervals: Sequence[
-            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
-        ],
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],
         GatewayArn: str
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
```

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/client.pyi` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,22 @@
     from mypy_boto3_backup_gateway.client import BackupGatewayClient
 
     session = Session()
     client: BackupGatewayClient = session.client("backup-gateway")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListGatewaysPaginator, ListHypervisorsPaginator, ListVirtualMachinesPaginator
 from .type_defs import (
     AssociateGatewayToServerOutputTypeDef,
-    BandwidthRateLimitIntervalOutputTypeDef,
-    BandwidthRateLimitIntervalTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayOutputTypeDef,
     DeleteGatewayOutputTypeDef,
     DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     GetGatewayOutputTypeDef,
     GetHypervisorOutputTypeDef,
@@ -254,17 +253,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_virtual_machines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/client/#list_virtual_machines)
         """
     def put_bandwidth_rate_limit_schedule(
         self,
         *,
-        BandwidthRateLimitIntervals: Sequence[
-            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
-        ],
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],
         GatewayArn: str
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
```

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/literals.py` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/literals.pyi` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/paginator.py` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/paginator.pyi` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/type_defs.py` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef
 
-    data: AssociateGatewayToServerInputRequestTypeDef = {...}
+    data: AssociateGatewayToServerInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import HypervisorStateType, SyncMetadataStatusType
@@ -72,15 +72,15 @@
     "StartVirtualMachinesMetadataSyncOutputTypeDef",
     "TagResourceOutputTypeDef",
     "UntagResourceOutputTypeDef",
     "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateHypervisorOutputTypeDef",
     "GetBandwidthRateLimitScheduleOutputTypeDef",
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    "BandwidthRateLimitIntervalUnionTypeDef",
     "CreateGatewayInputRequestTypeDef",
     "ImportHypervisorConfigurationInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "GatewayDetailsTypeDef",
     "ListGatewaysOutputTypeDef",
     "GetHypervisorOutputTypeDef",
@@ -88,14 +88,15 @@
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     "ListHypervisorsOutputTypeDef",
     "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListHypervisorsInputListHypervisorsPaginateTypeDef",
     "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesOutputTypeDef",
     "VirtualMachineDetailsTypeDef",
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayOutputTypeDef",
     "GetVirtualMachineOutputTypeDef",
 )
 
 AssociateGatewayToServerInputRequestTypeDef = TypedDict(
     "AssociateGatewayToServerInputRequestTypeDef",
     {
@@ -614,24 +615,17 @@
     {
         "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
         "GatewayArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "BandwidthRateLimitIntervals": Sequence[
-            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
-        ],
-        "GatewayArn": str,
-    },
-)
-
+BandwidthRateLimitIntervalUnionTypeDef = Union[
+    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
+]
 _RequiredCreateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
     },
@@ -798,14 +792,22 @@
         "Path": str,
         "ResourceArn": str,
         "VmwareTags": List[VmwareTagTypeDef],
     },
     total=False,
 )
 
+PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+        "GatewayArn": str,
+    },
+)
+
 GetGatewayOutputTypeDef = TypedDict(
     "GetGatewayOutputTypeDef",
     {
         "Gateway": GatewayDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/type_defs.pyi` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef
 
-    data: AssociateGatewayToServerInputRequestTypeDef = {...}
+    data: AssociateGatewayToServerInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import HypervisorStateType, SyncMetadataStatusType
@@ -71,15 +71,15 @@
     "StartVirtualMachinesMetadataSyncOutputTypeDef",
     "TagResourceOutputTypeDef",
     "UntagResourceOutputTypeDef",
     "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateHypervisorOutputTypeDef",
     "GetBandwidthRateLimitScheduleOutputTypeDef",
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    "BandwidthRateLimitIntervalUnionTypeDef",
     "CreateGatewayInputRequestTypeDef",
     "ImportHypervisorConfigurationInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "GatewayDetailsTypeDef",
     "ListGatewaysOutputTypeDef",
     "GetHypervisorOutputTypeDef",
@@ -87,14 +87,15 @@
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     "ListHypervisorsOutputTypeDef",
     "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListHypervisorsInputListHypervisorsPaginateTypeDef",
     "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesOutputTypeDef",
     "VirtualMachineDetailsTypeDef",
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayOutputTypeDef",
     "GetVirtualMachineOutputTypeDef",
 )
 
 AssociateGatewayToServerInputRequestTypeDef = TypedDict(
     "AssociateGatewayToServerInputRequestTypeDef",
     {
@@ -599,24 +600,17 @@
     {
         "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
         "GatewayArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "BandwidthRateLimitIntervals": Sequence[
-            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
-        ],
-        "GatewayArn": str,
-    },
-)
-
+BandwidthRateLimitIntervalUnionTypeDef = Union[
+    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
+]
 _RequiredCreateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
     },
@@ -779,14 +773,22 @@
         "Path": str,
         "ResourceArn": str,
         "VmwareTags": List[VmwareTagTypeDef],
     },
     total=False,
 )
 
+PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+        "GatewayArn": str,
+    },
+)
+
 GetGatewayOutputTypeDef = TypedDict(
     "GetGatewayOutputTypeDef",
     {
         "Gateway": GatewayDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/PKG-INFO` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup-gateway
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.BackupGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.BackupGateway 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 backup-gateway type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 backup-gateway type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup-gateway)](https://pepy.tech/project/mypy-boto3-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupGateway 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[boto3.BackupGateway 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [mypy-boto3-backup-gateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/).
 
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
@@ -324,20 +324,20 @@
 )
 
 
 def check_value(value: GatewayTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_backup_gateway.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_backup_gateway.type_defs import (
     AssociateGatewayToServerInputRequestTypeDef,
     ResponseMetadataTypeDef,
     BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
@@ -381,15 +381,15 @@
     StartVirtualMachinesMetadataSyncOutputTypeDef,
     TagResourceOutputTypeDef,
     UntagResourceOutputTypeDef,
     UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateHypervisorOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
-    PutBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayInputRequestTypeDef,
     ImportHypervisorConfigurationInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     GatewayDetailsTypeDef,
     ListGatewaysOutputTypeDef,
     GetHypervisorOutputTypeDef,
@@ -397,20 +397,21 @@
     PutHypervisorPropertyMappingsInputRequestTypeDef,
     ListHypervisorsOutputTypeDef,
     ListGatewaysInputListGatewaysPaginateTypeDef,
     ListHypervisorsInputListHypervisorsPaginateTypeDef,
     ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesOutputTypeDef,
     VirtualMachineDetailsTypeDef,
+    PutBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayOutputTypeDef,
     GetVirtualMachineOutputTypeDef,
 )
 
 
-def get_structure() -> AssociateGatewayToServerInputRequestTypeDef:
+def get_value() -> AssociateGatewayToServerInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/SOURCES.txt` & `mypy-boto3-backup-gateway-1.28.16/mypy_boto3_backup_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15.post1/setup.py` & `mypy-boto3-backup-gateway-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backup-gateway",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_backup_gateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BackupGateway 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.BackupGateway 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 backup-gateway type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 backup-gateway type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_backup_gateway": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

