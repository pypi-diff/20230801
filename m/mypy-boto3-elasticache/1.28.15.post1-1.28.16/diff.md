# Comparing `tmp/mypy-boto3-elasticache-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-elasticache-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticache-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:03 2023, max compression
+gzip compressed data, was "mypy-boto3-elasticache-1.28.16.tar", last modified: Tue Aug  1 11:36:42 2023, max compression
```

## Comparing `mypy-boto3-elasticache-1.28.15.post1.tar` & `mypy-boto3-elasticache-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:03.013130 mypy-boto3-elasticache-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27289 2023-07-29 10:03:03.013130 mypy-boto3-elasticache-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.993130 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68102 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68009 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-07-29 09:44:38.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86681 2023-07-29 09:44:40.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86614 2023-07-29 09:44:39.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:03.013130 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27289 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:03.013130 mypy-boto3-elasticache-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:44:34.000000 mypy-boto3-elasticache-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.916900 mypy-boto3-elasticache-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27341 2023-08-01 11:36:42.912900 mypy-boto3-elasticache-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25841 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.900900 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67982 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67889 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-08-01 11:17:13.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-08-01 11:17:13.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22637 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22618 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86817 2023-08-01 11:17:16.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86750 2023-08-01 11:17:14.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.912900 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27341 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:42.916900 mypy-boto3-elasticache-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/setup.py
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/LICENSE` & `mypy-boto3-elasticache-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15.post1/PKG-INFO` & `mypy-boto3-elasticache-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ElastiCache 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 elasticache type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 elasticache type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
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
@@ -456,20 +456,20 @@
 )
 
 
 def check_value(value: AZModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
@@ -488,16 +488,14 @@
     ParameterTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
-    NodeGroupConfigurationOutputTypeDef,
-    NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     DeleteCacheClusterMessageRequestTypeDef,
     DeleteCacheParameterGroupMessageRequestTypeDef,
     DeleteCacheSecurityGroupMessageRequestTypeDef,
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
@@ -510,22 +508,21 @@
     DescribeCacheClustersMessageRequestTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
+    TimestampTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
-    TimeRangeFilterTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
@@ -534,14 +531,16 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
+    NodeGroupConfigurationTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
@@ -573,46 +572,47 @@
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
-    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
     DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
     DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
-    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
-    DescribeUpdateActionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    TimeRangeFilterTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
+    NodeSnapshotTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
     UpdateActionResultsMessageTypeDef,
@@ -622,45 +622,47 @@
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
-    SnapshotTypeDef,
+    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
+    DescribeUpdateActionsMessageRequestTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
+    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ReplicationGroupPendingModifiedValuesTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
@@ -677,15 +679,15 @@
     ModifyReplicationGroupShardConfigurationResultTypeDef,
     ReplicationGroupMessageTypeDef,
     StartMigrationResponseTypeDef,
     TestFailoverResultTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/README.md` & `mypy-boto3-elasticache-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
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
@@ -424,20 +424,20 @@
 )
 
 
 def check_value(value: AZModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
@@ -456,16 +456,14 @@
     ParameterTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
-    NodeGroupConfigurationOutputTypeDef,
-    NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     DeleteCacheClusterMessageRequestTypeDef,
     DeleteCacheParameterGroupMessageRequestTypeDef,
     DeleteCacheSecurityGroupMessageRequestTypeDef,
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
@@ -478,22 +476,21 @@
     DescribeCacheClustersMessageRequestTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
+    TimestampTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
-    TimeRangeFilterTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
@@ -502,14 +499,16 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
+    NodeGroupConfigurationTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
@@ -541,46 +540,47 @@
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
-    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
     DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
     DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
-    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
-    DescribeUpdateActionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    TimeRangeFilterTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
+    NodeSnapshotTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
     UpdateActionResultsMessageTypeDef,
@@ -590,45 +590,47 @@
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
-    SnapshotTypeDef,
+    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
+    DescribeUpdateActionsMessageRequestTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
+    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ReplicationGroupPendingModifiedValuesTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
@@ -645,15 +647,15 @@
     ModifyReplicationGroupShardConfigurationResultTypeDef,
     ReplicationGroupMessageTypeDef,
     StartMigrationResponseTypeDef,
     TestFailoverResultTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__init__.py` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__init__.pyi` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__main__.py` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElastiCache 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ElastiCache 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
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

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/client.py` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_elasticache.client import ElastiCacheClient
 
     session = Session()
     client: ElastiCacheClient = session.client("elasticache")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthTokenUpdateStrategyTypeType,
     AZModeType,
     ClusterModeType,
@@ -92,16 +91,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
-    NodeGroupConfigurationOutputTypeDef,
-    NodeGroupConfigurationTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
@@ -110,14 +108,15 @@
     RevokeCacheSecurityGroupIngressResultTypeDef,
     ServiceUpdatesMessageTypeDef,
     StartMigrationResponseTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TestFailoverResultTypeDef,
     TimeRangeFilterTypeDef,
+    TimestampTypeDef,
     UpdateActionResultsMessageTypeDef,
     UpdateActionsMessageTypeDef,
     UserGroupResponseTypeDef,
     UserResponseTypeDef,
 )
 from .waiter import (
     CacheClusterAvailableWaiter,
@@ -430,17 +429,15 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[
-            Union[NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef]
-        ] = ...,
+        NodeGroupConfiguration: Sequence[NodeGroupConfigurationUnionTypeDef] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
@@ -741,16 +738,16 @@
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
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, cache security groups, and cache parameter
         groups.
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/client.pyi` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_elasticache.client import ElastiCacheClient
 
     session = Session()
     client: ElastiCacheClient = session.client("elasticache")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthTokenUpdateStrategyTypeType,
     AZModeType,
     ClusterModeType,
@@ -92,16 +91,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
-    NodeGroupConfigurationOutputTypeDef,
-    NodeGroupConfigurationTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
@@ -110,14 +108,15 @@
     RevokeCacheSecurityGroupIngressResultTypeDef,
     ServiceUpdatesMessageTypeDef,
     StartMigrationResponseTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TestFailoverResultTypeDef,
     TimeRangeFilterTypeDef,
+    TimestampTypeDef,
     UpdateActionResultsMessageTypeDef,
     UpdateActionsMessageTypeDef,
     UserGroupResponseTypeDef,
     UserResponseTypeDef,
 )
 from .waiter import (
     CacheClusterAvailableWaiter,
@@ -412,17 +411,15 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[
-            Union[NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef]
-        ] = ...,
+        NodeGroupConfiguration: Sequence[NodeGroupConfigurationUnionTypeDef] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
@@ -701,16 +698,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#describe_engine_default_parameters)
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
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, cache security groups, and cache parameter
         groups.
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/literals.py` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/literals.pyi` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/paginator.py` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,15 @@
     describe_service_updates_paginator: DescribeServiceUpdatesPaginator = client.get_paginator("describe_service_updates")
     describe_snapshots_paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")
     describe_update_actions_paginator: DescribeUpdateActionsPaginator = client.get_paginator("describe_update_actions")
     describe_user_groups_paginator: DescribeUserGroupsPaginator = client.get_paginator("describe_user_groups")
     describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ServiceUpdateStatusType, SourceTypeType, UpdateActionStatusType
 from .type_defs import (
     CacheClusterMessageTypeDef,
     CacheEngineVersionMessageTypeDef,
@@ -73,14 +72,15 @@
     FilterTypeDef,
     PaginatorConfigTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     ServiceUpdatesMessageTypeDef,
     TimeRangeFilterTypeDef,
+    TimestampTypeDef,
     UpdateActionsMessageTypeDef,
 )
 
 __all__ = (
     "DescribeCacheClustersPaginator",
     "DescribeCacheEngineVersionsPaginator",
     "DescribeCacheParameterGroupsPaginator",
@@ -238,16 +238,16 @@
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
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeeventspaginator)
         """
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/paginator.pyi` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,15 @@
     describe_service_updates_paginator: DescribeServiceUpdatesPaginator = client.get_paginator("describe_service_updates")
     describe_snapshots_paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")
     describe_update_actions_paginator: DescribeUpdateActionsPaginator = client.get_paginator("describe_update_actions")
     describe_user_groups_paginator: DescribeUserGroupsPaginator = client.get_paginator("describe_user_groups")
     describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ServiceUpdateStatusType, SourceTypeType, UpdateActionStatusType
 from .type_defs import (
     CacheClusterMessageTypeDef,
     CacheEngineVersionMessageTypeDef,
@@ -73,14 +72,15 @@
     FilterTypeDef,
     PaginatorConfigTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     ServiceUpdatesMessageTypeDef,
     TimeRangeFilterTypeDef,
+    TimestampTypeDef,
     UpdateActionsMessageTypeDef,
 )
 
 __all__ = (
     "DescribeCacheClustersPaginator",
     "DescribeCacheEngineVersionsPaginator",
     "DescribeCacheParameterGroupsPaginator",
@@ -228,16 +228,16 @@
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
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeeventspaginator)
         """
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/type_defs.py` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_elasticache.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -74,16 +74,14 @@
     "ParameterTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationOutputTypeDef",
-    "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
@@ -96,22 +94,21 @@
     "DescribeCacheClustersMessageRequestTypeDef",
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
     "DescribeCacheParametersMessageRequestTypeDef",
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     "DescribeReplicationGroupsMessageRequestTypeDef",
     "DescribeReservedCacheNodesMessageRequestTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
     "DescribeServiceUpdatesMessageRequestTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
-    "TimeRangeFilterTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
@@ -120,14 +117,16 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationOutputTypeDef",
+    "NodeGroupConfigurationTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -159,46 +158,47 @@
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
-    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
     "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
     "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
     "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
     "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
     "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
-    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
-    "DescribeUpdateActionsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "TimeRangeFilterTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
+    "NodeSnapshotTypeDef",
+    "NodeGroupConfigurationUnionTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
@@ -208,45 +208,47 @@
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
-    "SnapshotTypeDef",
+    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
+    "DescribeUpdateActionsMessageRequestTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
+    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -556,42 +558,14 @@
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
-NodeGroupConfigurationOutputTypeDef = TypedDict(
-    "NodeGroupConfigurationOutputTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
-NodeGroupConfigurationTypeDef = TypedDict(
-    "NodeGroupConfigurationTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": Sequence[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": Sequence[str],
-    },
-    total=False,
-)
-
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
     },
     total=False,
@@ -834,28 +808,15 @@
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeGlobalReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowMemberInfo": bool,
@@ -923,23 +884,14 @@
         "Marker": str,
         "MaxRecords": int,
         "ShowNodeGroupConfig": bool,
     },
     total=False,
 )
 
-TimeRangeFilterTypeDef = TypedDict(
-    "TimeRangeFilterTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 DescribeUserGroupsMessageRequestTypeDef = TypedDict(
     "DescribeUserGroupsMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1123,14 +1075,42 @@
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
 
+NodeGroupConfigurationOutputTypeDef = TypedDict(
+    "NodeGroupConfigurationOutputTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
+NodeGroupConfigurationTypeDef = TypedDict(
+    "NodeGroupConfigurationTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": Sequence[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": Sequence[str],
+    },
+    total=False,
+)
+
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1686,28 +1666,14 @@
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -1851,27 +1817,14 @@
 class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "ShowMemberInfo": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1942,47 +1895,50 @@
     {
         "UserGroupId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
-    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
-        "ServiceUpdateName": str,
-        "ReplicationGroupIds": Sequence[str],
-        "CacheClusterIds": Sequence[str],
-        "Engine": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
-        "UpdateActionStatus": Sequence[UpdateActionStatusType],
-        "ShowNodeLevelUpdateStatus": bool,
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
-    "DescribeUpdateActionsMessageRequestTypeDef",
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
     {
-        "ServiceUpdateName": str,
-        "ReplicationGroupIds": Sequence[str],
-        "CacheClusterIds": Sequence[str],
-        "Engine": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
-        "UpdateActionStatus": Sequence[UpdateActionStatusType],
-        "ShowNodeLevelUpdateStatus": bool,
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+TimeRangeFilterTypeDef = TypedDict(
+    "TimeRangeFilterTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeUsersMessageDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     {
         "Engine": str,
         "UserId": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2102,14 +2058,31 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
+NodeGroupConfigurationUnionTypeDef = Union[
+    NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef
+]
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2289,45 +2262,43 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
+DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
+    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
+        "ServiceUpdateName": str,
+        "ReplicationGroupIds": Sequence[str],
+        "CacheClusterIds": Sequence[str],
         "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
+        "UpdateActionStatus": Sequence[UpdateActionStatusType],
+        "ShowNodeLevelUpdateStatus": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
+    "DescribeUpdateActionsMessageRequestTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ReplicationGroupIds": Sequence[str],
+        "CacheClusterIds": Sequence[str],
+        "Engine": str,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
+        "UpdateActionStatus": Sequence[UpdateActionStatusType],
+        "ShowNodeLevelUpdateStatus": bool,
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
 LogDeliveryConfigurationRequestTypeDef = TypedDict(
     "LogDeliveryConfigurationRequestTypeDef",
     {
@@ -2457,14 +2428,49 @@
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2537,47 +2543,14 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalCreateCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2638,17 +2611,15 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[
-            Union[NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef]
-        ],
+        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationUnionTypeDef],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2801,14 +2772,47 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/type_defs.pyi` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_elasticache.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -73,16 +73,14 @@
     "ParameterTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationOutputTypeDef",
-    "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
@@ -95,22 +93,21 @@
     "DescribeCacheClustersMessageRequestTypeDef",
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
     "DescribeCacheParametersMessageRequestTypeDef",
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     "DescribeReplicationGroupsMessageRequestTypeDef",
     "DescribeReservedCacheNodesMessageRequestTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
     "DescribeServiceUpdatesMessageRequestTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
-    "TimeRangeFilterTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
@@ -119,14 +116,16 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationOutputTypeDef",
+    "NodeGroupConfigurationTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -158,46 +157,47 @@
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
-    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
     "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
     "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
     "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
     "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
     "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
-    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
-    "DescribeUpdateActionsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "TimeRangeFilterTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
+    "NodeSnapshotTypeDef",
+    "NodeGroupConfigurationUnionTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
@@ -207,45 +207,47 @@
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
-    "SnapshotTypeDef",
+    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
+    "DescribeUpdateActionsMessageRequestTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
+    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -545,42 +547,14 @@
 
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-NodeGroupConfigurationOutputTypeDef = TypedDict(
-    "NodeGroupConfigurationOutputTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
-NodeGroupConfigurationTypeDef = TypedDict(
-    "NodeGroupConfigurationTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": Sequence[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": Sequence[str],
-    },
-    total=False,
-)
-
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
     },
     total=False,
@@ -813,28 +787,15 @@
 
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeGlobalReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowMemberInfo": bool,
@@ -902,23 +863,14 @@
         "Marker": str,
         "MaxRecords": int,
         "ShowNodeGroupConfig": bool,
     },
     total=False,
 )
 
