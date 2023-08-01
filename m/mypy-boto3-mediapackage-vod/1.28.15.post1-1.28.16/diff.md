# Comparing `tmp/mypy-boto3-mediapackage-vod-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-mediapackage-vod-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-vod-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:40 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-vod-1.28.16.tar", last modified: Tue Aug  1 11:37:20 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1.tar` & `mypy-boto3-mediapackage-vod-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.209282 mypy-boto3-mediapackage-vod-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15978 2023-07-29 10:03:40.205282 mypy-boto3-mediapackage-vod-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.197282 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-29 09:51:15.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-29 09:51:15.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-07-29 09:51:15.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-07-29 09:51:15.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.205282 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15978 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:40.209282 mypy-boto3-mediapackage-vod-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.188822 mypy-boto3-mediapackage-vod-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-08-01 11:37:20.188822 mypy-boto3-mediapackage-vod-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.180822 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-01 11:24:11.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24947 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:10.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.188822 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:37:19.000000 mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:20.188822 mypy-boto3-mediapackage-vod-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-01 11:24:09.000000 mypy-boto3-mediapackage-vod-1.28.16/setup.py
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/LICENSE` & `mypy-boto3-mediapackage-vod-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaPackageVod 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaPackageVod 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediapackage-vod type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediapackage-vod type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage-vod)](https://pepy.tech/project/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
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
@@ -333,20 +333,20 @@
 )
 
 
 def check_value(value: AdMarkersType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediapackage_vod.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
     ResponseMetadataTypeDef,
@@ -404,20 +404,24 @@
     CmafPackageTypeDef,
     DashPackageTypeDef,
     HlsPackageTypeDef,
     MssPackageTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     PackagingConfigurationTypeDef,
+    CmafPackageUnionTypeDef,
+    DashPackageUnionTypeDef,
+    HlsPackageUnionTypeDef,
     CreatePackagingConfigurationRequestRequestTypeDef,
+    MssPackageUnionTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> AssetShallowTypeDef:
+def get_value() -> AssetShallowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/README.md` & `mypy-boto3-mediapackage-vod-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage-vod)](https://pepy.tech/project/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
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
@@ -301,20 +301,20 @@
 )
 
 
 def check_value(value: AdMarkersType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediapackage_vod.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
     ResponseMetadataTypeDef,
@@ -372,20 +372,24 @@
     CmafPackageTypeDef,
     DashPackageTypeDef,
     HlsPackageTypeDef,
     MssPackageTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     PackagingConfigurationTypeDef,
+    CmafPackageUnionTypeDef,
+    DashPackageUnionTypeDef,
+    HlsPackageUnionTypeDef,
     CreatePackagingConfigurationRequestRequestTypeDef,
+    MssPackageUnionTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> AssetShallowTypeDef:
+def get_value() -> AssetShallowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__init__.py` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__init__.pyi` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__main__.py` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackageVod 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MediaPackageVod 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod\nOther"
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

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/client.py` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,46 +10,42 @@
     from mypy_boto3_mediapackage_vod.client import MediaPackageVodClient
 
     session = Session()
     client: MediaPackageVodClient = session.client("mediapackage-vod")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListAssetsPaginator,
     ListPackagingConfigurationsPaginator,
     ListPackagingGroupsPaginator,
 )
 from .type_defs import (
     AuthorizationTypeDef,
-    CmafPackageOutputTypeDef,
-    CmafPackageTypeDef,
+    CmafPackageUnionTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateAssetResponseTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
-    DashPackageOutputTypeDef,
-    DashPackageTypeDef,
+    DashPackageUnionTypeDef,
     DescribeAssetResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
-    HlsPackageOutputTypeDef,
-    HlsPackageTypeDef,
+    HlsPackageUnionTypeDef,
     ListAssetsResponseTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
     ListPackagingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MssPackageOutputTypeDef,
-    MssPackageTypeDef,
+    MssPackageUnionTypeDef,
     UpdatePackagingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -140,18 +136,18 @@
         """
 
     def create_packaging_configuration(
         self,
         *,
         Id: str,
         PackagingGroupId: str,
-        CmafPackage: Union[CmafPackageTypeDef, CmafPackageOutputTypeDef] = ...,
-        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
-        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
-        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
+        CmafPackage: CmafPackageUnionTypeDef = ...,
+        DashPackage: DashPackageUnionTypeDef = ...,
+        HlsPackage: HlsPackageUnionTypeDef = ...,
+        MssPackage: MssPackageUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePackagingConfigurationResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/client/#create_packaging_configuration)
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/client.pyi` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,46 +10,42 @@
     from mypy_boto3_mediapackage_vod.client import MediaPackageVodClient
 
     session = Session()
     client: MediaPackageVodClient = session.client("mediapackage-vod")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListAssetsPaginator,
     ListPackagingConfigurationsPaginator,
     ListPackagingGroupsPaginator,
 )
 from .type_defs import (
     AuthorizationTypeDef,
-    CmafPackageOutputTypeDef,
-    CmafPackageTypeDef,
+    CmafPackageUnionTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateAssetResponseTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
-    DashPackageOutputTypeDef,
-    DashPackageTypeDef,
+    DashPackageUnionTypeDef,
     DescribeAssetResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
-    HlsPackageOutputTypeDef,
-    HlsPackageTypeDef,
+    HlsPackageUnionTypeDef,
     ListAssetsResponseTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
     ListPackagingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MssPackageOutputTypeDef,
-    MssPackageTypeDef,
+    MssPackageUnionTypeDef,
     UpdatePackagingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -131,18 +127,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/client/#create_asset)
         """
     def create_packaging_configuration(
         self,
         *,
         Id: str,
         PackagingGroupId: str,
-        CmafPackage: Union[CmafPackageTypeDef, CmafPackageOutputTypeDef] = ...,
-        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
-        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
-        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
+        CmafPackage: CmafPackageUnionTypeDef = ...,
+        DashPackage: DashPackageUnionTypeDef = ...,
+        HlsPackage: HlsPackageUnionTypeDef = ...,
+        MssPackage: MssPackageUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePackagingConfigurationResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/client/#create_packaging_configuration)
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/literals.py` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/literals.pyi` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/paginator.py` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/paginator.pyi` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/type_defs.py` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mediapackage_vod.type_defs import AssetShallowTypeDef
 
-    data: AssetShallowTypeDef = {...}
+    data: AssetShallowTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdMarkersType,
     EncryptionMethodType,
     ManifestLayoutType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
@@ -95,15 +95,19 @@
     "CmafPackageTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
     "CreatePackagingConfigurationResponseTypeDef",
     "DescribePackagingConfigurationResponseTypeDef",
     "PackagingConfigurationTypeDef",
+    "CmafPackageUnionTypeDef",
+    "DashPackageUnionTypeDef",
+    "HlsPackageUnionTypeDef",
     "CreatePackagingConfigurationRequestRequestTypeDef",
+    "MssPackageUnionTypeDef",
     "ListPackagingConfigurationsResponseTypeDef",
 )
 
 AssetShallowTypeDef = TypedDict(
     "AssetShallowTypeDef",
     {
         "Arn": str,
@@ -944,14 +948,17 @@
         "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+CmafPackageUnionTypeDef = Union[CmafPackageTypeDef, CmafPackageOutputTypeDef]
+DashPackageUnionTypeDef = Union[DashPackageTypeDef, DashPackageOutputTypeDef]
+HlsPackageUnionTypeDef = Union[HlsPackageTypeDef, HlsPackageOutputTypeDef]
 _RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
     {
         "Id": str,
         "PackagingGroupId": str,
     },
 )
@@ -971,14 +978,15 @@
 class CreatePackagingConfigurationRequestRequestTypeDef(
     _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
     _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+MssPackageUnionTypeDef = Union[MssPackageTypeDef, MssPackageOutputTypeDef]
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/type_defs.pyi` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mediapackage_vod.type_defs import AssetShallowTypeDef
 
-    data: AssetShallowTypeDef = {...}
+    data: AssetShallowTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdMarkersType,
     EncryptionMethodType,
     ManifestLayoutType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
@@ -94,15 +94,19 @@
     "CmafPackageTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
     "CreatePackagingConfigurationResponseTypeDef",
     "DescribePackagingConfigurationResponseTypeDef",
     "PackagingConfigurationTypeDef",
+    "CmafPackageUnionTypeDef",
+    "DashPackageUnionTypeDef",
+    "HlsPackageUnionTypeDef",
     "CreatePackagingConfigurationRequestRequestTypeDef",
+    "MssPackageUnionTypeDef",
     "ListPackagingConfigurationsResponseTypeDef",
 )
 
 AssetShallowTypeDef = TypedDict(
     "AssetShallowTypeDef",
     {
         "Arn": str,
@@ -907,14 +911,17 @@
         "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+CmafPackageUnionTypeDef = Union[CmafPackageTypeDef, CmafPackageOutputTypeDef]
+DashPackageUnionTypeDef = Union[DashPackageTypeDef, DashPackageOutputTypeDef]
+HlsPackageUnionTypeDef = Union[HlsPackageTypeDef, HlsPackageOutputTypeDef]
 _RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
     {
         "Id": str,
         "PackagingGroupId": str,
     },
 )
@@ -932,14 +939,15 @@
 
 class CreatePackagingConfigurationRequestRequestTypeDef(
     _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
     _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
 ):
     pass
 
+MssPackageUnionTypeDef = Union[MssPackageTypeDef, MssPackageOutputTypeDef]
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaPackageVod 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaPackageVod 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediapackage-vod type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediapackage-vod type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage-vod)](https://pepy.tech/project/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
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
@@ -333,20 +333,20 @@
 )
 
 
 def check_value(value: AdMarkersType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediapackage_vod.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
     ResponseMetadataTypeDef,
@@ -404,20 +404,24 @@
     CmafPackageTypeDef,
     DashPackageTypeDef,
     HlsPackageTypeDef,
     MssPackageTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     PackagingConfigurationTypeDef,
+    CmafPackageUnionTypeDef,
+    DashPackageUnionTypeDef,
+    HlsPackageUnionTypeDef,
     CreatePackagingConfigurationRequestRequestTypeDef,
+    MssPackageUnionTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> AssetShallowTypeDef:
+def get_value() -> AssetShallowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-vod-1.28.16/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15.post1/setup.py` & `mypy-boto3-mediapackage-vod-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage-vod",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_mediapackage_vod"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaPackageVod 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MediaPackageVod 1.28.16 service generated with"
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
-    keywords="boto3 mediapackage-vod type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 mediapackage-vod type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mediapackage_vod": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

