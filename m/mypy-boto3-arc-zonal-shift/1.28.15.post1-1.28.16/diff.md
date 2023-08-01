# Comparing `tmp/mypy-boto3-arc-zonal-shift-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-arc-zonal-shift-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-arc-zonal-shift-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
+gzip compressed data, was "mypy-boto3-arc-zonal-shift-1.28.16.tar", last modified: Tue Aug  1 11:36:15 2023, max compression
```

## Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1.tar` & `mypy-boto3-arc-zonal-shift-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.433021 mypy-boto3-arc-zonal-shift-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-29 10:02:34.433021 mypy-boto3-arc-zonal-shift-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.429021 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.433021 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-29 10:02:34.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:02:34.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:02:34.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.433021 mypy-boto3-arc-zonal-shift-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-29 09:38:37.000000 mypy-boto3-arc-zonal-shift-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.164945 mypy-boto3-arc-zonal-shift-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:08.000000 mypy-boto3-arc-zonal-shift-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-08-01 11:36:15.164945 mypy-boto3-arc-zonal-shift-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-08-01 11:11:08.000000 mypy-boto3-arc-zonal-shift-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.156945 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-01 11:11:08.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-01 11:11:08.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:11:08.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-08-01 11:11:09.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-01 11:11:08.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-08-01 11:11:09.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-08-01 11:11:09.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-01 11:11:09.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-08-01 11:11:09.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:08.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-08-01 11:11:09.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-08-01 11:11:09.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:08.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.164945 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-08-01 11:36:14.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 11:36:14.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:14.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:14.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:14.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:36:14.000000 mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:15.164945 mypy-boto3-arc-zonal-shift-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-08-01 11:11:08.000000 mypy-boto3-arc-zonal-shift-1.28.16/setup.py
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/LICENSE` & `mypy-boto3-arc-zonal-shift-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/PKG-INFO` & `mypy-boto3-arc-zonal-shift-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-arc-zonal-shift
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ARCZonalShift 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ARCZonalShift 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 arc-zonal-shift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 arc-zonal-shift type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-arc-zonal-shift)](https://pepy.tech/project/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
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
@@ -320,20 +320,20 @@
 )
 
 
 def check_value(value: AppliedStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_arc_zonal_shift.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
@@ -349,15 +349,15 @@
     ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
     ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
+def get_value() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/README.md` & `mypy-boto3-arc-zonal-shift-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-arc-zonal-shift)](https://pepy.tech/project/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
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
@@ -288,20 +288,20 @@
 )
 
 
 def check_value(value: AppliedStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_arc_zonal_shift.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
@@ -317,15 +317,15 @@
     ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
     ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
+def get_value() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/__init__.py` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/__init__.pyi` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/__main__.py` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ARCZonalShift 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ARCZonalShift 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift\nOther"
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

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/client.py` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/client.pyi` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/literals.py` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/literals.pyi` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/paginator.py` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/paginator.pyi` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/type_defs.py` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_arc_zonal_shift.type_defs import CancelZonalShiftRequestRequestTypeDef
 
-    data: CancelZonalShiftRequestRequestTypeDef = {...}
+    data: CancelZonalShiftRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import AppliedStatusType, ZonalShiftStatusType
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift/type_defs.pyi` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_arc_zonal_shift.type_defs import CancelZonalShiftRequestRequestTypeDef
 
-    data: CancelZonalShiftRequestRequestTypeDef = {...}
+    data: CancelZonalShiftRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import AppliedStatusType, ZonalShiftStatusType
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-arc-zonal-shift
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ARCZonalShift 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ARCZonalShift 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 arc-zonal-shift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 arc-zonal-shift type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-arc-zonal-shift)](https://pepy.tech/project/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
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
@@ -320,20 +320,20 @@
 )
 
 
 def check_value(value: AppliedStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_arc_zonal_shift.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
@@ -349,15 +349,15 @@
     ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
     ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
+def get_value() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt` & `mypy-boto3-arc-zonal-shift-1.28.16/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.15.post1/setup.py` & `mypy-boto3-arc-zonal-shift-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-arc-zonal-shift",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_arc_zonal_shift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ARCZonalShift 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.ARCZonalShift 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 arc-zonal-shift type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 arc-zonal-shift type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_arc_zonal_shift": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

