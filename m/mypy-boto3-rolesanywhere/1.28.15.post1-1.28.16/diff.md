# Comparing `tmp/mypy-boto3-rolesanywhere-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-rolesanywhere-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rolesanywhere-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:01 2023, max compression
+gzip compressed data, was "mypy-boto3-rolesanywhere-1.28.16.tar", last modified: Tue Aug  1 11:37:41 2023, max compression
```

## Comparing `mypy-boto3-rolesanywhere-1.28.15.post1.tar` & `mypy-boto3-rolesanywhere-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.609366 mypy-boto3-rolesanywhere-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:10.000000 mypy-boto3-rolesanywhere-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14978 2023-07-29 10:04:01.605366 mypy-boto3-rolesanywhere-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-07-29 09:57:10.000000 mypy-boto3-rolesanywhere-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.601366 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-29 09:57:10.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-29 09:57:10.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:57:10.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-07-29 09:57:11.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-07-29 09:57:11.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-29 09:57:11.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-29 09:57:11.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-29 09:57:11.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-29 09:57:11.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:10.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-07-29 09:57:15.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-07-29 09:57:15.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:10.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.601366 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14978 2023-07-29 10:04:01.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-29 10:04:01.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:01.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:04:01.000000 mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:01.609366 mypy-boto3-rolesanywhere-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-29 09:57:10.000000 mypy-boto3-rolesanywhere-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:41.464766 mypy-boto3-rolesanywhere-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:37.000000 mypy-boto3-rolesanywhere-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-08-01 11:37:41.464766 mypy-boto3-rolesanywhere-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-08-01 11:30:37.000000 mypy-boto3-rolesanywhere-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:41.460766 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-01 11:30:37.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-01 11:30:37.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-01 11:30:37.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-08-01 11:30:38.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-08-01 11:30:37.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-01 11:30:38.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-01 11:30:38.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-08-01 11:30:38.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-08-01 11:30:38.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:37.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-08-01 11:30:38.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-08-01 11:30:38.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:37.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:41.464766 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-08-01 11:37:41.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-01 11:37:41.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:41.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:41.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:41.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:37:41.000000 mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:41.464766 mypy-boto3-rolesanywhere-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-01 11:30:37.000000 mypy-boto3-rolesanywhere-1.28.16/setup.py
```

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/LICENSE` & `mypy-boto3-rolesanywhere-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/PKG-INFO` & `mypy-boto3-rolesanywhere-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rolesanywhere type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 rolesanywhere type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
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
@@ -325,23 +325,24 @@
 )
 
 
 def check_value(value: ListCrlsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rolesanywhere.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
+    BlobTypeDef,
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
     ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
@@ -353,16 +354,16 @@
     NotificationSettingKeyTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
+    UpdateCrlRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -383,15 +384,15 @@
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/README.md` & `mypy-boto3-rolesanywhere-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
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
@@ -293,23 +293,24 @@
 )
 
 
 def check_value(value: ListCrlsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rolesanywhere.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
+    BlobTypeDef,
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
     ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
@@ -321,16 +322,16 @@
     NotificationSettingKeyTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
+    UpdateCrlRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -351,15 +352,15 @@
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/__init__.py` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/__init__.pyi` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/__main__.py` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAMRolesAnywhere 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IAMRolesAnywhere 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\nOther"
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

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/client.py` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     from mypy_boto3_rolesanywhere.client import IAMRolesAnywhereClient
 
     session = Session()
     client: IAMRolesAnywhereClient = session.client("rolesanywhere")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     ListCrlsPaginator,
     ListProfilesPaginator,
     ListSubjectsPaginator,
     ListTrustAnchorsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSubjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustAnchorsResponseTypeDef,
     NotificationSettingKeyTypeDef,
@@ -256,15 +256,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.get_trust_anchor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#get_trust_anchor)
         """
 
     def import_crl(
         self,
         *,
-        crlData: Union[str, bytes, IO[Any], StreamingBody],
+        crlData: BlobTypeDef,
         name: str,
         trustAnchorArn: str,
         enabled: bool = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CrlDetailResponseTypeDef:
         """
         Imports the certificate revocation list (CRL).
@@ -357,19 +357,15 @@
         Removes tags from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#untag_resource)
         """
 
     def update_crl(
-        self,
-        *,
-        crlId: str,
-        crlData: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        name: str = ...
+        self, *, crlId: str, crlData: BlobTypeDef = ..., name: str = ...
     ) -> CrlDetailResponseTypeDef:
         """
         Updates the certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_crl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#update_crl)
         """
```

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/client.pyi` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     from mypy_boto3_rolesanywhere.client import IAMRolesAnywhereClient
 
     session = Session()
     client: IAMRolesAnywhereClient = session.client("rolesanywhere")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     ListCrlsPaginator,
     ListProfilesPaginator,
     ListSubjectsPaginator,
     ListTrustAnchorsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSubjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustAnchorsResponseTypeDef,
     NotificationSettingKeyTypeDef,
@@ -233,15 +233,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.get_trust_anchor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#get_trust_anchor)
         """
     def import_crl(
         self,
         *,
-        crlData: Union[str, bytes, IO[Any], StreamingBody],
+        crlData: BlobTypeDef,
         name: str,
         trustAnchorArn: str,
         enabled: bool = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CrlDetailResponseTypeDef:
         """
         Imports the certificate revocation list (CRL).
@@ -324,19 +324,15 @@
         """
         Removes tags from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#untag_resource)
         """
     def update_crl(
-        self,
-        *,
-        crlId: str,
-        crlData: Union[str, bytes, IO[Any], StreamingBody] = ...,
-        name: str = ...
+        self, *, crlId: str, crlData: BlobTypeDef = ..., name: str = ...
     ) -> CrlDetailResponseTypeDef:
         """
         Updates the certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_crl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#update_crl)
         """
```

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/literals.py` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/literals.pyi` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/paginator.py` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/paginator.pyi` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/type_defs.py` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for rolesanywhere service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rolesanywhere.type_defs import TagTypeDef
+    from mypy_boto3_rolesanywhere.type_defs import BlobTypeDef
 
-    data: TagTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -26,14 +26,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
     "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
@@ -45,16 +46,16 @@
     "NotificationSettingKeyTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
+    "UpdateCrlRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -74,14 +75,15 @@
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -303,57 +305,57 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateCrlRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCrlRequestRequestTypeDef",
+_RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProfileRequestRequestTypeDef",
     {
-        "crlId": str,
+        "profileId": str,
     },
 )
-_OptionalUpdateCrlRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCrlRequestRequestTypeDef",
+_OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProfileRequestRequestTypeDef",
     {
-        "crlData": Union[str, bytes, IO[Any], StreamingBody],
+        "durationSeconds": int,
+        "managedPolicyArns": Sequence[str],
         "name": str,
+        "roleArns": Sequence[str],
+        "sessionPolicy": str,
     },
     total=False,
 )
 
 
-class UpdateCrlRequestRequestTypeDef(
-    _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
+class UpdateProfileRequestRequestTypeDef(
+    _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateProfileRequestRequestTypeDef",
+_RequiredUpdateCrlRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCrlRequestRequestTypeDef",
     {
-        "profileId": str,
+        "crlId": str,
     },
 )
-_OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateProfileRequestRequestTypeDef",
+_OptionalUpdateCrlRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCrlRequestRequestTypeDef",
     {
-        "durationSeconds": int,
-        "managedPolicyArns": Sequence[str],
+        "crlData": BlobTypeDef,
         "name": str,
-        "roleArns": Sequence[str],
-        "sessionPolicy": str,
     },
     total=False,
 )
 
 
-class UpdateProfileRequestRequestTypeDef(
-    _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
+class UpdateCrlRequestRequestTypeDef(
+    _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
 ):
     pass
 
 
 _RequiredCreateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileRequestRequestTypeDef",
     {
@@ -380,15 +382,15 @@
 ):
     pass
 
 
 _RequiredImportCrlRequestRequestTypeDef = TypedDict(
     "_RequiredImportCrlRequestRequestTypeDef",
     {
-        "crlData": Union[str, bytes, IO[Any], StreamingBody],
+        "crlData": BlobTypeDef,
         "name": str,
         "trustAnchorArn": str,
     },
 )
 _OptionalImportCrlRequestRequestTypeDef = TypedDict(
     "_OptionalImportCrlRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere/type_defs.pyi` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for rolesanywhere service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rolesanywhere.type_defs import TagTypeDef
