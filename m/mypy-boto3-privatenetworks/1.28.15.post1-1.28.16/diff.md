# Comparing `tmp/mypy-boto3-privatenetworks-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-privatenetworks-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-privatenetworks-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:55 2023, max compression
+gzip compressed data, was "mypy-boto3-privatenetworks-1.28.16.tar", last modified: Tue Aug  1 11:37:34 2023, max compression
```

## Comparing `mypy-boto3-privatenetworks-1.28.15.post1.tar` & `mypy-boto3-privatenetworks-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21430 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29836 2023-07-29 09:53:31.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29781 2023-07-29 09:53:31.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.792785 mypy-boto3-privatenetworks-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-08-01 11:37:34.784785 mypy-boto3-privatenetworks-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.780785 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21357 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29938 2023-08-01 11:26:34.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-08-01 11:26:34.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.784785 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-08-01 11:37:34.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 11:37:34.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:34.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:34.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:34.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:37:34.000000 mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:34.792785 mypy-boto3-privatenetworks-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-01 11:26:33.000000 mypy-boto3-privatenetworks-1.28.16/setup.py
```

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/LICENSE` & `mypy-boto3-privatenetworks-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/PKG-INFO` & `mypy-boto3-privatenetworks-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Private5G 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 privatenetworks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 privatenetworks type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-privatenetworks)](https://pepy.tech/project/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
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
@@ -344,20 +344,20 @@
 )
 
 
 def check_value(value: AcknowledgmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_privatenetworks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
@@ -418,25 +418,26 @@
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     AcknowledgeOrderReceiptResponseTypeDef,
     GetOrderResponseTypeDef,
     ListOrdersResponseTypeDef,
     NetworkSiteTypeDef,
     CreateNetworkSiteRequestRequestTypeDef,
+    SitePlanUnionTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
+def get_value() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/README.md` & `mypy-boto3-privatenetworks-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-privatenetworks)](https://pepy.tech/project/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
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
@@ -312,20 +312,20 @@
 )
 
 
 def check_value(value: AcknowledgmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_privatenetworks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
@@ -386,25 +386,26 @@
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     AcknowledgeOrderReceiptResponseTypeDef,
     GetOrderResponseTypeDef,
     ListOrdersResponseTypeDef,
     NetworkSiteTypeDef,
     CreateNetworkSiteRequestRequestTypeDef,
+    SitePlanUnionTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
+def get_value() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__init__.py` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__init__.pyi` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__main__.py` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Private5G 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Private5G 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G\nOther"
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

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/client.py` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_privatenetworks.client import Private5GClient
 
     session = Session()
     client: Private5GClient = session.client("privatenetworks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeviceIdentifierFilterKeysType,
     NetworkResourceFilterKeysType,
     OrderFilterKeysType,
@@ -52,16 +52,15 @@
     ListNetworkResourcesResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListOrdersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     PositionTypeDef,
-    SitePlanOutputTypeDef,
-    SitePlanTypeDef,
+    SitePlanUnionTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -192,15 +191,15 @@
         *,
         networkArn: str,
         networkSiteName: str,
         availabilityZone: str = ...,
         availabilityZoneId: str = ...,
         clientToken: str = ...,
         description: str = ...,
-        pendingPlan: Union[SitePlanTypeDef, SitePlanOutputTypeDef] = ...,
+        pendingPlan: SitePlanUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkSiteResponseTypeDef:
         """
         Creates a network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#create_network_site)
@@ -422,19 +421,15 @@
         Updates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#update_network_site)
         """
 
     def update_network_site_plan(
-        self,
-        *,
-        networkSiteArn: str,
-        pendingPlan: Union[SitePlanTypeDef, SitePlanOutputTypeDef],
-        clientToken: str = ...
+        self, *, networkSiteArn: str, pendingPlan: SitePlanUnionTypeDef, clientToken: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#update_network_site_plan)
         """
```

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/client.pyi` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_privatenetworks.client import Private5GClient
 
     session = Session()
     client: Private5GClient = session.client("privatenetworks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeviceIdentifierFilterKeysType,
     NetworkResourceFilterKeysType,
     OrderFilterKeysType,
@@ -52,16 +52,15 @@
     ListNetworkResourcesResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListOrdersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     PositionTypeDef,
-    SitePlanOutputTypeDef,
-    SitePlanTypeDef,
+    SitePlanUnionTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -180,15 +179,15 @@
         *,
         networkArn: str,
         networkSiteName: str,
         availabilityZone: str = ...,
         availabilityZoneId: str = ...,
         clientToken: str = ...,
         description: str = ...,
-        pendingPlan: Union[SitePlanTypeDef, SitePlanOutputTypeDef] = ...,
+        pendingPlan: SitePlanUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkSiteResponseTypeDef:
         """
         Creates a network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#create_network_site)
@@ -389,19 +388,15 @@
         """
         Updates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#update_network_site)
         """
     def update_network_site_plan(
-        self,
-        *,
-        networkSiteArn: str,
-        pendingPlan: Union[SitePlanTypeDef, SitePlanOutputTypeDef],
-        clientToken: str = ...
+        self, *, networkSiteArn: str, pendingPlan: SitePlanUnionTypeDef, clientToken: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#update_network_site_plan)
         """
```

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/literals.py` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/literals.pyi` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/paginator.py` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/paginator.pyi` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/type_defs.py` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestRequestTypeDef
 
-    data: AcknowledgeOrderReceiptRequestRequestTypeDef = {...}
+    data: AcknowledgeOrderReceiptRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AcknowledgmentStatusType,
     CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
@@ -103,14 +103,15 @@
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
     "AcknowledgeOrderReceiptResponseTypeDef",
     "GetOrderResponseTypeDef",
     "ListOrdersResponseTypeDef",
     "NetworkSiteTypeDef",
     "CreateNetworkSiteRequestRequestTypeDef",
+    "SitePlanUnionTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
     "ListNetworkSitesResponseTypeDef",
     "UpdateNetworkSiteResponseTypeDef",
@@ -1080,14 +1081,15 @@
 
 class CreateNetworkSiteRequestRequestTypeDef(
     _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
 ):
     pass
 
 
+SitePlanUnionTypeDef = Union[SitePlanTypeDef, SitePlanOutputTypeDef]
 _RequiredUpdateNetworkSitePlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "pendingPlan": SitePlanTypeDef,
     },
 )
```

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/type_defs.pyi` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestRequestTypeDef
 
-    data: AcknowledgeOrderReceiptRequestRequestTypeDef = {...}
+    data: AcknowledgeOrderReceiptRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AcknowledgmentStatusType,
     CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
@@ -102,14 +102,15 @@
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
     "AcknowledgeOrderReceiptResponseTypeDef",
     "GetOrderResponseTypeDef",
     "ListOrdersResponseTypeDef",
     "NetworkSiteTypeDef",
     "CreateNetworkSiteRequestRequestTypeDef",
+    "SitePlanUnionTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
     "ListNetworkSitesResponseTypeDef",
     "UpdateNetworkSiteResponseTypeDef",
@@ -1027,14 +1028,15 @@
 )
 
 class CreateNetworkSiteRequestRequestTypeDef(
     _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
 ):
     pass
 
+SitePlanUnionTypeDef = Union[SitePlanTypeDef, SitePlanOutputTypeDef]
 _RequiredUpdateNetworkSitePlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "pendingPlan": SitePlanTypeDef,
     },
 )
```

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/PKG-INFO` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Private5G 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 privatenetworks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 privatenetworks type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-privatenetworks)](https://pepy.tech/project/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
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
@@ -344,20 +344,20 @@
 )
 
 
 def check_value(value: AcknowledgmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_privatenetworks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
@@ -418,25 +418,26 @@
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     AcknowledgeOrderReceiptResponseTypeDef,
     GetOrderResponseTypeDef,
     ListOrdersResponseTypeDef,
     NetworkSiteTypeDef,
     CreateNetworkSiteRequestRequestTypeDef,
+    SitePlanUnionTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
+def get_value() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/SOURCES.txt` & `mypy-boto3-privatenetworks-1.28.16/mypy_boto3_privatenetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15.post1/setup.py` & `mypy-boto3-privatenetworks-1.28.16/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-privatenetworks",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_privatenetworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Private5G 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 privatenetworks type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 privatenetworks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_privatenetworks": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