-TimeRangeFilterTypeDef = TypedDict(
-    "TimeRangeFilterTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 DescribeUserGroupsMessageRequestTypeDef = TypedDict(
     "DescribeUserGroupsMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1096,14 +1048,42 @@
 )
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
+NodeGroupConfigurationOutputTypeDef = TypedDict(
+    "NodeGroupConfigurationOutputTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
+NodeGroupConfigurationTypeDef = TypedDict(
+    "NodeGroupConfigurationTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": Sequence[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": Sequence[str],
+    },
+    total=False,
+)
+
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1637,28 +1617,14 @@
 
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -1798,27 +1764,14 @@
 
 class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "ShowMemberInfo": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1889,47 +1842,50 @@
     {
         "UserGroupId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
-    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
-        "ServiceUpdateName": str,
-        "ReplicationGroupIds": Sequence[str],
-        "CacheClusterIds": Sequence[str],
-        "Engine": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
-        "UpdateActionStatus": Sequence[UpdateActionStatusType],
-        "ShowNodeLevelUpdateStatus": bool,
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
-    "DescribeUpdateActionsMessageRequestTypeDef",
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
     {
-        "ServiceUpdateName": str,
-        "ReplicationGroupIds": Sequence[str],
-        "CacheClusterIds": Sequence[str],
-        "Engine": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
-        "UpdateActionStatus": Sequence[UpdateActionStatusType],
-        "ShowNodeLevelUpdateStatus": bool,
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+TimeRangeFilterTypeDef = TypedDict(
+    "TimeRangeFilterTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeUsersMessageDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     {
         "Engine": str,
         "UserId": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2045,14 +2001,31 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
+NodeGroupConfigurationUnionTypeDef = Union[
+    NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef
+]
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2232,45 +2205,43 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
+DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
+    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
+        "ServiceUpdateName": str,
+        "ReplicationGroupIds": Sequence[str],
+        "CacheClusterIds": Sequence[str],
         "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
+        "UpdateActionStatus": Sequence[UpdateActionStatusType],
+        "ShowNodeLevelUpdateStatus": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
+    "DescribeUpdateActionsMessageRequestTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ReplicationGroupIds": Sequence[str],
+        "CacheClusterIds": Sequence[str],
+        "Engine": str,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
+        "UpdateActionStatus": Sequence[UpdateActionStatusType],
+        "ShowNodeLevelUpdateStatus": bool,
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
 LogDeliveryConfigurationRequestTypeDef = TypedDict(
     "LogDeliveryConfigurationRequestTypeDef",
     {
@@ -2398,14 +2369,49 @@
 
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2478,47 +2484,14 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalCreateCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2577,17 +2550,15 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[
-            Union[NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef]
-        ],
+        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationUnionTypeDef],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2734,14 +2705,47 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/waiter.py` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/waiter.pyi` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/PKG-INFO` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ElastiCache 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 elasticache type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 elasticache type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
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
@@ -456,20 +456,20 @@
 )
 
 
 def check_value(value: AZModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
@@ -488,16 +488,14 @@
     ParameterTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
-    NodeGroupConfigurationOutputTypeDef,
-    NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     DeleteCacheClusterMessageRequestTypeDef,
     DeleteCacheParameterGroupMessageRequestTypeDef,
     DeleteCacheSecurityGroupMessageRequestTypeDef,
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
@@ -510,22 +508,21 @@
     DescribeCacheClustersMessageRequestTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
+    TimestampTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
-    TimeRangeFilterTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
@@ -534,14 +531,16 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
+    NodeGroupConfigurationTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
@@ -573,46 +572,47 @@
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
-    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
     DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
     DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
-    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
-    DescribeUpdateActionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    TimeRangeFilterTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
+    NodeSnapshotTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
     UpdateActionResultsMessageTypeDef,
@@ -622,45 +622,47 @@
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
-    SnapshotTypeDef,
+    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
+    DescribeUpdateActionsMessageRequestTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
+    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ReplicationGroupPendingModifiedValuesTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
@@ -677,15 +679,15 @@
     ModifyReplicationGroupShardConfigurationResultTypeDef,
     ReplicationGroupMessageTypeDef,
     StartMigrationResponseTypeDef,
     TestFailoverResultTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/SOURCES.txt` & `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15.post1/setup.py` & `mypy-boto3-elasticache-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticache",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.ElastiCache 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 elasticache type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 elasticache type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_elasticache": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