+    from mypy_boto3_rolesanywhere.type_defs import BlobTypeDef
 
-    data: TagTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -25,14 +25,15 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
     "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
@@ -44,16 +45,16 @@
     "NotificationSettingKeyTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
+    "UpdateCrlRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -73,14 +74,15 @@
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -296,54 +298,54 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateCrlRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCrlRequestRequestTypeDef",
+_RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProfileRequestRequestTypeDef",
     {
-        "crlId": str,
+        "profileId": str,
     },
 )
-_OptionalUpdateCrlRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCrlRequestRequestTypeDef",
+_OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProfileRequestRequestTypeDef",
     {
-        "crlData": Union[str, bytes, IO[Any], StreamingBody],
+        "durationSeconds": int,
+        "managedPolicyArns": Sequence[str],
         "name": str,
+        "roleArns": Sequence[str],
+        "sessionPolicy": str,
     },
     total=False,
 )
 
-class UpdateCrlRequestRequestTypeDef(
-    _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
+class UpdateProfileRequestRequestTypeDef(
+    _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateProfileRequestRequestTypeDef",
+_RequiredUpdateCrlRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCrlRequestRequestTypeDef",
     {
-        "profileId": str,
+        "crlId": str,
     },
 )
-_OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateProfileRequestRequestTypeDef",
+_OptionalUpdateCrlRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCrlRequestRequestTypeDef",
     {
-        "durationSeconds": int,
-        "managedPolicyArns": Sequence[str],
+        "crlData": BlobTypeDef,
         "name": str,
-        "roleArns": Sequence[str],
-        "sessionPolicy": str,
     },
     total=False,
 )
 
