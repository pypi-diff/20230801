# Comparing `tmp/mypy-boto3-marketplace-catalog-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-marketplace-catalog-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-marketplace-catalog-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:37 2023, max compression
+gzip compressed data, was "mypy-boto3-marketplace-catalog-1.28.16.tar", last modified: Tue Aug  1 11:37:17 2023, max compression
```

## Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1.tar` & `mypy-boto3-marketplace-catalog-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.489270 mypy-boto3-marketplace-catalog-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-07-29 10:03:37.489270 mypy-boto3-marketplace-catalog-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.489270 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:34.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.489270 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-07-29 10:03:37.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-29 10:03:37.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:37.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:37.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:37.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 10:03:37.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:37.489270 mypy-boto3-marketplace-catalog-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-29 09:50:33.000000 mypy-boto3-marketplace-catalog-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.244829 mypy-boto3-marketplace-catalog-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-08-01 11:37:17.244829 mypy-boto3-marketplace-catalog-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.228829 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-08-01 11:23:27.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-08-01 11:23:27.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.244829 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-08-01 11:37:16.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-01 11:37:17.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:16.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:16.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:16.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 11:37:16.000000 mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:17.244829 mypy-boto3-marketplace-catalog-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-01 11:23:26.000000 mypy-boto3-marketplace-catalog-1.28.16/setup.py
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/LICENSE` & `mypy-boto3-marketplace-catalog-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MarketplaceCatalog 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MarketplaceCatalog 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 marketplace-catalog type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 marketplace-catalog type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-catalog)](https://pepy.tech/project/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
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
@@ -317,20 +317,20 @@
 )
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_marketplace_catalog.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
@@ -362,15 +362,15 @@
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CancelChangeSetRequestRequestTypeDef:
+def get_value() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/README.md` & `mypy-boto3-marketplace-catalog-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-catalog)](https://pepy.tech/project/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
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
@@ -285,20 +285,20 @@
 )
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_marketplace_catalog.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
@@ -330,15 +330,15 @@
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CancelChangeSetRequestRequestTypeDef:
+def get_value() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/__init__.py` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/__init__.pyi` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/client.py` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/client.pyi` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/literals.py` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/literals.pyi` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/paginator.py` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/paginator.pyi` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/type_defs.py` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_marketplace_catalog.type_defs import CancelChangeSetRequestRequestTypeDef
 
-    data: CancelChangeSetRequestRequestTypeDef = {...}
+    data: CancelChangeSetRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import ChangeStatusType, FailureCodeType, OwnershipTypeType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChangeSetSummaryListItemTypeDef",
     "EntityTypeDef",
     "ErrorDetailTypeDef",
     "TagTypeDef",
@@ -102,19 +101,17 @@
     "_OptionalEntityTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
-
 class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
     pass
 
-
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -294,19 +291,17 @@
     {
         "EntityTags": Sequence[TagTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
-
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -341,22 +336,20 @@
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListChangeSetsRequestListChangeSetsPaginateTypeDef(
     _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef,
     _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListChangeSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestRequestTypeDef",
     {
         "Catalog": str,
     },
 )
 _OptionalListChangeSetsRequestRequestTypeDef = TypedDict(
@@ -366,21 +359,19 @@
         "Sort": SortTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChangeSetsRequestRequestTypeDef(
     _RequiredListChangeSetsRequestRequestTypeDef, _OptionalListChangeSetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
     "_RequiredListEntitiesRequestListEntitiesPaginateTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
 )
@@ -391,22 +382,20 @@
         "Sort": SortTypeDef,
         "OwnershipType": OwnershipTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListEntitiesRequestListEntitiesPaginateTypeDef(
     _RequiredListEntitiesRequestListEntitiesPaginateTypeDef,
     _OptionalListEntitiesRequestListEntitiesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitiesRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
 )
@@ -418,21 +407,19 @@
         "NextToken": str,
         "MaxResults": int,
         "OwnershipType": OwnershipTypeType,
     },
     total=False,
 )
 
-
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
-
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
@@ -458,12 +445,11 @@
         "ChangeSetName": str,
         "ClientRequestToken": str,
         "ChangeSetTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartChangeSetRequestRequestTypeDef(
     _RequiredStartChangeSetRequestRequestTypeDef, _OptionalStartChangeSetRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog/type_defs.pyi` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_marketplace_catalog.type_defs import CancelChangeSetRequestRequestTypeDef
 
-    data: CancelChangeSetRequestRequestTypeDef = {...}
+    data: CancelChangeSetRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import ChangeStatusType, FailureCodeType, OwnershipTypeType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChangeSetSummaryListItemTypeDef",
     "EntityTypeDef",
     "ErrorDetailTypeDef",
     "TagTypeDef",
@@ -101,17 +102,19 @@
     "_OptionalEntityTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
+
 class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
     pass
 
+
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -291,17 +294,19 @@
     {
         "EntityTags": Sequence[TagTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
+
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -336,20 +341,22 @@
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListChangeSetsRequestListChangeSetsPaginateTypeDef(
     _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef,
     _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListChangeSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestRequestTypeDef",
     {
         "Catalog": str,
     },
 )
 _OptionalListChangeSetsRequestRequestTypeDef = TypedDict(
@@ -359,19 +366,21 @@
         "Sort": SortTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChangeSetsRequestRequestTypeDef(
     _RequiredListChangeSetsRequestRequestTypeDef, _OptionalListChangeSetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
     "_RequiredListEntitiesRequestListEntitiesPaginateTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
 )
@@ -382,20 +391,22 @@
         "Sort": SortTypeDef,
         "OwnershipType": OwnershipTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListEntitiesRequestListEntitiesPaginateTypeDef(
     _RequiredListEntitiesRequestListEntitiesPaginateTypeDef,
     _OptionalListEntitiesRequestListEntitiesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitiesRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
 )
@@ -407,19 +418,21 @@
         "NextToken": str,
         "MaxResults": int,
         "OwnershipType": OwnershipTypeType,
     },
     total=False,
 )
 
+
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
+
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
@@ -445,11 +458,12 @@
         "ChangeSetName": str,
         "ClientRequestToken": str,
         "ChangeSetTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartChangeSetRequestRequestTypeDef(
     _RequiredStartChangeSetRequestRequestTypeDef, _OptionalStartChangeSetRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MarketplaceCatalog 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MarketplaceCatalog 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 marketplace-catalog type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 marketplace-catalog type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-catalog)](https://pepy.tech/project/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
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
@@ -317,20 +317,20 @@
 )
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_marketplace_catalog.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
@@ -362,15 +362,15 @@
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CancelChangeSetRequestRequestTypeDef:
+def get_value() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt` & `mypy-boto3-marketplace-catalog-1.28.16/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.15.post1/setup.py` & `mypy-boto3-marketplace-catalog-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-marketplace-catalog",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_marketplace_catalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceCatalog 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MarketplaceCatalog 1.28.16 service generated with"
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
-    keywords="boto3 marketplace-catalog type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 marketplace-catalog type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_marketplace_catalog": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/"
```

