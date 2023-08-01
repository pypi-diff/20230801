# Comparing `tmp/mypy-boto3-iot-data-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iot-data-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-data-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:19 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-data-1.28.16.tar", last modified: Tue Aug  1 11:36:59 2023, max compression
```

## Comparing `mypy-boto3-iot-data-1.28.15.post1.tar` & `mypy-boto3-iot-data-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.485180 mypy-boto3-iot-data-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-29 10:03:19.485180 mypy-boto3-iot-data-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.477180 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-29 09:47:43.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-07-29 09:47:43.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-07-29 09:47:43.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-29 09:47:43.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.485180 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-29 10:03:19.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:19.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:19.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:19.000000 mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:19.485180 mypy-boto3-iot-data-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-29 09:47:42.000000 mypy-boto3-iot-data-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.476867 mypy-boto3-iot-data-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-08-01 11:36:59.476867 mypy-boto3-iot-data-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.468866 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.476867 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-08-01 11:36:59.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:36:59.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:59.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:36:59.000000 mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:59.476867 mypy-boto3-iot-data-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-01 11:20:24.000000 mypy-boto3-iot-data-1.28.16/setup.py
```

### Comparing `mypy-boto3-iot-data-1.28.15.post1/LICENSE` & `mypy-boto3-iot-data-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.28.15.post1/PKG-INFO` & `mypy-boto3-iot-data-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-data
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTDataPlane 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTDataPlane 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iot-data type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-data)](https://pepy.tech/project/mypy-boto3-iot-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDataPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
+[boto3.IoTDataPlane 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
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
 [mypy-boto3-iot-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/).
 
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
@@ -312,23 +312,24 @@
 )
 
 
 def check_value(value: ListRetainedMessagesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot_data.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot_data.type_defs import (
+    BlobTypeDef,
     DeleteThingShadowRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetRetainedMessageRequestRequestTypeDef,
     GetThingShadowRequestRequestTypeDef,
     ListNamedShadowsForThingRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListRetainedMessagesRequestRequestTypeDef,
@@ -342,15 +343,15 @@
     ListNamedShadowsForThingResponseTypeDef,
     UpdateThingShadowResponseTypeDef,
     ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
     ListRetainedMessagesResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteThingShadowRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-data-1.28.15.post1/README.md` & `mypy-boto3-iot-data-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-data)](https://pepy.tech/project/mypy-boto3-iot-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDataPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
+[boto3.IoTDataPlane 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
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
 [mypy-boto3-iot-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/).
 
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
@@ -280,23 +280,24 @@
 )
 
 
 def check_value(value: ListRetainedMessagesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot_data.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot_data.type_defs import (
+    BlobTypeDef,
     DeleteThingShadowRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetRetainedMessageRequestRequestTypeDef,
     GetThingShadowRequestRequestTypeDef,
     ListNamedShadowsForThingRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListRetainedMessagesRequestRequestTypeDef,
@@ -310,15 +311,15 @@
     ListNamedShadowsForThingResponseTypeDef,
     UpdateThingShadowResponseTypeDef,
     ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
     ListRetainedMessagesResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteThingShadowRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/__init__.py` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/__init__.pyi` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/__main__.py` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTDataPlane 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTDataPlane 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane\nOther"
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

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/client.py` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -10,62 +10,58 @@
     from mypy_boto3_iot_data.client import IoTDataPlaneClient
 
     session = Session()
     client: IoTDataPlaneClient = session.client("iot-data")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import PayloadFormatIndicatorType
 from .paginator import ListRetainedMessagesPaginator
 from .type_defs import (
+    BlobTypeDef,
     DeleteThingShadowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRetainedMessageResponseTypeDef,
     GetThingShadowResponseTypeDef,
     ListNamedShadowsForThingResponseTypeDef,
     ListRetainedMessagesResponseTypeDef,
     UpdateThingShadowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTDataPlaneClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     MethodNotAllowedException: Type[BotocoreClientError]
     RequestEntityTooLargeException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnauthorizedException: Type[BotocoreClientError]
     UnsupportedDocumentEncodingException: Type[BotocoreClientError]
 
-
 class IoTDataPlaneClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/)
     """
 
     meta: ClientMeta
@@ -74,128 +70,113 @@
     def exceptions(self) -> Exceptions:
         """
         IoTDataPlaneClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#close)
         """
-
     def delete_thing_shadow(
         self, *, thingName: str, shadowName: str = ...
     ) -> DeleteThingShadowResponseTypeDef:
         """
         Deletes the shadow for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.delete_thing_shadow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#delete_thing_shadow)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#generate_presigned_url)
         """
-
     def get_retained_message(self, *, topic: str) -> GetRetainedMessageResponseTypeDef:
         """
         Gets the details of a single retained message for the specified topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.get_retained_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#get_retained_message)
         """
-
     def get_thing_shadow(
         self, *, thingName: str, shadowName: str = ...
     ) -> GetThingShadowResponseTypeDef:
         """
         Gets the shadow for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.get_thing_shadow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#get_thing_shadow)
         """
-
     def list_named_shadows_for_thing(
         self, *, thingName: str, nextToken: str = ..., pageSize: int = ...
     ) -> ListNamedShadowsForThingResponseTypeDef:
         """
         Lists the shadows for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.list_named_shadows_for_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#list_named_shadows_for_thing)
         """
-
     def list_retained_messages(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListRetainedMessagesResponseTypeDef:
         """
         Lists summary information about the retained messages stored for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.list_retained_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#list_retained_messages)
         """
-
     def publish(
         self,
         *,
         topic: str,
         qos: int = ...,
         retain: bool = ...,
-        payload: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        payload: BlobTypeDef = ...,
         userProperties: str = ...,
         payloadFormatIndicator: PayloadFormatIndicatorType = ...,
         contentType: str = ...,
         responseTopic: str = ...,
         correlationData: str = ...,
         messageExpiry: int = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Publishes an MQTT message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.publish)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#publish)
         """
-
     def update_thing_shadow(
-        self,
-        *,
-        thingName: str,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
-        shadowName: str = ...
+        self, *, thingName: str, payload: BlobTypeDef, shadowName: str = ...
     ) -> UpdateThingShadowResponseTypeDef:
         """
         Updates the shadow for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.update_thing_shadow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#update_thing_shadow)
         """
-
     def get_paginator(
         self, operation_name: Literal["list_retained_messages"]
     ) -> ListRetainedMessagesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/client.pyi` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,58 +10,62 @@
     from mypy_boto3_iot_data.client import IoTDataPlaneClient
 
     session = Session()
     client: IoTDataPlaneClient = session.client("iot-data")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import PayloadFormatIndicatorType
 from .paginator import ListRetainedMessagesPaginator
 from .type_defs import (
+    BlobTypeDef,
     DeleteThingShadowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRetainedMessageResponseTypeDef,
     GetThingShadowResponseTypeDef,
     ListNamedShadowsForThingResponseTypeDef,
     ListRetainedMessagesResponseTypeDef,
     UpdateThingShadowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("IoTDataPlaneClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     MethodNotAllowedException: Type[BotocoreClientError]
     RequestEntityTooLargeException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnauthorizedException: Type[BotocoreClientError]
     UnsupportedDocumentEncodingException: Type[BotocoreClientError]
 
+
 class IoTDataPlaneClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/)
     """
 
     meta: ClientMeta
@@ -70,117 +74,124 @@
     def exceptions(self) -> Exceptions:
         """
         IoTDataPlaneClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#close)
         """
+
     def delete_thing_shadow(
         self, *, thingName: str, shadowName: str = ...
     ) -> DeleteThingShadowResponseTypeDef:
         """
         Deletes the shadow for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.delete_thing_shadow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#delete_thing_shadow)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#generate_presigned_url)
         """
+
     def get_retained_message(self, *, topic: str) -> GetRetainedMessageResponseTypeDef:
         """
         Gets the details of a single retained message for the specified topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.get_retained_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#get_retained_message)
         """
+
     def get_thing_shadow(
         self, *, thingName: str, shadowName: str = ...
     ) -> GetThingShadowResponseTypeDef:
         """
         Gets the shadow for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.get_thing_shadow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#get_thing_shadow)
         """
+
     def list_named_shadows_for_thing(
         self, *, thingName: str, nextToken: str = ..., pageSize: int = ...
     ) -> ListNamedShadowsForThingResponseTypeDef:
         """
         Lists the shadows for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.list_named_shadows_for_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#list_named_shadows_for_thing)
         """
+
     def list_retained_messages(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListRetainedMessagesResponseTypeDef:
         """
         Lists summary information about the retained messages stored for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.list_retained_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#list_retained_messages)
         """
+
     def publish(
         self,
         *,
         topic: str,
         qos: int = ...,
         retain: bool = ...,
-        payload: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        payload: BlobTypeDef = ...,
         userProperties: str = ...,
         payloadFormatIndicator: PayloadFormatIndicatorType = ...,
         contentType: str = ...,
         responseTopic: str = ...,
         correlationData: str = ...,
         messageExpiry: int = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Publishes an MQTT message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.publish)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#publish)
         """
+
     def update_thing_shadow(
-        self,
-        *,
-        thingName: str,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
-        shadowName: str = ...
+        self, *, thingName: str, payload: BlobTypeDef, shadowName: str = ...
     ) -> UpdateThingShadowResponseTypeDef:
         """
         Updates the shadow for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.update_thing_shadow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#update_thing_shadow)
         """
+
     def get_paginator(
         self, operation_name: Literal["list_retained_messages"]
     ) -> ListRetainedMessagesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/literals.py` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/literals.pyi` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/paginator.py` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/paginator.pyi` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/type_defs.py` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 Type annotations for iot-data service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot_data.type_defs import DeleteThingShadowRequestRequestTypeDef
+    from mypy_boto3_iot_data.type_defs import BlobTypeDef
 
-    data: DeleteThingShadowRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
 
 from .literals import PayloadFormatIndicatorType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "BlobTypeDef",
     "DeleteThingShadowRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetRetainedMessageRequestRequestTypeDef",
     "GetThingShadowRequestRequestTypeDef",
     "ListNamedShadowsForThingRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListRetainedMessagesRequestRequestTypeDef",
@@ -41,35 +41,34 @@
     "GetThingShadowResponseTypeDef",
     "ListNamedShadowsForThingResponseTypeDef",
     "UpdateThingShadowResponseTypeDef",
     "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
     "ListRetainedMessagesResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredDeleteThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalDeleteThingShadowRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
-
 class DeleteThingShadowRequestRequestTypeDef(
     _RequiredDeleteThingShadowRequestRequestTypeDef, _OptionalDeleteThingShadowRequestRequestTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -94,21 +93,19 @@
     "_OptionalGetThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
-
 class GetThingShadowRequestRequestTypeDef(
     _RequiredGetThingShadowRequestRequestTypeDef, _OptionalGetThingShadowRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListNamedShadowsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListNamedShadowsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListNamedShadowsForThingRequestRequestTypeDef = TypedDict(
@@ -116,22 +113,20 @@
     {
         "nextToken": str,
         "pageSize": int,
     },
     total=False,
 )
 
-
 class ListNamedShadowsForThingRequestRequestTypeDef(
     _RequiredListNamedShadowsForThingRequestRequestTypeDef,
     _OptionalListNamedShadowsForThingRequestRequestTypeDef,
 ):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -165,54 +160,50 @@
     },
 )
 _OptionalPublishRequestRequestTypeDef = TypedDict(
     "_OptionalPublishRequestRequestTypeDef",
     {
         "qos": int,
         "retain": bool,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payload": BlobTypeDef,
         "userProperties": str,
         "payloadFormatIndicator": PayloadFormatIndicatorType,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
         "messageExpiry": int,
     },
     total=False,
 )
 
-
 class PublishRequestRequestTypeDef(
     _RequiredPublishRequestRequestTypeDef, _OptionalPublishRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payload": BlobTypeDef,
     },
 )
 _OptionalUpdateThingShadowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
-
 class UpdateThingShadowRequestRequestTypeDef(
     _RequiredUpdateThingShadowRequestRequestTypeDef, _OptionalUpdateThingShadowRequestRequestTypeDef
 ):
     pass
 
-
 DeleteThingShadowResponseTypeDef = TypedDict(
     "DeleteThingShadowResponseTypeDef",
     {
         "payload": StreamingBody,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data/type_defs.pyi` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 Type annotations for iot-data service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot_data.type_defs import DeleteThingShadowRequestRequestTypeDef
+    from mypy_boto3_iot_data.type_defs import BlobTypeDef
 
-    data: DeleteThingShadowRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
 
 from .literals import PayloadFormatIndicatorType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "BlobTypeDef",
     "DeleteThingShadowRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetRetainedMessageRequestRequestTypeDef",
     "GetThingShadowRequestRequestTypeDef",
     "ListNamedShadowsForThingRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListRetainedMessagesRequestRequestTypeDef",
@@ -40,33 +42,36 @@
     "GetThingShadowResponseTypeDef",
     "ListNamedShadowsForThingResponseTypeDef",
     "UpdateThingShadowResponseTypeDef",
     "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
     "ListRetainedMessagesResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredDeleteThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalDeleteThingShadowRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
+
 class DeleteThingShadowRequestRequestTypeDef(
     _RequiredDeleteThingShadowRequestRequestTypeDef, _OptionalDeleteThingShadowRequestRequestTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -91,19 +96,21 @@
     "_OptionalGetThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
+
 class GetThingShadowRequestRequestTypeDef(
     _RequiredGetThingShadowRequestRequestTypeDef, _OptionalGetThingShadowRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListNamedShadowsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListNamedShadowsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListNamedShadowsForThingRequestRequestTypeDef = TypedDict(
@@ -111,20 +118,22 @@
     {
         "nextToken": str,
         "pageSize": int,
     },
     total=False,
 )
 
+
 class ListNamedShadowsForThingRequestRequestTypeDef(
     _RequiredListNamedShadowsForThingRequestRequestTypeDef,
     _OptionalListNamedShadowsForThingRequestRequestTypeDef,
 ):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -158,50 +167,54 @@
     },
 )
 _OptionalPublishRequestRequestTypeDef = TypedDict(
     "_OptionalPublishRequestRequestTypeDef",
     {
         "qos": int,
         "retain": bool,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payload": BlobTypeDef,
         "userProperties": str,
         "payloadFormatIndicator": PayloadFormatIndicatorType,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
         "messageExpiry": int,
     },
     total=False,
 )
 
+
 class PublishRequestRequestTypeDef(
     _RequiredPublishRequestRequestTypeDef, _OptionalPublishRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payload": BlobTypeDef,
     },
 )
 _OptionalUpdateThingShadowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
+
 class UpdateThingShadowRequestRequestTypeDef(
     _RequiredUpdateThingShadowRequestRequestTypeDef, _OptionalUpdateThingShadowRequestRequestTypeDef
 ):
     pass
 
+
 DeleteThingShadowResponseTypeDef = TypedDict(
     "DeleteThingShadowResponseTypeDef",
     {
         "payload": StreamingBody,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data.egg-info/PKG-INFO` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-data
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTDataPlane 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTDataPlane 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iot-data type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-data)](https://pepy.tech/project/mypy-boto3-iot-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDataPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
+[boto3.IoTDataPlane 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
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
 [mypy-boto3-iot-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/).
 
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
@@ -312,23 +312,24 @@
 )
 
 
 def check_value(value: ListRetainedMessagesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot_data.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot_data.type_defs import (
+    BlobTypeDef,
     DeleteThingShadowRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetRetainedMessageRequestRequestTypeDef,
     GetThingShadowRequestRequestTypeDef,
     ListNamedShadowsForThingRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListRetainedMessagesRequestRequestTypeDef,
@@ -342,15 +343,15 @@
     ListNamedShadowsForThingResponseTypeDef,
     UpdateThingShadowResponseTypeDef,
     ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
     ListRetainedMessagesResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteThingShadowRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-data-1.28.15.post1/mypy_boto3_iot_data.egg-info/SOURCES.txt` & `mypy-boto3-iot-data-1.28.16/mypy_boto3_iot_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.28.15.post1/setup.py` & `mypy-boto3-iot-data-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot-data",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iot_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTDataPlane 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.IoTDataPlane 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 iot-data type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iot-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iot_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

