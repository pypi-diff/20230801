# Comparing `tmp/mypy-boto3-keyspaces-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-keyspaces-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-keyspaces-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:26 2023, max compression
+gzip compressed data, was "mypy-boto3-keyspaces-1.28.16.tar", last modified: Tue Aug  1 11:37:06 2023, max compression
```

## Comparing `mypy-boto3-keyspaces-1.28.15.post1.tar` & `mypy-boto3-keyspaces-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.885216 mypy-boto3-keyspaces-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-29 10:03:26.877216 mypy-boto3-keyspaces-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.869216 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13532 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-29 09:48:47.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-07-29 09:48:47.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.877216 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-29 10:03:26.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:26.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:26.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:26.000000 mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:26.885216 mypy-boto3-keyspaces-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:48:44.000000 mypy-boto3-keyspaces-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.656852 mypy-boto3-keyspaces-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:32.000000 mypy-boto3-keyspaces-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-08-01 11:37:06.656852 mypy-boto3-keyspaces-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-08-01 11:21:32.000000 mypy-boto3-keyspaces-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.640852 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-01 11:21:32.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 11:21:32.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:21:32.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-08-01 11:21:33.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-08-01 11:21:32.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-08-01 11:21:33.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-08-01 11:21:33.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-08-01 11:21:33.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-08-01 11:21:33.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:32.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17414 2023-08-01 11:21:33.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-08-01 11:21:33.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:32.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.656852 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-08-01 11:37:06.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:06.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:06.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:37:06.000000 mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:06.656852 mypy-boto3-keyspaces-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:21:32.000000 mypy-boto3-keyspaces-1.28.16/setup.py
```

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/LICENSE` & `mypy-boto3-keyspaces-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/PKG-INFO` & `mypy-boto3-keyspaces-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Keyspaces 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Keyspaces 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 keyspaces type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 keyspaces type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-keyspaces)](https://pepy.tech/project/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
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
 
 
 def check_value(value: ClientSideTimestampsStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
     ClientSideTimestampsTypeDef,
     ClusteringKeyTypeDef,
@@ -360,39 +360,41 @@
     KeyspaceSummaryTypeDef,
     PaginatorConfigTypeDef,
     ListKeyspacesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PartitionKeyTypeDef,
+    TimestampTypeDef,
     StaticColumnTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateKeyspaceResponseTypeDef,
     CreateTableResponseTypeDef,
     GetKeyspaceResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RestoreTableResponseTypeDef,
     UpdateTableResponseTypeDef,
-    RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
     ListKeyspacesRequestListKeyspacesPaginateTypeDef,
     ListTablesRequestListTablesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTablesResponseTypeDef,
+    RestoreTableRequestRequestTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     GetTableResponseTypeDef,
     CreateTableRequestRequestTypeDef,
+    SchemaDefinitionUnionTypeDef,
 )
 
 
-def get_structure() -> CapacitySpecificationSummaryTypeDef:
+def get_value() -> CapacitySpecificationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/README.md` & `mypy-boto3-keyspaces-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-keyspaces)](https://pepy.tech/project/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
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
 
 
 def check_value(value: ClientSideTimestampsStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
     ClientSideTimestampsTypeDef,
     ClusteringKeyTypeDef,
@@ -328,39 +328,41 @@
     KeyspaceSummaryTypeDef,
     PaginatorConfigTypeDef,
     ListKeyspacesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PartitionKeyTypeDef,
+    TimestampTypeDef,
     StaticColumnTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateKeyspaceResponseTypeDef,
     CreateTableResponseTypeDef,
     GetKeyspaceResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RestoreTableResponseTypeDef,
     UpdateTableResponseTypeDef,
-    RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
     ListKeyspacesRequestListKeyspacesPaginateTypeDef,
     ListTablesRequestListTablesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTablesResponseTypeDef,
+    RestoreTableRequestRequestTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     GetTableResponseTypeDef,
     CreateTableRequestRequestTypeDef,
+    SchemaDefinitionUnionTypeDef,
 )
 
 
-def get_structure() -> CapacitySpecificationSummaryTypeDef:
+def get_value() -> CapacitySpecificationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/__init__.py` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/__init__.pyi` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/__main__.py` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Keyspaces 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Keyspaces 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces\nOther"
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

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/client.py` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_keyspaces.client import KeyspacesClient
 
     session = Session()
     client: KeyspacesClient = session.client("keyspaces")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListKeyspacesPaginator, ListTablesPaginator, ListTagsForResourcePaginator
 from .type_defs import (
     CapacitySpecificationTypeDef,
     ClientSideTimestampsTypeDef,
@@ -32,17 +31,17 @@
     GetTableResponseTypeDef,
     ListKeyspacesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PointInTimeRecoveryTypeDef,
     ReplicationSpecificationTypeDef,
     RestoreTableResponseTypeDef,
-    SchemaDefinitionOutputTypeDef,
-    SchemaDefinitionTypeDef,
+    SchemaDefinitionUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimeToLiveTypeDef,
     UpdateTableResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -118,15 +117,15 @@
         """
 
     def create_table(
         self,
         *,
         keyspaceName: str,
         tableName: str,
-        schemaDefinition: Union[SchemaDefinitionTypeDef, SchemaDefinitionOutputTypeDef],
+        schemaDefinition: SchemaDefinitionUnionTypeDef,
         comment: CommentTypeDef = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
         defaultTimeToLive: int = ...,
         tags: Sequence[TagTypeDef] = ...,
@@ -220,15 +219,15 @@
     def restore_table(
         self,
         *,
         sourceKeyspaceName: str,
         sourceTableName: str,
         targetKeyspaceName: str,
         targetTableName: str,
-        restoreTimestamp: Union[datetime, str] = ...,
+        restoreTimestamp: TimestampTypeDef = ...,
         capacitySpecificationOverride: CapacitySpecificationTypeDef = ...,
         encryptionSpecificationOverride: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecoveryOverride: PointInTimeRecoveryTypeDef = ...,
         tagsOverride: Sequence[TagTypeDef] = ...
     ) -> RestoreTableResponseTypeDef:
         """
         Restores the specified table to the specified point in time within the
```

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/client.pyi` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_keyspaces.client import KeyspacesClient
 
     session = Session()
     client: KeyspacesClient = session.client("keyspaces")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListKeyspacesPaginator, ListTablesPaginator, ListTagsForResourcePaginator
 from .type_defs import (
     CapacitySpecificationTypeDef,
     ClientSideTimestampsTypeDef,
@@ -32,17 +31,17 @@
     GetTableResponseTypeDef,
     ListKeyspacesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PointInTimeRecoveryTypeDef,
     ReplicationSpecificationTypeDef,
     RestoreTableResponseTypeDef,
-    SchemaDefinitionOutputTypeDef,
-    SchemaDefinitionTypeDef,
+    SchemaDefinitionUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimeToLiveTypeDef,
     UpdateTableResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -110,15 +109,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/client/#create_keyspace)
         """
     def create_table(
         self,
         *,
         keyspaceName: str,
         tableName: str,
-        schemaDefinition: Union[SchemaDefinitionTypeDef, SchemaDefinitionOutputTypeDef],
+        schemaDefinition: SchemaDefinitionUnionTypeDef,
         comment: CommentTypeDef = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
         defaultTimeToLive: int = ...,
         tags: Sequence[TagTypeDef] = ...,
@@ -203,15 +202,15 @@
     def restore_table(
         self,
         *,
         sourceKeyspaceName: str,
         sourceTableName: str,
         targetKeyspaceName: str,
         targetTableName: str,
-        restoreTimestamp: Union[datetime, str] = ...,
+        restoreTimestamp: TimestampTypeDef = ...,
         capacitySpecificationOverride: CapacitySpecificationTypeDef = ...,
         encryptionSpecificationOverride: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecoveryOverride: PointInTimeRecoveryTypeDef = ...,
         tagsOverride: Sequence[TagTypeDef] = ...
     ) -> RestoreTableResponseTypeDef:
         """
         Restores the specified table to the specified point in time within the
```

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/literals.py` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/literals.pyi` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/paginator.py` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/paginator.pyi` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/type_defs.py` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_keyspaces.type_defs import CapacitySpecificationSummaryTypeDef
 
-    data: CapacitySpecificationSummaryTypeDef = {...}
+    data: CapacitySpecificationSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -55,35 +55,37 @@
     "KeyspaceSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListKeyspacesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PartitionKeyTypeDef",
+    "TimestampTypeDef",
     "StaticColumnTypeDef",
     "CreateKeyspaceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateKeyspaceResponseTypeDef",
     "CreateTableResponseTypeDef",
     "GetKeyspaceResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RestoreTableResponseTypeDef",
     "UpdateTableResponseTypeDef",
-    "RestoreTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "ListKeyspacesResponseTypeDef",
     "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     "ListTablesRequestListTablesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTablesResponseTypeDef",
+    "RestoreTableRequestRequestTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "GetTableResponseTypeDef",
     "CreateTableRequestRequestTypeDef",
+    "SchemaDefinitionUnionTypeDef",
 )
 
 _RequiredCapacitySpecificationSummaryTypeDef = TypedDict(
     "_RequiredCapacitySpecificationSummaryTypeDef",
     {
         "throughputMode": ThroughputModeType,
     },
@@ -380,14 +382,15 @@
 PartitionKeyTypeDef = TypedDict(
     "PartitionKeyTypeDef",
     {
         "name": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 StaticColumnTypeDef = TypedDict(
     "StaticColumnTypeDef",
     {
         "name": str,
     },
 )
 
@@ -477,42 +480,14 @@
     "UpdateTableResponseTypeDef",
     {
         "resourceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRestoreTableRequestRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableRequestRequestTypeDef",
-    {
-        "sourceKeyspaceName": str,
-        "sourceTableName": str,
-        "targetKeyspaceName": str,
-        "targetTableName": str,
-    },
-)
-_OptionalRestoreTableRequestRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableRequestRequestTypeDef",
-    {
-        "restoreTimestamp": Union[datetime, str],
-        "capacitySpecificationOverride": CapacitySpecificationTypeDef,
-        "encryptionSpecificationOverride": EncryptionSpecificationTypeDef,
-        "pointInTimeRecoveryOverride": PointInTimeRecoveryTypeDef,
-        "tagsOverride": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class RestoreTableRequestRequestTypeDef(
-    _RequiredRestoreTableRequestRequestTypeDef, _OptionalRestoreTableRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
@@ -603,14 +578,42 @@
     {
         "nextToken": str,
         "tables": List[TableSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredRestoreTableRequestRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableRequestRequestTypeDef",
+    {
+        "sourceKeyspaceName": str,
+        "sourceTableName": str,
+        "targetKeyspaceName": str,
+        "targetTableName": str,
+    },
+)
+_OptionalRestoreTableRequestRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableRequestRequestTypeDef",
+    {
+        "restoreTimestamp": TimestampTypeDef,
+        "capacitySpecificationOverride": CapacitySpecificationTypeDef,
+        "encryptionSpecificationOverride": EncryptionSpecificationTypeDef,
+        "pointInTimeRecoveryOverride": PointInTimeRecoveryTypeDef,
+        "tagsOverride": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class RestoreTableRequestRequestTypeDef(
+    _RequiredRestoreTableRequestRequestTypeDef, _OptionalRestoreTableRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredSchemaDefinitionOutputTypeDef = TypedDict(
     "_RequiredSchemaDefinitionOutputTypeDef",
     {
         "allColumns": List[ColumnDefinitionTypeDef],
         "partitionKeys": List[PartitionKeyTypeDef],
     },
 )
@@ -695,7 +698,10 @@
 )
 
 
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
+
+
+SchemaDefinitionUnionTypeDef = Union[SchemaDefinitionTypeDef, SchemaDefinitionOutputTypeDef]
```

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces/type_defs.pyi` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_keyspaces.type_defs import CapacitySpecificationSummaryTypeDef
 
-    data: CapacitySpecificationSummaryTypeDef = {...}
+    data: CapacitySpecificationSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -54,35 +54,37 @@
     "KeyspaceSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListKeyspacesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PartitionKeyTypeDef",
+    "TimestampTypeDef",
     "StaticColumnTypeDef",
     "CreateKeyspaceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateKeyspaceResponseTypeDef",
     "CreateTableResponseTypeDef",
     "GetKeyspaceResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RestoreTableResponseTypeDef",
     "UpdateTableResponseTypeDef",
-    "RestoreTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "ListKeyspacesResponseTypeDef",
     "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     "ListTablesRequestListTablesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTablesResponseTypeDef",
+    "RestoreTableRequestRequestTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "GetTableResponseTypeDef",
     "CreateTableRequestRequestTypeDef",
+    "SchemaDefinitionUnionTypeDef",
 )
 
 _RequiredCapacitySpecificationSummaryTypeDef = TypedDict(
     "_RequiredCapacitySpecificationSummaryTypeDef",
     {
         "throughputMode": ThroughputModeType,
     },
@@ -363,14 +365,15 @@
 PartitionKeyTypeDef = TypedDict(
     "PartitionKeyTypeDef",
     {
         "name": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 StaticColumnTypeDef = TypedDict(
     "StaticColumnTypeDef",
     {
         "name": str,
     },
 )
 
@@ -458,40 +461,14 @@
     "UpdateTableResponseTypeDef",
     {
         "resourceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRestoreTableRequestRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableRequestRequestTypeDef",
-    {
-        "sourceKeyspaceName": str,
-        "sourceTableName": str,
-        "targetKeyspaceName": str,
-        "targetTableName": str,
-    },
-)
-_OptionalRestoreTableRequestRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableRequestRequestTypeDef",
-    {
-        "restoreTimestamp": Union[datetime, str],
-        "capacitySpecificationOverride": CapacitySpecificationTypeDef,
-        "encryptionSpecificationOverride": EncryptionSpecificationTypeDef,
-        "pointInTimeRecoveryOverride": PointInTimeRecoveryTypeDef,
-        "tagsOverride": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class RestoreTableRequestRequestTypeDef(
-    _RequiredRestoreTableRequestRequestTypeDef, _OptionalRestoreTableRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
@@ -576,14 +553,40 @@
     {
         "nextToken": str,
         "tables": List[TableSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredRestoreTableRequestRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableRequestRequestTypeDef",
+    {
+        "sourceKeyspaceName": str,
+        "sourceTableName": str,
+        "targetKeyspaceName": str,
+        "targetTableName": str,
+    },
+)
+_OptionalRestoreTableRequestRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableRequestRequestTypeDef",
+    {
+        "restoreTimestamp": TimestampTypeDef,
+        "capacitySpecificationOverride": CapacitySpecificationTypeDef,
+        "encryptionSpecificationOverride": EncryptionSpecificationTypeDef,
+        "pointInTimeRecoveryOverride": PointInTimeRecoveryTypeDef,
+        "tagsOverride": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class RestoreTableRequestRequestTypeDef(
+    _RequiredRestoreTableRequestRequestTypeDef, _OptionalRestoreTableRequestRequestTypeDef
+):
+    pass
+
 _RequiredSchemaDefinitionOutputTypeDef = TypedDict(
     "_RequiredSchemaDefinitionOutputTypeDef",
     {
         "allColumns": List[ColumnDefinitionTypeDef],
         "partitionKeys": List[PartitionKeyTypeDef],
     },
 )
@@ -663,7 +666,9 @@
     total=False,
 )
 
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
+
+SchemaDefinitionUnionTypeDef = Union[SchemaDefinitionTypeDef, SchemaDefinitionOutputTypeDef]
```

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces.egg-info/PKG-INFO` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Keyspaces 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Keyspaces 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 keyspaces type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 keyspaces type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-keyspaces)](https://pepy.tech/project/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
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
 
 
 def check_value(value: ClientSideTimestampsStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
     ClientSideTimestampsTypeDef,
     ClusteringKeyTypeDef,
@@ -360,39 +360,41 @@
     KeyspaceSummaryTypeDef,
     PaginatorConfigTypeDef,
     ListKeyspacesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PartitionKeyTypeDef,
+    TimestampTypeDef,
     StaticColumnTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateKeyspaceResponseTypeDef,
     CreateTableResponseTypeDef,
     GetKeyspaceResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RestoreTableResponseTypeDef,
     UpdateTableResponseTypeDef,
-    RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
     ListKeyspacesRequestListKeyspacesPaginateTypeDef,
     ListTablesRequestListTablesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTablesResponseTypeDef,
+    RestoreTableRequestRequestTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     GetTableResponseTypeDef,
     CreateTableRequestRequestTypeDef,
+    SchemaDefinitionUnionTypeDef,
 )
 
 
-def get_structure() -> CapacitySpecificationSummaryTypeDef:
+def get_value() -> CapacitySpecificationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/mypy_boto3_keyspaces.egg-info/SOURCES.txt` & `mypy-boto3-keyspaces-1.28.16/mypy_boto3_keyspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.15.post1/setup.py` & `mypy-boto3-keyspaces-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-keyspaces",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_keyspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Keyspaces 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Keyspaces 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 keyspaces type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 keyspaces type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_keyspaces": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

