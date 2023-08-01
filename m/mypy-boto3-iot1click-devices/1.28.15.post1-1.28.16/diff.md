# Comparing `tmp/mypy-boto3-iot1click-devices-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iot1click-devices-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot1click-devices-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:18 2023, max compression
+gzip compressed data, was "mypy-boto3-iot1click-devices-1.28.16.tar", last modified: Tue Aug  1 11:36:58 2023, max compression
```

## Comparing `mypy-boto3-iot1click-devices-1.28.15.post1.tar` & `mypy-boto3-iot1click-devices-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:18.233176 mypy-boto3-iot1click-devices-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:45.000000 mypy-boto3-iot1click-devices-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-07-29 10:03:18.229176 mypy-boto3-iot1click-devices-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-07-29 09:47:45.000000 mypy-boto3-iot1click-devices-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:18.225176 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-29 09:47:45.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-29 09:47:45.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-29 09:47:45.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:45.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:45.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:18.229176 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-07-29 10:03:17.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 10:03:18.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:17.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:17.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:17.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:03:17.000000 mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:18.233176 mypy-boto3-iot1click-devices-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-29 09:47:45.000000 mypy-boto3-iot1click-devices-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:58.764868 mypy-boto3-iot1click-devices-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-08-01 11:36:58.760868 mypy-boto3-iot1click-devices-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:58.748868 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:58.760868 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:58.764868 mypy-boto3-iot1click-devices-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-01 11:20:27.000000 mypy-boto3-iot1click-devices-1.28.16/setup.py
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/LICENSE` & `mypy-boto3-iot1click-devices-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/PKG-INFO` & `mypy-boto3-iot1click-devices-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-devices
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot1click-devices type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iot1click-devices type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-devices)](https://pepy.tech/project/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
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
@@ -312,34 +312,34 @@
 )
 
 
 def check_value(value: ListDeviceEventsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot1click_devices.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
     DeviceMethodTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListDeviceEventsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
     ClaimDevicesByClaimCodeResponseTypeDef,
@@ -350,21 +350,22 @@
     ListTagsForResourceResponseTypeDef,
     UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListDevicesRequestListDevicesPaginateTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    ListDeviceEventsRequestRequestTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
-def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
+def get_value() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/README.md` & `mypy-boto3-iot1click-devices-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-devices)](https://pepy.tech/project/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
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
@@ -280,34 +280,34 @@
 )
 
 
 def check_value(value: ListDeviceEventsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot1click_devices.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
     DeviceMethodTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListDeviceEventsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
     ClaimDevicesByClaimCodeResponseTypeDef,
@@ -318,21 +318,22 @@
     ListTagsForResourceResponseTypeDef,
     UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListDevicesRequestListDevicesPaginateTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    ListDeviceEventsRequestRequestTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
-def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
+def get_value() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/__init__.py` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/__init__.pyi` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/client.py` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iot1click_devices.client import IoT1ClickDevicesServiceClient
 
     session = Session()
     client: IoT1ClickDevicesServiceClient = session.client("iot1click-devices")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListDeviceEventsPaginator, ListDevicesPaginator
 from .type_defs import (
     ClaimDevicesByClaimCodeResponseTypeDef,
     DescribeDeviceResponseTypeDef,
@@ -28,14 +27,15 @@
     FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InitiateDeviceClaimResponseTypeDef,
     InvokeDeviceMethodResponseTypeDef,
     ListDeviceEventsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TimestampTypeDef,
     UnclaimDeviceResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -171,16 +171,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/client/#invoke_device_method)
         """
 
     def list_device_events(
         self,
         *,
         DeviceId: str,
-        FromTimeStamp: Union[datetime, str],
-        ToTimeStamp: Union[datetime, str],
+        FromTimeStamp: TimestampTypeDef,
+        ToTimeStamp: TimestampTypeDef,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListDeviceEventsResponseTypeDef:
         """
         Using a device ID, returns a DeviceEventsResponse object containing an array of
         events for the device.
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/client.pyi` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iot1click_devices.client import IoT1ClickDevicesServiceClient
 
     session = Session()
     client: IoT1ClickDevicesServiceClient = session.client("iot1click-devices")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListDeviceEventsPaginator, ListDevicesPaginator
 from .type_defs import (
     ClaimDevicesByClaimCodeResponseTypeDef,
     DescribeDeviceResponseTypeDef,
@@ -28,14 +27,15 @@
     FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InitiateDeviceClaimResponseTypeDef,
     InvokeDeviceMethodResponseTypeDef,
     ListDeviceEventsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TimestampTypeDef,
     UnclaimDeviceResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -157,16 +157,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client.invoke_device_method)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/client/#invoke_device_method)
         """
     def list_device_events(
         self,
         *,
         DeviceId: str,
-        FromTimeStamp: Union[datetime, str],
-        ToTimeStamp: Union[datetime, str],
+        FromTimeStamp: TimestampTypeDef,
+        ToTimeStamp: TimestampTypeDef,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListDeviceEventsResponseTypeDef:
         """
         Using a device ID, returns a DeviceEventsResponse object containing an array of
         events for the device.
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/literals.py` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/literals.pyi` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/paginator.py` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     session = Session()
     client: IoT1ClickDevicesServiceClient = session.client("iot1click-devices")
 
     list_device_events_paginator: ListDeviceEventsPaginator = client.get_paginator("list_device_events")
     list_devices_paginator: ListDevicesPaginator = client.get_paginator("list_devices")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListDeviceEventsResponseTypeDef,
     ListDevicesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListDeviceEventsPaginator", "ListDevicesPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -51,16 +51,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdeviceeventspaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
-        FromTimeStamp: Union[datetime, str],
-        ToTimeStamp: Union[datetime, str],
+        FromTimeStamp: TimestampTypeDef,
+        ToTimeStamp: TimestampTypeDef,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/paginator.pyi` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     session = Session()
     client: IoT1ClickDevicesServiceClient = session.client("iot1click-devices")
 
     list_device_events_paginator: ListDeviceEventsPaginator = client.get_paginator("list_device_events")
     list_devices_paginator: ListDevicesPaginator = client.get_paginator("list_devices")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListDeviceEventsResponseTypeDef,
     ListDevicesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListDeviceEventsPaginator", "ListDevicesPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -48,16 +48,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdeviceeventspaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
-        FromTimeStamp: Union[datetime, str],
-        ToTimeStamp: Union[datetime, str],
+        FromTimeStamp: TimestampTypeDef,
+        ToTimeStamp: TimestampTypeDef,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/type_defs.py` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iot1click_devices.type_defs import ClaimDevicesByClaimCodeRequestRequestTypeDef
 
-    data: ClaimDevicesByClaimCodeRequestRequestTypeDef = {...}
+    data: ClaimDevicesByClaimCodeRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
@@ -28,15 +28,15 @@
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
     "DeviceMethodTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ListDeviceEventsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnclaimDeviceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceStateRequestRequestTypeDef",
     "ClaimDevicesByClaimCodeResponseTypeDef",
@@ -47,16 +47,17 @@
     "ListTagsForResourceResponseTypeDef",
     "UnclaimDeviceResponseTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "DeviceEventTypeDef",
     "GetDeviceMethodsResponseTypeDef",
     "InvokeDeviceMethodRequestRequestTypeDef",
-    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     "ListDevicesRequestListDevicesPaginateTypeDef",
+    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    "ListDeviceEventsRequestRequestTypeDef",
     "ListDeviceEventsResponseTypeDef",
 )
 
 ClaimDevicesByClaimCodeRequestRequestTypeDef = TypedDict(
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     {
         "ClaimCode": str,
@@ -156,38 +157,15 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestRequestTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class ListDeviceEventsRequestRequestTypeDef(
-    _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "DeviceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -354,20 +332,29 @@
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "DeviceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
     "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     {
         "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
+        "FromTimeStamp": TimestampTypeDef,
+        "ToTimeStamp": TimestampTypeDef,
     },
 )
 _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
     "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -378,23 +365,38 @@
 class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
     _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
 ):
     pass
 
 
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
+_RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestRequestTypeDef",
     {
-        "DeviceType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "DeviceId": str,
+        "FromTimeStamp": TimestampTypeDef,
+        "ToTimeStamp": TimestampTypeDef,
+    },
+)
+_OptionalListDeviceEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
+
+class ListDeviceEventsRequestRequestTypeDef(
+    _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
+):
+    pass
+
+
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices/type_defs.pyi` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iot1click_devices.type_defs import ClaimDevicesByClaimCodeRequestRequestTypeDef
 
-    data: ClaimDevicesByClaimCodeRequestRequestTypeDef = {...}
+    data: ClaimDevicesByClaimCodeRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
@@ -27,15 +27,15 @@
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
     "DeviceMethodTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ListDeviceEventsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnclaimDeviceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceStateRequestRequestTypeDef",
     "ClaimDevicesByClaimCodeResponseTypeDef",
@@ -46,16 +46,17 @@
     "ListTagsForResourceResponseTypeDef",
     "UnclaimDeviceResponseTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "DeviceEventTypeDef",
     "GetDeviceMethodsResponseTypeDef",
     "InvokeDeviceMethodRequestRequestTypeDef",
-    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     "ListDevicesRequestListDevicesPaginateTypeDef",
+    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    "ListDeviceEventsRequestRequestTypeDef",
     "ListDeviceEventsResponseTypeDef",
 )
 
 ClaimDevicesByClaimCodeRequestRequestTypeDef = TypedDict(
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     {
         "ClaimCode": str,
@@ -153,36 +154,15 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestRequestTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class ListDeviceEventsRequestRequestTypeDef(
-    _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "DeviceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -345,20 +325,29 @@
 
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "DeviceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
     "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     {
         "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
+        "FromTimeStamp": TimestampTypeDef,
+        "ToTimeStamp": TimestampTypeDef,
     },
 )
 _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
     "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -367,23 +356,36 @@
 
 class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
     _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
 ):
     pass
 
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
+_RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestRequestTypeDef",
     {
-        "DeviceType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "DeviceId": str,
+        "FromTimeStamp": TimestampTypeDef,
+        "ToTimeStamp": TimestampTypeDef,
+    },
+)
+_OptionalListDeviceEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
+class ListDeviceEventsRequestRequestTypeDef(
+    _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
+):
+    pass
+
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices.egg-info/PKG-INFO` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-devices
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot1click-devices type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iot1click-devices type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-devices)](https://pepy.tech/project/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
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
@@ -312,34 +312,34 @@
 )
 
 
 def check_value(value: ListDeviceEventsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot1click_devices.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
     DeviceMethodTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListDeviceEventsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
     ClaimDevicesByClaimCodeResponseTypeDef,
@@ -350,21 +350,22 @@
     ListTagsForResourceResponseTypeDef,
     UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListDevicesRequestListDevicesPaginateTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    ListDeviceEventsRequestRequestTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
-def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
+def get_value() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt` & `mypy-boto3-iot1click-devices-1.28.16/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.15.post1/setup.py` & `mypy-boto3-iot1click-devices-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot1click-devices",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iot1click_devices"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT1ClickDevicesService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.IoT1ClickDevicesService 1.28.16 service generated with"
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
-    keywords="boto3 iot1click-devices type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iot1click-devices type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iot1click_devices": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

