# Comparing `tmp/mypy-boto3-mediapackage-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-mediapackage-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:39 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-1.28.16.tar", last modified: Tue Aug  1 11:37:19 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-1.28.15.post1.tar` & `mypy-boto3-mediapackage-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:39.189277 mypy-boto3-mediapackage-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-07-29 10:03:39.185277 mypy-boto3-mediapackage-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14559 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:39.181277 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-29 09:51:13.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-29 09:51:13.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30177 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30146 2023-07-29 09:51:13.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:39.185277 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:39.189277 mypy-boto3-mediapackage-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:19.892823 mypy-boto3-mediapackage-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-08-01 11:37:19.888823 mypy-boto3-mediapackage-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:19.880823 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30501 2023-08-01 11:24:09.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30470 2023-08-01 11:24:09.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:08.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:19.888823 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:19.892823 mypy-boto3-mediapackage-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:24:07.000000 mypy-boto3-mediapackage-1.28.16/setup.py
```

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/LICENSE` & `mypy-boto3-mediapackage-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/PKG-INFO` & `mypy-boto3-mediapackage-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaPackage 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediapackage type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediapackage type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage)](https://pepy.tech/project/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
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
@@ -336,20 +336,20 @@
 )
 
 
 def check_value(value: AdMarkersType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediapackage.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage.type_defs import (
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
     IngressAccessLogsTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
@@ -413,21 +413,24 @@
     HlsPackageTypeDef,
     MssPackageTypeDef,
     ListChannelsResponseTypeDef,
     CreateOriginEndpointResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     OriginEndpointTypeDef,
     UpdateOriginEndpointResponseTypeDef,
+    DashPackageUnionTypeDef,
+    HlsPackageUnionTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
+    MssPackageUnionTypeDef,
     UpdateOriginEndpointRequestRequestTypeDef,
     ListOriginEndpointsResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationTypeDef:
+def get_value() -> AuthorizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/README.md` & `mypy-boto3-mediapackage-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage)](https://pepy.tech/project/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
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
@@ -304,20 +304,20 @@
 )
 
 
 def check_value(value: AdMarkersType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediapackage.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage.type_defs import (
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
     IngressAccessLogsTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
@@ -381,21 +381,24 @@
     HlsPackageTypeDef,
     MssPackageTypeDef,
     ListChannelsResponseTypeDef,
     CreateOriginEndpointResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     OriginEndpointTypeDef,
     UpdateOriginEndpointResponseTypeDef,
+    DashPackageUnionTypeDef,
+    HlsPackageUnionTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
+    MssPackageUnionTypeDef,
     UpdateOriginEndpointRequestRequestTypeDef,
     ListOriginEndpointsResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationTypeDef:
+def get_value() -> AuthorizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__init__.py` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__init__.pyi` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__main__.py` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackage 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MediaPackage 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage\nOther"
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

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/client.py` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,43 +10,40 @@
     from mypy_boto3_mediapackage.client import MediaPackageClient
 
     session = Session()
     client: MediaPackageClient = session.client("mediapackage")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OriginationType
 from .paginator import ListChannelsPaginator, ListHarvestJobsPaginator, ListOriginEndpointsPaginator
 from .type_defs import (
     AuthorizationTypeDef,
     CmafPackageCreateOrUpdateParametersTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateHarvestJobResponseTypeDef,
     CreateOriginEndpointResponseTypeDef,
-    DashPackageOutputTypeDef,
-    DashPackageTypeDef,
+    DashPackageUnionTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
-    HlsPackageOutputTypeDef,
-    HlsPackageTypeDef,
+    HlsPackageUnionTypeDef,
     IngressAccessLogsTypeDef,
     ListChannelsResponseTypeDef,
     ListHarvestJobsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MssPackageOutputTypeDef,
-    MssPackageTypeDef,
+    MssPackageUnionTypeDef,
     RotateChannelCredentialsResponseTypeDef,
     RotateIngestEndpointCredentialsResponseTypeDef,
     S3DestinationTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
 
@@ -155,19 +152,19 @@
     def create_origin_endpoint(
         self,
         *,
         ChannelId: str,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
+        DashPackage: DashPackageUnionTypeDef = ...,
         Description: str = ...,
-        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
+        HlsPackage: HlsPackageUnionTypeDef = ...,
         ManifestName: str = ...,
-        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
+        MssPackage: MssPackageUnionTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         Tags: Mapping[str, str] = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
         """
@@ -326,19 +323,19 @@
 
     def update_origin_endpoint(
         self,
         *,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
+        DashPackage: DashPackageUnionTypeDef = ...,
         Description: str = ...,
-        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
+        HlsPackage: HlsPackageUnionTypeDef = ...,
         ManifestName: str = ...,
-        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
+        MssPackage: MssPackageUnionTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Updates an existing OriginEndpoint.
```

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/client.pyi` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,43 +10,40 @@
     from mypy_boto3_mediapackage.client import MediaPackageClient
 
     session = Session()
     client: MediaPackageClient = session.client("mediapackage")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OriginationType
 from .paginator import ListChannelsPaginator, ListHarvestJobsPaginator, ListOriginEndpointsPaginator
 from .type_defs import (
     AuthorizationTypeDef,
     CmafPackageCreateOrUpdateParametersTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateHarvestJobResponseTypeDef,
     CreateOriginEndpointResponseTypeDef,
-    DashPackageOutputTypeDef,
-    DashPackageTypeDef,
+    DashPackageUnionTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
-    HlsPackageOutputTypeDef,
-    HlsPackageTypeDef,
+    HlsPackageUnionTypeDef,
     IngressAccessLogsTypeDef,
     ListChannelsResponseTypeDef,
     ListHarvestJobsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MssPackageOutputTypeDef,
-    MssPackageTypeDef,
+    MssPackageUnionTypeDef,
     RotateChannelCredentialsResponseTypeDef,
     RotateIngestEndpointCredentialsResponseTypeDef,
     S3DestinationTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
 
@@ -145,19 +142,19 @@
     def create_origin_endpoint(
         self,
         *,
         ChannelId: str,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
+        DashPackage: DashPackageUnionTypeDef = ...,
         Description: str = ...,
-        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
+        HlsPackage: HlsPackageUnionTypeDef = ...,
         ManifestName: str = ...,
-        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
+        MssPackage: MssPackageUnionTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         Tags: Mapping[str, str] = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
         """
@@ -300,19 +297,19 @@
         """
     def update_origin_endpoint(
         self,
         *,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
+        DashPackage: DashPackageUnionTypeDef = ...,
         Description: str = ...,
-        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
+        HlsPackage: HlsPackageUnionTypeDef = ...,
         ManifestName: str = ...,
-        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
+        MssPackage: MssPackageUnionTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Updates an existing OriginEndpoint.
```

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/literals.py` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/literals.pyi` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/paginator.py` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/paginator.pyi` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/type_defs.py` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mediapackage.type_defs import AuthorizationTypeDef
 
-    data: AuthorizationTypeDef = {...}
+    data: AuthorizationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdMarkersType,
     AdsOnDeliveryRestrictionsType,
     AdTriggersElementType,
     CmafEncryptionMethodType,
     EncryptionMethodType,
@@ -107,15 +107,18 @@
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "DescribeOriginEndpointResponseTypeDef",
     "OriginEndpointTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
+    "DashPackageUnionTypeDef",
+    "HlsPackageUnionTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
+    "MssPackageUnionTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
     "ListOriginEndpointsResponseTypeDef",
 )
 
 AuthorizationTypeDef = TypedDict(
     "AuthorizationTypeDef",
     {
@@ -1069,14 +1072,16 @@
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DashPackageUnionTypeDef = Union[DashPackageTypeDef, DashPackageOutputTypeDef]
+HlsPackageUnionTypeDef = Union[HlsPackageTypeDef, HlsPackageOutputTypeDef]
 _RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelId": str,
         "Id": str,
     },
 )
@@ -1103,14 +1108,15 @@
 class CreateOriginEndpointRequestRequestTypeDef(
     _RequiredCreateOriginEndpointRequestRequestTypeDef,
     _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
 
+MssPackageUnionTypeDef = Union[MssPackageTypeDef, MssPackageOutputTypeDef]
 _RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/type_defs.pyi` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mediapackage.type_defs import AuthorizationTypeDef
 
