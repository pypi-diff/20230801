# Comparing `tmp/mypy-boto3-memorydb-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-memorydb-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-memorydb-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:41 2023, max compression
+gzip compressed data, was "mypy-boto3-memorydb-1.28.16.tar", last modified: Tue Aug  1 11:37:21 2023, max compression
```

## Comparing `mypy-boto3-memorydb-1.28.15.post1.tar` & `mypy-boto3-memorydb-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:41.429287 mypy-boto3-memorydb-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19653 2023-07-29 10:03:41.429287 mypy-boto3-memorydb-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18156 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:41.425287 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41350 2023-07-29 09:51:29.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41315 2023-07-29 09:51:28.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:27.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:41.429287 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19653 2023-07-29 10:03:41.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:41.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:41.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:41.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:41.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:41.000000 mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:41.429287 mypy-boto3-memorydb-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:51:26.000000 mypy-boto3-memorydb-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:21.468819 mypy-boto3-memorydb-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-08-01 11:37:21.456819 mypy-boto3-memorydb-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18177 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:21.448819 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36282 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36225 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-08-01 11:24:24.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-08-01 11:24:24.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-08-01 11:24:24.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41396 2023-08-01 11:24:28.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41361 2023-08-01 11:24:27.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:21.456819 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-08-01 11:37:21.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:37:21.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:21.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:21.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:21.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:37:21.000000 mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:21.468819 mypy-boto3-memorydb-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:24:23.000000 mypy-boto3-memorydb-1.28.16/setup.py
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/LICENSE` & `mypy-boto3-memorydb-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.15.post1/PKG-INFO` & `mypy-boto3-memorydb-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-memorydb
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MemoryDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MemoryDB 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 memorydb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 memorydb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-memorydb)](https://pepy.tech/project/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
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
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
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
@@ -367,20 +367,20 @@
 )
 
 
 def check_value(value: AZStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_memorydb.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_memorydb.type_defs import (
     ACLPendingChangesTypeDef,
     ACLsUpdateStatusTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
@@ -400,15 +400,15 @@
     DeleteSubnetGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeACLsRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeEngineVersionsRequestRequestTypeDef,
     EngineVersionInfoTypeDef,
-    DescribeEventsRequestRequestTypeDef,
+    TimestampTypeDef,
     EventTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
     DescribeParametersRequestRequestTypeDef,
     ParameterTypeDef,
     DescribeReservedNodesOfferingsRequestRequestTypeDef,
     DescribeReservedNodesRequestRequestTypeDef,
     DescribeServiceUpdatesRequestRequestTypeDef,
@@ -452,23 +452,24 @@
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeACLsRequestDescribeACLsPaginateTypeDef,
     DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
     DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
     DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
     DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeEngineVersionsResponseTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeEventsRequestRequestTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     ReservedNodeTypeDef,
@@ -506,15 +507,15 @@
     CopySnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
 )
 
 
-def get_structure() -> ACLPendingChangesTypeDef:
+def get_value() -> ACLPendingChangesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/README.md` & `mypy-boto3-memorydb-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-memorydb)](https://pepy.tech/project/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
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
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
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
@@ -335,20 +335,20 @@
 )
 
 
 def check_value(value: AZStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_memorydb.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_memorydb.type_defs import (
     ACLPendingChangesTypeDef,
     ACLsUpdateStatusTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
@@ -368,15 +368,15 @@
     DeleteSubnetGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeACLsRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeEngineVersionsRequestRequestTypeDef,
     EngineVersionInfoTypeDef,
-    DescribeEventsRequestRequestTypeDef,
+    TimestampTypeDef,
     EventTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
     DescribeParametersRequestRequestTypeDef,
     ParameterTypeDef,
     DescribeReservedNodesOfferingsRequestRequestTypeDef,
     DescribeReservedNodesRequestRequestTypeDef,
     DescribeServiceUpdatesRequestRequestTypeDef,
@@ -420,23 +420,24 @@
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeACLsRequestDescribeACLsPaginateTypeDef,
     DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
     DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
     DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
     DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeEngineVersionsResponseTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeEventsRequestRequestTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     ReservedNodeTypeDef,
@@ -474,15 +475,15 @@
     CopySnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
 )
 
 
-def get_structure() -> ACLPendingChangesTypeDef:
+def get_value() -> ACLPendingChangesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/__init__.py` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/__init__.pyi` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/__main__.py` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MemoryDB 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MemoryDB 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB\nOther"
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

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/client.py` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_memorydb.client import MemoryDBClient
 
     session = Session()
     client: MemoryDBClient = session.client("memorydb")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ServiceUpdateStatusType, SourceTypeType
 from .paginator import (
     DescribeACLsPaginator,
     DescribeClustersPaginator,
@@ -70,14 +69,15 @@
     PurchaseReservedNodesOfferingResponseTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupResponseTypeDef,
     ServiceUpdateRequestTypeDef,
     ShardConfigurationRequestTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UntagResourceResponseTypeDef,
     UpdateACLResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     UpdateSubnetGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
@@ -414,16 +414,16 @@
         """
 
     def describe_events(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeEventsResponseTypeDef:
         """
         Returns events related to clusters, security groups, and parameter groups.
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/client.pyi` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_memorydb.client import MemoryDBClient
 
     session = Session()
     client: MemoryDBClient = session.client("memorydb")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ServiceUpdateStatusType, SourceTypeType
 from .paginator import (
     DescribeACLsPaginator,
     DescribeClustersPaginator,
@@ -70,14 +69,15 @@
     PurchaseReservedNodesOfferingResponseTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupResponseTypeDef,
     ServiceUpdateRequestTypeDef,
     ShardConfigurationRequestTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UntagResourceResponseTypeDef,
     UpdateACLResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     UpdateSubnetGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
@@ -390,16 +390,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#describe_engine_versions)
         """
     def describe_events(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeEventsResponseTypeDef:
         """
         Returns events related to clusters, security groups, and parameter groups.
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/literals.py` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/literals.pyi` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/paginator.py` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,15 @@
     describe_reserved_nodes_offerings_paginator: DescribeReservedNodesOfferingsPaginator = client.get_paginator("describe_reserved_nodes_offerings")
     describe_service_updates_paginator: DescribeServiceUpdatesPaginator = client.get_paginator("describe_service_updates")
     describe_snapshots_paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")
     describe_subnet_groups_paginator: DescribeSubnetGroupsPaginator = client.get_paginator("describe_subnet_groups")
     describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ServiceUpdateStatusType, SourceTypeType
 from .type_defs import (
     DescribeACLsResponseTypeDef,
     DescribeClustersResponseTypeDef,
@@ -58,14 +57,15 @@
     DescribeReservedNodesResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
     DescribeSubnetGroupsResponseTypeDef,
     DescribeUsersResponseTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeACLsPaginator",
     "DescribeClustersPaginator",
     "DescribeEngineVersionsPaginator",
     "DescribeEventsPaginator",
@@ -151,16 +151,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeeventspaginator)
         """
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/paginator.pyi` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,15 @@
     describe_reserved_nodes_offerings_paginator: DescribeReservedNodesOfferingsPaginator = client.get_paginator("describe_reserved_nodes_offerings")
     describe_service_updates_paginator: DescribeServiceUpdatesPaginator = client.get_paginator("describe_service_updates")
     describe_snapshots_paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")
     describe_subnet_groups_paginator: DescribeSubnetGroupsPaginator = client.get_paginator("describe_subnet_groups")
     describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ServiceUpdateStatusType, SourceTypeType
 from .type_defs import (
     DescribeACLsResponseTypeDef,
     DescribeClustersResponseTypeDef,
@@ -58,14 +57,15 @@
     DescribeReservedNodesResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
     DescribeSubnetGroupsResponseTypeDef,
     DescribeUsersResponseTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeACLsPaginator",
     "DescribeClustersPaginator",
     "DescribeEngineVersionsPaginator",
     "DescribeEventsPaginator",
@@ -145,16 +145,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeeventspaginator)
         """
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/type_defs.py` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_memorydb.type_defs import ACLPendingChangesTypeDef
 
-    data: ACLPendingChangesTypeDef = {...}
+    data: ACLPendingChangesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -55,15 +55,15 @@
     "DeleteSubnetGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeACLsRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeEngineVersionsRequestRequestTypeDef",
     "EngineVersionInfoTypeDef",
-    "DescribeEventsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "EventTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "ParameterTypeDef",
     "DescribeReservedNodesOfferingsRequestRequestTypeDef",
     "DescribeReservedNodesRequestRequestTypeDef",
     "DescribeServiceUpdatesRequestRequestTypeDef",
@@ -107,23 +107,24 @@
     "DeleteParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "ResetParameterGroupResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
     "DescribeACLsRequestDescribeACLsPaginateTypeDef",
     "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
     "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
     "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
     "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeEngineVersionsResponseTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeEventsRequestRequestTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "DescribeServiceUpdatesResponseTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "ReservedNodeTypeDef",
@@ -388,28 +389,15 @@
         "EngineVersion": str,
         "EnginePatchVersion": str,
         "ParameterGroupFamily": str,
     },
     total=False,
 )
 
-DescribeEventsRequestRequestTypeDef = TypedDict(
-    "DescribeEventsRequestRequestTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -1101,27 +1089,14 @@
         "ParameterGroupFamily": str,
         "DefaultOnly": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
     "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     {
         "ParameterGroupName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1211,14 +1186,41 @@
     {
         "NextToken": str,
         "EngineVersions": List[EngineVersionInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsRequestRequestTypeDef = TypedDict(
+    "DescribeEventsRequestRequestTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb/type_defs.pyi` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_memorydb.type_defs import ACLPendingChangesTypeDef
 
-    data: ACLPendingChangesTypeDef = {...}
+    data: ACLPendingChangesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -54,15 +54,15 @@
     "DeleteSubnetGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeACLsRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeEngineVersionsRequestRequestTypeDef",
     "EngineVersionInfoTypeDef",
-    "DescribeEventsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "EventTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "ParameterTypeDef",
     "DescribeReservedNodesOfferingsRequestRequestTypeDef",
     "DescribeReservedNodesRequestRequestTypeDef",
     "DescribeServiceUpdatesRequestRequestTypeDef",
@@ -106,23 +106,24 @@
     "DeleteParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "ResetParameterGroupResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
     "DescribeACLsRequestDescribeACLsPaginateTypeDef",
     "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
     "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
     "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
     "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeEngineVersionsResponseTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeEventsRequestRequestTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "DescribeServiceUpdatesResponseTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "ReservedNodeTypeDef",
@@ -385,28 +386,15 @@
         "EngineVersion": str,
         "EnginePatchVersion": str,
         "ParameterGroupFamily": str,
     },
     total=False,
 )
 
