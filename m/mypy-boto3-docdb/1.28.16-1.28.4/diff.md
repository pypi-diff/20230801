# Comparing `tmp/mypy-boto3-docdb-1.28.16.tar.gz` & `tmp/mypy-boto3-docdb-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-docdb-1.28.16.tar", last modified: Tue Aug  1 11:36:39 2023, max compression
+gzip compressed data, was "mypy-boto3-docdb-1.28.4.tar", last modified: Tue Jul 18 01:01:42 2023, max compression
```

## Comparing `mypy-boto3-docdb-1.28.16.tar` & `mypy-boto3-docdb-1.28.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.032907 mypy-boto3-docdb-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:15:13.000000 mypy-boto3-docdb-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22646 2023-08-01 11:36:39.032907 mypy-boto3-docdb-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21170 2023-08-01 11:15:13.000000 mypy-boto3-docdb-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.028907 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-08-01 11:15:13.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-01 11:15:13.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 11:15:13.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51178 2023-08-01 11:15:14.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51103 2023-08-01 11:15:14.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-08-01 11:15:14.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-08-01 11:15:14.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17366 2023-08-01 11:15:14.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17351 2023-08-01 11:15:14.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:15:13.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60511 2023-08-01 11:15:16.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60458 2023-08-01 11:15:15.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:15:13.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-01 11:15:14.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-01 11:15:14.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.032907 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22646 2023-08-01 11:36:38.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 11:36:38.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:38.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:36:38.000000 mypy-boto3-docdb-1.28.16/mypy_boto3_docdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:39.032907 mypy-boto3-docdb-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:15:13.000000 mypy-boto3-docdb-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22691 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51205 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51130 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60559 2023-07-18 01:00:30.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60506 2023-07-18 01:00:29.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22691 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-18 01:00:27.000000 mypy-boto3-docdb-1.28.4/setup.py
```

### Comparing `mypy-boto3-docdb-1.28.16/LICENSE` & `mypy-boto3-docdb-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.16/PKG-INFO` & `mypy-boto3-docdb-1.28.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.28.16
-Summary: Type annotations for boto3.DocDB 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.4
+Summary: Type annotations for boto3.DocDB 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 docdb type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 docdb type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -397,20 +397,20 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_docdb.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_docdb.type_defs import (
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
@@ -418,15 +418,15 @@
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
-    ParameterTypeDef,
+    ParameterOutputTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
@@ -436,32 +436,33 @@
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    TimestampTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
+    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
@@ -472,70 +473,70 @@
     CreateDBClusterMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    TagListMessageTypeDef,
+    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     CertificateMessageTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
     DBClusterParameterGroupsMessageTypeDef,
     CopyDBClusterSnapshotResultTypeDef,
     CreateDBClusterSnapshotResultTypeDef,
     DBClusterSnapshotMessageTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageRequestTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
     CreateDBClusterResultTypeDef,
     DBClusterMessageTypeDef,
@@ -562,15 +563,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_value() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
+def get_structure() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-docdb-1.28.16/README.md` & `mypy-boto3-docdb-1.28.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -365,20 +365,20 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_docdb.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_docdb.type_defs import (
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
@@ -386,15 +386,15 @@
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
-    ParameterTypeDef,
+    ParameterOutputTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
@@ -404,32 +404,33 @@
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    TimestampTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
+    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
@@ -440,70 +441,70 @@
     CreateDBClusterMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    TagListMessageTypeDef,
+    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     CertificateMessageTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
     DBClusterParameterGroupsMessageTypeDef,
     CopyDBClusterSnapshotResultTypeDef,
     CreateDBClusterSnapshotResultTypeDef,
     DBClusterSnapshotMessageTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageRequestTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
     CreateDBClusterResultTypeDef,
     DBClusterMessageTypeDef,
@@ -530,15 +531,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_value() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
+def get_structure() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/__init__.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/__init__.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/__main__.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DocDB 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.DocDB 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/client.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_docdb.client import DocDBClient
 
     session = Session()
     client: DocDBClient = session.client("docdb")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import SourceTypeType
 from .paginator import (
     DescribeCertificatesPaginator,
     DescribeDBClusterParameterGroupsPaginator,
@@ -84,15 +85,14 @@
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
     StartDBClusterResultTypeDef,
     StopDBClusterResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
-    TimestampTypeDef,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -658,16 +658,16 @@
         """
 
     def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: TimestampTypeDef = ...,
-        EndTime: TimestampTypeDef = ...,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
@@ -960,15 +960,15 @@
 
     def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
         SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
-        RestoreToTime: TimestampTypeDef = ...,
+        RestoreToTime: Union[datetime, str] = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/client.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_docdb.client import DocDBClient
 
     session = Session()
     client: DocDBClient = session.client("docdb")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import SourceTypeType
 from .paginator import (
     DescribeCertificatesPaginator,
     DescribeDBClusterParameterGroupsPaginator,
@@ -84,15 +85,14 @@
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
     StartDBClusterResultTypeDef,
     StopDBClusterResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
-    TimestampTypeDef,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -620,16 +620,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/client/#describe_event_subscriptions)
         """
     def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: TimestampTypeDef = ...,
-        EndTime: TimestampTypeDef = ...,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
@@ -902,15 +902,15 @@
         """
     def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
         SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
-        RestoreToTime: TimestampTypeDef = ...,
+        RestoreToTime: Union[datetime, str] = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/literals.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -273,28 +272,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/literals.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -271,28 +270,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/paginator.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
     describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
     describe_global_clusters_paginator: DescribeGlobalClustersPaginator = client.get_paginator("describe_global_clusters")
     describe_orderable_db_instance_options_paginator: DescribeOrderableDBInstanceOptionsPaginator = client.get_paginator("describe_orderable_db_instance_options")
     describe_pending_maintenance_actions_paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SourceTypeType
 from .type_defs import (
     CertificateMessageTypeDef,
     DBClusterMessageTypeDef,
@@ -60,15 +61,14 @@
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     FilterTypeDef,
     GlobalClustersMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeCertificatesPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
     "DescribeDBClusterSnapshotsPaginator",
@@ -282,16 +282,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: TimestampTypeDef = ...,
-        EndTime: TimestampTypeDef = ...,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEvents.paginate)
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/paginator.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
     describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
     describe_global_clusters_paginator: DescribeGlobalClustersPaginator = client.get_paginator("describe_global_clusters")
     describe_orderable_db_instance_options_paginator: DescribeOrderableDBInstanceOptionsPaginator = client.get_paginator("describe_orderable_db_instance_options")
     describe_pending_maintenance_actions_paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SourceTypeType
 from .type_defs import (
     CertificateMessageTypeDef,
     DBClusterMessageTypeDef,
@@ -60,15 +61,14 @@
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     FilterTypeDef,
     GlobalClustersMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeCertificatesPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
     "DescribeDBClusterSnapshotsPaginator",
@@ -270,16 +270,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: TimestampTypeDef = ...,
-        EndTime: TimestampTypeDef = ...,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEvents.paginate)
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/type_defs.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_docdb.type_defs import AddSourceIdentifierToSubscriptionMessageRequestTypeDef
 
-    data: AddSourceIdentifierToSubscriptionMessageRequestTypeDef = ...
+    data: AddSourceIdentifierToSubscriptionMessageRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplyMethodType, SourceTypeType
@@ -32,15 +32,15 @@
     "AvailabilityZoneTypeDef",
     "CertificateTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterMemberTypeDef",
-    "ParameterTypeDef",
+    "ParameterOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "EndpointTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
@@ -50,32 +50,33 @@
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "TimestampTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
+    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
+    "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
@@ -86,70 +87,70 @@
     "CreateDBClusterMessageRequestTypeDef",
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
-    "TagListMessageTypeDef",
+    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "CertificateMessageTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
     "DBClusterParameterGroupsMessageTypeDef",
     "CopyDBClusterSnapshotResultTypeDef",
     "CreateDBClusterSnapshotResultTypeDef",
     "DBClusterSnapshotMessageTypeDef",
     "DeleteDBClusterSnapshotResultTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBClusterTypeDef",
     "DBEngineVersionTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
     "DescribeDBInstancesMessageRequestTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
+    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "CreateDBClusterResultTypeDef",
     "DBClusterMessageTypeDef",
@@ -197,15 +198,14 @@
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -234,28 +234,26 @@
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateType": str,
         "Thumbprint": str,
         "ValidFrom": datetime,
         "ValidTill": datetime,
         "CertificateArn": str,
     },
-    total=False,
 )
 
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
@@ -267,15 +265,14 @@
     "DBClusterParameterGroupTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBClusterParameterGroupArn": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotTypeDef = TypedDict(
     "DBClusterSnapshotTypeDef",
     {
         "AvailabilityZones": List[str],
         "DBClusterSnapshotIdentifier": str,
@@ -291,15 +288,14 @@
         "SnapshotType": str,
         "PercentProgress": int,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "DBClusterSnapshotArn": str,
         "SourceDBClusterSnapshotArn": str,
     },
-    total=False,
 )
 
 _RequiredCreateGlobalClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
     },
@@ -329,92 +325,84 @@
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
     },
-    total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
-    total=False,
 )
 
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributeTypeDef = TypedDict(
     "DBClusterSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
-    total=False,
 )
 
 VpcSecurityGroupMembershipTypeDef = TypedDict(
     "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
-    total=False,
 )
 
 UpgradeTargetTypeDef = TypedDict(
     "UpgradeTargetTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "Description": str,
         "AutoUpgrade": bool,
         "IsMajorVersionUpgrade": bool,
     },
-    total=False,
 )
 
 DBInstanceStatusInfoTypeDef = TypedDict(
     "DBInstanceStatusInfoTypeDef",
     {
         "StatusType": str,
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -507,35 +495,32 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
-    total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
         "SourceArn": str,
     },
-    total=False,
 )
 
 FailoverDBClusterMessageRequestTypeDef = TypedDict(
     "FailoverDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "TargetDBInstanceIdentifier": str,
@@ -546,14 +531,30 @@
 GlobalClusterMemberTypeDef = TypedDict(
     "GlobalClusterMemberTypeDef",
     {
         "DBClusterArn": str,
         "Readers": List[str],
         "IsWriter": bool,
     },
+)
+
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+        "Description": str,
+        "Source": str,
+        "ApplyType": str,
+        "DataType": str,
+        "AllowedValues": str,
+        "IsModifiable": bool,
+        "MinimumEngineVersion": str,
+        "ApplyMethod": ApplyMethodType,
+    },
     total=False,
 )
 
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
@@ -680,28 +681,26 @@
 
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
-    total=False,
 )
 
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 _RequiredRebootDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
@@ -755,14 +754,22 @@
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1080,43 +1087,65 @@
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
+_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DBClusterIdentifier": str,
+        "SourceDBClusterIdentifier": str,
     },
 )
+_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
+    {
+        "RestoreType": str,
+        "RestoreToTime": Union[datetime, str],
+        "UseLatestRestorableTime": bool,
+        "Port": int,
+        "DBSubnetGroupName": str,
+        "VpcSecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "EnableCloudwatchLogsExports": Sequence[str],
+        "DeletionProtection": bool,
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
 
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "Vpc": bool,
     },
-    total=False,
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
@@ -1214,68 +1243,35 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterTypeDef],
-    },
-    total=False,
-)
-
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
     },
 )
 
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-    total=False,
-)
-
-
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
 DBClusterTypeDef = TypedDict(
     "DBClusterTypeDef",
     {
         "AvailabilityZones": List[str],
         "BackupRetentionPeriod": int,
@@ -1306,30 +1302,28 @@
         "DBClusterArn": str,
         "AssociatedRoles": List[DBClusterRoleTypeDef],
         "CloneGroupId": str,
         "ClusterCreateTime": datetime,
         "EnabledCloudwatchLogsExports": List[str],
         "DeletionProtection": bool,
     },
-    total=False,
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "DBEngineDescription": str,
         "DBEngineVersionDescription": str,
         "ValidUpgradeTarget": List[UpgradeTargetTypeDef],
         "ExportableLogTypes": List[str],
         "SupportsLogExportsToCloudwatchLogs": bool,
     },
-    total=False,
 )
 
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1479,14 +1473,30 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -1664,14 +1674,29 @@
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
     "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1737,77 +1762,14 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
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
-        "RestoreToTime": TimestampTypeDef,
-        "UseLatestRestorableTime": bool,
-        "Port": int,
-        "DBSubnetGroupName": str,
-        "VpcSecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "EnableCloudwatchLogsExports": Sequence[str],
-        "DeletionProtection": bool,
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
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1831,17 +1793,47 @@
         "Engine": str,
         "EngineVersion": str,
         "DatabaseName": str,
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
     },
+)
+
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
     total=False,
 )
 
+
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "DBInstanceClass": str,
         "AllocatedStorage": int,
         "MasterUserPassword": str,
         "Port": int,
@@ -1852,24 +1844,30 @@
         "Iops": int,
         "DBInstanceIdentifier": str,
         "StorageType": str,
         "CACertificateIdentifier": str,
         "DBSubnetGroupName": str,
         "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
     },
-    total=False,
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
+)
+
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
 )
 
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
@@ -1883,15 +1881,14 @@
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
     },
-    total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2089,15 +2086,14 @@
         "DbiResourceId": str,
         "CACertificateIdentifier": str,
         "CopyTagsToSnapshot": bool,
         "PromotionTier": int,
         "DBInstanceArn": str,
         "EnabledCloudwatchLogsExports": List[str],
     },
-    total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/type_defs.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_docdb.type_defs import AddSourceIdentifierToSubscriptionMessageRequestTypeDef
 
-    data: AddSourceIdentifierToSubscriptionMessageRequestTypeDef = ...
+    data: AddSourceIdentifierToSubscriptionMessageRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplyMethodType, SourceTypeType
@@ -31,15 +31,15 @@
     "AvailabilityZoneTypeDef",
     "CertificateTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterMemberTypeDef",
-    "ParameterTypeDef",
+    "ParameterOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "EndpointTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
@@ -49,32 +49,33 @@
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "TimestampTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
+    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
+    "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
@@ -85,70 +86,70 @@
     "CreateDBClusterMessageRequestTypeDef",
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
-    "TagListMessageTypeDef",
+    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "CertificateMessageTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
     "DBClusterParameterGroupsMessageTypeDef",
     "CopyDBClusterSnapshotResultTypeDef",
     "CreateDBClusterSnapshotResultTypeDef",
     "DBClusterSnapshotMessageTypeDef",
     "DeleteDBClusterSnapshotResultTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBClusterTypeDef",
     "DBEngineVersionTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
     "DescribeDBInstancesMessageRequestTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
+    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "CreateDBClusterResultTypeDef",
     "DBClusterMessageTypeDef",
@@ -196,15 +197,14 @@
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -233,28 +233,26 @@
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateType": str,
         "Thumbprint": str,
         "ValidFrom": datetime,
         "ValidTill": datetime,
         "CertificateArn": str,
     },
-    total=False,
 )
 
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
@@ -266,15 +264,14 @@
     "DBClusterParameterGroupTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBClusterParameterGroupArn": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotTypeDef = TypedDict(
     "DBClusterSnapshotTypeDef",
     {
         "AvailabilityZones": List[str],
         "DBClusterSnapshotIdentifier": str,
@@ -290,15 +287,14 @@
         "SnapshotType": str,
         "PercentProgress": int,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "DBClusterSnapshotArn": str,
         "SourceDBClusterSnapshotArn": str,
     },
-    total=False,
 )
 
 _RequiredCreateGlobalClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
     },
@@ -326,92 +322,84 @@
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
     },
-    total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
-    total=False,
 )
 
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributeTypeDef = TypedDict(
     "DBClusterSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
-    total=False,
 )
 
 VpcSecurityGroupMembershipTypeDef = TypedDict(
     "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
-    total=False,
 )
 
 UpgradeTargetTypeDef = TypedDict(
     "UpgradeTargetTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "Description": str,
         "AutoUpgrade": bool,
         "IsMajorVersionUpgrade": bool,
     },
-    total=False,
 )
 
 DBInstanceStatusInfoTypeDef = TypedDict(
     "DBInstanceStatusInfoTypeDef",
     {
         "StatusType": str,
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -502,35 +490,32 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
-    total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
         "SourceArn": str,
     },
-    total=False,
 )
 
 FailoverDBClusterMessageRequestTypeDef = TypedDict(
     "FailoverDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "TargetDBInstanceIdentifier": str,
@@ -541,14 +526,30 @@
 GlobalClusterMemberTypeDef = TypedDict(
     "GlobalClusterMemberTypeDef",
     {
         "DBClusterArn": str,
         "Readers": List[str],
         "IsWriter": bool,
     },
+)
+
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+        "Description": str,
+        "Source": str,
+        "ApplyType": str,
+        "DataType": str,
+        "AllowedValues": str,
+        "IsModifiable": bool,
+        "MinimumEngineVersion": str,
+        "ApplyMethod": ApplyMethodType,
+    },
     total=False,
 )
 
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
@@ -665,28 +666,26 @@
 
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
-    total=False,
 )
 
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 _RequiredRebootDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
@@ -738,14 +737,22 @@
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1045,43 +1052,63 @@
 
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
+_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DBClusterIdentifier": str,
+        "SourceDBClusterIdentifier": str,
+    },
+)
+_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
+    {
+        "RestoreType": str,
+        "RestoreToTime": Union[datetime, str],
+        "UseLatestRestorableTime": bool,
+        "Port": int,
+        "DBSubnetGroupName": str,
+        "VpcSecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "EnableCloudwatchLogsExports": Sequence[str],
+        "DeletionProtection": bool,
     },
+    total=False,
 )
 
+class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
+    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+):
+    pass
+
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "Vpc": bool,
     },
-    total=False,
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
@@ -1177,66 +1204,35 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterTypeDef],
-    },
-    total=False,
-)
-
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
     },
-    total=False,
 )
 
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
 DBClusterTypeDef = TypedDict(
     "DBClusterTypeDef",
     {
         "AvailabilityZones": List[str],
         "BackupRetentionPeriod": int,
@@ -1267,30 +1263,28 @@
         "DBClusterArn": str,
         "AssociatedRoles": List[DBClusterRoleTypeDef],
         "CloneGroupId": str,
         "ClusterCreateTime": datetime,
         "EnabledCloudwatchLogsExports": List[str],
         "DeletionProtection": bool,
     },
-    total=False,
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "DBEngineDescription": str,
         "DBEngineVersionDescription": str,
         "ValidUpgradeTarget": List[UpgradeTargetTypeDef],
         "ExportableLogTypes": List[str],
         "SupportsLogExportsToCloudwatchLogs": bool,
     },
-    total=False,
 )
 
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1436,14 +1430,30 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -1615,14 +1625,29 @@
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
     "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1686,75 +1711,14 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
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
-        "RestoreToTime": TimestampTypeDef,
-        "UseLatestRestorableTime": bool,
-        "Port": int,
-        "DBSubnetGroupName": str,
-        "VpcSecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "EnableCloudwatchLogsExports": Sequence[str],
-        "DeletionProtection": bool,
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
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1778,17 +1742,45 @@
         "Engine": str,
         "EngineVersion": str,
         "DatabaseName": str,
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
     },
+)
+
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
     total=False,
 )
 
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "DBInstanceClass": str,
         "AllocatedStorage": int,
         "MasterUserPassword": str,
         "Port": int,
@@ -1799,24 +1791,30 @@
         "Iops": int,
         "DBInstanceIdentifier": str,
         "StorageType": str,
         "CACertificateIdentifier": str,
         "DBSubnetGroupName": str,
         "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
     },
-    total=False,
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
+)
+
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
 )
 
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
@@ -1830,15 +1828,14 @@
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
     },
-    total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2036,15 +2033,14 @@
         "DbiResourceId": str,
         "CACertificateIdentifier": str,
         "CopyTagsToSnapshot": bool,
         "PromotionTier": int,
         "DBInstanceArn": str,
         "EnabledCloudwatchLogsExports": List[str],
     },
-    total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/waiter.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb/waiter.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb.egg-info/PKG-INFO` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.28.16
-Summary: Type annotations for boto3.DocDB 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.4
+Summary: Type annotations for boto3.DocDB 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 docdb type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 docdb type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -397,20 +397,20 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_docdb.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_docdb.type_defs import (
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
@@ -418,15 +418,15 @@
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
-    ParameterTypeDef,
+    ParameterOutputTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
@@ -436,32 +436,33 @@
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    TimestampTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
+    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
@@ -472,70 +473,70 @@
     CreateDBClusterMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    TagListMessageTypeDef,
+    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     CertificateMessageTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
     DBClusterParameterGroupsMessageTypeDef,
     CopyDBClusterSnapshotResultTypeDef,
     CreateDBClusterSnapshotResultTypeDef,
     DBClusterSnapshotMessageTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageRequestTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
     CreateDBClusterResultTypeDef,
     DBClusterMessageTypeDef,
@@ -562,15 +563,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_value() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
+def get_structure() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-docdb-1.28.16/mypy_boto3_docdb.egg-info/SOURCES.txt` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.16/setup.py` & `mypy-boto3-docdb-1.28.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-docdb",
-    version="1.28.16",
+    version="1.28.4",
     packages=["mypy_boto3_docdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DocDB 1.28.16 service generated with mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.DocDB 1.28.4 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -33,15 +33,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 docdb type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 docdb type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_docdb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

