# Comparing `tmp/mypy-boto3-neptune-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-neptune-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-neptune-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:45 2023, max compression
+gzip compressed data, was "mypy-boto3-neptune-1.28.16.tar", last modified: Tue Aug  1 11:37:26 2023, max compression
```

## Comparing `mypy-boto3-neptune-1.28.15.post1.tar` & `mypy-boto3-neptune-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:45.829307 mypy-boto3-neptune-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:58.000000 mypy-boto3-neptune-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25536 2023-07-29 10:03:45.821307 mypy-boto3-neptune-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-07-29 09:51:58.000000 mypy-boto3-neptune-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:45.821307 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-29 09:51:58.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-29 09:51:58.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:51:58.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67621 2023-07-29 09:51:58.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67527 2023-07-29 09:51:58.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-07-29 09:51:59.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-29 09:51:59.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-07-29 09:51:59.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-07-29 09:51:59.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:58.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    84422 2023-07-29 09:52:01.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    84345 2023-07-29 09:52:00.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:58.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-29 09:51:59.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-29 09:51:59.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:45.821307 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25536 2023-07-29 10:03:45.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-29 10:03:45.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:45.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:45.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:45.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:03:45.000000 mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:45.829307 mypy-boto3-neptune-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:51:57.000000 mypy-boto3-neptune-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:26.528806 mypy-boto3-neptune-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:55.000000 mypy-boto3-neptune-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25548 2023-08-01 11:37:26.524806 mypy-boto3-neptune-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-08-01 11:24:55.000000 mypy-boto3-neptune-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:26.520806 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-08-01 11:24:55.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-01 11:24:55.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:24:55.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67594 2023-08-01 11:24:59.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67500 2023-08-01 11:24:56.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-08-01 11:24:59.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-08-01 11:24:59.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-08-01 11:24:59.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-08-01 11:24:59.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:55.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    84464 2023-08-01 11:25:01.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84387 2023-08-01 11:25:00.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:55.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-08-01 11:24:59.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-01 11:24:59.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:26.524806 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25548 2023-08-01 11:37:26.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 11:37:26.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:26.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:26.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:26.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:37:26.000000 mypy-boto3-neptune-1.28.16/mypy_boto3_neptune.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:26.528806 mypy-boto3-neptune-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:24:55.000000 mypy-boto3-neptune-1.28.16/setup.py
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/LICENSE` & `mypy-boto3-neptune-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.15.post1/PKG-INFO` & `mypy-boto3-neptune-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-neptune
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Neptune 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Neptune 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 neptune type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 neptune type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-neptune)](https://pepy.tech/project/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [mypy-boto3-neptune docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/).
 
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
@@ -412,20 +412,20 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_neptune.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_neptune.type_defs import (
     AddRoleToDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
     ResponseMetadataTypeDef,
@@ -465,14 +465,15 @@
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
+    TimestampTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeValidDBInstanceModificationsMessageRequestTypeDef,
     DoubleRangeTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
@@ -530,15 +531,14 @@
     DeleteDBClusterSnapshotResultTypeDef,
     CopyDBParameterGroupResultTypeDef,
     CreateDBParameterGroupResultTypeDef,
     DBParameterGroupsMessageTypeDef,
     CreateDBClusterMessageRequestTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ModifyDBParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
@@ -555,15 +555,14 @@
     DescribeDBParameterGroupsMessageRequestTypeDef,
     DescribeDBParametersMessageRequestTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
@@ -571,20 +570,22 @@
     DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
     DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
@@ -622,15 +623,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_structure() -> AddRoleToDBClusterMessageRequestTypeDef:
+def get_value() -> AddRoleToDBClusterMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/README.md` & `mypy-boto3-neptune-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-neptune)](https://pepy.tech/project/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [mypy-boto3-neptune docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/).
 
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
@@ -380,20 +380,20 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_neptune.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_neptune.type_defs import (
     AddRoleToDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
     ResponseMetadataTypeDef,
@@ -433,14 +433,15 @@
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
+    TimestampTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeValidDBInstanceModificationsMessageRequestTypeDef,
     DoubleRangeTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
@@ -498,15 +499,14 @@
     DeleteDBClusterSnapshotResultTypeDef,
     CopyDBParameterGroupResultTypeDef,
     CreateDBParameterGroupResultTypeDef,
     DBParameterGroupsMessageTypeDef,
     CreateDBClusterMessageRequestTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ModifyDBParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
@@ -523,15 +523,14 @@
     DescribeDBParameterGroupsMessageRequestTypeDef,
     DescribeDBParametersMessageRequestTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
@@ -539,20 +538,22 @@
     DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
     DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
@@ -590,15 +591,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_structure() -> AddRoleToDBClusterMessageRequestTypeDef:
+def get_value() -> AddRoleToDBClusterMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/__init__.py` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/__init__.pyi` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/__main__.py` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Neptune 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Neptune 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune\nOther"
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

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/client.py` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_neptune.client import NeptuneClient
 
     session = Session()
     client: NeptuneClient = session.client("neptune")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import SourceTypeType
 from .paginator import (
     DescribeDBClusterEndpointsPaginator,
     DescribeDBClusterParameterGroupsPaginator,
@@ -101,14 +100,15 @@
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     StartDBClusterResultTypeDef,
     StopDBClusterResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -852,16 +852,16 @@
         """
 
     def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
@@ -1267,15 +1267,15 @@
 
     def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
         SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
-        RestoreToTime: Union[datetime, str] = ...,
+        RestoreToTime: TimestampTypeDef = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/client.pyi` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_neptune.client import NeptuneClient
 
     session = Session()
     client: NeptuneClient = session.client("neptune")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import SourceTypeType
 from .paginator import (
     DescribeDBClusterEndpointsPaginator,
     DescribeDBClusterParameterGroupsPaginator,
@@ -101,14 +100,15 @@
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     StartDBClusterResultTypeDef,
     StopDBClusterResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -805,16 +805,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/client/#describe_event_subscriptions)
         """
     def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
@@ -1193,15 +1193,15 @@
         """
     def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
         SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
-        RestoreToTime: Union[datetime, str] = ...,
+        RestoreToTime: TimestampTypeDef = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/literals.py` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/literals.pyi` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/paginator.py` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,15 @@
     describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
     describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
     describe_global_clusters_paginator: DescribeGlobalClustersPaginator = client.get_paginator("describe_global_clusters")
     describe_orderable_db_instance_options_paginator: DescribeOrderableDBInstanceOptionsPaginator = client.get_paginator("describe_orderable_db_instance_options")
     describe_pending_maintenance_actions_paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SourceTypeType
 from .type_defs import (
     DBClusterEndpointMessageTypeDef,
     DBClusterMessageTypeDef,
@@ -70,14 +69,15 @@
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     FilterTypeDef,
     GlobalClustersMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeDBClusterEndpointsPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
     "DescribeDBClusterSnapshotsPaginator",
@@ -353,16 +353,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents.paginate)
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/paginator.pyi` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,15 @@
     describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
     describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
     describe_global_clusters_paginator: DescribeGlobalClustersPaginator = client.get_paginator("describe_global_clusters")
     describe_orderable_db_instance_options_paginator: DescribeOrderableDBInstanceOptionsPaginator = client.get_paginator("describe_orderable_db_instance_options")
     describe_pending_maintenance_actions_paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SourceTypeType
 from .type_defs import (
     DBClusterEndpointMessageTypeDef,
     DBClusterMessageTypeDef,
@@ -70,14 +69,15 @@
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     FilterTypeDef,
     GlobalClustersMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeDBClusterEndpointsPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
     "DescribeDBClusterSnapshotsPaginator",
@@ -338,16 +338,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents.paginate)
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/type_defs.py` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_neptune.type_defs import AddRoleToDBClusterMessageRequestTypeDef
 
-    data: AddRoleToDBClusterMessageRequestTypeDef = {...}
+    data: AddRoleToDBClusterMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplyMethodType, SourceTypeType
@@ -64,14 +64,15 @@
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
+    "TimestampTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
     "DescribeValidDBInstanceModificationsMessageRequestTypeDef",
     "DoubleRangeTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "FailoverGlobalClusterMessageRequestTypeDef",
@@ -129,15 +130,14 @@
     "DeleteDBClusterSnapshotResultTypeDef",
     "CopyDBParameterGroupResultTypeDef",
     "CreateDBParameterGroupResultTypeDef",
     "DBParameterGroupsMessageTypeDef",
     "CreateDBClusterMessageRequestTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
-    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     "ModifyDBParameterGroupMessageRequestTypeDef",
     "ResetDBClusterParameterGroupMessageRequestTypeDef",
@@ -154,15 +154,14 @@
     "DescribeDBParameterGroupsMessageRequestTypeDef",
     "DescribeDBParametersMessageRequestTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
@@ -170,20 +169,22 @@
     "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
@@ -714,14 +715,15 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1781,50 +1783,14 @@
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
 
-_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
-    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "SourceDBClusterIdentifier": str,
-    },
-)
-_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
-    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    {
-        "RestoreType": str,
-        "RestoreToTime": Union[datetime, str],
-        "UseLatestRestorableTime": bool,
-        "Port": int,
-        "DBSubnetGroupName": str,
-        "OptionGroupName": str,
-        "VpcSecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "EnableIAMDatabaseAuthentication": bool,
-        "EnableCloudwatchLogsExports": Sequence[str],
-        "DBClusterParameterGroupName": str,
-        "DeletionProtection": bool,
-        "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
-    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-):
-    pass
-
-
 DBClusterEndpointMessageTypeDef = TypedDict(
     "DBClusterEndpointMessageTypeDef",
     {
         "Marker": str,
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2161,30 +2127,14 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
 _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
         "Engine": str,
     },
 )
 _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
@@ -2409,29 +2359,14 @@
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
     "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2496,14 +2431,81 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "SourceDBClusterIdentifier": str,
+    },
+)
+_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
+    {
+        "RestoreType": str,
+        "RestoreToTime": TimestampTypeDef,
+        "UseLatestRestorableTime": bool,
+        "Port": int,
+        "DBSubnetGroupName": str,
+        "OptionGroupName": str,
+        "VpcSecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "EnableIAMDatabaseAuthentication": bool,
+        "EnableCloudwatchLogsExports": Sequence[str],
+        "DBClusterParameterGroupName": str,
+        "DeletionProtection": bool,
+        "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
+    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+):
+    pass
+
+
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/type_defs.pyi` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_neptune.type_defs import AddRoleToDBClusterMessageRequestTypeDef
 
-    data: AddRoleToDBClusterMessageRequestTypeDef = {...}
+    data: AddRoleToDBClusterMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplyMethodType, SourceTypeType
@@ -63,14 +63,15 @@
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
+    "TimestampTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
     "DescribeValidDBInstanceModificationsMessageRequestTypeDef",
     "DoubleRangeTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "FailoverGlobalClusterMessageRequestTypeDef",
@@ -128,15 +129,14 @@
     "DeleteDBClusterSnapshotResultTypeDef",
     "CopyDBParameterGroupResultTypeDef",
     "CreateDBParameterGroupResultTypeDef",
     "DBParameterGroupsMessageTypeDef",
     "CreateDBClusterMessageRequestTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
-    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     "ModifyDBParameterGroupMessageRequestTypeDef",
     "ResetDBClusterParameterGroupMessageRequestTypeDef",
@@ -153,15 +153,14 @@
     "DescribeDBParameterGroupsMessageRequestTypeDef",
     "DescribeDBParametersMessageRequestTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
@@ -169,20 +168,22 @@
     "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
@@ -705,14 +706,15 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1730,48 +1732,14 @@
 
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
-_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
-    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "SourceDBClusterIdentifier": str,
-    },
-)
-_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
-    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    {
-        "RestoreType": str,
-        "RestoreToTime": Union[datetime, str],
-        "UseLatestRestorableTime": bool,
-        "Port": int,
-        "DBSubnetGroupName": str,
-        "OptionGroupName": str,
-        "VpcSecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "EnableIAMDatabaseAuthentication": bool,
-        "EnableCloudwatchLogsExports": Sequence[str],
-        "DBClusterParameterGroupName": str,
-        "DeletionProtection": bool,
-        "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
-    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-):
-    pass
-
 DBClusterEndpointMessageTypeDef = TypedDict(
     "DBClusterEndpointMessageTypeDef",
     {
         "Marker": str,
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2096,30 +2064,14 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
 _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
         "Engine": str,
     },
 )
 _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
@@ -2334,29 +2286,14 @@
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
     "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2419,14 +2356,79 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "SourceDBClusterIdentifier": str,
+    },
+)
+_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
+    {
+        "RestoreType": str,
+        "RestoreToTime": TimestampTypeDef,
+        "UseLatestRestorableTime": bool,
+        "Port": int,
+        "DBSubnetGroupName": str,
+        "OptionGroupName": str,
+        "VpcSecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "EnableIAMDatabaseAuthentication": bool,
+        "EnableCloudwatchLogsExports": Sequence[str],
+        "DBClusterParameterGroupName": str,
+        "DeletionProtection": bool,
+        "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
+    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+):
+    pass
+
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/waiter.py` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune/waiter.pyi` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune.egg-info/PKG-INFO` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-neptune
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Neptune 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Neptune 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 neptune type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 neptune type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-neptune)](https://pepy.tech/project/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [mypy-boto3-neptune docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/).
 
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
@@ -412,20 +412,20 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_neptune.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_neptune.type_defs import (
     AddRoleToDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
     ResponseMetadataTypeDef,
@@ -465,14 +465,15 @@
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
+    TimestampTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeValidDBInstanceModificationsMessageRequestTypeDef,
     DoubleRangeTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
@@ -530,15 +531,14 @@
     DeleteDBClusterSnapshotResultTypeDef,
     CopyDBParameterGroupResultTypeDef,
     CreateDBParameterGroupResultTypeDef,
     DBParameterGroupsMessageTypeDef,
     CreateDBClusterMessageRequestTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ModifyDBParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
@@ -555,15 +555,14 @@
     DescribeDBParameterGroupsMessageRequestTypeDef,
     DescribeDBParametersMessageRequestTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
@@ -571,20 +570,22 @@
     DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
     DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
@@ -622,15 +623,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_structure() -> AddRoleToDBClusterMessageRequestTypeDef:
+def get_value() -> AddRoleToDBClusterMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-neptune-1.28.15.post1/mypy_boto3_neptune.egg-info/SOURCES.txt` & `mypy-boto3-neptune-1.28.16/mypy_boto3_neptune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.15.post1/setup.py` & `mypy-boto3-neptune-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-neptune",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_neptune"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Neptune 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Neptune 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 neptune type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 neptune type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_neptune": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