-DescribeEventsRequestRequestTypeDef = TypedDict(
-    "DescribeEventsRequestRequestTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -1070,27 +1058,14 @@
         "ParameterGroupFamily": str,
         "DefaultOnly": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
     "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     {
         "ParameterGroupName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1178,14 +1153,41 @@
     {
         "NextToken": str,
         "EngineVersions": List[EngineVersionInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsRequestRequestTypeDef = TypedDict(
+    "DescribeEventsRequestRequestTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb.egg-info/PKG-INFO` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-memorydb
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MemoryDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MemoryDB 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 memorydb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 memorydb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-memorydb)](https://pepy.tech/project/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
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
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
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
@@ -367,20 +367,20 @@
 )
 
 
 def check_value(value: AZStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_memorydb.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_memorydb.type_defs import (
     ACLPendingChangesTypeDef,
     ACLsUpdateStatusTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
@@ -400,15 +400,15 @@
     DeleteSubnetGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeACLsRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeEngineVersionsRequestRequestTypeDef,
     EngineVersionInfoTypeDef,
-    DescribeEventsRequestRequestTypeDef,
+    TimestampTypeDef,
     EventTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
     DescribeParametersRequestRequestTypeDef,
     ParameterTypeDef,
     DescribeReservedNodesOfferingsRequestRequestTypeDef,
     DescribeReservedNodesRequestRequestTypeDef,
     DescribeServiceUpdatesRequestRequestTypeDef,
@@ -452,23 +452,24 @@
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeACLsRequestDescribeACLsPaginateTypeDef,
     DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
     DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
     DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
     DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeEngineVersionsResponseTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeEventsRequestRequestTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     ReservedNodeTypeDef,
@@ -506,15 +507,15 @@
     CopySnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
 )
 
 
-def get_structure() -> ACLPendingChangesTypeDef:
+def get_value() -> ACLPendingChangesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-memorydb-1.28.15.post1/mypy_boto3_memorydb.egg-info/SOURCES.txt` & `mypy-boto3-memorydb-1.28.16/mypy_boto3_memorydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.15.post1/setup.py` & `mypy-boto3-memorydb-1.28.16/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-memorydb",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_memorydb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MemoryDB 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.MemoryDB 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 memorydb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 memorydb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_memorydb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

