# Comparing `tmp/mypy-boto3-tnb-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-tnb-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-tnb-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:22 2023, max compression
+gzip compressed data, was "mypy-boto3-tnb-1.28.16.tar", last modified: Tue Aug  1 11:38:01 2023, max compression
```

## Comparing `mypy-boto3-tnb-1.28.15.post1.tar` & `mypy-boto3-tnb-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.417444 mypy-boto3-tnb-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-07-29 10:04:22.417444 mypy-boto3-tnb-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.413444 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25296 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-29 10:00:52.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-29 10:00:52.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-29 10:00:52.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34684 2023-07-29 10:00:53.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34653 2023-07-29 10:00:52.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.417444 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-07-29 10:04:22.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:04:22.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:22.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:22.000000 mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:22.417444 mypy-boto3-tnb-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-29 10:00:51.000000 mypy-boto3-tnb-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:01.784695 mypy-boto3-tnb-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:28.000000 mypy-boto3-tnb-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-08-01 11:38:01.780695 mypy-boto3-tnb-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-08-01 11:34:28.000000 mypy-boto3-tnb-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:01.776695 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-01 11:34:28.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-08-01 11:34:28.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 11:34:28.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25055 2023-08-01 11:34:29.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-08-01 11:34:29.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-08-01 11:34:29.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-08-01 11:34:29.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-08-01 11:34:29.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-08-01 11:34:29.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:28.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34571 2023-08-01 11:34:30.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34540 2023-08-01 11:34:29.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:28.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:01.780695 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-08-01 11:38:01.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:38:01.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:01.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:01.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:01.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:38:01.000000 mypy-boto3-tnb-1.28.16/mypy_boto3_tnb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:01.784695 mypy-boto3-tnb-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 11:34:28.000000 mypy-boto3-tnb-1.28.16/setup.py
```

### Comparing `mypy-boto3-tnb-1.28.15.post1/LICENSE` & `mypy-boto3-tnb-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.15.post1/PKG-INFO` & `mypy-boto3-tnb-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-tnb
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.TelcoNetworkBuilder 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.TelcoNetworkBuilder 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 tnb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 tnb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-tnb)](https://pepy.tech/project/mypy-boto3-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TelcoNetworkBuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[boto3.TelcoNetworkBuilder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [mypy-boto3-tnb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/).
 
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
@@ -346,23 +346,24 @@
 )
 
 
 def check_value(value: DescriptorContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_tnb.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_tnb.type_defs import (
+    BlobTypeDef,
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
@@ -394,22 +395,22 @@
     ListSolNetworkInstanceMetadataTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PutSolFunctionPackageContentInputRequestTypeDef,
-    PutSolNetworkPackageContentInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
     UpdateSolNetworkModifyTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
+    PutSolFunctionPackageContentInputRequestTypeDef,
+    PutSolNetworkPackageContentInputRequestTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
     CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetSolFunctionPackageContentOutputTypeDef,
@@ -457,15 +458,15 @@
     GetSolNetworkPackageOutputTypeDef,
     PutSolNetworkPackageContentOutputTypeDef,
     ValidateSolNetworkPackageContentOutputTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
 )
 
 
-def get_structure() -> CancelSolNetworkOperationInputRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-tnb-1.28.15.post1/README.md` & `mypy-boto3-tnb-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-tnb)](https://pepy.tech/project/mypy-boto3-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TelcoNetworkBuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[boto3.TelcoNetworkBuilder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [mypy-boto3-tnb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/).
 
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
@@ -314,23 +314,24 @@
 )
 
 
 def check_value(value: DescriptorContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_tnb.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_tnb.type_defs import (
+    BlobTypeDef,
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
@@ -362,22 +363,22 @@
     ListSolNetworkInstanceMetadataTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PutSolFunctionPackageContentInputRequestTypeDef,
-    PutSolNetworkPackageContentInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
     UpdateSolNetworkModifyTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
+    PutSolFunctionPackageContentInputRequestTypeDef,
+    PutSolNetworkPackageContentInputRequestTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
     CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetSolFunctionPackageContentOutputTypeDef,
@@ -425,15 +426,15 @@
     GetSolNetworkPackageOutputTypeDef,
     PutSolNetworkPackageContentOutputTypeDef,
     ValidateSolNetworkPackageContentOutputTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
 )
 
 
-def get_structure() -> CancelSolNetworkOperationInputRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/__init__.py` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/__init__.pyi` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/client.py` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     from mypy_boto3_tnb.client import TelcoNetworkBuilderClient
 
     session = Session()
     client: TelcoNetworkBuilderClient = session.client("tnb")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import NsdOperationalStateType, OperationalStateType
 from .paginator import (
     ListSolFunctionInstancesPaginator,
     ListSolFunctionPackagesPaginator,
     ListSolNetworkInstancesPaginator,
     ListSolNetworkOperationsPaginator,
     ListSolNetworkPackagesPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
     GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorOutputTypeDef,
@@ -359,33 +359,25 @@
         Lists tags for AWS TNB resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#list_tags_for_resource)
         """
 
     def put_sol_function_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        vnfPkgId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, vnfPkgId: str, contentType: Literal["application/zip"] = ...
     ) -> PutSolFunctionPackageContentOutputTypeDef:
         """
         Uploads the contents of a function package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.put_sol_function_package_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#put_sol_function_package_content)
         """
 
     def put_sol_network_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        nsdInfoId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, nsdInfoId: str, contentType: Literal["application/zip"] = ...
     ) -> PutSolNetworkPackageContentOutputTypeDef:
         """
         Uploads the contents of a network package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.put_sol_network_package_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#put_sol_network_package_content)
         """
@@ -448,33 +440,25 @@
         Updates the operational state of a network package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.update_sol_network_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#update_sol_network_package)
         """
 
     def validate_sol_function_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        vnfPkgId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, vnfPkgId: str, contentType: Literal["application/zip"] = ...
     ) -> ValidateSolFunctionPackageContentOutputTypeDef:
         """
         Validates function package content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.validate_sol_function_package_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#validate_sol_function_package_content)
         """
 
     def validate_sol_network_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        nsdInfoId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, nsdInfoId: str, contentType: Literal["application/zip"] = ...
     ) -> ValidateSolNetworkPackageContentOutputTypeDef:
         """
         Validates network package content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.validate_sol_network_package_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#validate_sol_network_package_content)
         """
```

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/client.pyi` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     from mypy_boto3_tnb.client import TelcoNetworkBuilderClient
 
     session = Session()
     client: TelcoNetworkBuilderClient = session.client("tnb")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import NsdOperationalStateType, OperationalStateType
 from .paginator import (
     ListSolFunctionInstancesPaginator,
     ListSolFunctionPackagesPaginator,
     ListSolNetworkInstancesPaginator,
     ListSolNetworkOperationsPaginator,
     ListSolNetworkPackagesPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
     GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorOutputTypeDef,
@@ -328,32 +328,24 @@
         """
         Lists tags for AWS TNB resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#list_tags_for_resource)
         """
     def put_sol_function_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        vnfPkgId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, vnfPkgId: str, contentType: Literal["application/zip"] = ...
     ) -> PutSolFunctionPackageContentOutputTypeDef:
         """
         Uploads the contents of a function package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.put_sol_function_package_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#put_sol_function_package_content)
         """
     def put_sol_network_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        nsdInfoId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, nsdInfoId: str, contentType: Literal["application/zip"] = ...
     ) -> PutSolNetworkPackageContentOutputTypeDef:
         """
         Uploads the contents of a network package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.put_sol_network_package_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#put_sol_network_package_content)
         """
@@ -409,32 +401,24 @@
         """
         Updates the operational state of a network package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.update_sol_network_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#update_sol_network_package)
         """
     def validate_sol_function_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        vnfPkgId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, vnfPkgId: str, contentType: Literal["application/zip"] = ...
     ) -> ValidateSolFunctionPackageContentOutputTypeDef:
         """
         Validates function package content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.validate_sol_function_package_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#validate_sol_function_package_content)
         """
     def validate_sol_network_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        nsdInfoId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, nsdInfoId: str, contentType: Literal["application/zip"] = ...
     ) -> ValidateSolNetworkPackageContentOutputTypeDef:
         """
         Validates network package content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.validate_sol_network_package_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/client/#validate_sol_network_package_content)
         """
```

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/literals.py` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/literals.pyi` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/paginator.py` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/paginator.pyi` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/type_defs.py` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for tnb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_tnb.type_defs import CancelSolNetworkOperationInputRequestTypeDef
+    from mypy_boto3_tnb.type_defs import BlobTypeDef
 
-    data: CancelSolNetworkOperationInputRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -39,14 +39,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "CancelSolNetworkOperationInputRequestTypeDef",
     "CreateSolFunctionPackageInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateSolNetworkInstanceInputRequestTypeDef",
     "CreateSolNetworkPackageInputRequestTypeDef",
     "DeleteSolFunctionPackageInputRequestTypeDef",
     "DeleteSolNetworkInstanceInputRequestTypeDef",
@@ -78,22 +79,22 @@
     "ListSolNetworkInstanceMetadataTypeDef",
     "ListSolNetworkInstancesInputRequestTypeDef",
     "ListSolNetworkOperationsMetadataTypeDef",
     "ListSolNetworkOperationsInputRequestTypeDef",
     "ListSolNetworkPackageMetadataTypeDef",
     "ListSolNetworkPackagesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PutSolFunctionPackageContentInputRequestTypeDef",
-    "PutSolNetworkPackageContentInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "TerminateSolNetworkInstanceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateSolFunctionPackageInputRequestTypeDef",
     "UpdateSolNetworkModifyTypeDef",
     "UpdateSolNetworkPackageInputRequestTypeDef",
+    "PutSolFunctionPackageContentInputRequestTypeDef",
+    "PutSolNetworkPackageContentInputRequestTypeDef",
     "ValidateSolFunctionPackageContentInputRequestTypeDef",
     "ValidateSolNetworkPackageContentInputRequestTypeDef",
     "CreateSolFunctionPackageOutputTypeDef",
     "CreateSolNetworkInstanceOutputTypeDef",
     "CreateSolNetworkPackageOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetSolFunctionPackageContentOutputTypeDef",
@@ -140,14 +141,15 @@
     "ValidateSolFunctionPackageContentOutputTypeDef",
     "GetSolNetworkPackageOutputTypeDef",
     "PutSolNetworkPackageContentOutputTypeDef",
     "ValidateSolNetworkPackageContentOutputTypeDef",
     "GetSolFunctionInstanceOutputTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSolNetworkOperationInputRequestTypeDef = TypedDict(
     "CancelSolNetworkOperationInputRequestTypeDef",
     {
         "nsLcmOpOccId": str,
     },
 )
 
@@ -497,60 +499,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
-    "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
-    {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
-        "vnfPkgId": str,
-    },
-)
-_OptionalPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
-    "_OptionalPutSolFunctionPackageContentInputRequestTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-    },
-    total=False,
-)
-
-
-class PutSolFunctionPackageContentInputRequestTypeDef(
-    _RequiredPutSolFunctionPackageContentInputRequestTypeDef,
-    _OptionalPutSolFunctionPackageContentInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
-    "_RequiredPutSolNetworkPackageContentInputRequestTypeDef",
-    {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
-        "nsdInfoId": str,
-    },
-)
-_OptionalPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
-    "_OptionalPutSolNetworkPackageContentInputRequestTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-    },
-    total=False,
-)
-
-
-class PutSolNetworkPackageContentInputRequestTypeDef(
-    _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
-    _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
-):
-    pass
-
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -605,18 +561,64 @@
     "UpdateSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
         "nsdOperationalState": NsdOperationalStateType,
     },
 )
 
+_RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
+    "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
+    {
+        "file": BlobTypeDef,
+        "vnfPkgId": str,
+    },
+)
+_OptionalPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
+    "_OptionalPutSolFunctionPackageContentInputRequestTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+    },
+    total=False,
+)
+
+
+class PutSolFunctionPackageContentInputRequestTypeDef(
+    _RequiredPutSolFunctionPackageContentInputRequestTypeDef,
+    _OptionalPutSolFunctionPackageContentInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
+    "_RequiredPutSolNetworkPackageContentInputRequestTypeDef",
+    {
+        "file": BlobTypeDef,
+        "nsdInfoId": str,
+    },
+)
+_OptionalPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
+    "_OptionalPutSolNetworkPackageContentInputRequestTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+    },
+    total=False,
+)
+
+
+class PutSolNetworkPackageContentInputRequestTypeDef(
+    _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
+    _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
+        "file": BlobTypeDef,
         "vnfPkgId": str,
     },
 )
 _OptionalValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_OptionalValidateSolFunctionPackageContentInputRequestTypeDef",
     {
         "contentType": Literal["application/zip"],
@@ -631,15 +633,15 @@
 ):
     pass
 
 
 _RequiredValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredValidateSolNetworkPackageContentInputRequestTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
+        "file": BlobTypeDef,
         "nsdInfoId": str,
     },
 )
 _OptionalValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
     "_OptionalValidateSolNetworkPackageContentInputRequestTypeDef",
     {
         "contentType": Literal["application/zip"],
```

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb/type_defs.pyi` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for tnb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_tnb.type_defs import CancelSolNetworkOperationInputRequestTypeDef
+    from mypy_boto3_tnb.type_defs import BlobTypeDef
 
-    data: CancelSolNetworkOperationInputRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -38,14 +38,15 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "CancelSolNetworkOperationInputRequestTypeDef",
     "CreateSolFunctionPackageInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateSolNetworkInstanceInputRequestTypeDef",
     "CreateSolNetworkPackageInputRequestTypeDef",
     "DeleteSolFunctionPackageInputRequestTypeDef",
     "DeleteSolNetworkInstanceInputRequestTypeDef",
@@ -77,22 +78,22 @@
     "ListSolNetworkInstanceMetadataTypeDef",
     "ListSolNetworkInstancesInputRequestTypeDef",
     "ListSolNetworkOperationsMetadataTypeDef",
     "ListSolNetworkOperationsInputRequestTypeDef",
     "ListSolNetworkPackageMetadataTypeDef",
     "ListSolNetworkPackagesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PutSolFunctionPackageContentInputRequestTypeDef",
-    "PutSolNetworkPackageContentInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "TerminateSolNetworkInstanceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateSolFunctionPackageInputRequestTypeDef",
     "UpdateSolNetworkModifyTypeDef",
     "UpdateSolNetworkPackageInputRequestTypeDef",
+    "PutSolFunctionPackageContentInputRequestTypeDef",
+    "PutSolNetworkPackageContentInputRequestTypeDef",
     "ValidateSolFunctionPackageContentInputRequestTypeDef",
     "ValidateSolNetworkPackageContentInputRequestTypeDef",
     "CreateSolFunctionPackageOutputTypeDef",
     "CreateSolNetworkInstanceOutputTypeDef",
     "CreateSolNetworkPackageOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetSolFunctionPackageContentOutputTypeDef",
@@ -139,14 +140,15 @@
     "ValidateSolFunctionPackageContentOutputTypeDef",
     "GetSolNetworkPackageOutputTypeDef",
     "PutSolNetworkPackageContentOutputTypeDef",
     "ValidateSolNetworkPackageContentOutputTypeDef",
     "GetSolFunctionInstanceOutputTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSolNetworkOperationInputRequestTypeDef = TypedDict(
     "CancelSolNetworkOperationInputRequestTypeDef",
     {
         "nsLcmOpOccId": str,
     },
 )
 
@@ -490,56 +492,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
-    "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
-    {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
-        "vnfPkgId": str,
-    },
-)
-_OptionalPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
-    "_OptionalPutSolFunctionPackageContentInputRequestTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-    },
-    total=False,
-)
-
-class PutSolFunctionPackageContentInputRequestTypeDef(
-    _RequiredPutSolFunctionPackageContentInputRequestTypeDef,
-    _OptionalPutSolFunctionPackageContentInputRequestTypeDef,
-):
-    pass
-
-_RequiredPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
-    "_RequiredPutSolNetworkPackageContentInputRequestTypeDef",
-    {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
-        "nsdInfoId": str,
-    },
-)
-_OptionalPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
-    "_OptionalPutSolNetworkPackageContentInputRequestTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-    },
-    total=False,
-)
-
-class PutSolNetworkPackageContentInputRequestTypeDef(
-    _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
-    _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
-):
-    pass
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -592,18 +552,60 @@
     "UpdateSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
         "nsdOperationalState": NsdOperationalStateType,
     },
 )
 
+_RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
+    "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
+    {
+        "file": BlobTypeDef,
+        "vnfPkgId": str,
+    },
+)
+_OptionalPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
+    "_OptionalPutSolFunctionPackageContentInputRequestTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+    },
+    total=False,
+)
+
+class PutSolFunctionPackageContentInputRequestTypeDef(
+    _RequiredPutSolFunctionPackageContentInputRequestTypeDef,
+    _OptionalPutSolFunctionPackageContentInputRequestTypeDef,
+):
+    pass
+
+_RequiredPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
+    "_RequiredPutSolNetworkPackageContentInputRequestTypeDef",
+    {
+        "file": BlobTypeDef,
+        "nsdInfoId": str,
+    },
+)
+_OptionalPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
+    "_OptionalPutSolNetworkPackageContentInputRequestTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+    },
+    total=False,
+)
+
+class PutSolNetworkPackageContentInputRequestTypeDef(
+    _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
+    _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
+):
+    pass
+
 _RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
+        "file": BlobTypeDef,
         "vnfPkgId": str,
     },
 )
 _OptionalValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_OptionalValidateSolFunctionPackageContentInputRequestTypeDef",
     {
         "contentType": Literal["application/zip"],
@@ -616,15 +618,15 @@
     _OptionalValidateSolFunctionPackageContentInputRequestTypeDef,
 ):
     pass
 
 _RequiredValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredValidateSolNetworkPackageContentInputRequestTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
+        "file": BlobTypeDef,
         "nsdInfoId": str,
     },
 )
 _OptionalValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
     "_OptionalValidateSolNetworkPackageContentInputRequestTypeDef",
     {
         "contentType": Literal["application/zip"],
```

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb.egg-info/PKG-INFO` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-tnb
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.TelcoNetworkBuilder 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.TelcoNetworkBuilder 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 tnb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 tnb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-tnb)](https://pepy.tech/project/mypy-boto3-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TelcoNetworkBuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[boto3.TelcoNetworkBuilder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [mypy-boto3-tnb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/).
 
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
@@ -346,23 +346,24 @@
 )
 
 
 def check_value(value: DescriptorContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_tnb.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_tnb.type_defs import (
+    BlobTypeDef,
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
@@ -394,22 +395,22 @@
     ListSolNetworkInstanceMetadataTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PutSolFunctionPackageContentInputRequestTypeDef,
-    PutSolNetworkPackageContentInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
     UpdateSolNetworkModifyTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
+    PutSolFunctionPackageContentInputRequestTypeDef,
+    PutSolNetworkPackageContentInputRequestTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
     CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetSolFunctionPackageContentOutputTypeDef,
@@ -457,15 +458,15 @@
     GetSolNetworkPackageOutputTypeDef,
     PutSolNetworkPackageContentOutputTypeDef,
     ValidateSolNetworkPackageContentOutputTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
 )
 
 
-def get_structure() -> CancelSolNetworkOperationInputRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-tnb-1.28.15.post1/mypy_boto3_tnb.egg-info/SOURCES.txt` & `mypy-boto3-tnb-1.28.16/mypy_boto3_tnb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.15.post1/setup.py` & `mypy-boto3-tnb-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-tnb",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_tnb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TelcoNetworkBuilder 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.TelcoNetworkBuilder 1.28.16 service generated with"
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
-    keywords="boto3 tnb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 tnb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_tnb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

