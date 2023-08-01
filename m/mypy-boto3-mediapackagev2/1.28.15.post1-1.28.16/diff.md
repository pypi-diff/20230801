# Comparing `tmp/mypy-boto3-mediapackagev2-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-mediapackagev2-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackagev2-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:40 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackagev2-1.28.16.tar", last modified: Tue Aug  1 11:37:20 2023, max compression
```

## Comparing `mypy-boto3-mediapackagev2-1.28.15.post1.tar` & `mypy-boto3-mediapackagev2-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.573284 mypy-boto3-mediapackagev2-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-07-29 10:03:40.573284 mypy-boto3-mediapackagev2-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.573284 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20369 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28402 2023-07-29 09:51:17.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28360 2023-07-29 09:51:17.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.573284 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-07-29 10:03:40.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:03:40.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:40.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:40.000000 mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:40.573284 mypy-boto3-mediapackagev2-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:51:16.000000 mypy-boto3-mediapackagev2-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.576821 mypy-boto3-mediapackagev2-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-08-01 11:37:20.576821 mypy-boto3-mediapackagev2-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.572821 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20293 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20259 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-08-01 11:24:12.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-08-01 11:24:12.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-01 11:24:12.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-08-01 11:24:12.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-08-01 11:24:15.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28458 2023-08-01 11:24:12.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.576821 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-08-01 11:37:20.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:37:20.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:20.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:20.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:20.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:37:20.000000 mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:20.576821 mypy-boto3-mediapackagev2-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:24:11.000000 mypy-boto3-mediapackagev2-1.28.16/setup.py
```

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/LICENSE` & `mypy-boto3-mediapackagev2-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/PKG-INFO` & `mypy-boto3-mediapackagev2-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.mediapackagev2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.mediapackagev2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediapackagev2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediapackagev2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [mypy-boto3-mediapackagev2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/).
 
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
@@ -331,20 +331,20 @@
 )
 
 
 def check_value(value: AdMarkerHlsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediapackagev2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediapackagev2.type_defs import (
     ChannelGroupListConfigurationTypeDef,
     ChannelListConfigurationTypeDef,
     CreateChannelGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -405,19 +405,20 @@
     ListOriginEndpointsResponseTypeDef,
     SegmentOutputTypeDef,
     SegmentTypeDef,
     CreateOriginEndpointResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
+    SegmentUnionTypeDef,
     UpdateOriginEndpointRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ChannelGroupListConfigurationTypeDef:
+def get_value() -> ChannelGroupListConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/README.md` & `mypy-boto3-mediapackagev2-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [mypy-boto3-mediapackagev2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/).
 
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
@@ -299,20 +299,20 @@
 )
 
 
 def check_value(value: AdMarkerHlsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediapackagev2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediapackagev2.type_defs import (
     ChannelGroupListConfigurationTypeDef,
     ChannelListConfigurationTypeDef,
     CreateChannelGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -373,19 +373,20 @@
     ListOriginEndpointsResponseTypeDef,
     SegmentOutputTypeDef,
     SegmentTypeDef,
     CreateOriginEndpointResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
+    SegmentUnionTypeDef,
     UpdateOriginEndpointRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ChannelGroupListConfigurationTypeDef:
+def get_value() -> ChannelGroupListConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/__init__.py` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/__init__.pyi` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/__main__.py` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mediapackagev2 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.mediapackagev2 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2\nOther"
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

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/client.py` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_mediapackagev2.client import mediapackagev2Client
 
     session = Session()
     client: mediapackagev2Client = session.client("mediapackagev2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ContainerTypeType
 from .paginator import (
     ListChannelGroupsPaginator,
     ListChannelsPaginator,
@@ -36,16 +36,15 @@
     GetChannelResponseTypeDef,
     GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    SegmentOutputTypeDef,
-    SegmentTypeDef,
+    SegmentUnionTypeDef,
     UpdateChannelGroupResponseTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -142,15 +141,15 @@
     def create_origin_endpoint(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
-        Segment: Union[SegmentTypeDef, SegmentOutputTypeDef] = ...,
+        Segment: SegmentUnionTypeDef = ...,
         ClientToken: str = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
@@ -385,15 +384,15 @@
     def update_origin_endpoint(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
-        Segment: Union[SegmentTypeDef, SegmentOutputTypeDef] = ...,
+        Segment: SegmentUnionTypeDef = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Update the specified origin endpoint.
```

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/client.pyi` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_mediapackagev2.client import mediapackagev2Client
 
     session = Session()
     client: mediapackagev2Client = session.client("mediapackagev2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ContainerTypeType
 from .paginator import (
     ListChannelGroupsPaginator,
     ListChannelsPaginator,
@@ -36,16 +36,15 @@
     GetChannelResponseTypeDef,
     GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    SegmentOutputTypeDef,
-    SegmentTypeDef,
+    SegmentUnionTypeDef,
     UpdateChannelGroupResponseTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -133,15 +132,15 @@
     def create_origin_endpoint(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
-        Segment: Union[SegmentTypeDef, SegmentOutputTypeDef] = ...,
+        Segment: SegmentUnionTypeDef = ...,
         ClientToken: str = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
@@ -354,15 +353,15 @@
     def update_origin_endpoint(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
-        Segment: Union[SegmentTypeDef, SegmentOutputTypeDef] = ...,
+        Segment: SegmentUnionTypeDef = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Update the specified origin endpoint.
```

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/literals.py` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/literals.pyi` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/paginator.py` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/paginator.pyi` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/type_defs.py` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mediapackagev2.type_defs import ChannelGroupListConfigurationTypeDef
 
-    data: ChannelGroupListConfigurationTypeDef = {...}
+    data: ChannelGroupListConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CmafEncryptionMethodType,
     ContainerTypeType,
     DrmSystemType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ChannelGroupListConfigurationTypeDef",
     "ChannelListConfigurationTypeDef",
     "CreateChannelGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "IngestEndpointTypeDef",
@@ -97,14 +96,15 @@
     "ListOriginEndpointsResponseTypeDef",
     "SegmentOutputTypeDef",
     "SegmentTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
+    "SegmentUnionTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
 )
 
 _RequiredChannelGroupListConfigurationTypeDef = TypedDict(
     "_RequiredChannelGroupListConfigurationTypeDef",
     {
         "ChannelGroupName": str,
@@ -117,21 +117,19 @@
     "_OptionalChannelGroupListConfigurationTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class ChannelGroupListConfigurationTypeDef(
     _RequiredChannelGroupListConfigurationTypeDef, _OptionalChannelGroupListConfigurationTypeDef
 ):
     pass
 
-
 _RequiredChannelListConfigurationTypeDef = TypedDict(
     "_RequiredChannelListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
@@ -142,21 +140,19 @@
     "_OptionalChannelListConfigurationTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class ChannelListConfigurationTypeDef(
     _RequiredChannelListConfigurationTypeDef, _OptionalChannelListConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCreateChannelGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelGroupRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 _OptionalCreateChannelGroupRequestRequestTypeDef = TypedDict(
@@ -165,22 +161,20 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateChannelGroupRequestRequestTypeDef(
     _RequiredCreateChannelGroupRequestRequestTypeDef,
     _OptionalCreateChannelGroupRequestRequestTypeDef,
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
@@ -201,21 +195,19 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
 IngestEndpointTypeDef = TypedDict(
     "IngestEndpointTypeDef",
     {
         "Id": str,
         "Url": str,
     },
     total=False,
@@ -358,21 +350,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChannelsRequestRequestTypeDef(
     _RequiredListChannelsRequestRequestTypeDef, _OptionalListChannelsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredListHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalListHlsManifestConfigurationTypeDef = TypedDict(
@@ -380,21 +370,19 @@
     {
         "ChildManifestName": str,
         "Url": str,
     },
     total=False,
 )
 
-
 class ListHlsManifestConfigurationTypeDef(
     _RequiredListHlsManifestConfigurationTypeDef, _OptionalListHlsManifestConfigurationTypeDef
 ):
     pass
 
-
 _RequiredListLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredListLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalListLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
@@ -402,22 +390,20 @@
     {
         "ChildManifestName": str,
         "Url": str,
     },
     total=False,
 )
 
-
 class ListLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredListLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalListLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -426,22 +412,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListOriginEndpointsRequestRequestTypeDef(
     _RequiredListOriginEndpointsRequestRequestTypeDef,
     _OptionalListOriginEndpointsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -506,22 +490,20 @@
     "_OptionalUpdateChannelGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateChannelGroupRequestRequestTypeDef(
     _RequiredUpdateChannelGroupRequestRequestTypeDef,
     _OptionalUpdateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -529,21 +511,19 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-
 CreateChannelGroupResponseTypeDef = TypedDict(
     "CreateChannelGroupResponseTypeDef",
     {
         "ChannelGroupName": str,
         "Arn": str,
         "EgressDomain": str,
         "CreatedAt": datetime,
@@ -694,21 +674,19 @@
         "ScteHls": ScteHlsTypeDef,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class CreateHlsManifestConfigurationTypeDef(
     _RequiredCreateHlsManifestConfigurationTypeDef, _OptionalCreateHlsManifestConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredCreateLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
@@ -718,22 +696,20 @@
         "ScteHls": ScteHlsTypeDef,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class CreateLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredGetHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
@@ -744,21 +720,19 @@
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
         "ScteHls": ScteHlsTypeDef,
     },
     total=False,
 )
 
-
 class GetHlsManifestConfigurationTypeDef(
     _RequiredGetHlsManifestConfigurationTypeDef, _OptionalGetHlsManifestConfigurationTypeDef
 ):
     pass
 
-
 _RequiredGetLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
@@ -769,22 +743,20 @@
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
         "ScteHls": ScteHlsTypeDef,
     },
     total=False,
 )
 
-
 class GetLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredGetLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalGetLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
-
 SpekeKeyProviderOutputTypeDef = TypedDict(
     "SpekeKeyProviderOutputTypeDef",
     {
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
         "ResourceId": str,
         "DrmSystems": List[DrmSystemType],
         "RoleArn": str,
@@ -821,22 +793,20 @@
     "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListChannelsRequestListChannelsPaginateTypeDef(
     _RequiredListChannelsRequestListChannelsPaginateTypeDef,
     _OptionalListChannelsRequestListChannelsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
     "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -844,22 +814,20 @@
     "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
     _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredOriginEndpointListConfigurationTypeDef = TypedDict(
     "_RequiredOriginEndpointListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
@@ -874,21 +842,19 @@
         "ModifiedAt": datetime,
         "HlsManifests": List[ListHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[ListLowLatencyHlsManifestConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class OriginEndpointListConfigurationTypeDef(
     _RequiredOriginEndpointListConfigurationTypeDef, _OptionalOriginEndpointListConfigurationTypeDef
 ):
     pass
 
-
 _RequiredEncryptionOutputTypeDef = TypedDict(
     "_RequiredEncryptionOutputTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
 )
@@ -897,19 +863,17 @@
     {
         "ConstantInitializationVector": str,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
     pass
 
-
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
@@ -918,19 +882,17 @@
     {
         "ConstantInitializationVector": str,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
-
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1043,22 +1005,21 @@
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateOriginEndpointRequestRequestTypeDef(
     _RequiredCreateOriginEndpointRequestRequestTypeDef,
     _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
-
+SegmentUnionTypeDef = Union[SegmentTypeDef, SegmentOutputTypeDef]
 _RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
@@ -1072,13 +1033,12 @@
         "StartoverWindowSeconds": int,
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateOriginEndpointRequestRequestTypeDef(
     _RequiredUpdateOriginEndpointRequestRequestTypeDef,
     _OptionalUpdateOriginEndpointRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2/type_defs.pyi` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mediapackagev2.type_defs import ChannelGroupListConfigurationTypeDef
 
