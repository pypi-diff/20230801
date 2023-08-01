# Comparing `tmp/mypy-boto3-iotsecuretunneling-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iotsecuretunneling-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotsecuretunneling-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:22 2023, max compression
+gzip compressed data, was "mypy-boto3-iotsecuretunneling-1.28.16.tar", last modified: Tue Aug  1 11:37:02 2023, max compression
```

## Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1.tar` & `mypy-boto3-iotsecuretunneling-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:22.885194 mypy-boto3-iotsecuretunneling-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-07-29 10:03:22.881194 mypy-boto3-iotsecuretunneling-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:22.869194 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-29 09:48:04.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:22.881194 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-07-29 10:03:22.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-29 10:03:22.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:22.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:22.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:22.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 10:03:22.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:22.885194 mypy-boto3-iotsecuretunneling-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-29 09:48:03.000000 mypy-boto3-iotsecuretunneling-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:02.952859 mypy-boto3-iotsecuretunneling-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:48.000000 mypy-boto3-iotsecuretunneling-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-08-01 11:37:02.952859 mypy-boto3-iotsecuretunneling-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-08-01 11:20:48.000000 mypy-boto3-iotsecuretunneling-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:02.944859 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-01 11:20:48.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-01 11:20:48.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 11:20:48.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-08-01 11:20:49.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-08-01 11:20:49.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-08-01 11:20:49.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-08-01 11:20:49.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:48.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-08-01 11:20:49.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-08-01 11:20:49.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:48.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:02.948859 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-08-01 11:37:02.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 11:37:02.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:02.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:02.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:02.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 11:37:02.000000 mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:02.952859 mypy-boto3-iotsecuretunneling-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-01 11:20:48.000000 mypy-boto3-iotsecuretunneling-1.28.16/setup.py
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/LICENSE` & `mypy-boto3-iotsecuretunneling-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/PKG-INFO` & `mypy-boto3-iotsecuretunneling-1.28.16/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsecuretunneling
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTSecureTunneling 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTSecureTunneling 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotsecuretunneling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotsecuretunneling type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsecuretunneling)](https://pepy.tech/project/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -291,20 +291,20 @@
 )
 
 
 def check_value(value: ClientModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotsecuretunneling.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -314,25 +314,26 @@
     TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
     TimeoutConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
+    DestinationConfigUnionTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
-def get_structure() -> CloseTunnelRequestRequestTypeDef:
+def get_value() -> CloseTunnelRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/README.md` & `mypy-boto3-iotsecuretunneling-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsecuretunneling)](https://pepy.tech/project/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -259,20 +259,20 @@
 )
 
 
 def check_value(value: ClientModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotsecuretunneling.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -282,25 +282,26 @@
     TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
     TimeoutConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
+    DestinationConfigUnionTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
-def get_structure() -> CloseTunnelRequestRequestTypeDef:
+def get_value() -> CloseTunnelRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/__main__.py` & `mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTSecureTunneling 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTSecureTunneling 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling\nOther"
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

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/client.py` & `mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,22 @@
     from boto3.session import Session
     from mypy_boto3_iotsecuretunneling.client import IoTSecureTunnelingClient
 
     session = Session()
     client: IoTSecureTunnelingClient = session.client("iotsecuretunneling")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ClientModeType
 from .type_defs import (
     DescribeTunnelResponseTypeDef,
-    DestinationConfigOutputTypeDef,
-    DestinationConfigTypeDef,
+    DestinationConfigUnionTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelResponseTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
     TagTypeDef,
     TimeoutConfigTypeDef,
 )
@@ -129,15 +128,15 @@
         """
 
     def open_tunnel(
         self,
         *,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        destinationConfig: Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef] = ...,
+        destinationConfig: DestinationConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...
     ) -> OpenTunnelResponseTypeDef:
         """
         Creates a new tunnel, and returns two client access tokens for clients to use to
         connect to the IoT Secure Tunneling proxy server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)
@@ -145,15 +144,15 @@
         """
 
     def rotate_tunnel_access_token(
         self,
         *,
         tunnelId: str,
         clientMode: ClientModeType,
-        destinationConfig: Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef] = ...
+        destinationConfig: DestinationConfigUnionTypeDef = ...
     ) -> RotateTunnelAccessTokenResponseTypeDef:
         """
         Revokes the current client access token (CAT) and returns new CAT for clients to
         use when reconnecting to secure tunneling to access the same tunnel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.rotate_tunnel_access_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/client/#rotate_tunnel_access_token)
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/client.pyi` & `mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,22 @@
     from boto3.session import Session
     from mypy_boto3_iotsecuretunneling.client import IoTSecureTunnelingClient
 
     session = Session()
     client: IoTSecureTunnelingClient = session.client("iotsecuretunneling")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ClientModeType
 from .type_defs import (
     DescribeTunnelResponseTypeDef,
-    DestinationConfigOutputTypeDef,
-    DestinationConfigTypeDef,
+    DestinationConfigUnionTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelResponseTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
     TagTypeDef,
     TimeoutConfigTypeDef,
 )
@@ -118,30 +117,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/client/#list_tunnels)
         """
     def open_tunnel(
         self,
         *,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        destinationConfig: Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef] = ...,
+        destinationConfig: DestinationConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...
     ) -> OpenTunnelResponseTypeDef:
         """
         Creates a new tunnel, and returns two client access tokens for clients to use to
         connect to the IoT Secure Tunneling proxy server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/client/#open_tunnel)
         """
     def rotate_tunnel_access_token(
         self,
         *,
         tunnelId: str,
         clientMode: ClientModeType,
-        destinationConfig: Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef] = ...
+        destinationConfig: DestinationConfigUnionTypeDef = ...
     ) -> RotateTunnelAccessTokenResponseTypeDef:
         """
         Revokes the current client access token (CAT) and returns new CAT for clients to
         use when reconnecting to secure tunneling to access the same tunnel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.rotate_tunnel_access_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/client/#rotate_tunnel_access_token)
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/literals.py` & `mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/literals.pyi` & `mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/type_defs.py` & `mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef
 
-    data: CloseTunnelRequestRequestTypeDef = {...}
+    data: CloseTunnelRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ClientModeType, ConnectionStatusType, TunnelStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -34,14 +34,15 @@
     "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
     "TimeoutConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
+    "DestinationConfigUnionTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
@@ -208,14 +209,15 @@
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationConfigUnionTypeDef = Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef]
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
         "clientMode": ClientModeType,
     },
 )
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling/type_defs.pyi` & `mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef
 
-    data: CloseTunnelRequestRequestTypeDef = {...}
+    data: CloseTunnelRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ClientModeType, ConnectionStatusType, TunnelStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -33,14 +33,15 @@
     "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
     "TimeoutConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
+    "DestinationConfigUnionTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
@@ -201,14 +202,15 @@
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationConfigUnionTypeDef = Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef]
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
         "clientMode": ClientModeType,
     },
 )
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO` & `mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsecuretunneling
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTSecureTunneling 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTSecureTunneling 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotsecuretunneling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotsecuretunneling type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsecuretunneling)](https://pepy.tech/project/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -291,20 +291,20 @@
 )
 
 
 def check_value(value: ClientModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotsecuretunneling.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -314,25 +314,26 @@
     TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
     TimeoutConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
+    DestinationConfigUnionTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
-def get_structure() -> CloseTunnelRequestRequestTypeDef:
+def get_value() -> CloseTunnelRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt` & `mypy-boto3-iotsecuretunneling-1.28.16/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.15.post1/setup.py` & `mypy-boto3-iotsecuretunneling-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotsecuretunneling",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iotsecuretunneling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTSecureTunneling 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.IoTSecureTunneling 1.28.16 service generated with"
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
-    keywords="boto3 iotsecuretunneling type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iotsecuretunneling type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iotsecuretunneling": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/"
```

