# Comparing `tmp/mypy-boto3-opsworkscm-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-opsworkscm-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworkscm-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:48 2023, max compression
+gzip compressed data, was "mypy-boto3-opsworkscm-1.28.16.tar", last modified: Tue Aug  1 11:37:29 2023, max compression
```

## Comparing `mypy-boto3-opsworkscm-1.28.15.post1.tar` & `mypy-boto3-opsworkscm-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:48.601319 mypy-boto3-opsworkscm-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-07-29 10:03:48.601319 mypy-boto3-opsworkscm-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14282 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:48.593319 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-07-29 09:52:41.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-29 09:52:40.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:48.601319 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-07-29 10:03:48.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-29 10:03:48.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:48.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:48.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:48.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:48.000000 mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:48.601319 mypy-boto3-opsworkscm-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:52:39.000000 mypy-boto3-opsworkscm-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:29.000800 mypy-boto3-opsworkscm-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-08-01 11:37:29.000800 mypy-boto3-opsworkscm-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:29.000800 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-08-01 11:25:42.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:29.000800 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-08-01 11:37:28.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 11:37:28.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:28.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:28.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:28.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:37:28.000000 mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:29.000800 mypy-boto3-opsworkscm-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:25:41.000000 mypy-boto3-opsworkscm-1.28.16/setup.py
```

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/LICENSE` & `mypy-boto3-opsworkscm-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/PKG-INFO` & `mypy-boto3-opsworkscm-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworkscm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.OpsWorksCM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.OpsWorksCM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 opsworkscm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 opsworkscm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworkscm)](https://pepy.tech/project/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
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
@@ -350,20 +350,20 @@
 )
 
 
 def check_value(value: BackupStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_opsworkscm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
     ResponseMetadataTypeDef,
     BackupTypeDef,
@@ -409,15 +409,15 @@
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
 
 
-def get_structure() -> AccountAttributeTypeDef:
+def get_value() -> AccountAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/README.md` & `mypy-boto3-opsworkscm-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworkscm)](https://pepy.tech/project/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
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
@@ -318,20 +318,20 @@
 )
 
 
 def check_value(value: BackupStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_opsworkscm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
     ResponseMetadataTypeDef,
     BackupTypeDef,
@@ -377,15 +377,15 @@
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
 
 
-def get_structure() -> AccountAttributeTypeDef:
+def get_value() -> AccountAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/__init__.py` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/__init__.pyi` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/__main__.py` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpsWorksCM 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.OpsWorksCM 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM\nOther"
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

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/client.py` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/client.pyi` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/literals.py` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/literals.pyi` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/paginator.py` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/paginator.pyi` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/type_defs.py` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_opsworkscm.type_defs import AccountAttributeTypeDef
 
-    data: AccountAttributeTypeDef = {...}
+    data: AccountAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/type_defs.pyi` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_opsworkscm.type_defs import AccountAttributeTypeDef
 
-    data: AccountAttributeTypeDef = {...}
+    data: AccountAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/waiter.py` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm/waiter.pyi` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm.egg-info/PKG-INFO` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworkscm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.OpsWorksCM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.OpsWorksCM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 opsworkscm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 opsworkscm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworkscm)](https://pepy.tech/project/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
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
@@ -350,20 +350,20 @@
 )
 
 
 def check_value(value: BackupStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_opsworkscm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
     ResponseMetadataTypeDef,
     BackupTypeDef,
@@ -409,15 +409,15 @@
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
 
 
-def get_structure() -> AccountAttributeTypeDef:
+def get_value() -> AccountAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/mypy_boto3_opsworkscm.egg-info/SOURCES.txt` & `mypy-boto3-opsworkscm-1.28.16/mypy_boto3_opsworkscm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.15.post1/setup.py` & `mypy-boto3-opsworkscm-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworkscm",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_opsworkscm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpsWorksCM 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.OpsWorksCM 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 opsworkscm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 opsworkscm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_opsworkscm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