-    data: ChannelGroupListConfigurationTypeDef = {...}
+    data: ChannelGroupListConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CmafEncryptionMethodType,
     ContainerTypeType,
     DrmSystemType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
@@ -30,14 +30,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ChannelGroupListConfigurationTypeDef",
     "ChannelListConfigurationTypeDef",
     "CreateChannelGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "IngestEndpointTypeDef",
@@ -96,14 +97,15 @@
     "ListOriginEndpointsResponseTypeDef",
     "SegmentOutputTypeDef",
     "SegmentTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
+    "SegmentUnionTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
 )
 
 _RequiredChannelGroupListConfigurationTypeDef = TypedDict(
     "_RequiredChannelGroupListConfigurationTypeDef",
     {
         "ChannelGroupName": str,
@@ -116,19 +118,21 @@
     "_OptionalChannelGroupListConfigurationTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class ChannelGroupListConfigurationTypeDef(
     _RequiredChannelGroupListConfigurationTypeDef, _OptionalChannelGroupListConfigurationTypeDef
 ):
     pass
 
+
 _RequiredChannelListConfigurationTypeDef = TypedDict(
     "_RequiredChannelListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
@@ -139,19 +143,21 @@
     "_OptionalChannelListConfigurationTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class ChannelListConfigurationTypeDef(
     _RequiredChannelListConfigurationTypeDef, _OptionalChannelListConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCreateChannelGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelGroupRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 _OptionalCreateChannelGroupRequestRequestTypeDef = TypedDict(
@@ -160,20 +166,22 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateChannelGroupRequestRequestTypeDef(
     _RequiredCreateChannelGroupRequestRequestTypeDef,
     _OptionalCreateChannelGroupRequestRequestTypeDef,
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
@@ -194,19 +202,21 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+
 IngestEndpointTypeDef = TypedDict(
     "IngestEndpointTypeDef",
     {
         "Id": str,
         "Url": str,
     },
     total=False,
@@ -349,19 +359,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChannelsRequestRequestTypeDef(
     _RequiredListChannelsRequestRequestTypeDef, _OptionalListChannelsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredListHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalListHlsManifestConfigurationTypeDef = TypedDict(
@@ -369,19 +381,21 @@
     {
         "ChildManifestName": str,
         "Url": str,
     },
     total=False,
 )
 
+
 class ListHlsManifestConfigurationTypeDef(
     _RequiredListHlsManifestConfigurationTypeDef, _OptionalListHlsManifestConfigurationTypeDef
 ):
     pass
 
+
 _RequiredListLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredListLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalListLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
@@ -389,20 +403,22 @@
     {
         "ChildManifestName": str,
         "Url": str,
     },
     total=False,
 )
 
+
 class ListLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredListLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalListLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -411,20 +427,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListOriginEndpointsRequestRequestTypeDef(
     _RequiredListOriginEndpointsRequestRequestTypeDef,
     _OptionalListOriginEndpointsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -489,20 +507,22 @@
     "_OptionalUpdateChannelGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateChannelGroupRequestRequestTypeDef(
     _RequiredUpdateChannelGroupRequestRequestTypeDef,
     _OptionalUpdateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -510,19 +530,21 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
 CreateChannelGroupResponseTypeDef = TypedDict(
     "CreateChannelGroupResponseTypeDef",
     {
         "ChannelGroupName": str,
         "Arn": str,
         "EgressDomain": str,
         "CreatedAt": datetime,
@@ -673,19 +695,21 @@
         "ScteHls": ScteHlsTypeDef,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class CreateHlsManifestConfigurationTypeDef(
     _RequiredCreateHlsManifestConfigurationTypeDef, _OptionalCreateHlsManifestConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredCreateLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
@@ -695,20 +719,22 @@
         "ScteHls": ScteHlsTypeDef,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class CreateLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredGetHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
@@ -719,19 +745,21 @@
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
         "ScteHls": ScteHlsTypeDef,
     },
     total=False,
 )
 
+
 class GetHlsManifestConfigurationTypeDef(
     _RequiredGetHlsManifestConfigurationTypeDef, _OptionalGetHlsManifestConfigurationTypeDef
 ):
     pass
 
+
 _RequiredGetLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
@@ -742,20 +770,22 @@
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
         "ScteHls": ScteHlsTypeDef,
     },
     total=False,
 )
 
+
 class GetLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredGetLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalGetLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
+
 SpekeKeyProviderOutputTypeDef = TypedDict(
     "SpekeKeyProviderOutputTypeDef",
     {
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
         "ResourceId": str,
         "DrmSystems": List[DrmSystemType],
         "RoleArn": str,
@@ -792,20 +822,22 @@
     "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListChannelsRequestListChannelsPaginateTypeDef(
     _RequiredListChannelsRequestListChannelsPaginateTypeDef,
     _OptionalListChannelsRequestListChannelsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
     "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -813,20 +845,22 @@
     "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
     _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredOriginEndpointListConfigurationTypeDef = TypedDict(
     "_RequiredOriginEndpointListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
@@ -841,19 +875,21 @@
         "ModifiedAt": datetime,
         "HlsManifests": List[ListHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[ListLowLatencyHlsManifestConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class OriginEndpointListConfigurationTypeDef(
     _RequiredOriginEndpointListConfigurationTypeDef, _OptionalOriginEndpointListConfigurationTypeDef
 ):
     pass
 
+
 _RequiredEncryptionOutputTypeDef = TypedDict(
     "_RequiredEncryptionOutputTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
 )
@@ -862,17 +898,19 @@
     {
         "ConstantInitializationVector": str,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
     pass
 
+
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
@@ -881,17 +919,19 @@
     {
         "ConstantInitializationVector": str,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
+
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1004,20 +1044,23 @@
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateOriginEndpointRequestRequestTypeDef(
     _RequiredCreateOriginEndpointRequestRequestTypeDef,
     _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
+
+SegmentUnionTypeDef = Union[SegmentTypeDef, SegmentOutputTypeDef]
 _RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
@@ -1031,12 +1074,13 @@
         "StartoverWindowSeconds": int,
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateOriginEndpointRequestRequestTypeDef(
     _RequiredUpdateOriginEndpointRequestRequestTypeDef,
     _OptionalUpdateOriginEndpointRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2.egg-info/PKG-INFO` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.mediapackagev2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.mediapackagev2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediapackagev2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediapackagev2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [mypy-boto3-mediapackagev2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/).
 
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
@@ -331,20 +331,20 @@
 )
 
 
 def check_value(value: AdMarkerHlsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediapackagev2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediapackagev2.type_defs import (
     ChannelGroupListConfigurationTypeDef,
     ChannelListConfigurationTypeDef,
     CreateChannelGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -405,19 +405,20 @@
     ListOriginEndpointsResponseTypeDef,
     SegmentOutputTypeDef,
     SegmentTypeDef,
     CreateOriginEndpointResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
+    SegmentUnionTypeDef,
     UpdateOriginEndpointRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ChannelGroupListConfigurationTypeDef:
+def get_value() -> ChannelGroupListConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt` & `mypy-boto3-mediapackagev2-1.28.16/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.15.post1/setup.py` & `mypy-boto3-mediapackagev2-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackagev2",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_mediapackagev2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.mediapackagev2 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.mediapackagev2 1.28.16 service generated with"
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
-    keywords="boto3 mediapackagev2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 mediapackagev2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mediapackagev2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

