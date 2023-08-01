# Comparing `tmp/mypy-boto3-amplifybackend-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-amplifybackend-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifybackend-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:27 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifybackend-1.28.16.tar", last modified: Tue Aug  1 11:36:08 2023, max compression
```

## Comparing `mypy-boto3-amplifybackend-1.28.15.post1.tar` & `mypy-boto3-amplifybackend-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.704993 mypy-boto3-amplifybackend-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17588 2023-07-29 10:02:27.700993 mypy-boto3-amplifybackend-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.688993 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-07-29 09:37:42.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-07-29 09:37:42.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-29 09:37:43.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-29 09:37:43.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-29 09:37:42.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-29 09:37:42.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44075 2023-07-29 09:37:44.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44010 2023-07-29 09:37:43.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.696993 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17588 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:27.704993 mypy-boto3-amplifybackend-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.412956 mypy-boto3-amplifybackend-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:11.000000 mypy-boto3-amplifybackend-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-08-01 11:36:08.412956 mypy-boto3-amplifybackend-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-08-01 11:10:11.000000 mypy-boto3-amplifybackend-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.408956 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 11:10:11.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-01 11:10:11.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:10:11.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-08-01 11:10:12.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-08-01 11:10:12.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-08-01 11:10:13.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-08-01 11:10:12.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-01 11:10:12.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-01 11:10:12.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:11.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44442 2023-08-01 11:10:14.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44377 2023-08-01 11:10:13.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:11.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.412956 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-08-01 11:36:08.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:36:08.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:08.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:36:08.000000 mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:08.412956 mypy-boto3-amplifybackend-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:10:11.000000 mypy-boto3-amplifybackend-1.28.16/setup.py
```

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/LICENSE` & `mypy-boto3-amplifybackend-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/PKG-INFO` & `mypy-boto3-amplifybackend-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifybackend
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AmplifyBackend 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AmplifyBackend 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amplifybackend type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 amplifybackend type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifybackend)](https://pepy.tech/project/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
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
@@ -327,20 +327,20 @@
 )
 
 
 def check_value(value: AdditionalConstraintsElementType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amplifybackend.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amplifybackend.type_defs import (
     BackendAPIAppSyncAuthSettingsTypeDef,
     BackendAPIConflictResolutionTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
@@ -429,31 +429,33 @@
     CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
     GetBackendStorageResponseTypeDef,
     CreateBackendStorageRequestRequestTypeDef,
     UpdateBackendStorageRequestRequestTypeDef,
     GetBackendAPIResponseTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CreateBackendAPIRequestRequestTypeDef,
     DeleteBackendAPIRequestRequestTypeDef,
     GetBackendAPIRequestRequestTypeDef,
     UpdateBackendAPIRequestRequestTypeDef,
     CreateBackendAuthUserPoolConfigOutputTypeDef,
     CreateBackendAuthUserPoolConfigTypeDef,
     UpdateBackendAuthUserPoolConfigTypeDef,
     CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     UpdateBackendAuthResourceConfigTypeDef,
     GetBackendAuthResponseTypeDef,
     CreateBackendAuthRequestRequestTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
+def get_value() -> BackendAPIAppSyncAuthSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/README.md` & `mypy-boto3-amplifybackend-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifybackend)](https://pepy.tech/project/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
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
@@ -295,20 +295,20 @@
 )
 
 
 def check_value(value: AdditionalConstraintsElementType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amplifybackend.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amplifybackend.type_defs import (
     BackendAPIAppSyncAuthSettingsTypeDef,
     BackendAPIConflictResolutionTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
@@ -397,31 +397,33 @@
     CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
     GetBackendStorageResponseTypeDef,
     CreateBackendStorageRequestRequestTypeDef,
     UpdateBackendStorageRequestRequestTypeDef,
     GetBackendAPIResponseTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CreateBackendAPIRequestRequestTypeDef,
     DeleteBackendAPIRequestRequestTypeDef,
     GetBackendAPIRequestRequestTypeDef,
     UpdateBackendAPIRequestRequestTypeDef,
     CreateBackendAuthUserPoolConfigOutputTypeDef,
     CreateBackendAuthUserPoolConfigTypeDef,
     UpdateBackendAuthUserPoolConfigTypeDef,
     CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     UpdateBackendAuthResourceConfigTypeDef,
     GetBackendAuthResponseTypeDef,
     CreateBackendAuthRequestRequestTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
+def get_value() -> BackendAPIAppSyncAuthSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__init__.py` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__init__.pyi` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__main__.py` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AmplifyBackend 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AmplifyBackend 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend\nOther"
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

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/client.py` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,26 +10,24 @@
     from mypy_boto3_amplifybackend.client import AmplifyBackendClient
 
     session = Session()
     client: AmplifyBackendClient = session.client("amplifybackend")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListBackendJobsPaginator
 from .type_defs import (
-    BackendAPIResourceConfigOutputTypeDef,
-    BackendAPIResourceConfigTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
-    CreateBackendAuthResourceConfigOutputTypeDef,
-    CreateBackendAuthResourceConfigTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResponseTypeDef,
     CreateTokenResponseTypeDef,
     DeleteBackendAPIResponseTypeDef,
@@ -146,34 +144,30 @@
         """
 
     def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: Union[
-            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-        ],
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef,
         ResourceName: str
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend_api)
         """
 
     def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: Union[
-            CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
-        ],
+        ResourceConfig: CreateBackendAuthResourceConfigUnionTypeDef,
         ResourceName: str
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend_auth)
@@ -225,17 +219,15 @@
 
     def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: Union[
-            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-        ] = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#delete_backend_api)
         """
@@ -309,17 +301,15 @@
 
     def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: Union[
-            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-        ] = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#get_backend_api)
         """
@@ -450,17 +440,15 @@
 
     def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: Union[
-            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-        ] = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#update_backend_api)
         """
```

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/client.pyi` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,24 @@
     from mypy_boto3_amplifybackend.client import AmplifyBackendClient
 
     session = Session()
     client: AmplifyBackendClient = session.client("amplifybackend")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListBackendJobsPaginator
 from .type_defs import (
-    BackendAPIResourceConfigOutputTypeDef,
-    BackendAPIResourceConfigTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
-    CreateBackendAuthResourceConfigOutputTypeDef,
-    CreateBackendAuthResourceConfigTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResponseTypeDef,
     CreateTokenResponseTypeDef,
     DeleteBackendAPIResponseTypeDef,
@@ -137,33 +135,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend)
         """
     def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: Union[
-            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-        ],
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef,
         ResourceName: str
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend_api)
         """
     def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: Union[
-            CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
-        ],
+        ResourceConfig: CreateBackendAuthResourceConfigUnionTypeDef,
         ResourceName: str
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend_auth)
@@ -210,17 +204,15 @@
         """
     def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: Union[
-            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-        ] = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#delete_backend_api)
         """
@@ -287,17 +279,15 @@
         """
     def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: Union[
-            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-        ] = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#get_backend_api)
         """
@@ -416,17 +406,15 @@
         """
     def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: Union[
-            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-        ] = ...
+        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#update_backend_api)
         """
```

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/literals.py` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/literals.pyi` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/paginator.py` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/paginator.pyi` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/type_defs.py` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
 
-    data: BackendAPIAppSyncAuthSettingsTypeDef = {...}
+    data: BackendAPIAppSyncAuthSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdditionalConstraintsElementType,
     AuthenticatedElementType,
     AuthResourcesType,
     DeliveryMethodType,
     MFAModeType,
@@ -131,26 +131,28 @@
     "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
     "GetBackendStorageResponseTypeDef",
     "CreateBackendStorageRequestRequestTypeDef",
     "UpdateBackendStorageRequestRequestTypeDef",
     "GetBackendAPIResponseTypeDef",
+    "BackendAPIResourceConfigUnionTypeDef",
     "CreateBackendAPIRequestRequestTypeDef",
     "DeleteBackendAPIRequestRequestTypeDef",
     "GetBackendAPIRequestRequestTypeDef",
     "UpdateBackendAPIRequestRequestTypeDef",
     "CreateBackendAuthUserPoolConfigOutputTypeDef",
     "CreateBackendAuthUserPoolConfigTypeDef",
     "UpdateBackendAuthUserPoolConfigTypeDef",
     "CreateBackendAuthResourceConfigOutputTypeDef",
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
     "GetBackendAuthResponseTypeDef",
     "CreateBackendAuthRequestRequestTypeDef",
+    "CreateBackendAuthResourceConfigUnionTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
@@ -1426,14 +1428,17 @@
         "Error": str,
         "ResourceConfig": BackendAPIResourceConfigOutputTypeDef,
         "ResourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BackendAPIResourceConfigUnionTypeDef = Union[
+    BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+]
 CreateBackendAPIRequestRequestTypeDef = TypedDict(
     "CreateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
         "ResourceName": str,
@@ -1664,14 +1669,17 @@
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
     },
 )
 
+CreateBackendAuthResourceConfigUnionTypeDef = Union[
+    CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
+]
 UpdateBackendAuthRequestRequestTypeDef = TypedDict(
     "UpdateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
```

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/type_defs.pyi` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
 
-    data: BackendAPIAppSyncAuthSettingsTypeDef = {...}
+    data: BackendAPIAppSyncAuthSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdditionalConstraintsElementType,
     AuthenticatedElementType,
     AuthResourcesType,
     DeliveryMethodType,
     MFAModeType,
@@ -130,26 +130,28 @@
     "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
     "GetBackendStorageResponseTypeDef",
     "CreateBackendStorageRequestRequestTypeDef",
     "UpdateBackendStorageRequestRequestTypeDef",
     "GetBackendAPIResponseTypeDef",
+    "BackendAPIResourceConfigUnionTypeDef",
     "CreateBackendAPIRequestRequestTypeDef",
     "DeleteBackendAPIRequestRequestTypeDef",
     "GetBackendAPIRequestRequestTypeDef",
     "UpdateBackendAPIRequestRequestTypeDef",
     "CreateBackendAuthUserPoolConfigOutputTypeDef",
     "CreateBackendAuthUserPoolConfigTypeDef",
     "UpdateBackendAuthUserPoolConfigTypeDef",
     "CreateBackendAuthResourceConfigOutputTypeDef",
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
     "GetBackendAuthResponseTypeDef",
     "CreateBackendAuthRequestRequestTypeDef",
+    "CreateBackendAuthResourceConfigUnionTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
@@ -1377,14 +1379,17 @@
         "Error": str,
         "ResourceConfig": BackendAPIResourceConfigOutputTypeDef,
         "ResourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BackendAPIResourceConfigUnionTypeDef = Union[
+    BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+]
 CreateBackendAPIRequestRequestTypeDef = TypedDict(
     "CreateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
         "ResourceName": str,
@@ -1599,14 +1604,17 @@
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
     },
 )
 
+CreateBackendAuthResourceConfigUnionTypeDef = Union[
+    CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
+]
 UpdateBackendAuthRequestRequestTypeDef = TypedDict(
     "UpdateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
```

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/PKG-INFO` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifybackend
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AmplifyBackend 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AmplifyBackend 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amplifybackend type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 amplifybackend type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifybackend)](https://pepy.tech/project/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
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
@@ -327,20 +327,20 @@
 )
 
 
 def check_value(value: AdditionalConstraintsElementType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amplifybackend.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amplifybackend.type_defs import (
     BackendAPIAppSyncAuthSettingsTypeDef,
     BackendAPIConflictResolutionTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
@@ -429,31 +429,33 @@
     CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
     GetBackendStorageResponseTypeDef,
     CreateBackendStorageRequestRequestTypeDef,
     UpdateBackendStorageRequestRequestTypeDef,
     GetBackendAPIResponseTypeDef,
+    BackendAPIResourceConfigUnionTypeDef,
     CreateBackendAPIRequestRequestTypeDef,
     DeleteBackendAPIRequestRequestTypeDef,
     GetBackendAPIRequestRequestTypeDef,
     UpdateBackendAPIRequestRequestTypeDef,
     CreateBackendAuthUserPoolConfigOutputTypeDef,
     CreateBackendAuthUserPoolConfigTypeDef,
     UpdateBackendAuthUserPoolConfigTypeDef,
     CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     UpdateBackendAuthResourceConfigTypeDef,
     GetBackendAuthResponseTypeDef,
     CreateBackendAuthRequestRequestTypeDef,
+    CreateBackendAuthResourceConfigUnionTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
+def get_value() -> BackendAPIAppSyncAuthSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/SOURCES.txt` & `mypy-boto3-amplifybackend-1.28.16/mypy_boto3_amplifybackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15.post1/setup.py` & `mypy-boto3-amplifybackend-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifybackend",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_amplifybackend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AmplifyBackend 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.AmplifyBackend 1.28.16 service generated with"
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
-    keywords="boto3 amplifybackend type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 amplifybackend type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_amplifybackend": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

