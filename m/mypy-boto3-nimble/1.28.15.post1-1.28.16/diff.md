# Comparing `tmp/mypy-boto3-nimble-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-nimble-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-nimble-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:47 2023, max compression
+gzip compressed data, was "mypy-boto3-nimble-1.28.16.tar", last modified: Tue Aug  1 11:37:27 2023, max compression
```

## Comparing `mypy-boto3-nimble-1.28.15.post1.tar` & `mypy-boto3-nimble-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.389314 mypy-boto3-nimble-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24630 2023-07-29 10:03:47.381314 mypy-boto3-nimble-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23135 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.373314 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44726 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44648 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-29 09:52:17.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71497 2023-07-29 09:52:18.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71378 2023-07-29 09:52:17.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.381314 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24630 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:47.389314 mypy-boto3-nimble-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:27.284804 mypy-boto3-nimble-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:25:13.000000 mypy-boto3-nimble-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-08-01 11:37:27.284804 mypy-boto3-nimble-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23180 2023-08-01 11:25:13.000000 mypy-boto3-nimble-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:27.272804 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-08-01 11:25:13.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44543 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44465 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-08-01 11:25:15.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71685 2023-08-01 11:25:19.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71566 2023-08-01 11:25:15.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:25:13.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-08-01 11:25:14.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:27.284804 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-08-01 11:37:27.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:27.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:27.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:27.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:27.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:37:27.000000 mypy-boto3-nimble-1.28.16/mypy_boto3_nimble.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:27.284804 mypy-boto3-nimble-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-01 11:25:13.000000 mypy-boto3-nimble-1.28.16/setup.py
```

### Comparing `mypy-boto3-nimble-1.28.15.post1/LICENSE` & `mypy-boto3-nimble-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/PKG-INFO` & `mypy-boto3-nimble-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-nimble
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.NimbleStudio 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.NimbleStudio 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 nimble type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 nimble type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-nimble.svg?color=blue)](https://pypi.org/project/mypy-boto3-nimble)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-nimble)](https://pepy.tech/project/mypy-boto3-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NimbleStudio 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[boto3.NimbleStudio 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [mypy-boto3-nimble docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -457,20 +457,20 @@
 )
 
 
 def check_value(value: AutomaticTerminationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_nimble.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_nimble.type_defs import (
     AcceptEulasRequestRequestTypeDef,
     EulaAcceptanceTypeDef,
     ResponseMetadataTypeDef,
     ActiveDirectoryComputerAttributeTypeDef,
@@ -604,14 +604,15 @@
     CreateStreamingImageResponseTypeDef,
     DeleteStreamingImageResponseTypeDef,
     GetStreamingImageResponseTypeDef,
     ListStreamingImagesResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     StudioComponentTypeDef,
     CreateStudioComponentRequestRequestTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     UpdateStudioComponentRequestRequestTypeDef,
     GetLaunchProfileInitializationResponseTypeDef,
     LaunchProfileTypeDef,
     CreateLaunchProfileRequestRequestTypeDef,
     UpdateLaunchProfileRequestRequestTypeDef,
     CreateStudioComponentResponseTypeDef,
     DeleteStudioComponentResponseTypeDef,
@@ -623,15 +624,15 @@
     GetLaunchProfileDetailsResponseTypeDef,
     GetLaunchProfileResponseTypeDef,
     ListLaunchProfilesResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptEulasRequestRequestTypeDef:
+def get_value() -> AcceptEulasRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-nimble-1.28.15.post1/README.md` & `mypy-boto3-nimble-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-nimble.svg?color=blue)](https://pypi.org/project/mypy-boto3-nimble)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-nimble)](https://pepy.tech/project/mypy-boto3-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NimbleStudio 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[boto3.NimbleStudio 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [mypy-boto3-nimble docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -425,20 +425,20 @@
 )
 
 
 def check_value(value: AutomaticTerminationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_nimble.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_nimble.type_defs import (
     AcceptEulasRequestRequestTypeDef,
     EulaAcceptanceTypeDef,
     ResponseMetadataTypeDef,
     ActiveDirectoryComputerAttributeTypeDef,
@@ -572,14 +572,15 @@
     CreateStreamingImageResponseTypeDef,
     DeleteStreamingImageResponseTypeDef,
     GetStreamingImageResponseTypeDef,
     ListStreamingImagesResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     StudioComponentTypeDef,
     CreateStudioComponentRequestRequestTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     UpdateStudioComponentRequestRequestTypeDef,
     GetLaunchProfileInitializationResponseTypeDef,
     LaunchProfileTypeDef,
     CreateLaunchProfileRequestRequestTypeDef,
     UpdateLaunchProfileRequestRequestTypeDef,
     CreateStudioComponentResponseTypeDef,
     DeleteStudioComponentResponseTypeDef,
@@ -591,15 +592,15 @@
     GetLaunchProfileDetailsResponseTypeDef,
     GetLaunchProfileResponseTypeDef,
     ListLaunchProfilesResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptEulasRequestRequestTypeDef:
+def get_value() -> AcceptEulasRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__init__.py` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__init__.pyi` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__main__.py` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.NimbleStudio 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.NimbleStudio 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio\nOther"
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

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/client.py` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_nimble.client import NimbleStudioClient
 
     session = Session()
     client: NimbleStudioClient = session.client("nimble")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     LaunchProfileStateType,
     StreamingInstanceTypeType,
     StudioComponentStateType,
@@ -77,16 +77,15 @@
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
     ScriptParameterKeyValueTypeDef,
     StartStreamingSessionResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
     StreamConfigurationCreateTypeDef,
-    StudioComponentConfigurationOutputTypeDef,
-    StudioComponentConfigurationTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     StudioComponentInitializationScriptTypeDef,
     StudioEncryptionConfigurationTypeDef,
     UpdateLaunchProfileMemberResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
     UpdateStudioResponseTypeDef,
@@ -268,17 +267,15 @@
     def create_studio_component(
         self,
         *,
         name: str,
         studioId: str,
         type: StudioComponentTypeType,
         clientToken: str = ...,
-        configuration: Union[
-            StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
-        ] = ...,
+        configuration: StudioComponentConfigurationUnionTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
@@ -774,17 +771,15 @@
 
     def update_studio_component(
         self,
         *,
         studioComponentId: str,
         studioId: str,
         clientToken: str = ...,
-        configuration: Union[
-            StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
-        ] = ...,
+        configuration: StudioComponentConfigurationUnionTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
```

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/client.pyi` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_nimble.client import NimbleStudioClient
 
     session = Session()
     client: NimbleStudioClient = session.client("nimble")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     LaunchProfileStateType,
     StreamingInstanceTypeType,
     StudioComponentStateType,
@@ -77,16 +77,15 @@
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
     ScriptParameterKeyValueTypeDef,
     StartStreamingSessionResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
     StreamConfigurationCreateTypeDef,
-    StudioComponentConfigurationOutputTypeDef,
-    StudioComponentConfigurationTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     StudioComponentInitializationScriptTypeDef,
     StudioEncryptionConfigurationTypeDef,
     UpdateLaunchProfileMemberResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
     UpdateStudioResponseTypeDef,
@@ -255,17 +254,15 @@
     def create_studio_component(
         self,
         *,
         name: str,
         studioId: str,
         type: StudioComponentTypeType,
         clientToken: str = ...,
-        configuration: Union[
-            StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
-        ] = ...,
+        configuration: StudioComponentConfigurationUnionTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
@@ -718,17 +715,15 @@
         """
     def update_studio_component(
         self,
         *,
         studioComponentId: str,
         studioId: str,
         clientToken: str = ...,
-        configuration: Union[
-            StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
-        ] = ...,
+        configuration: StudioComponentConfigurationUnionTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
```

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/literals.py` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/literals.pyi` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/paginator.py` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/paginator.pyi` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/type_defs.py` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_nimble.type_defs import AcceptEulasRequestRequestTypeDef
 
-    data: AcceptEulasRequestRequestTypeDef = {...}
+    data: AcceptEulasRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AutomaticTerminationModeType,
     LaunchProfilePlatformType,
     LaunchProfileStateType,
     LaunchProfileStatusCodeType,
     LaunchProfileValidationStateType,
@@ -189,14 +189,15 @@
     "CreateStreamingImageResponseTypeDef",
     "DeleteStreamingImageResponseTypeDef",
     "GetStreamingImageResponseTypeDef",
     "ListStreamingImagesResponseTypeDef",
     "UpdateStreamingImageResponseTypeDef",
     "StudioComponentTypeDef",
     "CreateStudioComponentRequestRequestTypeDef",
+    "StudioComponentConfigurationUnionTypeDef",
     "UpdateStudioComponentRequestRequestTypeDef",
     "GetLaunchProfileInitializationResponseTypeDef",
     "LaunchProfileTypeDef",
     "CreateLaunchProfileRequestRequestTypeDef",
     "UpdateLaunchProfileRequestRequestTypeDef",
     "CreateStudioComponentResponseTypeDef",
     "DeleteStudioComponentResponseTypeDef",
@@ -2362,14 +2363,17 @@
 class CreateStudioComponentRequestRequestTypeDef(
     _RequiredCreateStudioComponentRequestRequestTypeDef,
     _OptionalCreateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
 
+StudioComponentConfigurationUnionTypeDef = Union[
+    StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
+]
 _RequiredUpdateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
```

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/type_defs.pyi` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_nimble.type_defs import AcceptEulasRequestRequestTypeDef
 
-    data: AcceptEulasRequestRequestTypeDef = {...}
+    data: AcceptEulasRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AutomaticTerminationModeType,
     LaunchProfilePlatformType,
     LaunchProfileStateType,
     LaunchProfileStatusCodeType,
     LaunchProfileValidationStateType,
@@ -188,14 +188,15 @@
     "CreateStreamingImageResponseTypeDef",
     "DeleteStreamingImageResponseTypeDef",
     "GetStreamingImageResponseTypeDef",
     "ListStreamingImagesResponseTypeDef",
     "UpdateStreamingImageResponseTypeDef",
     "StudioComponentTypeDef",
     "CreateStudioComponentRequestRequestTypeDef",
+    "StudioComponentConfigurationUnionTypeDef",
     "UpdateStudioComponentRequestRequestTypeDef",
     "GetLaunchProfileInitializationResponseTypeDef",
     "LaunchProfileTypeDef",
     "CreateLaunchProfileRequestRequestTypeDef",
     "UpdateLaunchProfileRequestRequestTypeDef",
     "CreateStudioComponentResponseTypeDef",
     "DeleteStudioComponentResponseTypeDef",
@@ -2249,14 +2250,17 @@
 
 class CreateStudioComponentRequestRequestTypeDef(
     _RequiredCreateStudioComponentRequestRequestTypeDef,
     _OptionalCreateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
+StudioComponentConfigurationUnionTypeDef = Union[
+    StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
+]
 _RequiredUpdateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
```

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/waiter.py` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/waiter.pyi` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/PKG-INFO` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-nimble
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.NimbleStudio 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.NimbleStudio 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 nimble type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 nimble type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-nimble.svg?color=blue)](https://pypi.org/project/mypy-boto3-nimble)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-nimble)](https://pepy.tech/project/mypy-boto3-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NimbleStudio 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[boto3.NimbleStudio 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [mypy-boto3-nimble docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -457,20 +457,20 @@
 )
 
 
 def check_value(value: AutomaticTerminationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_nimble.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_nimble.type_defs import (
     AcceptEulasRequestRequestTypeDef,
     EulaAcceptanceTypeDef,
     ResponseMetadataTypeDef,
     ActiveDirectoryComputerAttributeTypeDef,
@@ -604,14 +604,15 @@
     CreateStreamingImageResponseTypeDef,
     DeleteStreamingImageResponseTypeDef,
     GetStreamingImageResponseTypeDef,
     ListStreamingImagesResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     StudioComponentTypeDef,
     CreateStudioComponentRequestRequestTypeDef,
+    StudioComponentConfigurationUnionTypeDef,
     UpdateStudioComponentRequestRequestTypeDef,
     GetLaunchProfileInitializationResponseTypeDef,
     LaunchProfileTypeDef,
     CreateLaunchProfileRequestRequestTypeDef,
     UpdateLaunchProfileRequestRequestTypeDef,
     CreateStudioComponentResponseTypeDef,
     DeleteStudioComponentResponseTypeDef,
@@ -623,15 +624,15 @@
     GetLaunchProfileDetailsResponseTypeDef,
     GetLaunchProfileResponseTypeDef,
     ListLaunchProfilesResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptEulasRequestRequestTypeDef:
+def get_value() -> AcceptEulasRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/SOURCES.txt` & `mypy-boto3-nimble-1.28.16/mypy_boto3_nimble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15.post1/setup.py` & `mypy-boto3-nimble-1.28.16/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-nimble",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_nimble"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.NimbleStudio 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.NimbleStudio 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 nimble type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 nimble type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_nimble": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