-    data: AuthorizationTypeDef = {...}
+    data: AuthorizationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdMarkersType,
     AdsOnDeliveryRestrictionsType,
     AdTriggersElementType,
     CmafEncryptionMethodType,
     EncryptionMethodType,
@@ -106,15 +106,18 @@
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "DescribeOriginEndpointResponseTypeDef",
     "OriginEndpointTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
+    "DashPackageUnionTypeDef",
+    "HlsPackageUnionTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
+    "MssPackageUnionTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
     "ListOriginEndpointsResponseTypeDef",
 )
 
 AuthorizationTypeDef = TypedDict(
     "AuthorizationTypeDef",
     {
@@ -1042,14 +1045,16 @@
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DashPackageUnionTypeDef = Union[DashPackageTypeDef, DashPackageOutputTypeDef]
+HlsPackageUnionTypeDef = Union[HlsPackageTypeDef, HlsPackageOutputTypeDef]
 _RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelId": str,
         "Id": str,
     },
 )
@@ -1074,14 +1079,15 @@
 
 class CreateOriginEndpointRequestRequestTypeDef(
     _RequiredCreateOriginEndpointRequestRequestTypeDef,
     _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
+MssPackageUnionTypeDef = Union[MssPackageTypeDef, MssPackageOutputTypeDef]
 _RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaPackage 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediapackage type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediapackage type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage)](https://pepy.tech/project/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
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
@@ -336,20 +336,20 @@
 )
 
 
 def check_value(value: AdMarkersType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediapackage.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage.type_defs import (
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
     IngressAccessLogsTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
@@ -413,21 +413,24 @@
     HlsPackageTypeDef,
     MssPackageTypeDef,
     ListChannelsResponseTypeDef,
     CreateOriginEndpointResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     OriginEndpointTypeDef,
     UpdateOriginEndpointResponseTypeDef,
+    DashPackageUnionTypeDef,
+    HlsPackageUnionTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
+    MssPackageUnionTypeDef,
     UpdateOriginEndpointRequestRequestTypeDef,
     ListOriginEndpointsResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationTypeDef:
+def get_value() -> AuthorizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-1.28.16/mypy_boto3_mediapackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15.post1/setup.py` & `mypy-boto3-mediapackage-1.28.16/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_mediapackage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.MediaPackage 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 mediapackage type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 mediapackage type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mediapackage": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

