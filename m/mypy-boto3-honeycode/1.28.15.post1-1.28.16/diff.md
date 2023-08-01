# Comparing `tmp/mypy-boto3-honeycode-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-honeycode-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-honeycode-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:15 2023, max compression
+gzip compressed data, was "mypy-boto3-honeycode-1.28.16.tar", last modified: Tue Aug  1 11:36:56 2023, max compression
```

## Comparing `mypy-boto3-honeycode-1.28.15.post1.tar` & `mypy-boto3-honeycode-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:15.981173 mypy-boto3-honeycode-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-29 10:03:15.981173 mypy-boto3-honeycode-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:15.973173 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-29 09:46:55.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:15.981173 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:15.981173 mypy-boto3-honeycode-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:46:53.000000 mypy-boto3-honeycode-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.048874 mypy-boto3-honeycode-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-08-01 11:36:56.036874 mypy-boto3-honeycode-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.032873 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-08-01 11:19:33.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-08-01 11:19:33.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-08-01 11:19:33.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-08-01 11:19:33.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21390 2023-08-01 11:19:33.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.036874 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-08-01 11:36:55.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:36:55.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:55.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:55.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:55.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:36:55.000000 mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:56.048874 mypy-boto3-honeycode-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:19:32.000000 mypy-boto3-honeycode-1.28.16/setup.py
```

### Comparing `mypy-boto3-honeycode-1.28.15.post1/LICENSE` & `mypy-boto3-honeycode-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15.post1/PKG-INFO` & `mypy-boto3-honeycode-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Honeycode 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 honeycode type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 honeycode type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-honeycode)](https://pepy.tech/project/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
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
@@ -326,20 +326,20 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_honeycode.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_honeycode.type_defs import (
     FailedBatchItemTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
@@ -393,20 +393,21 @@
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
     ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     BatchUpsertTableRowsRequestRequestTypeDef,
     GetScreenDataResultTypeDef,
     TableDataImportJobMetadataTypeDef,
+    ImportOptionsUnionTypeDef,
     StartTableDataImportJobRequestRequestTypeDef,
     DescribeTableDataImportJobResultTypeDef,
 )
 
 
-def get_structure() -> FailedBatchItemTypeDef:
+def get_value() -> FailedBatchItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-honeycode-1.28.15.post1/README.md` & `mypy-boto3-honeycode-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-honeycode)](https://pepy.tech/project/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
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
@@ -294,20 +294,20 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_honeycode.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_honeycode.type_defs import (
     FailedBatchItemTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
@@ -361,20 +361,21 @@
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
     ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     BatchUpsertTableRowsRequestRequestTypeDef,
     GetScreenDataResultTypeDef,
     TableDataImportJobMetadataTypeDef,
+    ImportOptionsUnionTypeDef,
     StartTableDataImportJobRequestRequestTypeDef,
     DescribeTableDataImportJobResultTypeDef,
 )
 
 
-def get_structure() -> FailedBatchItemTypeDef:
+def get_value() -> FailedBatchItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__init__.py` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__init__.pyi` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__main__.py` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Honeycode 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Honeycode 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode\nOther"
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

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/client.py` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_honeycode.client import HoneycodeClient
 
     session = Session()
     client: HoneycodeClient = session.client("honeycode")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListTableColumnsPaginator,
     ListTableRowsPaginator,
     ListTablesPaginator,
@@ -30,16 +30,15 @@
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     DescribeTableDataImportJobResultTypeDef,
     FilterTypeDef,
     GetScreenDataResultTypeDef,
     ImportDataSourceTypeDef,
-    ImportOptionsOutputTypeDef,
-    ImportOptionsTypeDef,
+    ImportOptionsUnionTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsResultTypeDef,
     ListTableRowsResultTypeDef,
     ListTablesResultTypeDef,
     ListTagsForResourceResultTypeDef,
     QueryTableRowsResultTypeDef,
     StartTableDataImportJobResultTypeDef,
@@ -298,15 +297,15 @@
     def start_table_data_import_job(
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
-        importOptions: Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef],
+        importOptions: ImportOptionsUnionTypeDef,
         clientRequestToken: str
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/client/#start_table_data_import_job)
```

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/client.pyi` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_honeycode.client import HoneycodeClient
 
     session = Session()
     client: HoneycodeClient = session.client("honeycode")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListTableColumnsPaginator,
     ListTableRowsPaginator,
     ListTablesPaginator,
@@ -30,16 +30,15 @@
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     DescribeTableDataImportJobResultTypeDef,
     FilterTypeDef,
     GetScreenDataResultTypeDef,
     ImportDataSourceTypeDef,
-    ImportOptionsOutputTypeDef,
-    ImportOptionsTypeDef,
+    ImportOptionsUnionTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsResultTypeDef,
     ListTableRowsResultTypeDef,
     ListTablesResultTypeDef,
     ListTagsForResourceResultTypeDef,
     QueryTableRowsResultTypeDef,
     StartTableDataImportJobResultTypeDef,
@@ -278,15 +277,15 @@
     def start_table_data_import_job(
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
-        importOptions: Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef],
+        importOptions: ImportOptionsUnionTypeDef,
         clientRequestToken: str
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/client/#start_table_data_import_job)
```

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/literals.py` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/literals.pyi` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/paginator.py` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/paginator.pyi` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/type_defs.py` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_honeycode.type_defs import FailedBatchItemTypeDef
 
-    data: FailedBatchItemTypeDef = {...}
+    data: FailedBatchItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ErrorCodeType,
     FormatType,
     ImportDataCharacterEncodingType,
     TableDataImportJobStatusType,
     UpsertActionType,
@@ -88,14 +88,15 @@
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
     "ImportOptionsOutputTypeDef",
     "ImportOptionsTypeDef",
     "BatchUpsertTableRowsRequestRequestTypeDef",
     "GetScreenDataResultTypeDef",
     "TableDataImportJobMetadataTypeDef",
+    "ImportOptionsUnionTypeDef",
     "StartTableDataImportJobRequestRequestTypeDef",
     "DescribeTableDataImportJobResultTypeDef",
 )
 
 FailedBatchItemTypeDef = TypedDict(
     "FailedBatchItemTypeDef",
     {
@@ -853,14 +854,15 @@
         "submitter": ImportJobSubmitterTypeDef,
         "submitTime": datetime,
         "importOptions": ImportOptionsOutputTypeDef,
         "dataSource": ImportDataSourceTypeDef,
     },
 )
 