-class UpdateProfileRequestRequestTypeDef(
-    _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
+class UpdateCrlRequestRequestTypeDef(
+    _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
 ):
     pass
 
 _RequiredCreateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileRequestRequestTypeDef",
     {
         "name": str,
@@ -367,15 +369,15 @@
     _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
 ):
     pass
 
 _RequiredImportCrlRequestRequestTypeDef = TypedDict(
     "_RequiredImportCrlRequestRequestTypeDef",
     {
-        "crlData": Union[str, bytes, IO[Any], StreamingBody],
+        "crlData": BlobTypeDef,
         "name": str,
         "trustAnchorArn": str,
     },
 )
 _OptionalImportCrlRequestRequestTypeDef = TypedDict(
     "_OptionalImportCrlRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere.egg-info/PKG-INFO` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rolesanywhere type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 rolesanywhere type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
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
@@ -325,23 +325,24 @@
 )
 
 
 def check_value(value: ListCrlsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rolesanywhere.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
+    BlobTypeDef,
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
     ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
@@ -353,16 +354,16 @@
     NotificationSettingKeyTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
+    UpdateCrlRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -383,15 +384,15 @@
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt` & `mypy-boto3-rolesanywhere-1.28.16/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.15.post1/setup.py` & `mypy-boto3-rolesanywhere-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rolesanywhere",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IAMRolesAnywhere 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.IAMRolesAnywhere 1.28.16 service generated with"
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
-    keywords="boto3 rolesanywhere type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 rolesanywhere type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_rolesanywhere": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

