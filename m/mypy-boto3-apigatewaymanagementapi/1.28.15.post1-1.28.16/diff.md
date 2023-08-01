# Comparing `tmp/mypy-boto3-apigatewaymanagementapi-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-apigatewaymanagementapi-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigatewaymanagementapi-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:27 2023, max compression
+gzip compressed data, was "mypy-boto3-apigatewaymanagementapi-1.28.16.tar", last modified: Tue Aug  1 11:36:08 2023, max compression
```

## Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1.tar` & `mypy-boto3-apigatewaymanagementapi-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.692993 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-07-29 10:02:27.688993 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.684993 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.688993 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-07-29 10:02:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-29 10:02:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 10:02:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:27.692993 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-29 09:37:56.000000 mypy-boto3-apigatewaymanagementapi-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.548956 mypy-boto3-apigatewaymanagementapi-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-08-01 11:36:08.548956 mypy-boto3-apigatewaymanagementapi-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.540955 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-08-01 11:10:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-08-01 11:10:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-01 11:10:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-01 11:10:27.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.548956 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-08-01 11:36:08.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-01 11:36:08.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:08.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 11:36:08.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:08.548956 mypy-boto3-apigatewaymanagementapi-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-01 11:10:26.000000 mypy-boto3-apigatewaymanagementapi-1.28.16/setup.py
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/LICENSE` & `mypy-boto3-apigatewaymanagementapi-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/PKG-INFO` & `mypy-boto3-apigatewaymanagementapi-1.28.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewaymanagementapi
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 apigatewaymanagementapi type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 apigatewaymanagementapi type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewaymanagementapi)](https://pepy.tech/project/mypy-boto3-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayManagementApi 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
+[boto3.ApiGatewayManagementApi 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
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
 [mypy-boto3-apigatewaymanagementapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/).
 
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
@@ -287,34 +287,35 @@
 )
 
 
 def check_value(value: ApiGatewayManagementApiServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_apigatewaymanagementapi.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_apigatewaymanagementapi.type_defs import (
+    BlobTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetConnectionRequestRequestTypeDef,
     IdentityTypeDef,
     PostToConnectionRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetConnectionResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteConnectionRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/README.md` & `mypy-boto3-apigatewaymanagementapi-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewaymanagementapi)](https://pepy.tech/project/mypy-boto3-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayManagementApi 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
+[boto3.ApiGatewayManagementApi 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
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
 [mypy-boto3-apigatewaymanagementapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/).
 
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
@@ -255,34 +255,35 @@
 )
 
 
 def check_value(value: ApiGatewayManagementApiServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_apigatewaymanagementapi.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_apigatewaymanagementapi.type_defs import (
+    BlobTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetConnectionRequestRequestTypeDef,
     IdentityTypeDef,
     PostToConnectionRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetConnectionResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteConnectionRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/__main__.py` & `mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApiGatewayManagementApi 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ApiGatewayManagementApi 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi\nOther"
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

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/client.py` & `mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,19 @@
     from boto3.session import Session
     from mypy_boto3_apigatewaymanagementapi.client import ApiGatewayManagementApiClient
 
     session = Session()
     client: ApiGatewayManagementApiClient = session.client("apigatewaymanagementapi")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
-from .type_defs import EmptyResponseMetadataTypeDef, GetConnectionResponseTypeDef
+from .type_defs import BlobTypeDef, EmptyResponseMetadataTypeDef, GetConnectionResponseTypeDef
 
 __all__ = ("ApiGatewayManagementApiClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -99,15 +98,15 @@
         Get information about the connection with the provided id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.get_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/client/#get_connection)
         """
 
     def post_to_connection(
-        self, *, Data: Union[str, bytes, IO[Any], StreamingBody], ConnectionId: str
+        self, *, Data: BlobTypeDef, ConnectionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sends the provided data to the specified connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.post_to_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/client/#post_to_connection)
         """
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/client.pyi` & `mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,19 @@
     from boto3.session import Session
     from mypy_boto3_apigatewaymanagementapi.client import ApiGatewayManagementApiClient
 
     session = Session()
     client: ApiGatewayManagementApiClient = session.client("apigatewaymanagementapi")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
-from .type_defs import EmptyResponseMetadataTypeDef, GetConnectionResponseTypeDef
+from .type_defs import BlobTypeDef, EmptyResponseMetadataTypeDef, GetConnectionResponseTypeDef
 
 __all__ = ("ApiGatewayManagementApiClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -90,15 +89,15 @@
         """
         Get information about the connection with the provided id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.get_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/client/#get_connection)
         """
     def post_to_connection(
-        self, *, Data: Union[str, bytes, IO[Any], StreamingBody], ConnectionId: str
+        self, *, Data: BlobTypeDef, ConnectionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sends the provided data to the specified connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.post_to_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/client/#post_to_connection)
         """
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/literals.py` & `mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/literals.pyi` & `mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/type_defs.py` & `mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for apigatewaymanagementapi service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_apigatewaymanagementapi.type_defs import DeleteConnectionRequestRequestTypeDef
+    from mypy_boto3_apigatewaymanagementapi.type_defs import BlobTypeDef
 
-    data: DeleteConnectionRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, Union
 
 from botocore.response import StreamingBody
@@ -20,23 +20,25 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "IdentityTypeDef",
     "PostToConnectionRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetConnectionResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
     },
 )
 
@@ -65,15 +67,15 @@
         "UserAgent": str,
     },
 )
 
 PostToConnectionRequestRequestTypeDef = TypedDict(
     "PostToConnectionRequestRequestTypeDef",
     {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Data": BlobTypeDef,
         "ConnectionId": str,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi/type_defs.pyi` & `mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 Type annotations for apigatewaymanagementapi service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_apigatewaymanagementapi.type_defs import DeleteConnectionRequestRequestTypeDef
+    from mypy_boto3_apigatewaymanagementapi.type_defs import BlobTypeDef
 
-    data: DeleteConnectionRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, Union
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "IdentityTypeDef",
     "PostToConnectionRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetConnectionResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
     },
 )
 
@@ -64,15 +66,15 @@
         "UserAgent": str,
     },
 )
 
 PostToConnectionRequestRequestTypeDef = TypedDict(
     "PostToConnectionRequestRequestTypeDef",
     {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Data": BlobTypeDef,
         "ConnectionId": str,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO` & `mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewaymanagementapi
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 apigatewaymanagementapi type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 apigatewaymanagementapi type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewaymanagementapi)](https://pepy.tech/project/mypy-boto3-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayManagementApi 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
+[boto3.ApiGatewayManagementApi 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
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
 [mypy-boto3-apigatewaymanagementapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/).
 
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
@@ -287,34 +287,35 @@
 )
 
 
 def check_value(value: ApiGatewayManagementApiServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_apigatewaymanagementapi.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_apigatewaymanagementapi.type_defs import (
+    BlobTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetConnectionRequestRequestTypeDef,
     IdentityTypeDef,
     PostToConnectionRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetConnectionResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteConnectionRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt` & `mypy-boto3-apigatewaymanagementapi-1.28.16/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.15.post1/setup.py` & `mypy-boto3-apigatewaymanagementapi-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigatewaymanagementapi",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_apigatewaymanagementapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApiGatewayManagementApi 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ApiGatewayManagementApi 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,17 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords=(
-        "boto3 apigatewaymanagementapi type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="boto3 apigatewaymanagementapi type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_apigatewaymanagementapi": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/"
```