+ImportOptionsUnionTypeDef = Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef]
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "dataSource": ImportDataSourceTypeDef,
         "dataFormat": Literal["DELIMITED_TEXT"],
         "destinationTableId": str,
```

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/type_defs.pyi` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_honeycode.type_defs import FailedBatchItemTypeDef
 
-    data: FailedBatchItemTypeDef = {...}
+    data: FailedBatchItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ErrorCodeType,
     FormatType,
     ImportDataCharacterEncodingType,
     TableDataImportJobStatusType,
     UpsertActionType,
@@ -87,14 +87,15 @@
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
     "ImportOptionsOutputTypeDef",
     "ImportOptionsTypeDef",
     "BatchUpsertTableRowsRequestRequestTypeDef",
     "GetScreenDataResultTypeDef",
     "TableDataImportJobMetadataTypeDef",
+    "ImportOptionsUnionTypeDef",
     "StartTableDataImportJobRequestRequestTypeDef",
     "DescribeTableDataImportJobResultTypeDef",
 )
 
 FailedBatchItemTypeDef = TypedDict(
     "FailedBatchItemTypeDef",
     {
@@ -818,14 +819,15 @@
         "submitter": ImportJobSubmitterTypeDef,
         "submitTime": datetime,
         "importOptions": ImportOptionsOutputTypeDef,
         "dataSource": ImportDataSourceTypeDef,
     },
 )
 
+ImportOptionsUnionTypeDef = Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef]
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "dataSource": ImportDataSourceTypeDef,
         "dataFormat": Literal["DELIMITED_TEXT"],
         "destinationTableId": str,
```

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/PKG-INFO` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Honeycode 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 honeycode type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 honeycode type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-honeycode)](https://pepy.tech/project/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
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
@@ -326,20 +326,20 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_honeycode.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_honeycode.type_defs import (
     FailedBatchItemTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
@@ -393,20 +393,21 @@
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
     ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     BatchUpsertTableRowsRequestRequestTypeDef,
     GetScreenDataResultTypeDef,
     TableDataImportJobMetadataTypeDef,
+    ImportOptionsUnionTypeDef,
     StartTableDataImportJobRequestRequestTypeDef,
     DescribeTableDataImportJobResultTypeDef,
 )
 
 
-def get_structure() -> FailedBatchItemTypeDef:
+def get_value() -> FailedBatchItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/SOURCES.txt` & `mypy-boto3-honeycode-1.28.16/mypy_boto3_honeycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15.post1/setup.py` & `mypy-boto3-honeycode-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-honeycode",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_honeycode"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Honeycode 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 honeycode type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 honeycode type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_honeycode": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

