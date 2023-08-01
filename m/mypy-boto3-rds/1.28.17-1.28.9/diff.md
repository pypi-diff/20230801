# Comparing `tmp/mypy-boto3-rds-1.28.17.tar.gz` & `tmp/mypy-boto3-rds-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rds-1.28.17.tar", last modified: Tue Aug  1 19:33:25 2023, max compression
+gzip compressed data, was "mypy-boto3-rds-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-rds-1.28.17.tar` & `mypy-boto3-rds-1.28.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.435422 mypy-boto3-rds-1.28.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 19:32:39.000000 mypy-boto3-rds-1.28.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41645 2023-08-01 19:33:25.435422 mypy-boto3-rds-1.28.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40177 2023-08-01 19:32:39.000000 mypy-boto3-rds-1.28.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.435422 mypy-boto3-rds-1.28.17/mypy_boto3_rds/
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-08-01 19:32:39.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-08-01 19:32:39.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 19:32:39.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   146049 2023-08-01 19:32:40.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   145854 2023-08-01 19:32:39.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18039 2023-08-01 19:32:42.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-08-01 19:32:41.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    45265 2023-08-01 19:32:41.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    45228 2023-08-01 19:32:41.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:32:39.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   194519 2023-08-01 19:32:46.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   194342 2023-08-01 19:32:44.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 19:32:39.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-08-01 19:32:41.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-08-01 19:32:41.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.435422 mypy-boto3-rds-1.28.17/mypy_boto3_rds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41645 2023-08-01 19:33:25.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 19:33:25.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:33:25.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:33:25.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 19:33:25.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 19:33:25.000000 mypy-boto3-rds-1.28.17/mypy_boto3_rds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:33:25.435422 mypy-boto3-rds-1.28.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 19:32:39.000000 mypy-boto3-rds-1.28.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-rds-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:32:38.000000 mypy-boto3-rds-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41451 2023-07-21 20:32:58.243903 mypy-boto3-rds-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39982 2023-07-21 20:32:38.000000 mypy-boto3-rds-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.227903 mypy-boto3-rds-1.28.9/mypy_boto3_rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-21 20:32:38.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-21 20:32:38.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-21 20:32:38.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144266 2023-07-21 20:32:40.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144073 2023-07-21 20:32:38.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-07-21 20:32:40.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-07-21 20:32:40.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    45248 2023-07-21 20:32:40.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45211 2023-07-21 20:32:40.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:38.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   191017 2023-07-21 20:32:46.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190840 2023-07-21 20:32:43.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:32:38.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-07-21 20:32:40.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-07-21 20:32:40.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41451 2023-07-21 20:32:58.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 20:32:58.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 20:32:58.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 20:32:58.000000 mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.243903 mypy-boto3-rds-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 20:32:37.000000 mypy-boto3-rds-1.28.9/setup.py
```

### Comparing `mypy-boto3-rds-1.28.17/LICENSE` & `mypy-boto3-rds-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.17/PKG-INFO` & `mypy-boto3-rds-1.28.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.28.17
-Summary: Type annotations for boto3.RDS 1.28.17 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.9
+Summary: Type annotations for boto3.RDS 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rds type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 rds type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rds"></a>
 
 # mypy-boto3-rds
 
 [![PyPI - mypy-boto3-rds](https://img.shields.io/pypi/v/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rds?color=blue)](https://pypistats.org/packages/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
 [mypy-boto3-rds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/).
 
 See how it helps to find and fix potential bugs:
 
@@ -76,15 +76,15 @@
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
@@ -562,15 +562,14 @@
     DescribeReservedDBInstancesPaginatorName,
     DescribeSourceRegionsPaginatorName,
     DownloadDBLogFilePortionPaginatorName,
     EngineFamilyType,
     ExportSourceTypeType,
     FailoverStatusType,
     IAMAuthModeType,
-    LocalWriteForwardingStatusType,
     ReplicaModeType,
     SourceTypeType,
     TargetHealthReasonType,
     TargetRoleType,
     TargetStateType,
     TargetTypeType,
     WriteForwardingStatusType,
@@ -583,37 +582,38 @@
 )
 
 
 def check_value(value: ActivityStreamModeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_rds.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rds.type_defs import (
     AccountQuotaTypeDef,
     ResponseMetadataTypeDef,
     AddRoleToDBClusterMessageRequestTypeDef,
     AddRoleToDBInstanceMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     AvailableProcessorFeatureTypeDef,
-    TimestampTypeDef,
+    BacktrackDBClusterMessageRequestTypeDef,
     BlueGreenDeploymentTaskTypeDef,
     SwitchoverDetailTypeDef,
+    TagOutputTypeDef,
     CancelExportTaskMessageRequestTypeDef,
     CertificateDetailsTypeDef,
     CertificateTypeDef,
     CharacterSetTypeDef,
     ClientGenerateDbAuthTokenRequestTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
@@ -624,15 +624,14 @@
     ScalingConfigurationTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     ProcessorFeatureTypeDef,
     DBProxyEndpointTypeDef,
     UserAuthConfigTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     CustomDBEngineVersionAMITypeDef,
-    RestoreWindowTypeDef,
     DBClusterBacktrackTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
     ParameterOutputTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
@@ -640,28 +639,29 @@
     MasterUserSecretTypeDef,
     ScalingConfigurationInfoTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceAutomatedBackupsReplicationTypeDef,
+    RestoreWindowTypeDef,
     DBInstanceRoleTypeDef,
     DBInstanceStatusInfoTypeDef,
     DBParameterGroupStatusTypeDef,
     DBSecurityGroupMembershipTypeDef,
     EndpointTypeDef,
     OptionGroupMembershipTypeDef,
+    ProcessorFeatureOutputTypeDef,
     TargetHealthTypeDef,
     UserAuthConfigInfoTypeDef,
     EC2SecurityGroupTypeDef,
     IPRangeTypeDef,
     DBSnapshotAttributeTypeDef,
     DeleteBlueGreenDeploymentRequestRequestTypeDef,
     DeleteCustomDBEngineVersionMessageRequestTypeDef,
-    DeleteDBClusterAutomatedBackupMessageRequestTypeDef,
     DeleteDBClusterEndpointMessageRequestTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceAutomatedBackupMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBParameterGroupMessageRequestTypeDef,
@@ -692,25 +692,26 @@
     GlobalClusterMemberTypeDef,
     MinimumEngineVersionPerAllowedValueTypeDef,
     ModifyActivityStreamRequestRequestTypeDef,
     ModifyCertificatesMessageRequestTypeDef,
     ModifyCurrentDBClusterCapacityMessageRequestTypeDef,
     ModifyCustomDBEngineVersionMessageRequestTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBProxyEndpointRequestRequestTypeDef,
     ModifyDBSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSnapshotMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     OptionSettingTypeDef,
     OptionVersionTypeDef,
+    OptionSettingOutputTypeDef,
     OutpostTypeDef,
-    ParameterTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
     PromoteReadReplicaMessageRequestTypeDef,
     RangeTypeDef,
     RebootDBClusterMessageRequestTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RecurringChargeTypeDef,
@@ -730,22 +731,22 @@
     StopActivityStreamRequestRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     StopDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
     StopDBInstanceMessageRequestTypeDef,
     SwitchoverBlueGreenDeploymentRequestRequestTypeDef,
     SwitchoverReadReplicaMessageRequestTypeDef,
     AccountAttributesMessageTypeDef,
-    DBClusterBacktrackResponseTypeDef,
+    DBClusterBacktrackResponseMetadataTypeDef,
     DBClusterCapacityInfoTypeDef,
-    DBClusterEndpointResponseTypeDef,
+    DBClusterEndpointResponseMetadataTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DBParameterGroupNameMessageTypeDef,
     DownloadDBLogFilePortionDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
-    ExportTaskResponseTypeDef,
+    ExportTaskResponseMetadataTypeDef,
     ModifyActivityStreamResponseTypeDef,
     StartActivityStreamResponseTypeDef,
     StopActivityStreamResponseTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EventSubscriptionsMessageTypeDef,
@@ -765,20 +766,19 @@
     CreateDBParameterGroupMessageRequestTypeDef,
     CreateDBProxyEndpointRequestRequestTypeDef,
     CreateDBSecurityGroupMessageRequestTypeDef,
     CreateDBSnapshotMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateOptionGroupMessageRequestTypeDef,
-    DBClusterSnapshotTypeDef,
     PurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
-    BacktrackDBClusterMessageRequestTypeDef,
     BlueGreenDeploymentTypeDef,
+    DBClusterSnapshotTypeDef,
+    TagListMessageTypeDef,
     CertificateMessageTypeDef,
     ModifyCertificatesResultTypeDef,
     ClusterPendingModifiedValuesTypeDef,
     DBProxyTargetGroupTypeDef,
     ModifyDBProxyTargetGroupRequestRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -789,43 +789,41 @@
     CreateDBClusterMessageRequestTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromS3MessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBInstanceReadReplicaMessageRequestTypeDef,
-    DBSnapshotTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
-    PendingModifiedValuesTypeDef,
     RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
     RestoreDBInstanceFromS3MessageRequestTypeDef,
     RestoreDBInstanceToPointInTimeMessageRequestTypeDef,
     CreateDBProxyEndpointResponseTypeDef,
     DeleteDBProxyEndpointResponseTypeDef,
     DescribeDBProxyEndpointsResponseTypeDef,
     ModifyDBProxyEndpointResponseTypeDef,
     CreateDBProxyRequestRequestTypeDef,
     ModifyDBProxyRequestRequestTypeDef,
-    DBClusterAutomatedBackupTypeDef,
     DBClusterBacktrackMessageTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
-    DBEngineVersionResponseTypeDef,
+    DBEngineVersionResponseMetadataTypeDef,
     DBEngineVersionTypeDef,
     DBInstanceAutomatedBackupTypeDef,
+    DBSnapshotTypeDef,
+    PendingModifiedValuesTypeDef,
     DBProxyTargetTypeDef,
     DBProxyTypeDef,
     DBSecurityGroupTypeDef,
     DBSnapshotAttributesResultTypeDef,
     DescribeBlueGreenDeploymentsRequestRequestTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
-    DescribeDBClusterAutomatedBackupsMessageRequestTypeDef,
     DescribeDBClusterBacktracksMessageRequestTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
@@ -902,51 +900,52 @@
     DescribeDBSnapshotsMessageDBSnapshotDeletedWaitTypeDef,
     DescribeDBLogFilesResponseTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     ExportTasksMessageTypeDef,
     GlobalClusterTypeDef,
     OptionGroupOptionSettingTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ModifyDBParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBParameterGroupMessageRequestTypeDef,
     OptionConfigurationTypeDef,
     OptionTypeDef,
     SubnetTypeDef,
-    ParameterUnionTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
     ReservedDBInstanceTypeDef,
     ReservedDBInstancesOfferingTypeDef,
     SourceRegionMessageTypeDef,
-    CopyDBClusterSnapshotResultTypeDef,
-    CreateDBClusterSnapshotResultTypeDef,
-    DBClusterSnapshotMessageTypeDef,
-    DeleteDBClusterSnapshotResultTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     CreateBlueGreenDeploymentResponseTypeDef,
     DeleteBlueGreenDeploymentResponseTypeDef,
     DescribeBlueGreenDeploymentsResponseTypeDef,
     SwitchoverBlueGreenDeploymentResponseTypeDef,
+    CopyDBClusterSnapshotResultTypeDef,
+    CreateDBClusterSnapshotResultTypeDef,
+    DBClusterSnapshotMessageTypeDef,
+    DeleteDBClusterSnapshotResultTypeDef,
     DBClusterTypeDef,
     DescribeDBProxyTargetGroupsResponseTypeDef,
     ModifyDBProxyTargetGroupResponseTypeDef,
-    CopyDBSnapshotResultTypeDef,
-    CreateDBSnapshotResultTypeDef,
-    DBSnapshotMessageTypeDef,
-    DeleteDBSnapshotResultTypeDef,
-    ModifyDBSnapshotResultTypeDef,
-    DBClusterAutomatedBackupMessageTypeDef,
-    DeleteDBClusterAutomatedBackupResultTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
     DBEngineVersionMessageTypeDef,
     DBInstanceAutomatedBackupMessageTypeDef,
     DeleteDBInstanceAutomatedBackupResultTypeDef,
     StartDBInstanceAutomatedBackupsReplicationResultTypeDef,
     StopDBInstanceAutomatedBackupsReplicationResultTypeDef,
+    CopyDBSnapshotResultTypeDef,
+    CreateDBSnapshotResultTypeDef,
+    DBSnapshotMessageTypeDef,
+    DeleteDBSnapshotResultTypeDef,
+    ModifyDBSnapshotResultTypeDef,
     DescribeDBProxyTargetsResponseTypeDef,
     RegisterDBProxyTargetsResponseTypeDef,
     CreateDBProxyResponseTypeDef,
     DeleteDBProxyResponseTypeDef,
     DescribeDBProxiesResponseTypeDef,
     ModifyDBProxyResponseTypeDef,
     AuthorizeDBSecurityGroupIngressResultTypeDef,
@@ -961,18 +960,14 @@
     GlobalClustersMessageTypeDef,
     ModifyGlobalClusterResultTypeDef,
     RemoveFromGlobalClusterResultTypeDef,
     OptionGroupOptionTypeDef,
     ModifyOptionGroupMessageRequestTypeDef,
     OptionGroupTypeDef,
     DBSubnetGroupTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ModifyDBParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBParameterGroupMessageRequestTypeDef,
     ApplyPendingMaintenanceActionResultTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ValidDBInstanceModificationsMessageTypeDef,
     PurchaseReservedDBInstancesOfferingResultTypeDef,
     ReservedDBInstanceMessageTypeDef,
     ReservedDBInstancesOfferingMessageTypeDef,
     CreateDBClusterResultTypeDef,
@@ -1009,15 +1004,15 @@
     RestoreDBInstanceToPointInTimeResultTypeDef,
     StartDBInstanceResultTypeDef,
     StopDBInstanceResultTypeDef,
     SwitchoverReadReplicaResultTypeDef,
 )
 
 
-def get_value() -> AccountQuotaTypeDef:
+def get_structure() -> AccountQuotaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rds-1.28.17/README.md` & `mypy-boto3-rds-1.28.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-rds"></a>
 
 # mypy-boto3-rds
 
 [![PyPI - mypy-boto3-rds](https://img.shields.io/pypi/v/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rds?color=blue)](https://pypistats.org/packages/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
 [mypy-boto3-rds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/).
 
 See how it helps to find and fix potential bugs:
 
@@ -44,15 +44,15 @@
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
@@ -530,15 +530,14 @@
     DescribeReservedDBInstancesPaginatorName,
     DescribeSourceRegionsPaginatorName,
     DownloadDBLogFilePortionPaginatorName,
     EngineFamilyType,
     ExportSourceTypeType,
     FailoverStatusType,
     IAMAuthModeType,
-    LocalWriteForwardingStatusType,
     ReplicaModeType,
     SourceTypeType,
     TargetHealthReasonType,
     TargetRoleType,
     TargetStateType,
     TargetTypeType,
     WriteForwardingStatusType,
@@ -551,37 +550,38 @@
 )
 
 
 def check_value(value: ActivityStreamModeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_rds.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rds.type_defs import (
     AccountQuotaTypeDef,
     ResponseMetadataTypeDef,
     AddRoleToDBClusterMessageRequestTypeDef,
     AddRoleToDBInstanceMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     AvailableProcessorFeatureTypeDef,
-    TimestampTypeDef,
+    BacktrackDBClusterMessageRequestTypeDef,
     BlueGreenDeploymentTaskTypeDef,
     SwitchoverDetailTypeDef,
+    TagOutputTypeDef,
     CancelExportTaskMessageRequestTypeDef,
     CertificateDetailsTypeDef,
     CertificateTypeDef,
     CharacterSetTypeDef,
     ClientGenerateDbAuthTokenRequestTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
@@ -592,15 +592,14 @@
     ScalingConfigurationTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     ProcessorFeatureTypeDef,
     DBProxyEndpointTypeDef,
     UserAuthConfigTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     CustomDBEngineVersionAMITypeDef,
-    RestoreWindowTypeDef,
     DBClusterBacktrackTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
     ParameterOutputTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
@@ -608,28 +607,29 @@
     MasterUserSecretTypeDef,
     ScalingConfigurationInfoTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceAutomatedBackupsReplicationTypeDef,
+    RestoreWindowTypeDef,
     DBInstanceRoleTypeDef,
     DBInstanceStatusInfoTypeDef,
     DBParameterGroupStatusTypeDef,
     DBSecurityGroupMembershipTypeDef,
     EndpointTypeDef,
     OptionGroupMembershipTypeDef,
+    ProcessorFeatureOutputTypeDef,
     TargetHealthTypeDef,
     UserAuthConfigInfoTypeDef,
     EC2SecurityGroupTypeDef,
     IPRangeTypeDef,
     DBSnapshotAttributeTypeDef,
     DeleteBlueGreenDeploymentRequestRequestTypeDef,
     DeleteCustomDBEngineVersionMessageRequestTypeDef,
-    DeleteDBClusterAutomatedBackupMessageRequestTypeDef,
     DeleteDBClusterEndpointMessageRequestTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceAutomatedBackupMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBParameterGroupMessageRequestTypeDef,
@@ -660,25 +660,26 @@
     GlobalClusterMemberTypeDef,
     MinimumEngineVersionPerAllowedValueTypeDef,
     ModifyActivityStreamRequestRequestTypeDef,
     ModifyCertificatesMessageRequestTypeDef,
     ModifyCurrentDBClusterCapacityMessageRequestTypeDef,
     ModifyCustomDBEngineVersionMessageRequestTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBProxyEndpointRequestRequestTypeDef,
     ModifyDBSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSnapshotMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     OptionSettingTypeDef,
     OptionVersionTypeDef,
+    OptionSettingOutputTypeDef,
     OutpostTypeDef,
-    ParameterTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
     PromoteReadReplicaMessageRequestTypeDef,
     RangeTypeDef,
     RebootDBClusterMessageRequestTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RecurringChargeTypeDef,
@@ -698,22 +699,22 @@
     StopActivityStreamRequestRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     StopDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
     StopDBInstanceMessageRequestTypeDef,
     SwitchoverBlueGreenDeploymentRequestRequestTypeDef,
     SwitchoverReadReplicaMessageRequestTypeDef,
     AccountAttributesMessageTypeDef,
-    DBClusterBacktrackResponseTypeDef,
+    DBClusterBacktrackResponseMetadataTypeDef,
     DBClusterCapacityInfoTypeDef,
-    DBClusterEndpointResponseTypeDef,
+    DBClusterEndpointResponseMetadataTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DBParameterGroupNameMessageTypeDef,
     DownloadDBLogFilePortionDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
-    ExportTaskResponseTypeDef,
+    ExportTaskResponseMetadataTypeDef,
     ModifyActivityStreamResponseTypeDef,
     StartActivityStreamResponseTypeDef,
     StopActivityStreamResponseTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EventSubscriptionsMessageTypeDef,
@@ -733,20 +734,19 @@
     CreateDBParameterGroupMessageRequestTypeDef,
     CreateDBProxyEndpointRequestRequestTypeDef,
     CreateDBSecurityGroupMessageRequestTypeDef,
     CreateDBSnapshotMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateOptionGroupMessageRequestTypeDef,
-    DBClusterSnapshotTypeDef,
     PurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
-    BacktrackDBClusterMessageRequestTypeDef,
     BlueGreenDeploymentTypeDef,
+    DBClusterSnapshotTypeDef,
+    TagListMessageTypeDef,
     CertificateMessageTypeDef,
     ModifyCertificatesResultTypeDef,
     ClusterPendingModifiedValuesTypeDef,
     DBProxyTargetGroupTypeDef,
     ModifyDBProxyTargetGroupRequestRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -757,43 +757,41 @@
     CreateDBClusterMessageRequestTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromS3MessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBInstanceReadReplicaMessageRequestTypeDef,
-    DBSnapshotTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
-    PendingModifiedValuesTypeDef,
     RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
     RestoreDBInstanceFromS3MessageRequestTypeDef,
     RestoreDBInstanceToPointInTimeMessageRequestTypeDef,
     CreateDBProxyEndpointResponseTypeDef,
     DeleteDBProxyEndpointResponseTypeDef,
     DescribeDBProxyEndpointsResponseTypeDef,
     ModifyDBProxyEndpointResponseTypeDef,
     CreateDBProxyRequestRequestTypeDef,
     ModifyDBProxyRequestRequestTypeDef,
-    DBClusterAutomatedBackupTypeDef,
     DBClusterBacktrackMessageTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
-    DBEngineVersionResponseTypeDef,
+    DBEngineVersionResponseMetadataTypeDef,
     DBEngineVersionTypeDef,
     DBInstanceAutomatedBackupTypeDef,
+    DBSnapshotTypeDef,
+    PendingModifiedValuesTypeDef,
     DBProxyTargetTypeDef,
     DBProxyTypeDef,
     DBSecurityGroupTypeDef,
     DBSnapshotAttributesResultTypeDef,
     DescribeBlueGreenDeploymentsRequestRequestTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
-    DescribeDBClusterAutomatedBackupsMessageRequestTypeDef,
     DescribeDBClusterBacktracksMessageRequestTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
@@ -870,51 +868,52 @@
     DescribeDBSnapshotsMessageDBSnapshotDeletedWaitTypeDef,
     DescribeDBLogFilesResponseTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     ExportTasksMessageTypeDef,
     GlobalClusterTypeDef,
     OptionGroupOptionSettingTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ModifyDBParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBParameterGroupMessageRequestTypeDef,
     OptionConfigurationTypeDef,
     OptionTypeDef,
     SubnetTypeDef,
-    ParameterUnionTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
     ReservedDBInstanceTypeDef,
     ReservedDBInstancesOfferingTypeDef,
     SourceRegionMessageTypeDef,
-    CopyDBClusterSnapshotResultTypeDef,
-    CreateDBClusterSnapshotResultTypeDef,
-    DBClusterSnapshotMessageTypeDef,
-    DeleteDBClusterSnapshotResultTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     CreateBlueGreenDeploymentResponseTypeDef,
     DeleteBlueGreenDeploymentResponseTypeDef,
     DescribeBlueGreenDeploymentsResponseTypeDef,
     SwitchoverBlueGreenDeploymentResponseTypeDef,
+    CopyDBClusterSnapshotResultTypeDef,
+    CreateDBClusterSnapshotResultTypeDef,
+    DBClusterSnapshotMessageTypeDef,
+    DeleteDBClusterSnapshotResultTypeDef,
     DBClusterTypeDef,
     DescribeDBProxyTargetGroupsResponseTypeDef,
     ModifyDBProxyTargetGroupResponseTypeDef,
-    CopyDBSnapshotResultTypeDef,
-    CreateDBSnapshotResultTypeDef,
-    DBSnapshotMessageTypeDef,
-    DeleteDBSnapshotResultTypeDef,
-    ModifyDBSnapshotResultTypeDef,
-    DBClusterAutomatedBackupMessageTypeDef,
-    DeleteDBClusterAutomatedBackupResultTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
     DBEngineVersionMessageTypeDef,
     DBInstanceAutomatedBackupMessageTypeDef,
     DeleteDBInstanceAutomatedBackupResultTypeDef,
     StartDBInstanceAutomatedBackupsReplicationResultTypeDef,
     StopDBInstanceAutomatedBackupsReplicationResultTypeDef,
+    CopyDBSnapshotResultTypeDef,
+    CreateDBSnapshotResultTypeDef,
+    DBSnapshotMessageTypeDef,
+    DeleteDBSnapshotResultTypeDef,
+    ModifyDBSnapshotResultTypeDef,
     DescribeDBProxyTargetsResponseTypeDef,
     RegisterDBProxyTargetsResponseTypeDef,
     CreateDBProxyResponseTypeDef,
     DeleteDBProxyResponseTypeDef,
     DescribeDBProxiesResponseTypeDef,
     ModifyDBProxyResponseTypeDef,
     AuthorizeDBSecurityGroupIngressResultTypeDef,
@@ -929,18 +928,14 @@
     GlobalClustersMessageTypeDef,
     ModifyGlobalClusterResultTypeDef,
     RemoveFromGlobalClusterResultTypeDef,
     OptionGroupOptionTypeDef,
     ModifyOptionGroupMessageRequestTypeDef,
     OptionGroupTypeDef,
     DBSubnetGroupTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ModifyDBParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBParameterGroupMessageRequestTypeDef,
     ApplyPendingMaintenanceActionResultTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ValidDBInstanceModificationsMessageTypeDef,
     PurchaseReservedDBInstancesOfferingResultTypeDef,
     ReservedDBInstanceMessageTypeDef,
     ReservedDBInstancesOfferingMessageTypeDef,
     CreateDBClusterResultTypeDef,
@@ -977,15 +972,15 @@
     RestoreDBInstanceToPointInTimeResultTypeDef,
     StartDBInstanceResultTypeDef,
     StopDBInstanceResultTypeDef,
     SwitchoverReadReplicaResultTypeDef,
 )
 
 
-def get_value() -> AccountQuotaTypeDef:
+def get_structure() -> AccountQuotaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/__init__.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/__init__.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/__main__.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RDS 1.28.17\nVersion:         1.28.17\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.RDS 1.28.9\nVersion:         1.28.9\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.17")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/client.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_rds.client import RDSClient
 
     session = Session()
     client: RDSClient = session.client("rds")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Optional, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Optional, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActivityStreamModeType,
     AuditPolicyStateType,
     AutomationModeType,
@@ -90,37 +91,35 @@
     CreateDBProxyResponseTypeDef,
     CreateDBSecurityGroupResultTypeDef,
     CreateDBSnapshotResultTypeDef,
     CreateDBSubnetGroupResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateGlobalClusterResultTypeDef,
     CreateOptionGroupResultTypeDef,
-    DBClusterAutomatedBackupMessageTypeDef,
     DBClusterBacktrackMessageTypeDef,
-    DBClusterBacktrackResponseTypeDef,
+    DBClusterBacktrackResponseMetadataTypeDef,
     DBClusterCapacityInfoTypeDef,
     DBClusterEndpointMessageTypeDef,
-    DBClusterEndpointResponseTypeDef,
+    DBClusterEndpointResponseMetadataTypeDef,
     DBClusterMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DBClusterParameterGroupsMessageTypeDef,
     DBClusterSnapshotMessageTypeDef,
     DBEngineVersionMessageTypeDef,
-    DBEngineVersionResponseTypeDef,
+    DBEngineVersionResponseMetadataTypeDef,
     DBInstanceAutomatedBackupMessageTypeDef,
     DBInstanceMessageTypeDef,
     DBParameterGroupDetailsTypeDef,
     DBParameterGroupNameMessageTypeDef,
     DBParameterGroupsMessageTypeDef,
     DBSecurityGroupMessageTypeDef,
     DBSnapshotMessageTypeDef,
     DBSubnetGroupMessageTypeDef,
     DeleteBlueGreenDeploymentResponseTypeDef,
-    DeleteDBClusterAutomatedBackupResultTypeDef,
     DeleteDBClusterResultTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DeleteDBInstanceAutomatedBackupResultTypeDef,
     DeleteDBInstanceResultTypeDef,
     DeleteDBProxyEndpointResponseTypeDef,
     DeleteDBProxyResponseTypeDef,
     DeleteDBSnapshotResultTypeDef,
@@ -138,15 +137,15 @@
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeValidDBInstanceModificationsResultTypeDef,
     DownloadDBLogFilePortionDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
-    ExportTaskResponseTypeDef,
+    ExportTaskResponseMetadataTypeDef,
     ExportTasksMessageTypeDef,
     FailoverDBClusterResultTypeDef,
     FailoverGlobalClusterResultTypeDef,
     FilterTypeDef,
     GlobalClustersMessageTypeDef,
     ModifyActivityStreamResponseTypeDef,
     ModifyCertificatesResultTypeDef,
@@ -162,15 +161,15 @@
     ModifyEventSubscriptionResultTypeDef,
     ModifyGlobalClusterResultTypeDef,
     ModifyOptionGroupResultTypeDef,
     OptionConfigurationTypeDef,
     OptionGroupOptionsMessageTypeDef,
     OptionGroupsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
-    ParameterUnionTypeDef,
+    ParameterTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ProcessorFeatureTypeDef,
     PromoteReadReplicaDBClusterResultTypeDef,
     PromoteReadReplicaResultTypeDef,
     PurchaseReservedDBInstancesOfferingResultTypeDef,
     RebootDBClusterResultTypeDef,
     RebootDBInstanceResultTypeDef,
@@ -197,15 +196,14 @@
     StopDBClusterResultTypeDef,
     StopDBInstanceAutomatedBackupsReplicationResultTypeDef,
     StopDBInstanceResultTypeDef,
     SwitchoverBlueGreenDeploymentResponseTypeDef,
     SwitchoverReadReplicaResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
-    TimestampTypeDef,
     UserAuthConfigTypeDef,
 )
 from .waiter import (
     DBClusterAvailableWaiter,
     DBClusterDeletedWaiter,
     DBClusterSnapshotAvailableWaiter,
     DBClusterSnapshotDeletedWaiter,
@@ -244,16 +242,14 @@
     ClientError: Type[BotocoreClientError]
     CreateCustomDBEngineVersionFault: Type[BotocoreClientError]
     CustomAvailabilityZoneNotFoundFault: Type[BotocoreClientError]
     CustomDBEngineVersionAlreadyExistsFault: Type[BotocoreClientError]
     CustomDBEngineVersionNotFoundFault: Type[BotocoreClientError]
     CustomDBEngineVersionQuotaExceededFault: Type[BotocoreClientError]
     DBClusterAlreadyExistsFault: Type[BotocoreClientError]
-    DBClusterAutomatedBackupNotFoundFault: Type[BotocoreClientError]
-    DBClusterAutomatedBackupQuotaExceededFault: Type[BotocoreClientError]
     DBClusterBacktrackNotFoundFault: Type[BotocoreClientError]
     DBClusterEndpointAlreadyExistsFault: Type[BotocoreClientError]
     DBClusterEndpointNotFoundFault: Type[BotocoreClientError]
     DBClusterEndpointQuotaExceededFault: Type[BotocoreClientError]
     DBClusterNotFoundFault: Type[BotocoreClientError]
     DBClusterParameterGroupNotFoundFault: Type[BotocoreClientError]
     DBClusterQuotaExceededFault: Type[BotocoreClientError]
@@ -308,15 +304,14 @@
     InstanceQuotaExceededFault: Type[BotocoreClientError]
     InsufficientAvailableIPsInSubnetFault: Type[BotocoreClientError]
     InsufficientDBClusterCapacityFault: Type[BotocoreClientError]
     InsufficientDBInstanceCapacityFault: Type[BotocoreClientError]
     InsufficientStorageClusterCapacityFault: Type[BotocoreClientError]
     InvalidBlueGreenDeploymentStateFault: Type[BotocoreClientError]
     InvalidCustomDBEngineVersionStateFault: Type[BotocoreClientError]
-    InvalidDBClusterAutomatedBackupStateFault: Type[BotocoreClientError]
     InvalidDBClusterCapacityFault: Type[BotocoreClientError]
     InvalidDBClusterEndpointStateFault: Type[BotocoreClientError]
     InvalidDBClusterSnapshotStateFault: Type[BotocoreClientError]
     InvalidDBClusterStateFault: Type[BotocoreClientError]
     InvalidDBInstanceAutomatedBackupStateFault: Type[BotocoreClientError]
     InvalidDBInstanceStateFault: Type[BotocoreClientError]
     InvalidDBParameterGroupStateFault: Type[BotocoreClientError]
@@ -451,18 +446,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#authorize_db_security_group_ingress)
         """
 
     def backtrack_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
-        BacktrackTo: TimestampTypeDef,
+        BacktrackTo: Union[datetime, str],
         Force: bool = ...,
         UseEarliestTimeOnPointInTimeUnavailable: bool = ...
-    ) -> DBClusterBacktrackResponseTypeDef:
+    ) -> DBClusterBacktrackResponseMetadataTypeDef:
         """
         Backtracks a DB cluster to a specific time, without creating a new DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.backtrack_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#backtrack_db_cluster)
         """
 
@@ -470,15 +465,15 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#can_paginate)
         """
 
-    def cancel_export_task(self, *, ExportTaskIdentifier: str) -> ExportTaskResponseTypeDef:
+    def cancel_export_task(self, *, ExportTaskIdentifier: str) -> ExportTaskResponseMetadataTypeDef:
         """
         Cancels an export task in progress that is exporting a snapshot or cluster to
         Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.cancel_export_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#cancel_export_task)
         """
@@ -600,15 +595,15 @@
         DatabaseInstallationFilesS3BucketName: str = ...,
         DatabaseInstallationFilesS3Prefix: str = ...,
         ImageId: str = ...,
         KMSKeyId: str = ...,
         Description: str = ...,
         Manifest: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> DBEngineVersionResponseTypeDef:
+    ) -> DBEngineVersionResponseMetadataTypeDef:
         """
         Creates a custom DB engine version (CEV).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_custom_db_engine_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#create_custom_db_engine_version)
         """
 
@@ -660,15 +655,14 @@
         PerformanceInsightsKMSKeyId: str = ...,
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         DBSystemId: str = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
-        EnableLocalWriteForwarding: bool = ...,
         SourceRegion: str = ...
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon Aurora DB cluster or Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#create_db_cluster)
@@ -679,15 +673,15 @@
         *,
         DBClusterIdentifier: str,
         DBClusterEndpointIdentifier: str,
         EndpointType: str,
         StaticMembers: Sequence[str] = ...,
         ExcludedMembers: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> DBClusterEndpointResponseTypeDef:
+    ) -> DBClusterEndpointResponseMetadataTypeDef:
         """
         Creates a new custom endpoint and associates it with an Amazon Aurora DB
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#create_db_cluster_endpoint)
         """
@@ -1004,51 +998,39 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_blue_green_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_blue_green_deployment)
         """
 
     def delete_custom_db_engine_version(
         self, *, Engine: str, EngineVersion: str
-    ) -> DBEngineVersionResponseTypeDef:
+    ) -> DBEngineVersionResponseMetadataTypeDef:
         """
         Deletes a custom engine version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_custom_db_engine_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_custom_db_engine_version)
         """
 
     def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...,
-        DeleteAutomatedBackups: bool = ...
+        FinalDBSnapshotIdentifier: str = ...
     ) -> DeleteDBClusterResultTypeDef:
         """
         The DeleteDBCluster action deletes a previously provisioned DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_db_cluster)
         """
 
-    def delete_db_cluster_automated_backup(
-        self, *, DbClusterResourceId: str
-    ) -> DeleteDBClusterAutomatedBackupResultTypeDef:
-        """
-        Deletes automated backups using the `DbClusterResourceId` value of the source DB
-        cluster or the Amazon Resource Name (ARN) of the automated backups.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster_automated_backup)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_db_cluster_automated_backup)
-        """
-
     def delete_db_cluster_endpoint(
         self, *, DBClusterEndpointIdentifier: str
-    ) -> DBClusterEndpointResponseTypeDef:
+    ) -> DBClusterEndpointResponseMetadataTypeDef:
         """
         Deletes a custom endpoint and removes it from an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_db_cluster_endpoint)
         """
 
@@ -1229,30 +1211,14 @@
         Lists the set of CA certificates provided by Amazon RDS for this Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#describe_certificates)
         """
 
-    def describe_db_cluster_automated_backups(
-        self,
-        *,
-        DbClusterResourceId: str = ...,
-        DBClusterIdentifier: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...,
-        MaxRecords: int = ...,
-        Marker: str = ...
-    ) -> DBClusterAutomatedBackupMessageTypeDef:
-        """
-        Displays backups for both current and deleted DB clusters.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_automated_backups)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#describe_db_cluster_automated_backups)
-        """
-
     def describe_db_cluster_backtracks(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
@@ -1329,16 +1295,15 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...
+        IncludePublic: bool = ...
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about DB cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#describe_db_cluster_snapshots)
         """
@@ -1645,16 +1610,16 @@
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
@@ -1949,15 +1914,15 @@
     def modify_custom_db_engine_version(
         self,
         *,
         Engine: str,
         EngineVersion: str,
         Description: str = ...,
         Status: CustomEngineVersionStatusType = ...
-    ) -> DBEngineVersionResponseTypeDef:
+    ) -> DBEngineVersionResponseMetadataTypeDef:
         """
         Modifies the status of a custom engine version (CEV).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_custom_db_engine_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_custom_db_engine_version)
         """
 
@@ -2000,16 +1965,15 @@
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         ManageMasterUserPassword: bool = ...,
         RotateMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         EngineMode: str = ...,
-        AllowEngineModeChange: bool = ...,
-        EnableLocalWriteForwarding: bool = ...
+        AllowEngineModeChange: bool = ...
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies the settings of an Amazon Aurora DB cluster or a Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster)
         """
@@ -2017,24 +1981,24 @@
     def modify_db_cluster_endpoint(
         self,
         *,
         DBClusterEndpointIdentifier: str,
         EndpointType: str = ...,
         StaticMembers: Sequence[str] = ...,
         ExcludedMembers: Sequence[str] = ...
-    ) -> DBClusterEndpointResponseTypeDef:
+    ) -> DBClusterEndpointResponseMetadataTypeDef:
         """
         Modifies the properties of an endpoint in an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster_endpoint)
         """
 
     def modify_db_cluster_parameter_group(
-        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
+        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster_parameter_group)
         """
@@ -2121,15 +2085,15 @@
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_instance)
         """
 
     def modify_db_parameter_group(
-        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
+        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_parameter_group)
         """
@@ -2244,15 +2208,15 @@
         GlobalClusterIdentifier: str = ...,
         NewGlobalClusterIdentifier: str = ...,
         DeletionProtection: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...
     ) -> ModifyGlobalClusterResultTypeDef:
         """
-        Modifies a setting for an Amazon Aurora global cluster.
+        Modify a setting for an Amazon Aurora global cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_global_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_global_cluster)
         """
 
     def modify_option_group(
         self,
@@ -2396,29 +2360,29 @@
         """
 
     def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterUnionTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_cluster_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#reset_db_cluster_parameter_group)
         """
 
     def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterUnionTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#reset_db_parameter_group)
@@ -2511,17 +2475,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#restore_db_cluster_from_snapshot)
         """
 
     def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
+        SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
-        SourceDBClusterIdentifier: str = ...,
-        RestoreToTime: TimestampTypeDef = ...,
+        RestoreToTime: Union[datetime, str] = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
@@ -2536,16 +2500,15 @@
         ScalingConfiguration: ScalingConfigurationTypeDef = ...,
         EngineMode: str = ...,
         DBClusterInstanceClass: str = ...,
         StorageType: str = ...,
         PubliclyAccessible: bool = ...,
         Iops: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        NetworkType: str = ...,
-        SourceDbClusterResourceId: str = ...
+        NetworkType: str = ...
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a DB cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_to_point_in_time)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#restore_db_cluster_to_point_in_time)
         """
@@ -2661,15 +2624,15 @@
         """
 
     def restore_db_instance_to_point_in_time(
         self,
         *,
         TargetDBInstanceIdentifier: str,
         SourceDBInstanceIdentifier: str = ...,
-        RestoreTime: TimestampTypeDef = ...,
+        RestoreTime: Union[datetime, str] = ...,
         UseLatestRestorableTime: bool = ...,
         DBInstanceClass: str = ...,
         Port: int = ...,
         AvailabilityZone: str = ...,
         DBSubnetGroupName: str = ...,
         MultiAZ: bool = ...,
         PubliclyAccessible: bool = ...,
@@ -2788,15 +2751,15 @@
         ExportTaskIdentifier: str,
         SourceArn: str,
         S3BucketName: str,
         IamRoleArn: str,
         KmsKeyId: str,
         S3Prefix: str = ...,
         ExportOnly: Sequence[str] = ...
-    ) -> ExportTaskResponseTypeDef:
+    ) -> ExportTaskResponseMetadataTypeDef:
         """
         Starts an export of DB snapshot or DB cluster data to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.start_export_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#start_export_task)
         """
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/client.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_rds.client import RDSClient
 
     session = Session()
     client: RDSClient = session.client("rds")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Optional, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Optional, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActivityStreamModeType,
     AuditPolicyStateType,
     AutomationModeType,
@@ -90,37 +91,35 @@
     CreateDBProxyResponseTypeDef,
     CreateDBSecurityGroupResultTypeDef,
     CreateDBSnapshotResultTypeDef,
     CreateDBSubnetGroupResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateGlobalClusterResultTypeDef,
     CreateOptionGroupResultTypeDef,
-    DBClusterAutomatedBackupMessageTypeDef,
     DBClusterBacktrackMessageTypeDef,
-    DBClusterBacktrackResponseTypeDef,
+    DBClusterBacktrackResponseMetadataTypeDef,
     DBClusterCapacityInfoTypeDef,
     DBClusterEndpointMessageTypeDef,
-    DBClusterEndpointResponseTypeDef,
+    DBClusterEndpointResponseMetadataTypeDef,
     DBClusterMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DBClusterParameterGroupsMessageTypeDef,
     DBClusterSnapshotMessageTypeDef,
     DBEngineVersionMessageTypeDef,
-    DBEngineVersionResponseTypeDef,
+    DBEngineVersionResponseMetadataTypeDef,
     DBInstanceAutomatedBackupMessageTypeDef,
     DBInstanceMessageTypeDef,
     DBParameterGroupDetailsTypeDef,
     DBParameterGroupNameMessageTypeDef,
     DBParameterGroupsMessageTypeDef,
     DBSecurityGroupMessageTypeDef,
     DBSnapshotMessageTypeDef,
     DBSubnetGroupMessageTypeDef,
     DeleteBlueGreenDeploymentResponseTypeDef,
-    DeleteDBClusterAutomatedBackupResultTypeDef,
     DeleteDBClusterResultTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DeleteDBInstanceAutomatedBackupResultTypeDef,
     DeleteDBInstanceResultTypeDef,
     DeleteDBProxyEndpointResponseTypeDef,
     DeleteDBProxyResponseTypeDef,
     DeleteDBSnapshotResultTypeDef,
@@ -138,15 +137,15 @@
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeValidDBInstanceModificationsResultTypeDef,
     DownloadDBLogFilePortionDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
-    ExportTaskResponseTypeDef,
+    ExportTaskResponseMetadataTypeDef,
     ExportTasksMessageTypeDef,
     FailoverDBClusterResultTypeDef,
     FailoverGlobalClusterResultTypeDef,
     FilterTypeDef,
     GlobalClustersMessageTypeDef,
     ModifyActivityStreamResponseTypeDef,
     ModifyCertificatesResultTypeDef,
@@ -162,15 +161,15 @@
     ModifyEventSubscriptionResultTypeDef,
     ModifyGlobalClusterResultTypeDef,
     ModifyOptionGroupResultTypeDef,
     OptionConfigurationTypeDef,
     OptionGroupOptionsMessageTypeDef,
     OptionGroupsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
-    ParameterUnionTypeDef,
+    ParameterTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ProcessorFeatureTypeDef,
     PromoteReadReplicaDBClusterResultTypeDef,
     PromoteReadReplicaResultTypeDef,
     PurchaseReservedDBInstancesOfferingResultTypeDef,
     RebootDBClusterResultTypeDef,
     RebootDBInstanceResultTypeDef,
@@ -197,15 +196,14 @@
     StopDBClusterResultTypeDef,
     StopDBInstanceAutomatedBackupsReplicationResultTypeDef,
     StopDBInstanceResultTypeDef,
     SwitchoverBlueGreenDeploymentResponseTypeDef,
     SwitchoverReadReplicaResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
-    TimestampTypeDef,
     UserAuthConfigTypeDef,
 )
 from .waiter import (
     DBClusterAvailableWaiter,
     DBClusterDeletedWaiter,
     DBClusterSnapshotAvailableWaiter,
     DBClusterSnapshotDeletedWaiter,
@@ -241,16 +239,14 @@
     ClientError: Type[BotocoreClientError]
     CreateCustomDBEngineVersionFault: Type[BotocoreClientError]
     CustomAvailabilityZoneNotFoundFault: Type[BotocoreClientError]
     CustomDBEngineVersionAlreadyExistsFault: Type[BotocoreClientError]
     CustomDBEngineVersionNotFoundFault: Type[BotocoreClientError]
     CustomDBEngineVersionQuotaExceededFault: Type[BotocoreClientError]
     DBClusterAlreadyExistsFault: Type[BotocoreClientError]
-    DBClusterAutomatedBackupNotFoundFault: Type[BotocoreClientError]
-    DBClusterAutomatedBackupQuotaExceededFault: Type[BotocoreClientError]
     DBClusterBacktrackNotFoundFault: Type[BotocoreClientError]
     DBClusterEndpointAlreadyExistsFault: Type[BotocoreClientError]
     DBClusterEndpointNotFoundFault: Type[BotocoreClientError]
     DBClusterEndpointQuotaExceededFault: Type[BotocoreClientError]
     DBClusterNotFoundFault: Type[BotocoreClientError]
     DBClusterParameterGroupNotFoundFault: Type[BotocoreClientError]
     DBClusterQuotaExceededFault: Type[BotocoreClientError]
@@ -305,15 +301,14 @@
     InstanceQuotaExceededFault: Type[BotocoreClientError]
     InsufficientAvailableIPsInSubnetFault: Type[BotocoreClientError]
     InsufficientDBClusterCapacityFault: Type[BotocoreClientError]
     InsufficientDBInstanceCapacityFault: Type[BotocoreClientError]
     InsufficientStorageClusterCapacityFault: Type[BotocoreClientError]
     InvalidBlueGreenDeploymentStateFault: Type[BotocoreClientError]
     InvalidCustomDBEngineVersionStateFault: Type[BotocoreClientError]
-    InvalidDBClusterAutomatedBackupStateFault: Type[BotocoreClientError]
     InvalidDBClusterCapacityFault: Type[BotocoreClientError]
     InvalidDBClusterEndpointStateFault: Type[BotocoreClientError]
     InvalidDBClusterSnapshotStateFault: Type[BotocoreClientError]
     InvalidDBClusterStateFault: Type[BotocoreClientError]
     InvalidDBInstanceAutomatedBackupStateFault: Type[BotocoreClientError]
     InvalidDBInstanceStateFault: Type[BotocoreClientError]
     InvalidDBParameterGroupStateFault: Type[BotocoreClientError]
@@ -440,32 +435,32 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.authorize_db_security_group_ingress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#authorize_db_security_group_ingress)
         """
     def backtrack_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
-        BacktrackTo: TimestampTypeDef,
+        BacktrackTo: Union[datetime, str],
         Force: bool = ...,
         UseEarliestTimeOnPointInTimeUnavailable: bool = ...
-    ) -> DBClusterBacktrackResponseTypeDef:
+    ) -> DBClusterBacktrackResponseMetadataTypeDef:
         """
         Backtracks a DB cluster to a specific time, without creating a new DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.backtrack_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#backtrack_db_cluster)
         """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#can_paginate)
         """
-    def cancel_export_task(self, *, ExportTaskIdentifier: str) -> ExportTaskResponseTypeDef:
+    def cancel_export_task(self, *, ExportTaskIdentifier: str) -> ExportTaskResponseMetadataTypeDef:
         """
         Cancels an export task in progress that is exporting a snapshot or cluster to
         Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.cancel_export_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#cancel_export_task)
         """
@@ -579,15 +574,15 @@
         DatabaseInstallationFilesS3BucketName: str = ...,
         DatabaseInstallationFilesS3Prefix: str = ...,
         ImageId: str = ...,
         KMSKeyId: str = ...,
         Description: str = ...,
         Manifest: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> DBEngineVersionResponseTypeDef:
+    ) -> DBEngineVersionResponseMetadataTypeDef:
         """
         Creates a custom DB engine version (CEV).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_custom_db_engine_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#create_custom_db_engine_version)
         """
     def create_db_cluster(
@@ -638,15 +633,14 @@
         PerformanceInsightsKMSKeyId: str = ...,
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         DBSystemId: str = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
-        EnableLocalWriteForwarding: bool = ...,
         SourceRegion: str = ...
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon Aurora DB cluster or Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#create_db_cluster)
@@ -656,15 +650,15 @@
         *,
         DBClusterIdentifier: str,
         DBClusterEndpointIdentifier: str,
         EndpointType: str,
         StaticMembers: Sequence[str] = ...,
         ExcludedMembers: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> DBClusterEndpointResponseTypeDef:
+    ) -> DBClusterEndpointResponseMetadataTypeDef:
         """
         Creates a new custom endpoint and associates it with an Amazon Aurora DB
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#create_db_cluster_endpoint)
         """
@@ -966,48 +960,37 @@
         Deletes a blue/green deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_blue_green_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_blue_green_deployment)
         """
     def delete_custom_db_engine_version(
         self, *, Engine: str, EngineVersion: str
-    ) -> DBEngineVersionResponseTypeDef:
+    ) -> DBEngineVersionResponseMetadataTypeDef:
         """
         Deletes a custom engine version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_custom_db_engine_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_custom_db_engine_version)
         """
     def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...,
-        DeleteAutomatedBackups: bool = ...
+        FinalDBSnapshotIdentifier: str = ...
     ) -> DeleteDBClusterResultTypeDef:
         """
         The DeleteDBCluster action deletes a previously provisioned DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_db_cluster)
         """
-    def delete_db_cluster_automated_backup(
-        self, *, DbClusterResourceId: str
-    ) -> DeleteDBClusterAutomatedBackupResultTypeDef:
-        """
-        Deletes automated backups using the `DbClusterResourceId` value of the source DB
-        cluster or the Amazon Resource Name (ARN) of the automated backups.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster_automated_backup)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_db_cluster_automated_backup)
-        """
     def delete_db_cluster_endpoint(
         self, *, DBClusterEndpointIdentifier: str
-    ) -> DBClusterEndpointResponseTypeDef:
+    ) -> DBClusterEndpointResponseMetadataTypeDef:
         """
         Deletes a custom endpoint and removes it from an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_db_cluster_endpoint)
         """
     def delete_db_cluster_parameter_group(
@@ -1170,29 +1153,14 @@
         """
         Lists the set of CA certificates provided by Amazon RDS for this Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#describe_certificates)
         """
-    def describe_db_cluster_automated_backups(
-        self,
-        *,
-        DbClusterResourceId: str = ...,
-        DBClusterIdentifier: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...,
-        MaxRecords: int = ...,
-        Marker: str = ...
-    ) -> DBClusterAutomatedBackupMessageTypeDef:
-        """
-        Displays backups for both current and deleted DB clusters.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_automated_backups)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#describe_db_cluster_automated_backups)
-        """
     def describe_db_cluster_backtracks(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
@@ -1264,16 +1232,15 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...
+        IncludePublic: bool = ...
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about DB cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#describe_db_cluster_snapshots)
         """
@@ -1560,16 +1527,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#describe_event_subscriptions)
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
@@ -1844,15 +1811,15 @@
     def modify_custom_db_engine_version(
         self,
         *,
         Engine: str,
         EngineVersion: str,
         Description: str = ...,
         Status: CustomEngineVersionStatusType = ...
-    ) -> DBEngineVersionResponseTypeDef:
+    ) -> DBEngineVersionResponseMetadataTypeDef:
         """
         Modifies the status of a custom engine version (CEV).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_custom_db_engine_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_custom_db_engine_version)
         """
     def modify_db_cluster(
@@ -1894,39 +1861,38 @@
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         ManageMasterUserPassword: bool = ...,
         RotateMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         EngineMode: str = ...,
-        AllowEngineModeChange: bool = ...,
-        EnableLocalWriteForwarding: bool = ...
+        AllowEngineModeChange: bool = ...
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies the settings of an Amazon Aurora DB cluster or a Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster)
         """
     def modify_db_cluster_endpoint(
         self,
         *,
         DBClusterEndpointIdentifier: str,
         EndpointType: str = ...,
         StaticMembers: Sequence[str] = ...,
         ExcludedMembers: Sequence[str] = ...
-    ) -> DBClusterEndpointResponseTypeDef:
+    ) -> DBClusterEndpointResponseMetadataTypeDef:
         """
         Modifies the properties of an endpoint in an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster_endpoint)
         """
     def modify_db_cluster_parameter_group(
-        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
+        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster_parameter_group)
         """
@@ -2010,15 +1976,15 @@
         """
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_instance)
         """
     def modify_db_parameter_group(
-        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
+        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_parameter_group)
         """
@@ -2125,15 +2091,15 @@
         GlobalClusterIdentifier: str = ...,
         NewGlobalClusterIdentifier: str = ...,
         DeletionProtection: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...
     ) -> ModifyGlobalClusterResultTypeDef:
         """
-        Modifies a setting for an Amazon Aurora global cluster.
+        Modify a setting for an Amazon Aurora global cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_global_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_global_cluster)
         """
     def modify_option_group(
         self,
         *,
@@ -2264,28 +2230,28 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#remove_tags_from_resource)
         """
     def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterUnionTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_cluster_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#reset_db_cluster_parameter_group)
         """
     def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterUnionTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#reset_db_parameter_group)
@@ -2375,17 +2341,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_from_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#restore_db_cluster_from_snapshot)
         """
     def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
+        SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
-        SourceDBClusterIdentifier: str = ...,
-        RestoreToTime: TimestampTypeDef = ...,
+        RestoreToTime: Union[datetime, str] = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
@@ -2400,16 +2366,15 @@
         ScalingConfiguration: ScalingConfigurationTypeDef = ...,
         EngineMode: str = ...,
         DBClusterInstanceClass: str = ...,
         StorageType: str = ...,
         PubliclyAccessible: bool = ...,
         Iops: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        NetworkType: str = ...,
-        SourceDbClusterResourceId: str = ...
+        NetworkType: str = ...
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a DB cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_to_point_in_time)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#restore_db_cluster_to_point_in_time)
         """
@@ -2522,15 +2487,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#restore_db_instance_from_s3)
         """
     def restore_db_instance_to_point_in_time(
         self,
         *,
         TargetDBInstanceIdentifier: str,
         SourceDBInstanceIdentifier: str = ...,
-        RestoreTime: TimestampTypeDef = ...,
+        RestoreTime: Union[datetime, str] = ...,
         UseLatestRestorableTime: bool = ...,
         DBInstanceClass: str = ...,
         Port: int = ...,
         AvailabilityZone: str = ...,
         DBSubnetGroupName: str = ...,
         MultiAZ: bool = ...,
         PubliclyAccessible: bool = ...,
@@ -2643,15 +2608,15 @@
         ExportTaskIdentifier: str,
         SourceArn: str,
         S3BucketName: str,
         IamRoleArn: str,
         KmsKeyId: str,
         S3Prefix: str = ...,
         ExportOnly: Sequence[str] = ...
-    ) -> ExportTaskResponseTypeDef:
+    ) -> ExportTaskResponseMetadataTypeDef:
         """
         Starts an export of DB snapshot or DB cluster data to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.start_export_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#start_export_task)
         """
     def stop_activity_stream(
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/literals.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     "DescribeReservedDBInstancesPaginatorName",
     "DescribeSourceRegionsPaginatorName",
     "DownloadDBLogFilePortionPaginatorName",
     "EngineFamilyType",
     "ExportSourceTypeType",
     "FailoverStatusType",
     "IAMAuthModeType",
-    "LocalWriteForwardingStatusType",
     "ReplicaModeType",
     "SourceTypeType",
     "TargetHealthReasonType",
     "TargetRoleType",
     "TargetStateType",
     "TargetTypeType",
     "WriteForwardingStatusType",
@@ -176,17 +175,14 @@
 DescribeReservedDBInstancesPaginatorName = Literal["describe_reserved_db_instances"]
 DescribeSourceRegionsPaginatorName = Literal["describe_source_regions"]
 DownloadDBLogFilePortionPaginatorName = Literal["download_db_log_file_portion"]
 EngineFamilyType = Literal["MYSQL", "POSTGRESQL", "SQLSERVER"]
 ExportSourceTypeType = Literal["CLUSTER", "SNAPSHOT"]
 FailoverStatusType = Literal["cancelling", "failing-over", "pending"]
 IAMAuthModeType = Literal["DISABLED", "ENABLED", "REQUIRED"]
-LocalWriteForwardingStatusType = Literal[
-    "disabled", "disabling", "enabled", "enabling", "requested"
-]
 ReplicaModeType = Literal["mounted", "open-read-only"]
 SourceTypeType = Literal[
     "blue-green-deployment",
     "custom-engine-version",
     "db-cluster",
     "db-cluster-snapshot",
     "db-instance",
@@ -322,15 +318,14 @@
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
@@ -409,15 +404,14 @@
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
@@ -639,15 +633,14 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/literals.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     "DescribeReservedDBInstancesPaginatorName",
     "DescribeSourceRegionsPaginatorName",
     "DownloadDBLogFilePortionPaginatorName",
     "EngineFamilyType",
     "ExportSourceTypeType",
     "FailoverStatusType",
     "IAMAuthModeType",
-    "LocalWriteForwardingStatusType",
     "ReplicaModeType",
     "SourceTypeType",
     "TargetHealthReasonType",
     "TargetRoleType",
     "TargetStateType",
     "TargetTypeType",
     "WriteForwardingStatusType",
@@ -174,17 +173,14 @@
 DescribeReservedDBInstancesPaginatorName = Literal["describe_reserved_db_instances"]
 DescribeSourceRegionsPaginatorName = Literal["describe_source_regions"]
 DownloadDBLogFilePortionPaginatorName = Literal["download_db_log_file_portion"]
 EngineFamilyType = Literal["MYSQL", "POSTGRESQL", "SQLSERVER"]
 ExportSourceTypeType = Literal["CLUSTER", "SNAPSHOT"]
 FailoverStatusType = Literal["cancelling", "failing-over", "pending"]
 IAMAuthModeType = Literal["DISABLED", "ENABLED", "REQUIRED"]
-LocalWriteForwardingStatusType = Literal[
-    "disabled", "disabling", "enabled", "enabling", "requested"
-]
 ReplicaModeType = Literal["mounted", "open-read-only"]
 SourceTypeType = Literal[
     "blue-green-deployment",
     "custom-engine-version",
     "db-cluster",
     "db-cluster-snapshot",
     "db-instance",
@@ -320,15 +316,14 @@
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
@@ -407,15 +402,14 @@
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
@@ -637,15 +631,14 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/paginator.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,16 @@
     describe_pending_maintenance_actions_paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")
     describe_reserved_db_instances_paginator: DescribeReservedDBInstancesPaginator = client.get_paginator("describe_reserved_db_instances")
     describe_reserved_db_instances_offerings_paginator: DescribeReservedDBInstancesOfferingsPaginator = client.get_paginator("describe_reserved_db_instances_offerings")
     describe_source_regions_paginator: DescribeSourceRegionsPaginator = client.get_paginator("describe_source_regions")
     download_db_log_file_portion_paginator: DownloadDBLogFilePortionPaginator = client.get_paginator("download_db_log_file_portion")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ExportSourceTypeType, SourceTypeType
 from .type_defs import (
     CertificateMessageTypeDef,
     DBClusterBacktrackMessageTypeDef,
@@ -126,15 +127,14 @@
     OptionGroupsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ReservedDBInstanceMessageTypeDef,
     ReservedDBInstancesOfferingMessageTypeDef,
     SourceRegionMessageTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeBlueGreenDeploymentsPaginator",
     "DescribeCertificatesPaginator",
     "DescribeDBClusterBacktracksPaginator",
     "DescribeDBClusterEndpointsPaginator",
@@ -310,15 +310,14 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/paginators/#describedbclustersnapshotspaginator)
         """
 
@@ -674,16 +673,16 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEvents.paginate)
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/paginator.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,16 @@
     describe_pending_maintenance_actions_paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")
     describe_reserved_db_instances_paginator: DescribeReservedDBInstancesPaginator = client.get_paginator("describe_reserved_db_instances")
     describe_reserved_db_instances_offerings_paginator: DescribeReservedDBInstancesOfferingsPaginator = client.get_paginator("describe_reserved_db_instances_offerings")
     describe_source_regions_paginator: DescribeSourceRegionsPaginator = client.get_paginator("describe_source_regions")
     download_db_log_file_portion_paginator: DownloadDBLogFilePortionPaginator = client.get_paginator("download_db_log_file_portion")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ExportSourceTypeType, SourceTypeType
 from .type_defs import (
     CertificateMessageTypeDef,
     DBClusterBacktrackMessageTypeDef,
@@ -126,15 +127,14 @@
     OptionGroupsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ReservedDBInstanceMessageTypeDef,
     ReservedDBInstancesOfferingMessageTypeDef,
     SourceRegionMessageTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeBlueGreenDeploymentsPaginator",
     "DescribeCertificatesPaginator",
     "DescribeDBClusterBacktracksPaginator",
     "DescribeDBClusterEndpointsPaginator",
@@ -301,15 +301,14 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/paginators/#describedbclustersnapshotspaginator)
         """
 
@@ -647,16 +646,16 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEvents.paginate)
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/type_defs.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_rds.type_defs import AccountQuotaTypeDef
 
-    data: AccountQuotaTypeDef = ...
+    data: AccountQuotaTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Optional, Sequence, Union
 
 from .literals import (
@@ -27,15 +27,14 @@
     DBProxyEndpointStatusType,
     DBProxyEndpointTargetRoleType,
     DBProxyStatusType,
     EngineFamilyType,
     ExportSourceTypeType,
     FailoverStatusType,
     IAMAuthModeType,
-    LocalWriteForwardingStatusType,
     ReplicaModeType,
     SourceTypeType,
     TargetHealthReasonType,
     TargetRoleType,
     TargetStateType,
     TargetTypeType,
     WriteForwardingStatusType,
@@ -46,30 +45,30 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountQuotaTypeDef",
     "ResponseMetadataTypeDef",
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddRoleToDBInstanceMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AuthorizeDBSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "AvailableProcessorFeatureTypeDef",
-    "TimestampTypeDef",
+    "BacktrackDBClusterMessageRequestTypeDef",
     "BlueGreenDeploymentTaskTypeDef",
     "SwitchoverDetailTypeDef",
+    "TagOutputTypeDef",
     "CancelExportTaskMessageRequestTypeDef",
     "CertificateDetailsTypeDef",
     "CertificateTypeDef",
     "CharacterSetTypeDef",
     "ClientGenerateDbAuthTokenRequestTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
@@ -80,15 +79,14 @@
     "ScalingConfigurationTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "ProcessorFeatureTypeDef",
     "DBProxyEndpointTypeDef",
     "UserAuthConfigTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "CustomDBEngineVersionAMITypeDef",
-    "RestoreWindowTypeDef",
     "DBClusterBacktrackTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
     "ParameterOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
@@ -96,28 +94,29 @@
     "MasterUserSecretTypeDef",
     "ScalingConfigurationInfoTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceAutomatedBackupsReplicationTypeDef",
+    "RestoreWindowTypeDef",
     "DBInstanceRoleTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
+    "ProcessorFeatureOutputTypeDef",
     "TargetHealthTypeDef",
     "UserAuthConfigInfoTypeDef",
     "EC2SecurityGroupTypeDef",
     "IPRangeTypeDef",
     "DBSnapshotAttributeTypeDef",
     "DeleteBlueGreenDeploymentRequestRequestTypeDef",
     "DeleteCustomDBEngineVersionMessageRequestTypeDef",
-    "DeleteDBClusterAutomatedBackupMessageRequestTypeDef",
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceAutomatedBackupMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBParameterGroupMessageRequestTypeDef",
@@ -148,25 +147,26 @@
     "GlobalClusterMemberTypeDef",
     "MinimumEngineVersionPerAllowedValueTypeDef",
     "ModifyActivityStreamRequestRequestTypeDef",
     "ModifyCertificatesMessageRequestTypeDef",
     "ModifyCurrentDBClusterCapacityMessageRequestTypeDef",
     "ModifyCustomDBEngineVersionMessageRequestTypeDef",
     "ModifyDBClusterEndpointMessageRequestTypeDef",
+    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBProxyEndpointRequestRequestTypeDef",
     "ModifyDBSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBSnapshotMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "OptionSettingTypeDef",
     "OptionVersionTypeDef",
+    "OptionSettingOutputTypeDef",
     "OutpostTypeDef",
-    "ParameterTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "PromoteReadReplicaMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBClusterMessageRequestTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RecurringChargeTypeDef",
@@ -186,22 +186,22 @@
     "StopActivityStreamRequestRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
     "StopDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef",
     "StopDBInstanceMessageRequestTypeDef",
     "SwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     "SwitchoverReadReplicaMessageRequestTypeDef",
     "AccountAttributesMessageTypeDef",
-    "DBClusterBacktrackResponseTypeDef",
+    "DBClusterBacktrackResponseMetadataTypeDef",
     "DBClusterCapacityInfoTypeDef",
-    "DBClusterEndpointResponseTypeDef",
+    "DBClusterEndpointResponseMetadataTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DBParameterGroupNameMessageTypeDef",
     "DownloadDBLogFilePortionDetailsTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "ExportTaskResponseTypeDef",
+    "ExportTaskResponseMetadataTypeDef",
     "ModifyActivityStreamResponseTypeDef",
     "StartActivityStreamResponseTypeDef",
     "StopActivityStreamResponseTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EventSubscriptionsMessageTypeDef",
@@ -221,20 +221,19 @@
     "CreateDBParameterGroupMessageRequestTypeDef",
     "CreateDBProxyEndpointRequestRequestTypeDef",
     "CreateDBSecurityGroupMessageRequestTypeDef",
     "CreateDBSnapshotMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateOptionGroupMessageRequestTypeDef",
-    "DBClusterSnapshotTypeDef",
     "PurchaseReservedDBInstancesOfferingMessageRequestTypeDef",
-    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
-    "BacktrackDBClusterMessageRequestTypeDef",
     "BlueGreenDeploymentTypeDef",
+    "DBClusterSnapshotTypeDef",
+    "TagListMessageTypeDef",
     "CertificateMessageTypeDef",
     "ModifyCertificatesResultTypeDef",
     "ClusterPendingModifiedValuesTypeDef",
     "DBProxyTargetGroupTypeDef",
     "ModifyDBProxyTargetGroupRequestRequestTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
@@ -245,43 +244,41 @@
     "CreateDBClusterMessageRequestTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromS3MessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
     "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBInstanceReadReplicaMessageRequestTypeDef",
-    "DBSnapshotTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
-    "PendingModifiedValuesTypeDef",
     "RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef",
     "RestoreDBInstanceFromS3MessageRequestTypeDef",
     "RestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     "CreateDBProxyEndpointResponseTypeDef",
     "DeleteDBProxyEndpointResponseTypeDef",
     "DescribeDBProxyEndpointsResponseTypeDef",
     "ModifyDBProxyEndpointResponseTypeDef",
     "CreateDBProxyRequestRequestTypeDef",
     "ModifyDBProxyRequestRequestTypeDef",
-    "DBClusterAutomatedBackupTypeDef",
     "DBClusterBacktrackMessageTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
-    "DBEngineVersionResponseTypeDef",
+    "DBEngineVersionResponseMetadataTypeDef",
     "DBEngineVersionTypeDef",
     "DBInstanceAutomatedBackupTypeDef",
+    "DBSnapshotTypeDef",
+    "PendingModifiedValuesTypeDef",
     "DBProxyTargetTypeDef",
     "DBProxyTypeDef",
     "DBSecurityGroupTypeDef",
     "DBSnapshotAttributesResultTypeDef",
     "DescribeBlueGreenDeploymentsRequestRequestTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
-    "DescribeDBClusterAutomatedBackupsMessageRequestTypeDef",
     "DescribeDBClusterBacktracksMessageRequestTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
@@ -358,51 +355,52 @@
     "DescribeDBSnapshotsMessageDBSnapshotDeletedWaitTypeDef",
     "DescribeDBLogFilesResponseTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "ExportTasksMessageTypeDef",
     "GlobalClusterTypeDef",
     "OptionGroupOptionSettingTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "OptionConfigurationTypeDef",
     "OptionTypeDef",
     "SubnetTypeDef",
-    "ParameterUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
     "ReservedDBInstanceTypeDef",
     "ReservedDBInstancesOfferingTypeDef",
     "SourceRegionMessageTypeDef",
-    "CopyDBClusterSnapshotResultTypeDef",
-    "CreateDBClusterSnapshotResultTypeDef",
-    "DBClusterSnapshotMessageTypeDef",
-    "DeleteDBClusterSnapshotResultTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "CreateBlueGreenDeploymentResponseTypeDef",
     "DeleteBlueGreenDeploymentResponseTypeDef",
     "DescribeBlueGreenDeploymentsResponseTypeDef",
     "SwitchoverBlueGreenDeploymentResponseTypeDef",
+    "CopyDBClusterSnapshotResultTypeDef",
+    "CreateDBClusterSnapshotResultTypeDef",
+    "DBClusterSnapshotMessageTypeDef",
+    "DeleteDBClusterSnapshotResultTypeDef",
     "DBClusterTypeDef",
     "DescribeDBProxyTargetGroupsResponseTypeDef",
     "ModifyDBProxyTargetGroupResponseTypeDef",
-    "CopyDBSnapshotResultTypeDef",
-    "CreateDBSnapshotResultTypeDef",
-    "DBSnapshotMessageTypeDef",
-    "DeleteDBSnapshotResultTypeDef",
-    "ModifyDBSnapshotResultTypeDef",
-    "DBClusterAutomatedBackupMessageTypeDef",
-    "DeleteDBClusterAutomatedBackupResultTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "DBEngineVersionMessageTypeDef",
     "DBInstanceAutomatedBackupMessageTypeDef",
     "DeleteDBInstanceAutomatedBackupResultTypeDef",
     "StartDBInstanceAutomatedBackupsReplicationResultTypeDef",
     "StopDBInstanceAutomatedBackupsReplicationResultTypeDef",
+    "CopyDBSnapshotResultTypeDef",
+    "CreateDBSnapshotResultTypeDef",
+    "DBSnapshotMessageTypeDef",
+    "DeleteDBSnapshotResultTypeDef",
+    "ModifyDBSnapshotResultTypeDef",
     "DescribeDBProxyTargetsResponseTypeDef",
     "RegisterDBProxyTargetsResponseTypeDef",
     "CreateDBProxyResponseTypeDef",
     "DeleteDBProxyResponseTypeDef",
     "DescribeDBProxiesResponseTypeDef",
     "ModifyDBProxyResponseTypeDef",
     "AuthorizeDBSecurityGroupIngressResultTypeDef",
@@ -417,18 +415,14 @@
     "GlobalClustersMessageTypeDef",
     "ModifyGlobalClusterResultTypeDef",
     "RemoveFromGlobalClusterResultTypeDef",
     "OptionGroupOptionTypeDef",
     "ModifyOptionGroupMessageRequestTypeDef",
     "OptionGroupTypeDef",
     "DBSubnetGroupTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "ApplyPendingMaintenanceActionResultTypeDef",
     "PendingMaintenanceActionsMessageTypeDef",
     "ValidDBInstanceModificationsMessageTypeDef",
     "PurchaseReservedDBInstancesOfferingResultTypeDef",
     "ReservedDBInstanceMessageTypeDef",
     "ReservedDBInstancesOfferingMessageTypeDef",
     "CreateDBClusterResultTypeDef",
@@ -471,15 +465,14 @@
 AccountQuotaTypeDef = TypedDict(
     "AccountQuotaTypeDef",
     {
         "AccountQuotaName": str,
         "Used": int,
         "Max": int,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -500,22 +493,20 @@
     "_OptionalAddRoleToDBClusterMessageRequestTypeDef",
     {
         "FeatureName": str,
     },
     total=False,
 )
 
-
 class AddRoleToDBClusterMessageRequestTypeDef(
     _RequiredAddRoleToDBClusterMessageRequestTypeDef,
     _OptionalAddRoleToDBClusterMessageRequestTypeDef,
 ):
     pass
 
-
 AddRoleToDBInstanceMessageRequestTypeDef = TypedDict(
     "AddRoleToDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "RoleArn": str,
         "FeatureName": str,
     },
@@ -539,15 +530,14 @@
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -577,58 +567,81 @@
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-
 class AuthorizeDBSecurityGroupIngressMessageRequestTypeDef(
     _RequiredAuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
     _OptionalAuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 AvailableProcessorFeatureTypeDef = TypedDict(
     "AvailableProcessorFeatureTypeDef",
     {
         "Name": str,
         "DefaultValue": str,
         "AllowedValues": str,
     },
+)
+
+_RequiredBacktrackDBClusterMessageRequestTypeDef = TypedDict(
+    "_RequiredBacktrackDBClusterMessageRequestTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "BacktrackTo": Union[datetime, str],
+    },
+)
+_OptionalBacktrackDBClusterMessageRequestTypeDef = TypedDict(
+    "_OptionalBacktrackDBClusterMessageRequestTypeDef",
+    {
+        "Force": bool,
+        "UseEarliestTimeOnPointInTimeUnavailable": bool,
+    },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
+class BacktrackDBClusterMessageRequestTypeDef(
+    _RequiredBacktrackDBClusterMessageRequestTypeDef,
+    _OptionalBacktrackDBClusterMessageRequestTypeDef,
+):
+    pass
+
 BlueGreenDeploymentTaskTypeDef = TypedDict(
     "BlueGreenDeploymentTaskTypeDef",
     {
         "Name": str,
         "Status": str,
     },
-    total=False,
 )
 
 SwitchoverDetailTypeDef = TypedDict(
     "SwitchoverDetailTypeDef",
     {
         "SourceMember": str,
         "TargetMember": str,
         "Status": str,
     },
-    total=False,
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
 )
 
 CancelExportTaskMessageRequestTypeDef = TypedDict(
     "CancelExportTaskMessageRequestTypeDef",
     {
         "ExportTaskIdentifier": str,
     },
@@ -636,39 +649,36 @@
 
 CertificateDetailsTypeDef = TypedDict(
     "CertificateDetailsTypeDef",
     {
         "CAIdentifier": str,
         "ValidTill": datetime,
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
         "CustomerOverride": bool,
         "CustomerOverrideValidTill": datetime,
     },
-    total=False,
 )
 
 CharacterSetTypeDef = TypedDict(
     "CharacterSetTypeDef",
     {
         "CharacterSetName": str,
         "CharacterSetDescription": str,
     },
-    total=False,
 )
 
 _RequiredClientGenerateDbAuthTokenRequestTypeDef = TypedDict(
     "_RequiredClientGenerateDbAuthTokenRequestTypeDef",
     {
         "DBHostname": str,
         "Port": int,
@@ -679,22 +689,20 @@
     "_OptionalClientGenerateDbAuthTokenRequestTypeDef",
     {
         "Region": Optional[str],
     },
     total=False,
 )
 
-
 class ClientGenerateDbAuthTokenRequestTypeDef(
     _RequiredClientGenerateDbAuthTokenRequestTypeDef,
     _OptionalClientGenerateDbAuthTokenRequestTypeDef,
 ):
     pass
 
-
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
     },
     total=False,
@@ -702,27 +710,25 @@
 
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
-    total=False,
 )
 
 ConnectionPoolConfigurationInfoTypeDef = TypedDict(
     "ConnectionPoolConfigurationInfoTypeDef",
     {
         "MaxConnectionsPercent": int,
         "MaxIdleConnectionsPercent": int,
         "ConnectionBorrowTimeout": int,
         "SessionPinningFilters": List[str],
         "InitQuery": str,
     },
-    total=False,
 )
 
 ConnectionPoolConfigurationTypeDef = TypedDict(
     "ConnectionPoolConfigurationTypeDef",
     {
         "MaxConnectionsPercent": int,
         "MaxIdleConnectionsPercent": int,
@@ -737,26 +743,24 @@
     "DBClusterParameterGroupTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBClusterParameterGroupArn": str,
     },
-    total=False,
 )
 
 DBParameterGroupTypeDef = TypedDict(
     "DBParameterGroupTypeDef",
     {
         "DBParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBParameterGroupArn": str,
     },
-    total=False,
 )
 
 ScalingConfigurationTypeDef = TypedDict(
     "ScalingConfigurationTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
@@ -797,15 +801,14 @@
         "VpcSecurityGroupIds": List[str],
         "VpcSubnetIds": List[str],
         "Endpoint": str,
         "CreatedDate": datetime,
         "TargetRole": DBProxyEndpointTargetRoleType,
         "IsDefault": bool,
     },
-    total=False,
 )
 
 UserAuthConfigTypeDef = TypedDict(
     "UserAuthConfigTypeDef",
     {
         "Description": str,
         "UserName": str,
@@ -833,37 +836,26 @@
 
 CustomDBEngineVersionAMITypeDef = TypedDict(
     "CustomDBEngineVersionAMITypeDef",
     {
         "ImageId": str,
         "Status": str,
     },
-    total=False,
-)
-
-RestoreWindowTypeDef = TypedDict(
-    "RestoreWindowTypeDef",
-    {
-        "EarliestTime": datetime,
-        "LatestTime": datetime,
-    },
-    total=False,
 )
 
 DBClusterBacktrackTypeDef = TypedDict(
     "DBClusterBacktrackTypeDef",
     {
         "DBClusterIdentifier": str,
         "BacktrackIdentifier": str,
         "BacktrackTo": datetime,
         "BacktrackedFrom": datetime,
         "BacktrackRequestCreationTime": datetime,
         "Status": str,
     },
-    total=False,
 )
 
 DBClusterEndpointTypeDef = TypedDict(
     "DBClusterEndpointTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
         "DBClusterIdentifier": str,
@@ -872,35 +864,32 @@
         "Status": str,
         "EndpointType": str,
         "CustomEndpointType": str,
         "StaticMembers": List[str],
         "ExcludedMembers": List[str],
         "DBClusterEndpointArn": str,
     },
-    total=False,
 )
 
 DBClusterMemberTypeDef = TypedDict(
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
     },
-    total=False,
 )
 
 DBClusterOptionGroupStatusTypeDef = TypedDict(
     "DBClusterOptionGroupStatusTypeDef",
     {
         "DBClusterOptionGroupName": str,
         "Status": str,
     },
-    total=False,
 )
 
 ParameterOutputTypeDef = TypedDict(
     "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
@@ -910,232 +899,225 @@
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
         "SupportedEngineModes": List[str],
     },
-    total=False,
 )
 
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
         "FeatureName": str,
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
 
 DomainMembershipTypeDef = TypedDict(
     "DomainMembershipTypeDef",
     {
         "Domain": str,
         "Status": str,
         "FQDN": str,
         "IAMRoleName": str,
         "OU": str,
         "AuthSecretArn": str,
         "DnsIps": List[str],
     },
-    total=False,
 )
 
 MasterUserSecretTypeDef = TypedDict(
     "MasterUserSecretTypeDef",
     {
         "SecretArn": str,
         "SecretStatus": str,
         "KmsKeyId": str,
     },
-    total=False,
 )
 
 ScalingConfigurationInfoTypeDef = TypedDict(
     "ScalingConfigurationInfoTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
         "AutoPause": bool,
         "SecondsUntilAutoPause": int,
         "TimeoutAction": str,
         "SecondsBeforeTimeout": int,
     },
-    total=False,
 )
 
 ServerlessV2ScalingConfigurationInfoTypeDef = TypedDict(
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     {
         "MinCapacity": float,
         "MaxCapacity": float,
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
 
 TimezoneTypeDef = TypedDict(
     "TimezoneTypeDef",
     {
         "TimezoneName": str,
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
         "SupportedEngineModes": List[str],
         "SupportsParallelQuery": bool,
         "SupportsGlobalDatabases": bool,
         "SupportsBabelfish": bool,
-        "SupportsLocalWriteForwarding": bool,
     },
-    total=False,
 )
 
 DBInstanceAutomatedBackupsReplicationTypeDef = TypedDict(
     "DBInstanceAutomatedBackupsReplicationTypeDef",
     {
         "DBInstanceAutomatedBackupsArn": str,
     },
-    total=False,
+)
+
+RestoreWindowTypeDef = TypedDict(
+    "RestoreWindowTypeDef",
+    {
+        "EarliestTime": datetime,
+        "LatestTime": datetime,
+    },
 )
 
 DBInstanceRoleTypeDef = TypedDict(
     "DBInstanceRoleTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
         "Status": str,
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
 
 DBParameterGroupStatusTypeDef = TypedDict(
     "DBParameterGroupStatusTypeDef",
     {
         "DBParameterGroupName": str,
         "ParameterApplyStatus": str,
     },
-    total=False,
 )
 
 DBSecurityGroupMembershipTypeDef = TypedDict(
     "DBSecurityGroupMembershipTypeDef",
     {
         "DBSecurityGroupName": str,
         "Status": str,
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
 
 OptionGroupMembershipTypeDef = TypedDict(
     "OptionGroupMembershipTypeDef",
     {
         "OptionGroupName": str,
         "Status": str,
     },
-    total=False,
+)
+
+ProcessorFeatureOutputTypeDef = TypedDict(
+    "ProcessorFeatureOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
 )
 
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetStateType,
         "Reason": TargetHealthReasonType,
         "Description": str,
     },
-    total=False,
 )
 
 UserAuthConfigInfoTypeDef = TypedDict(
     "UserAuthConfigInfoTypeDef",
     {
         "Description": str,
         "UserName": str,
         "AuthScheme": Literal["SECRETS"],
         "SecretArn": str,
         "IAMAuth": IAMAuthModeType,
         "ClientPasswordAuthType": ClientPasswordAuthTypeType,
     },
-    total=False,
 )
 
 EC2SecurityGroupTypeDef = TypedDict(
     "EC2SecurityGroupTypeDef",
     {
         "Status": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
-    total=False,
 )
 
 IPRangeTypeDef = TypedDict(
     "IPRangeTypeDef",
     {
         "Status": str,
         "CIDRIP": str,
     },
-    total=False,
 )
 
 DBSnapshotAttributeTypeDef = TypedDict(
     "DBSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
-    total=False,
 )
 
 _RequiredDeleteBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
     },
@@ -1144,37 +1126,28 @@
     "_OptionalDeleteBlueGreenDeploymentRequestRequestTypeDef",
     {
         "DeleteTarget": bool,
     },
     total=False,
 )
 
-
 class DeleteBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredDeleteBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalDeleteBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "DeleteCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
 
-DeleteDBClusterAutomatedBackupMessageRequestTypeDef = TypedDict(
-    "DeleteDBClusterAutomatedBackupMessageRequestTypeDef",
-    {
-        "DbClusterResourceId": str,
-    },
-)
-
 DeleteDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 
@@ -1185,26 +1158,23 @@
     },
 )
 _OptionalDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_OptionalDeleteDBClusterMessageRequestTypeDef",
     {
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
-        "DeleteAutomatedBackups": bool,
     },
     total=False,
 )
 
-
 class DeleteDBClusterMessageRequestTypeDef(
     _RequiredDeleteDBClusterMessageRequestTypeDef, _OptionalDeleteDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 DeleteDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 
@@ -1236,21 +1206,19 @@
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
         "DeleteAutomatedBackups": bool,
     },
     total=False,
 )
 
-
 class DeleteDBInstanceMessageRequestTypeDef(
     _RequiredDeleteDBInstanceMessageRequestTypeDef, _OptionalDeleteDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 DeleteDBParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBParameterGroupMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
     },
 )
 
@@ -1322,22 +1290,20 @@
         "TargetGroupName": str,
         "DBInstanceIdentifiers": Sequence[str],
         "DBClusterIdentifiers": Sequence[str],
     },
     total=False,
 )
 
-
 class DeregisterDBProxyTargetsRequestRequestTypeDef(
     _RequiredDeregisterDBProxyTargetsRequestRequestTypeDef,
     _OptionalDeregisterDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -1371,15 +1337,14 @@
 DescribeDBLogFilesDetailsTypeDef = TypedDict(
     "DescribeDBLogFilesDetailsTypeDef",
     {
         "LogFileName": str,
         "LastWritten": int,
         "Size": int,
     },
-    total=False,
 )
 
 DescribeDBSnapshotAttributesMessageRequestTypeDef = TypedDict(
     "DescribeDBSnapshotAttributesMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
@@ -1394,15 +1359,14 @@
 
 DoubleRangeTypeDef = TypedDict(
     "DoubleRangeTypeDef",
     {
         "From": float,
         "To": float,
     },
-    total=False,
 )
 
 _RequiredDownloadDBLogFilePortionMessageRequestTypeDef = TypedDict(
     "_RequiredDownloadDBLogFilePortionMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "LogFileName": str,
@@ -1413,42 +1377,38 @@
     {
         "Marker": str,
         "NumberOfLines": int,
     },
     total=False,
 )
 
-
 class DownloadDBLogFilePortionMessageRequestTypeDef(
     _RequiredDownloadDBLogFilePortionMessageRequestTypeDef,
     _OptionalDownloadDBLogFilePortionMessageRequestTypeDef,
 ):
     pass
 
-
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
 
 ExportTaskTypeDef = TypedDict(
     "ExportTaskTypeDef",
     {
         "ExportTaskIdentifier": str,
         "SourceArn": str,
@@ -1463,15 +1423,14 @@
         "Status": str,
         "PercentProgress": int,
         "TotalExtractedDataInGB": int,
         "FailureCause": str,
         "WarningMessage": str,
         "SourceType": ExportSourceTypeType,
     },
-    total=False,
 )
 
 _RequiredFailoverDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredFailoverDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -1480,21 +1439,19 @@
     "_OptionalFailoverDBClusterMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
     },
     total=False,
 )
 
-
 class FailoverDBClusterMessageRequestTypeDef(
     _RequiredFailoverDBClusterMessageRequestTypeDef, _OptionalFailoverDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 FailoverGlobalClusterMessageRequestTypeDef = TypedDict(
     "FailoverGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "TargetDbClusterIdentifier": str,
     },
 )
@@ -1502,35 +1459,32 @@
 FailoverStateTypeDef = TypedDict(
     "FailoverStateTypeDef",
     {
         "Status": FailoverStatusType,
         "FromDbClusterArn": str,
         "ToDbClusterArn": str,
     },
-    total=False,
 )
 
 GlobalClusterMemberTypeDef = TypedDict(
     "GlobalClusterMemberTypeDef",
     {
         "DBClusterArn": str,
         "Readers": List[str],
         "IsWriter": bool,
         "GlobalWriteForwardingStatus": WriteForwardingStatusType,
     },
-    total=False,
 )
 
 MinimumEngineVersionPerAllowedValueTypeDef = TypedDict(
     "MinimumEngineVersionPerAllowedValueTypeDef",
     {
         "AllowedValue": str,
         "MinimumEngineVersion": str,
     },
-    total=False,
 )
 
 ModifyActivityStreamRequestRequestTypeDef = TypedDict(
     "ModifyActivityStreamRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "AuditPolicyState": AuditPolicyStateType,
@@ -1559,22 +1513,20 @@
         "Capacity": int,
         "SecondsBeforeTimeout": int,
         "TimeoutAction": str,
     },
     total=False,
 )
 
-
 class ModifyCurrentDBClusterCapacityMessageRequestTypeDef(
     _RequiredModifyCurrentDBClusterCapacityMessageRequestTypeDef,
     _OptionalModifyCurrentDBClusterCapacityMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
@@ -1583,22 +1535,20 @@
     {
         "Description": str,
         "Status": CustomEngineVersionStatusType,
     },
     total=False,
 )
 
-
 class ModifyCustomDBEngineVersionMessageRequestTypeDef(
     _RequiredModifyCustomDBEngineVersionMessageRequestTypeDef,
     _OptionalModifyCustomDBEngineVersionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 _OptionalModifyDBClusterEndpointMessageRequestTypeDef = TypedDict(
@@ -1607,21 +1557,37 @@
         "EndpointType": str,
         "StaticMembers": Sequence[str],
         "ExcludedMembers": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBClusterEndpointMessageRequestTypeDef(
     _RequiredModifyDBClusterEndpointMessageRequestTypeDef,
     _OptionalModifyDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
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
+        "SupportedEngineModes": Sequence[str],
+    },
+    total=False,
+)
 
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
@@ -1631,22 +1597,20 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBClusterSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBProxyEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyEndpointRequestRequestTypeDef",
     {
         "DBProxyEndpointName": str,
     },
 )
 _OptionalModifyDBProxyEndpointRequestRequestTypeDef = TypedDict(
@@ -1654,22 +1618,20 @@
     {
         "NewDBProxyEndpointName": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBProxyEndpointRequestRequestTypeDef(
     _RequiredModifyDBProxyEndpointRequestRequestTypeDef,
     _OptionalModifyDBProxyEndpointRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSnapshotAttributeMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1678,22 +1640,20 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSnapshotMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
 )
 _OptionalModifyDBSnapshotMessageRequestTypeDef = TypedDict(
@@ -1701,21 +1661,19 @@
     {
         "EngineVersion": str,
         "OptionGroupName": str,
     },
     total=False,
 )
 
-
 class ModifyDBSnapshotMessageRequestTypeDef(
     _RequiredModifyDBSnapshotMessageRequestTypeDef, _OptionalModifyDBSnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -1723,22 +1681,20 @@
     "_OptionalModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupDescription": str,
     },
     total=False,
 )
 
-
 class ModifyDBSubnetGroupMessageRequestTypeDef(
     _RequiredModifyDBSubnetGroupMessageRequestTypeDef,
     _OptionalModifyDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -1748,22 +1704,20 @@
         "SourceType": str,
         "EventCategories": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 ModifyGlobalClusterMessageRequestTypeDef = TypedDict(
     "ModifyGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "NewGlobalClusterIdentifier": str,
         "DeletionProtection": bool,
         "EngineVersion": str,
@@ -1790,54 +1744,48 @@
 
 OptionVersionTypeDef = TypedDict(
     "OptionVersionTypeDef",
     {
         "Version": str,
         "IsDefault": bool,
     },
-    total=False,
 )
 
-OutpostTypeDef = TypedDict(
-    "OutpostTypeDef",
+OptionSettingOutputTypeDef = TypedDict(
+    "OptionSettingOutputTypeDef",
     {
-        "Arn": str,
-    },
-    total=False,
-)
-
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
+        "Name": str,
+        "Value": str,
+        "DefaultValue": str,
         "Description": str,
-        "Source": str,
         "ApplyType": str,
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
-        "MinimumEngineVersion": str,
-        "ApplyMethod": ApplyMethodType,
-        "SupportedEngineModes": Sequence[str],
+        "IsCollection": bool,
+    },
+)
+
+OutpostTypeDef = TypedDict(
+    "OutpostTypeDef",
+    {
+        "Arn": str,
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
 
 PromoteReadReplicaDBClusterMessageRequestTypeDef = TypedDict(
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -1854,30 +1802,27 @@
     {
         "BackupRetentionPeriod": int,
         "PreferredBackupWindow": str,
     },
     total=False,
 )
 
-
 class PromoteReadReplicaMessageRequestTypeDef(
     _RequiredPromoteReadReplicaMessageRequestTypeDef,
     _OptionalPromoteReadReplicaMessageRequestTypeDef,
 ):
     pass
 
-
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "From": int,
         "To": int,
         "Step": int,
     },
-    total=False,
 )
 
 RebootDBClusterMessageRequestTypeDef = TypedDict(
     "RebootDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -1893,28 +1838,25 @@
     "_OptionalRebootDBInstanceMessageRequestTypeDef",
     {
         "ForceFailover": bool,
     },
     total=False,
 )
 
-
 class RebootDBInstanceMessageRequestTypeDef(
     _RequiredRebootDBInstanceMessageRequestTypeDef, _OptionalRebootDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
-    total=False,
 )
 
 _RequiredRegisterDBProxyTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDBProxyTargetsRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
@@ -1925,22 +1867,20 @@
         "TargetGroupName": str,
         "DBInstanceIdentifiers": Sequence[str],
         "DBClusterIdentifiers": Sequence[str],
     },
     total=False,
 )
 
-
 class RegisterDBProxyTargetsRequestRequestTypeDef(
     _RequiredRegisterDBProxyTargetsRequestRequestTypeDef,
     _OptionalRegisterDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 RemoveFromGlobalClusterMessageRequestTypeDef = TypedDict(
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "DbClusterIdentifier": str,
     },
     total=False,
@@ -1957,22 +1897,20 @@
     "_OptionalRemoveRoleFromDBClusterMessageRequestTypeDef",
     {
         "FeatureName": str,
     },
     total=False,
 )
 
-
 class RemoveRoleFromDBClusterMessageRequestTypeDef(
     _RequiredRemoveRoleFromDBClusterMessageRequestTypeDef,
     _OptionalRemoveRoleFromDBClusterMessageRequestTypeDef,
 ):
     pass
 
-
 RemoveRoleFromDBInstanceMessageRequestTypeDef = TypedDict(
     "RemoveRoleFromDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "RoleArn": str,
         "FeatureName": str,
     },
@@ -2007,31 +1945,28 @@
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-
 class RevokeDBSecurityGroupIngressMessageRequestTypeDef(
     _RequiredRevokeDBSecurityGroupIngressMessageRequestTypeDef,
     _OptionalRevokeDBSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
-
 SourceRegionTypeDef = TypedDict(
     "SourceRegionTypeDef",
     {
         "RegionName": str,
         "Endpoint": str,
         "Status": str,
         "SupportsDBInstanceAutomatedBackupsReplication": bool,
     },
-    total=False,
 )
 
 _RequiredStartActivityStreamRequestRequestTypeDef = TypedDict(
     "_RequiredStartActivityStreamRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Mode": ActivityStreamModeType,
@@ -2043,22 +1978,20 @@
     {
         "ApplyImmediately": bool,
         "EngineNativeAuditFieldsIncluded": bool,
     },
     total=False,
 )
 
-
 class StartActivityStreamRequestRequestTypeDef(
     _RequiredStartActivityStreamRequestRequestTypeDef,
     _OptionalStartActivityStreamRequestRequestTypeDef,
 ):
     pass
 
-
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -2075,22 +2008,20 @@
         "KmsKeyId": str,
         "PreSignedUrl": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class StartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef(
     _RequiredStartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
     _OptionalStartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
 ):
     pass
 
-
 StartDBInstanceMessageRequestTypeDef = TypedDict(
     "StartDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 
@@ -2109,43 +2040,39 @@
     {
         "S3Prefix": str,
         "ExportOnly": Sequence[str],
     },
     total=False,
 )
 
-
 class StartExportTaskMessageRequestTypeDef(
     _RequiredStartExportTaskMessageRequestTypeDef, _OptionalStartExportTaskMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredStopActivityStreamRequestRequestTypeDef = TypedDict(
     "_RequiredStopActivityStreamRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalStopActivityStreamRequestRequestTypeDef = TypedDict(
     "_OptionalStopActivityStreamRequestRequestTypeDef",
     {
         "ApplyImmediately": bool,
     },
     total=False,
 )
 
-
 class StopActivityStreamRequestRequestTypeDef(
     _RequiredStopActivityStreamRequestRequestTypeDef,
     _OptionalStopActivityStreamRequestRequestTypeDef,
 ):
     pass
 
-
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -2166,43 +2093,39 @@
     "_OptionalStopDBInstanceMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
     total=False,
 )
 
-
 class StopDBInstanceMessageRequestTypeDef(
     _RequiredStopDBInstanceMessageRequestTypeDef, _OptionalStopDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
     },
 )
 _OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     {
         "SwitchoverTimeout": int,
     },
     total=False,
 )
 
-
 class SwitchoverBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 SwitchoverReadReplicaMessageRequestTypeDef = TypedDict(
     "SwitchoverReadReplicaMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 
@@ -2210,16 +2133,16 @@
     "AccountAttributesMessageTypeDef",
     {
         "AccountQuotas": List[AccountQuotaTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DBClusterBacktrackResponseTypeDef = TypedDict(
-    "DBClusterBacktrackResponseTypeDef",
+DBClusterBacktrackResponseMetadataTypeDef = TypedDict(
+    "DBClusterBacktrackResponseMetadataTypeDef",
     {
         "DBClusterIdentifier": str,
         "BacktrackIdentifier": str,
         "BacktrackTo": datetime,
         "BacktrackedFrom": datetime,
         "BacktrackRequestCreationTime": datetime,
         "Status": str,
@@ -2235,16 +2158,16 @@
         "CurrentCapacity": int,
         "SecondsBeforeTimeout": int,
         "TimeoutAction": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DBClusterEndpointResponseTypeDef = TypedDict(
-    "DBClusterEndpointResponseTypeDef",
+DBClusterEndpointResponseMetadataTypeDef = TypedDict(
+    "DBClusterEndpointResponseMetadataTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
         "DBClusterIdentifier": str,
         "DBClusterEndpointResourceIdentifier": str,
         "Endpoint": str,
         "Status": str,
         "EndpointType": str,
@@ -2285,16 +2208,16 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ExportTaskResponseTypeDef = TypedDict(
-    "ExportTaskResponseTypeDef",
+ExportTaskResponseMetadataTypeDef = TypedDict(
+    "ExportTaskResponseMetadataTypeDef",
     {
         "ExportTaskIdentifier": str,
         "SourceArn": str,
         "ExportOnly": List[str],
         "SnapshotTime": datetime,
         "TaskStartTime": datetime,
         "TaskEndTime": datetime,
@@ -2417,22 +2340,20 @@
     "_OptionalCopyDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCopyDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBClusterSnapshotMessageRequestTypeDef",
     {
         "SourceDBClusterSnapshotIdentifier": str,
         "TargetDBClusterSnapshotIdentifier": str,
     },
 )
@@ -2444,22 +2365,20 @@
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CopyDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCopyDBParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBParameterGroupMessageRequestTypeDef",
     {
         "SourceDBParameterGroupIdentifier": str,
         "TargetDBParameterGroupIdentifier": str,
         "TargetDBParameterGroupDescription": str,
     },
@@ -2468,22 +2387,20 @@
     "_OptionalCopyDBParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyDBParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCopyDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBSnapshotMessageRequestTypeDef",
     {
         "SourceDBSnapshotIdentifier": str,
         "TargetDBSnapshotIdentifier": str,
     },
 )
@@ -2498,21 +2415,19 @@
         "TargetCustomAvailabilityZone": str,
         "CopyOptionGroup": bool,
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CopyDBSnapshotMessageRequestTypeDef(
     _RequiredCopyDBSnapshotMessageRequestTypeDef, _OptionalCopyDBSnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCopyOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCopyOptionGroupMessageRequestTypeDef",
     {
         "SourceOptionGroupIdentifier": str,
         "TargetOptionGroupIdentifier": str,
         "TargetOptionGroupDescription": str,
     },
@@ -2521,21 +2436,19 @@
     "_OptionalCopyOptionGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyOptionGroupMessageRequestTypeDef(
     _RequiredCopyOptionGroupMessageRequestTypeDef, _OptionalCopyOptionGroupMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentName": str,
         "Source": str,
     },
 )
@@ -2546,22 +2459,20 @@
         "TargetDBParameterGroupName": str,
         "TargetDBClusterParameterGroupName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredCreateBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalCreateBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
@@ -2575,22 +2486,20 @@
         "Description": str,
         "Manifest": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCustomDBEngineVersionMessageRequestTypeDef(
     _RequiredCreateCustomDBEngineVersionMessageRequestTypeDef,
     _OptionalCreateCustomDBEngineVersionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "EndpointType": str,
     },
@@ -2601,22 +2510,20 @@
         "StaticMembers": Sequence[str],
         "ExcludedMembers": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBClusterEndpointMessageRequestTypeDef(
     _RequiredCreateDBClusterEndpointMessageRequestTypeDef,
     _OptionalCreateDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -2625,22 +2532,20 @@
     "_OptionalCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterIdentifier": str,
     },
 )
@@ -2648,22 +2553,20 @@
     "_OptionalCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBParameterGroupMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -2672,22 +2575,20 @@
     "_OptionalCreateDBParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBProxyEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDBProxyEndpointRequestRequestTypeDef",
     {
         "DBProxyName": str,
         "DBProxyEndpointName": str,
         "VpcSubnetIds": Sequence[str],
     },
@@ -2698,22 +2599,20 @@
         "VpcSecurityGroupIds": Sequence[str],
         "TargetRole": DBProxyEndpointTargetRoleType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBProxyEndpointRequestRequestTypeDef(
     _RequiredCreateDBProxyEndpointRequestRequestTypeDef,
     _OptionalCreateDBProxyEndpointRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSecurityGroupMessageRequestTypeDef",
     {
         "DBSecurityGroupName": str,
         "DBSecurityGroupDescription": str,
     },
 )
@@ -2721,22 +2620,20 @@
     "_OptionalCreateDBSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBSecurityGroupMessageRequestTypeDef(
     _RequiredCreateDBSecurityGroupMessageRequestTypeDef,
     _OptionalCreateDBSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSnapshotMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "DBInstanceIdentifier": str,
     },
 )
@@ -2744,21 +2641,19 @@
     "_OptionalCreateDBSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBSnapshotMessageRequestTypeDef(
     _RequiredCreateDBSnapshotMessageRequestTypeDef, _OptionalCreateDBSnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -2767,22 +2662,20 @@
     "_OptionalCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBSubnetGroupMessageRequestTypeDef(
     _RequiredCreateDBSubnetGroupMessageRequestTypeDef,
     _OptionalCreateDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "SnsTopicArn": str,
     },
 )
@@ -2794,22 +2687,20 @@
         "SourceIds": Sequence[str],
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateOptionGroupMessageRequestTypeDef",
     {
         "OptionGroupName": str,
         "EngineName": str,
         "MajorEngineVersion": str,
         "OptionGroupDescription": str,
@@ -2819,53 +2710,19 @@
     "_OptionalCreateOptionGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateOptionGroupMessageRequestTypeDef(
     _RequiredCreateOptionGroupMessageRequestTypeDef, _OptionalCreateOptionGroupMessageRequestTypeDef
 ):
     pass
 
-
-DBClusterSnapshotTypeDef = TypedDict(
-    "DBClusterSnapshotTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "DBClusterSnapshotIdentifier": str,
-        "DBClusterIdentifier": str,
-        "SnapshotCreateTime": datetime,
-        "Engine": str,
-        "EngineMode": str,
-        "AllocatedStorage": int,
-        "Status": str,
-        "Port": int,
-        "VpcId": str,
-        "ClusterCreateTime": datetime,
-        "MasterUsername": str,
-        "EngineVersion": str,
-        "LicenseModel": str,
-        "SnapshotType": str,
-        "PercentProgress": int,
-        "StorageEncrypted": bool,
-        "KmsKeyId": str,
-        "DBClusterSnapshotArn": str,
-        "SourceDBClusterSnapshotArn": str,
-        "IAMDatabaseAuthenticationEnabled": bool,
-        "TagList": List[TagTypeDef],
-        "DBSystemId": str,
-        "StorageType": str,
-        "DbClusterResourceId": str,
-    },
-    total=False,
-)
-
 _RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef",
     {
         "ReservedDBInstancesOfferingId": str,
     },
 )
 _OptionalPurchaseReservedDBInstancesOfferingMessageRequestTypeDef = TypedDict(
@@ -2874,30 +2731,20 @@
         "ReservedDBInstanceId": str,
         "DBInstanceCount": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PurchaseReservedDBInstancesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
 ):
     pass
 
-
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
@@ -2929,57 +2776,69 @@
         "SupportedNetworkTypes": List[str],
         "SupportsStorageThroughput": bool,
         "MinStorageThroughputPerDbInstance": int,
         "MaxStorageThroughputPerDbInstance": int,
         "MinStorageThroughputPerIops": float,
         "MaxStorageThroughputPerIops": float,
     },
-    total=False,
-)
-
-_RequiredBacktrackDBClusterMessageRequestTypeDef = TypedDict(
-    "_RequiredBacktrackDBClusterMessageRequestTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "BacktrackTo": TimestampTypeDef,
-    },
-)
-_OptionalBacktrackDBClusterMessageRequestTypeDef = TypedDict(
-    "_OptionalBacktrackDBClusterMessageRequestTypeDef",
-    {
-        "Force": bool,
-        "UseEarliestTimeOnPointInTimeUnavailable": bool,
-    },
-    total=False,
 )
 
-
-class BacktrackDBClusterMessageRequestTypeDef(
-    _RequiredBacktrackDBClusterMessageRequestTypeDef,
-    _OptionalBacktrackDBClusterMessageRequestTypeDef,
-):
-    pass
-
-
 BlueGreenDeploymentTypeDef = TypedDict(
     "BlueGreenDeploymentTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "BlueGreenDeploymentName": str,
         "Source": str,
         "Target": str,
         "SwitchoverDetails": List[SwitchoverDetailTypeDef],
         "Tasks": List[BlueGreenDeploymentTaskTypeDef],
         "Status": str,
         "StatusDetails": str,
         "CreateTime": datetime,
         "DeleteTime": datetime,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
+    },
+)
+
+DBClusterSnapshotTypeDef = TypedDict(
+    "DBClusterSnapshotTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "DBClusterSnapshotIdentifier": str,
+        "DBClusterIdentifier": str,
+        "SnapshotCreateTime": datetime,
+        "Engine": str,
+        "EngineMode": str,
+        "AllocatedStorage": int,
+        "Status": str,
+        "Port": int,
+        "VpcId": str,
+        "ClusterCreateTime": datetime,
+        "MasterUsername": str,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "SnapshotType": str,
+        "PercentProgress": int,
+        "StorageEncrypted": bool,
+        "KmsKeyId": str,
+        "DBClusterSnapshotArn": str,
+        "SourceDBClusterSnapshotArn": str,
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "TagList": List[TagOutputTypeDef],
+        "DBSystemId": str,
+        "StorageType": str,
+    },
+)
+
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
@@ -3004,30 +2863,28 @@
         "IAMDatabaseAuthenticationEnabled": bool,
         "EngineVersion": str,
         "BackupRetentionPeriod": int,
         "AllocatedStorage": int,
         "Iops": int,
         "StorageType": str,
     },
-    total=False,
 )
 
 DBProxyTargetGroupTypeDef = TypedDict(
     "DBProxyTargetGroupTypeDef",
     {
         "DBProxyName": str,
         "TargetGroupName": str,
         "TargetGroupArn": str,
         "IsDefault": bool,
         "Status": str,
         "ConnectionPoolConfig": ConnectionPoolConfigurationInfoTypeDef,
         "CreatedDate": datetime,
         "UpdatedDate": datetime,
     },
-    total=False,
 )
 
 _RequiredModifyDBProxyTargetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyTargetGroupRequestRequestTypeDef",
     {
         "TargetGroupName": str,
         "DBProxyName": str,
@@ -3038,22 +2895,20 @@
     {
         "ConnectionPoolConfig": ConnectionPoolConfigurationTypeDef,
         "NewName": str,
     },
     total=False,
 )
 
-
 class ModifyDBProxyTargetGroupRequestRequestTypeDef(
     _RequiredModifyDBProxyTargetGroupRequestRequestTypeDef,
     _OptionalModifyDBProxyTargetGroupRequestRequestTypeDef,
 ):
     pass
 
-
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3153,27 +3008,24 @@
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
         "DBSystemId": str,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
-        "EnableLocalWriteForwarding": bool,
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CreateDBClusterMessageRequestTypeDef(
     _RequiredCreateDBClusterMessageRequestTypeDef, _OptionalCreateDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalModifyDBClusterMessageRequestTypeDef = TypedDict(
@@ -3215,26 +3067,23 @@
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
         "ManageMasterUserPassword": bool,
         "RotateMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "EngineMode": str,
         "AllowEngineModeChange": bool,
-        "EnableLocalWriteForwarding": bool,
     },
     total=False,
 )
 
-
 class ModifyDBClusterMessageRequestTypeDef(
     _RequiredModifyDBClusterMessageRequestTypeDef, _OptionalModifyDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredRestoreDBClusterFromS3MessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromS3MessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Engine": str,
         "MasterUsername": str,
         "SourceEngine": str,
@@ -3275,22 +3124,20 @@
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "StorageType": str,
     },
     total=False,
 )
 
-
 class RestoreDBClusterFromS3MessageRequestTypeDef(
     _RequiredRestoreDBClusterFromS3MessageRequestTypeDef,
     _OptionalRestoreDBClusterFromS3MessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "Engine": str,
     },
@@ -3323,34 +3170,32 @@
         "PubliclyAccessible": bool,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
     },
     total=False,
 )
 
-
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
+        "SourceDBClusterIdentifier": str,
     },
 )
 _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "RestoreType": str,
-        "SourceDBClusterIdentifier": str,
-        "RestoreToTime": TimestampTypeDef,
+        "RestoreToTime": Union[datetime, str],
         "UseLatestRestorableTime": bool,
         "Port": int,
         "DBSubnetGroupName": str,
         "OptionGroupName": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
@@ -3366,27 +3211,24 @@
         "EngineMode": str,
         "DBClusterInstanceClass": str,
         "StorageType": str,
         "PubliclyAccessible": bool,
         "Iops": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
-        "SourceDbClusterResourceId": str,
     },
     total=False,
 )
 
-
 class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
     },
@@ -3451,21 +3293,19 @@
         "MasterUserSecretKmsKeyId": str,
         "CACertificateIdentifier": str,
         "DBSystemId": str,
     },
     total=False,
 )
 
-
 class CreateDBInstanceMessageRequestTypeDef(
     _RequiredCreateDBInstanceMessageRequestTypeDef, _OptionalCreateDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalCreateDBInstanceReadReplicaMessageRequestTypeDef = TypedDict(
@@ -3513,63 +3353,20 @@
         "AllocatedStorage": int,
         "SourceDBClusterIdentifier": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CreateDBInstanceReadReplicaMessageRequestTypeDef(
     _RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef,
     _OptionalCreateDBInstanceReadReplicaMessageRequestTypeDef,
 ):
     pass
 
-
-DBSnapshotTypeDef = TypedDict(
-    "DBSnapshotTypeDef",
-    {
-        "DBSnapshotIdentifier": str,
-        "DBInstanceIdentifier": str,
-        "SnapshotCreateTime": datetime,
-        "Engine": str,
-        "AllocatedStorage": int,
-        "Status": str,
-        "Port": int,
-        "AvailabilityZone": str,
-        "VpcId": str,
-        "InstanceCreateTime": datetime,
-        "MasterUsername": str,
-        "EngineVersion": str,
-        "LicenseModel": str,
-        "SnapshotType": str,
-        "Iops": int,
-        "OptionGroupName": str,
-        "PercentProgress": int,
-        "SourceRegion": str,
-        "SourceDBSnapshotIdentifier": str,
-        "StorageType": str,
-        "TdeCredentialArn": str,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "DBSnapshotArn": str,
-        "Timezone": str,
-        "IAMDatabaseAuthenticationEnabled": bool,
-        "ProcessorFeatures": List[ProcessorFeatureTypeDef],
-        "DbiResourceId": str,
-        "TagList": List[TagTypeDef],
-        "OriginalSnapshotCreateTime": datetime,
-        "SnapshotDatabaseTime": datetime,
-        "SnapshotTarget": str,
-        "StorageThroughput": int,
-        "DBSystemId": str,
-    },
-    total=False,
-)
-
 _RequiredModifyDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalModifyDBInstanceMessageRequestTypeDef = TypedDict(
@@ -3632,48 +3429,19 @@
         "RotateMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "Engine": str,
     },
     total=False,
 )
 
-
 class ModifyDBInstanceMessageRequestTypeDef(
     _RequiredModifyDBInstanceMessageRequestTypeDef, _OptionalModifyDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
-PendingModifiedValuesTypeDef = TypedDict(
-    "PendingModifiedValuesTypeDef",
-    {
-        "DBInstanceClass": str,
-        "AllocatedStorage": int,
-        "MasterUserPassword": str,
-        "Port": int,
-        "BackupRetentionPeriod": int,
-        "MultiAZ": bool,
-        "EngineVersion": str,
-        "LicenseModel": str,
-        "Iops": int,
-        "DBInstanceIdentifier": str,
-        "StorageType": str,
-        "CACertificateIdentifier": str,
-        "DBSubnetGroupName": str,
-        "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
-        "ProcessorFeatures": List[ProcessorFeatureTypeDef],
-        "IAMDatabaseAuthenticationEnabled": bool,
-        "AutomationMode": AutomationModeType,
-        "ResumeFullAutomationModeTime": datetime,
-        "StorageThroughput": int,
-        "Engine": str,
-    },
-    total=False,
-)
-
 _RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef = TypedDict(
@@ -3717,22 +3485,20 @@
         "StorageThroughput": int,
         "DBClusterSnapshotIdentifier": str,
         "AllocatedStorage": int,
     },
     total=False,
 )
 
-
 class RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreDBInstanceFromS3MessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceFromS3MessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
         "SourceEngine": str,
@@ -3785,33 +3551,31 @@
         "StorageThroughput": int,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
     },
     total=False,
 )
 
-
 class RestoreDBInstanceFromS3MessageRequestTypeDef(
     _RequiredRestoreDBInstanceFromS3MessageRequestTypeDef,
     _OptionalRestoreDBInstanceFromS3MessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
     },
 )
 _OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
     "_OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     {
         "SourceDBInstanceIdentifier": str,
-        "RestoreTime": TimestampTypeDef,
+        "RestoreTime": Union[datetime, str],
         "UseLatestRestorableTime": bool,
         "DBInstanceClass": str,
         "Port": int,
         "AvailabilityZone": str,
         "DBSubnetGroupName": str,
         "MultiAZ": bool,
         "PubliclyAccessible": bool,
@@ -3848,22 +3612,20 @@
         "NetworkType": str,
         "StorageThroughput": int,
         "AllocatedStorage": int,
     },
     total=False,
 )
 
-
 class RestoreDBInstanceToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
-
 CreateDBProxyEndpointResponseTypeDef = TypedDict(
     "CreateDBProxyEndpointResponseTypeDef",
     {
         "DBProxyEndpoint": DBProxyEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3911,21 +3673,19 @@
         "IdleClientTimeout": int,
         "DebugLogging": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBProxyRequestRequestTypeDef(
     _RequiredCreateDBProxyRequestRequestTypeDef, _OptionalCreateDBProxyRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyDBProxyRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalModifyDBProxyRequestRequestTypeDef = TypedDict(
@@ -3938,51 +3698,19 @@
         "DebugLogging": bool,
         "RoleArn": str,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBProxyRequestRequestTypeDef(
     _RequiredModifyDBProxyRequestRequestTypeDef, _OptionalModifyDBProxyRequestRequestTypeDef
 ):
     pass
 
-
-DBClusterAutomatedBackupTypeDef = TypedDict(
-    "DBClusterAutomatedBackupTypeDef",
-    {
-        "Engine": str,
-        "VpcId": str,
-        "DBClusterAutomatedBackupsArn": str,
-        "DBClusterIdentifier": str,
-        "RestoreWindow": RestoreWindowTypeDef,
-        "MasterUsername": str,
-        "DbClusterResourceId": str,
-        "Region": str,
-        "LicenseModel": str,
-        "Status": str,
-        "IAMDatabaseAuthenticationEnabled": bool,
-        "ClusterCreateTime": datetime,
-        "StorageEncrypted": bool,
-        "AllocatedStorage": int,
-        "EngineVersion": str,
-        "DBClusterArn": str,
-        "BackupRetentionPeriod": int,
-        "EngineMode": str,
-        "AvailabilityZones": List[str],
-        "Port": int,
-        "KmsKeyId": str,
-        "StorageType": str,
-        "Iops": int,
-    },
-    total=False,
-)
-
 DBClusterBacktrackMessageTypeDef = TypedDict(
     "DBClusterBacktrackMessageTypeDef",
     {
         "Marker": str,
         "DBClusterBacktracks": List[DBClusterBacktrackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4018,28 +3746,26 @@
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
         "Parameters": List[ParameterOutputTypeDef],
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
-DBEngineVersionResponseTypeDef = TypedDict(
-    "DBEngineVersionResponseTypeDef",
+DBEngineVersionResponseMetadataTypeDef = TypedDict(
+    "DBEngineVersionResponseMetadataTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "DBEngineDescription": str,
         "DBEngineVersionDescription": str,
         "DefaultCharacterSet": CharacterSetTypeDef,
@@ -4059,20 +3785,19 @@
         "SupportsGlobalDatabases": bool,
         "MajorEngineVersion": str,
         "DatabaseInstallationFilesS3BucketName": str,
         "DatabaseInstallationFilesS3Prefix": str,
         "DBEngineVersionArn": str,
         "KMSKeyId": str,
         "CreateTime": datetime,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "SupportsBabelfish": bool,
         "CustomDBEngineVersionManifest": str,
         "SupportsCertificateRotationWithoutRestart": bool,
         "SupportedCACertificateIdentifiers": List[str],
-        "SupportsLocalWriteForwarding": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
@@ -4098,22 +3823,20 @@
         "SupportsGlobalDatabases": bool,
         "MajorEngineVersion": str,
         "DatabaseInstallationFilesS3BucketName": str,
         "DatabaseInstallationFilesS3Prefix": str,
         "DBEngineVersionArn": str,
         "KMSKeyId": str,
         "CreateTime": datetime,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "SupportsBabelfish": bool,
         "CustomDBEngineVersionManifest": str,
         "SupportsCertificateRotationWithoutRestart": bool,
         "SupportedCACertificateIdentifiers": List[str],
-        "SupportsLocalWriteForwarding": bool,
     },
-    total=False,
 )
 
 DBInstanceAutomatedBackupTypeDef = TypedDict(
     "DBInstanceAutomatedBackupTypeDef",
     {
         "DBInstanceArn": str,
         "DbiResourceId": str,
@@ -4142,30 +3865,94 @@
         "DBInstanceAutomatedBackupsArn": str,
         "DBInstanceAutomatedBackupsReplications": List[
             DBInstanceAutomatedBackupsReplicationTypeDef
         ],
         "BackupTarget": str,
         "StorageThroughput": int,
     },
-    total=False,
+)
+
+DBSnapshotTypeDef = TypedDict(
+    "DBSnapshotTypeDef",
+    {
+        "DBSnapshotIdentifier": str,
+        "DBInstanceIdentifier": str,
+        "SnapshotCreateTime": datetime,
+        "Engine": str,
+        "AllocatedStorage": int,
+        "Status": str,
+        "Port": int,
+        "AvailabilityZone": str,
+        "VpcId": str,
+        "InstanceCreateTime": datetime,
+        "MasterUsername": str,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "SnapshotType": str,
+        "Iops": int,
+        "OptionGroupName": str,
+        "PercentProgress": int,
+        "SourceRegion": str,
+        "SourceDBSnapshotIdentifier": str,
+        "StorageType": str,
+        "TdeCredentialArn": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "DBSnapshotArn": str,
+        "Timezone": str,
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "ProcessorFeatures": List[ProcessorFeatureOutputTypeDef],
+        "DbiResourceId": str,
+        "TagList": List[TagOutputTypeDef],
+        "OriginalSnapshotCreateTime": datetime,
+        "SnapshotDatabaseTime": datetime,
+        "SnapshotTarget": str,
+        "StorageThroughput": int,
+        "DBSystemId": str,
+    },
+)
+
+PendingModifiedValuesTypeDef = TypedDict(
+    "PendingModifiedValuesTypeDef",
+    {
+        "DBInstanceClass": str,
+        "AllocatedStorage": int,
+        "MasterUserPassword": str,
+        "Port": int,
+        "BackupRetentionPeriod": int,
+        "MultiAZ": bool,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "Iops": int,
+        "DBInstanceIdentifier": str,
+        "StorageType": str,
+        "CACertificateIdentifier": str,
+        "DBSubnetGroupName": str,
+        "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
+        "ProcessorFeatures": List[ProcessorFeatureOutputTypeDef],
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "AutomationMode": AutomationModeType,
+        "ResumeFullAutomationModeTime": datetime,
+        "StorageThroughput": int,
+        "Engine": str,
+    },
 )
 
 DBProxyTargetTypeDef = TypedDict(
     "DBProxyTargetTypeDef",
     {
         "TargetArn": str,
         "Endpoint": str,
         "TrackedClusterId": str,
         "RdsResourceId": str,
         "Port": int,
         "Type": TargetTypeType,
         "Role": TargetRoleType,
         "TargetHealth": TargetHealthTypeDef,
     },
-    total=False,
 )
 
 DBProxyTypeDef = TypedDict(
     "DBProxyTypeDef",
     {
         "DBProxyName": str,
         "DBProxyArn": str,
@@ -4179,38 +3966,35 @@
         "Endpoint": str,
         "RequireTLS": bool,
         "IdleClientTimeout": int,
         "DebugLogging": bool,
         "CreatedDate": datetime,
         "UpdatedDate": datetime,
     },
-    total=False,
 )
 
 DBSecurityGroupTypeDef = TypedDict(
     "DBSecurityGroupTypeDef",
     {
         "OwnerId": str,
         "DBSecurityGroupName": str,
         "DBSecurityGroupDescription": str,
         "VpcId": str,
         "EC2SecurityGroups": List[EC2SecurityGroupTypeDef],
         "IPRanges": List[IPRangeTypeDef],
         "DBSecurityGroupArn": str,
     },
-    total=False,
 )
 
 DBSnapshotAttributesResultTypeDef = TypedDict(
     "DBSnapshotAttributesResultTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "DBSnapshotAttributes": List[DBSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
 DescribeBlueGreenDeploymentsRequestRequestTypeDef = TypedDict(
     "DescribeBlueGreenDeploymentsRequestRequestTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
@@ -4227,26 +4011,14 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBClusterAutomatedBackupsMessageRequestTypeDef = TypedDict(
-    "DescribeDBClusterAutomatedBackupsMessageRequestTypeDef",
-    {
-        "DbClusterResourceId": str,
-        "DBClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
 _RequiredDescribeDBClusterBacktracksMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterBacktracksMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalDescribeDBClusterBacktracksMessageRequestTypeDef = TypedDict(
@@ -4256,22 +4028,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDBClusterBacktracksMessageRequestTypeDef(
     _RequiredDescribeDBClusterBacktracksMessageRequestTypeDef,
     _OptionalDescribeDBClusterBacktracksMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeDBClusterEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
@@ -4304,34 +4074,31 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
-        "DbClusterResourceId": str,
     },
     total=False,
 )
 
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
@@ -4400,22 +4167,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDBLogFilesMessageRequestTypeDef(
     _RequiredDescribeDBLogFilesMessageRequestTypeDef,
     _OptionalDescribeDBLogFilesMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -4436,22 +4201,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDBParametersMessageRequestTypeDef(
     _RequiredDescribeDBParametersMessageRequestTypeDef,
     _OptionalDescribeDBParametersMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeDBProxiesRequestRequestTypeDef = TypedDict(
     "DescribeDBProxiesRequestRequestTypeDef",
     {
         "DBProxyName": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4484,22 +4247,20 @@
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeDBProxyTargetGroupsRequestRequestTypeDef(
     _RequiredDescribeDBProxyTargetGroupsRequestRequestTypeDef,
     _OptionalDescribeDBProxyTargetGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDBProxyTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDBProxyTargetsRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalDescribeDBProxyTargetsRequestRequestTypeDef = TypedDict(
@@ -4509,22 +4270,20 @@
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeDBProxyTargetsRequestRequestTypeDef(
     _RequiredDescribeDBProxyTargetsRequestRequestTypeDef,
     _OptionalDescribeDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDBSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSecurityGroupsMessageRequestTypeDef",
     {
         "DBSecurityGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -4571,22 +4330,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -4595,22 +4352,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
@@ -4628,16 +4383,16 @@
 )
 
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
         "Duration": int,
         "EventCategories": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
@@ -4680,22 +4435,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeOptionGroupOptionsMessageRequestTypeDef(
     _RequiredDescribeOptionGroupOptionsMessageRequestTypeDef,
     _OptionalDescribeOptionGroupOptionsMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeOptionGroupsMessageRequestTypeDef = TypedDict(
     "DescribeOptionGroupsMessageRequestTypeDef",
     {
         "OptionGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4722,22 +4475,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
-
 DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4800,22 +4551,20 @@
     "_OptionalListTagsForResourceMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class ListTagsForResourceMessageRequestTypeDef(
     _RequiredListTagsForResourceMessageRequestTypeDef,
     _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeBlueGreenDeploymentsRequestDescribeBlueGreenDeploymentsPaginateTypeDef = TypedDict(
     "DescribeBlueGreenDeploymentsRequestDescribeBlueGreenDeploymentsPaginateTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4844,22 +4593,20 @@
         "BacktrackIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef(
     _RequiredDescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef,
     _OptionalDescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4889,32 +4636,29 @@
         "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
     _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "IncludeShared": bool,
         "IncludePublic": bool,
-        "DbClusterResourceId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
     "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
@@ -4979,22 +4723,20 @@
         "FileSize": int,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef(
     _RequiredDescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef,
     _OptionalDescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5013,22 +4755,20 @@
         "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
     _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef = TypedDict(
     "DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef",
     {
         "DBProxyName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5058,22 +4798,20 @@
         "TargetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef(
     _RequiredDescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef,
     _OptionalDescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef = TypedDict(
@@ -5082,22 +4820,20 @@
         "TargetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef(
     _RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef,
     _OptionalDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef = TypedDict(
     "DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef",
     {
         "DBSecurityGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5140,22 +4876,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
@@ -5163,22 +4897,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
-
 DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5186,16 +4918,16 @@
 )
 
 DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
         "Duration": int,
         "EventCategories": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -5234,22 +4966,20 @@
         "MajorEngineVersion": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef(
     _RequiredDescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef,
     _OptionalDescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef,
 ):
     pass
 
-
 DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef = TypedDict(
     "DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef",
     {
         "OptionGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "EngineName": str,
         "MajorEngineVersion": str,
@@ -5274,22 +5004,20 @@
         "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
 ):
     pass
 
-
 DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
     TypedDict(
         "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
         {
             "ResourceIdentifier": str,
             "Filters": Sequence[FilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
@@ -5351,34 +5079,31 @@
     "_OptionalDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef(
     _RequiredDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef,
     _OptionalDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
-        "DbClusterResourceId": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef",
@@ -5387,15 +5112,14 @@
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
-        "DbClusterResourceId": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClustersMessageDBClusterAvailableWaitTypeDef = TypedDict(
     "DescribeDBClustersMessageDBClusterAvailableWaitTypeDef",
@@ -5544,32 +5268,88 @@
         "EngineVersion": str,
         "DatabaseName": str,
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
         "FailoverState": FailoverStateTypeDef,
     },
-    total=False,
 )
 
 OptionGroupOptionSettingTypeDef = TypedDict(
     "OptionGroupOptionSettingTypeDef",
     {
         "SettingName": str,
         "SettingDescription": str,
         "DefaultValue": str,
         "ApplyType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "IsRequired": bool,
         "MinimumEngineVersionPerAllowedValue": List[MinimumEngineVersionPerAllowedValueTypeDef],
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
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
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
+    total=False,
+)
+
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+    },
+)
+_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
     total=False,
 )
 
+class ResetDBParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+):
+    pass
+
 _RequiredOptionConfigurationTypeDef = TypedDict(
     "_RequiredOptionConfigurationTypeDef",
     {
         "OptionName": str,
     },
 )
 _OptionalOptionConfigurationTypeDef = TypedDict(
@@ -5580,70 +5360,63 @@
         "DBSecurityGroupMemberships": Sequence[str],
         "VpcSecurityGroupMemberships": Sequence[str],
         "OptionSettings": Sequence[OptionSettingTypeDef],
     },
     total=False,
 )
 
-
 class OptionConfigurationTypeDef(
     _RequiredOptionConfigurationTypeDef, _OptionalOptionConfigurationTypeDef
 ):
     pass
 
-
 OptionTypeDef = TypedDict(
     "OptionTypeDef",
     {
         "OptionName": str,
         "OptionDescription": str,
         "Persistent": bool,
         "Permanent": bool,
         "Port": int,
         "OptionVersion": str,
-        "OptionSettings": List[OptionSettingTypeDef],
+        "OptionSettings": List[OptionSettingOutputTypeDef],
         "DBSecurityGroupMemberships": List[DBSecurityGroupMembershipTypeDef],
         "VpcSecurityGroupMemberships": List[VpcSecurityGroupMembershipTypeDef],
     },
-    total=False,
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetOutpost": OutpostTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
-ParameterUnionTypeDef = Union[ParameterTypeDef, ParameterOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
 )
 
 ValidStorageOptionsTypeDef = TypedDict(
     "ValidStorageOptionsTypeDef",
     {
         "StorageType": str,
         "StorageSize": List[RangeTypeDef],
         "ProvisionedIops": List[RangeTypeDef],
         "IopsToStorageRatio": List[DoubleRangeTypeDef],
         "SupportsStorageAutoscaling": bool,
         "ProvisionedStorageThroughput": List[RangeTypeDef],
         "StorageThroughputToIopsRatio": List[DoubleRangeTypeDef],
     },
-    total=False,
 )
 
 ReservedDBInstanceTypeDef = TypedDict(
     "ReservedDBInstanceTypeDef",
     {
         "ReservedDBInstanceId": str,
         "ReservedDBInstancesOfferingId": str,
@@ -5658,15 +5431,14 @@
         "OfferingType": str,
         "MultiAZ": bool,
         "State": str,
         "RecurringCharges": List[RecurringChargeTypeDef],
         "ReservedDBInstanceArn": str,
         "LeaseId": str,
     },
-    total=False,
 )
 
 ReservedDBInstancesOfferingTypeDef = TypedDict(
     "ReservedDBInstancesOfferingTypeDef",
     {
         "ReservedDBInstancesOfferingId": str,
         "DBInstanceClass": str,
@@ -5675,97 +5447,96 @@
         "UsagePrice": float,
         "CurrencyCode": str,
         "ProductDescription": str,
         "OfferingType": str,
         "MultiAZ": bool,
         "RecurringCharges": List[RecurringChargeTypeDef],
     },
-    total=False,
 )
 
 SourceRegionMessageTypeDef = TypedDict(
     "SourceRegionMessageTypeDef",
     {
         "Marker": str,
         "SourceRegions": List[SourceRegionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CopyDBClusterSnapshotResultTypeDef = TypedDict(
-    "CopyDBClusterSnapshotResultTypeDef",
+OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
+    "OrderableDBInstanceOptionsMessageTypeDef",
     {
-        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
+        "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
+        "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateDBClusterSnapshotResultTypeDef = TypedDict(
-    "CreateDBClusterSnapshotResultTypeDef",
+CreateBlueGreenDeploymentResponseTypeDef = TypedDict(
+    "CreateBlueGreenDeploymentResponseTypeDef",
     {
-        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
+        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DBClusterSnapshotMessageTypeDef = TypedDict(
-    "DBClusterSnapshotMessageTypeDef",
+DeleteBlueGreenDeploymentResponseTypeDef = TypedDict(
+    "DeleteBlueGreenDeploymentResponseTypeDef",
     {
-        "Marker": str,
-        "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
+        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteDBClusterSnapshotResultTypeDef = TypedDict(
-    "DeleteDBClusterSnapshotResultTypeDef",
+DescribeBlueGreenDeploymentsResponseTypeDef = TypedDict(
+    "DescribeBlueGreenDeploymentsResponseTypeDef",
     {
-        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
+        "BlueGreenDeployments": List[BlueGreenDeploymentTypeDef],
+        "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
-    "OrderableDBInstanceOptionsMessageTypeDef",
+SwitchoverBlueGreenDeploymentResponseTypeDef = TypedDict(
+    "SwitchoverBlueGreenDeploymentResponseTypeDef",
     {
-        "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
-        "Marker": str,
+        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateBlueGreenDeploymentResponseTypeDef = TypedDict(
-    "CreateBlueGreenDeploymentResponseTypeDef",
+CopyDBClusterSnapshotResultTypeDef = TypedDict(
+    "CopyDBClusterSnapshotResultTypeDef",
     {
-        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
+        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteBlueGreenDeploymentResponseTypeDef = TypedDict(
-    "DeleteBlueGreenDeploymentResponseTypeDef",
+CreateDBClusterSnapshotResultTypeDef = TypedDict(
+    "CreateDBClusterSnapshotResultTypeDef",
     {
-        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
+        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeBlueGreenDeploymentsResponseTypeDef = TypedDict(
-    "DescribeBlueGreenDeploymentsResponseTypeDef",
+DBClusterSnapshotMessageTypeDef = TypedDict(
+    "DBClusterSnapshotMessageTypeDef",
     {
-        "BlueGreenDeployments": List[BlueGreenDeploymentTypeDef],
         "Marker": str,
+        "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SwitchoverBlueGreenDeploymentResponseTypeDef = TypedDict(
-    "SwitchoverBlueGreenDeploymentResponseTypeDef",
+DeleteDBClusterSnapshotResultTypeDef = TypedDict(
+    "DeleteDBClusterSnapshotResultTypeDef",
     {
-        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
+        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterTypeDef = TypedDict(
     "DBClusterTypeDef",
     {
@@ -5818,15 +5589,15 @@
         "ActivityStreamMode": ActivityStreamModeType,
         "ActivityStreamStatus": ActivityStreamStatusType,
         "ActivityStreamKmsKeyId": str,
         "ActivityStreamKinesisStreamName": str,
         "CopyTagsToSnapshot": bool,
         "CrossAccountClone": bool,
         "DomainMemberships": List[DomainMembershipTypeDef],
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "GlobalWriteForwardingStatus": WriteForwardingStatusType,
         "GlobalWriteForwardingRequested": bool,
         "PendingModifiedValues": ClusterPendingModifiedValuesTypeDef,
         "DBClusterInstanceClass": str,
         "StorageType": str,
         "Iops": int,
         "PubliclyAccessible": bool,
@@ -5837,17 +5608,15 @@
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationInfoTypeDef,
         "NetworkType": str,
         "DBSystemId": str,
         "MasterUserSecret": MasterUserSecretTypeDef,
         "IOOptimizedNextAllowedModificationTime": datetime,
-        "LocalWriteForwardingStatus": LocalWriteForwardingStatusType,
     },
-    total=False,
 )
 
 DescribeDBProxyTargetGroupsResponseTypeDef = TypedDict(
     "DescribeDBProxyTargetGroupsResponseTypeDef",
     {
         "TargetGroups": List[DBProxyTargetGroupTypeDef],
         "Marker": str,
@@ -5859,72 +5628,14 @@
     "ModifyDBProxyTargetGroupResponseTypeDef",
     {
         "DBProxyTargetGroup": DBProxyTargetGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CopyDBSnapshotResultTypeDef = TypedDict(
-    "CopyDBSnapshotResultTypeDef",
-    {
-        "DBSnapshot": DBSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDBSnapshotResultTypeDef = TypedDict(
-    "CreateDBSnapshotResultTypeDef",
-    {
-        "DBSnapshot": DBSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DBSnapshotMessageTypeDef = TypedDict(
-    "DBSnapshotMessageTypeDef",
-    {
-        "Marker": str,
-        "DBSnapshots": List[DBSnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDBSnapshotResultTypeDef = TypedDict(
-    "DeleteDBSnapshotResultTypeDef",
-    {
-        "DBSnapshot": DBSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyDBSnapshotResultTypeDef = TypedDict(
-    "ModifyDBSnapshotResultTypeDef",
-    {
-        "DBSnapshot": DBSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DBClusterAutomatedBackupMessageTypeDef = TypedDict(
-    "DBClusterAutomatedBackupMessageTypeDef",
-    {
-        "Marker": str,
-        "DBClusterAutomatedBackups": List[DBClusterAutomatedBackupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDBClusterAutomatedBackupResultTypeDef = TypedDict(
-    "DeleteDBClusterAutomatedBackupResultTypeDef",
-    {
-        "DBClusterAutomatedBackup": DBClusterAutomatedBackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5991,14 +5702,55 @@
     "StopDBInstanceAutomatedBackupsReplicationResultTypeDef",
     {
         "DBInstanceAutomatedBackup": DBInstanceAutomatedBackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CopyDBSnapshotResultTypeDef = TypedDict(
+    "CopyDBSnapshotResultTypeDef",
+    {
+        "DBSnapshot": DBSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDBSnapshotResultTypeDef = TypedDict(
+    "CreateDBSnapshotResultTypeDef",
+    {
+        "DBSnapshot": DBSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBSnapshotMessageTypeDef = TypedDict(
+    "DBSnapshotMessageTypeDef",
+    {
+        "Marker": str,
+        "DBSnapshots": List[DBSnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDBSnapshotResultTypeDef = TypedDict(
+    "DeleteDBSnapshotResultTypeDef",
+    {
+        "DBSnapshot": DBSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyDBSnapshotResultTypeDef = TypedDict(
+    "ModifyDBSnapshotResultTypeDef",
+    {
+        "DBSnapshot": DBSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeDBProxyTargetsResponseTypeDef = TypedDict(
     "DescribeDBProxyTargetsResponseTypeDef",
     {
         "Targets": List[DBProxyTargetTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6160,15 +5912,14 @@
         "RequiresAutoMinorEngineVersionUpgrade": bool,
         "VpcOnly": bool,
         "SupportsOptionVersionDowngrade": bool,
         "OptionGroupOptionSettings": List[OptionGroupOptionSettingTypeDef],
         "OptionGroupOptionVersions": List[OptionVersionTypeDef],
         "CopyableCrossAccount": bool,
     },
-    total=False,
 )
 
 _RequiredModifyOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyOptionGroupMessageRequestTypeDef",
     {
         "OptionGroupName": str,
     },
@@ -6179,21 +5930,19 @@
         "OptionsToInclude": Sequence[OptionConfigurationTypeDef],
         "OptionsToRemove": Sequence[str],
         "ApplyImmediately": bool,
     },
     total=False,
 )
 
-
 class ModifyOptionGroupMessageRequestTypeDef(
     _RequiredModifyOptionGroupMessageRequestTypeDef, _OptionalModifyOptionGroupMessageRequestTypeDef
 ):
     pass
 
-
 OptionGroupTypeDef = TypedDict(
     "OptionGroupTypeDef",
     {
         "OptionGroupName": str,
         "OptionGroupDescription": str,
         "EngineName": str,
         "MajorEngineVersion": str,
@@ -6201,93 +5950,29 @@
         "AllowsVpcAndNonVpcInstanceMemberships": bool,
         "VpcId": str,
         "OptionGroupArn": str,
         "SourceOptionGroup": str,
         "SourceAccountId": str,
         "CopyTimestamp": datetime,
     },
-    total=False,
 )
 
 DBSubnetGroupTypeDef = TypedDict(
     "DBSubnetGroupTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
         "SupportedNetworkTypes": List[str],
     },
-    total=False,
-)
-
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
 )
 
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterUnionTypeDef],
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
-        "Parameters": Sequence[ParameterUnionTypeDef],
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
-_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-    },
-)
-_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class ResetDBParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6303,15 +5988,14 @@
 
 ValidDBInstanceModificationsMessageTypeDef = TypedDict(
     "ValidDBInstanceModificationsMessageTypeDef",
     {
         "Storage": List[ValidStorageOptionsTypeDef],
         "ValidProcessorFeatures": List[AvailableProcessorFeatureTypeDef],
     },
-    total=False,
 )
 
 PurchaseReservedDBInstancesOfferingResultTypeDef = TypedDict(
     "PurchaseReservedDBInstancesOfferingResultTypeDef",
     {
         "ReservedDBInstance": ReservedDBInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6538,20 +6222,20 @@
         "DBInstanceArn": str,
         "Timezone": str,
         "IAMDatabaseAuthenticationEnabled": bool,
         "PerformanceInsightsEnabled": bool,
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "EnabledCloudwatchLogsExports": List[str],
-        "ProcessorFeatures": List[ProcessorFeatureTypeDef],
+        "ProcessorFeatures": List[ProcessorFeatureOutputTypeDef],
         "DeletionProtection": bool,
         "AssociatedRoles": List[DBInstanceRoleTypeDef],
         "ListenerEndpoint": EndpointTypeDef,
         "MaxAllocatedStorage": int,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "DBInstanceAutomatedBackupsReplications": List[
             DBInstanceAutomatedBackupsReplicationTypeDef
         ],
         "CustomerOwnedIpEnabled": bool,
         "AwsBackupRecoveryPointArn": str,
         "ActivityStreamStatus": ActivityStreamStatusType,
         "ActivityStreamKmsKeyId": str,
@@ -6565,17 +6249,15 @@
         "NetworkType": str,
         "ActivityStreamPolicyStatus": ActivityStreamPolicyStatusType,
         "StorageThroughput": int,
         "DBSystemId": str,
         "MasterUserSecret": MasterUserSecretTypeDef,
         "CertificateDetails": CertificateDetailsTypeDef,
         "ReadReplicaSourceDBClusterIdentifier": str,
-        "PercentProgress": str,
     },
-    total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/type_defs.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_rds.type_defs import AccountQuotaTypeDef
 
-    data: AccountQuotaTypeDef = ...
+    data: AccountQuotaTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Optional, Sequence, Union
 
 from .literals import (
@@ -27,15 +27,14 @@
     DBProxyEndpointStatusType,
     DBProxyEndpointTargetRoleType,
     DBProxyStatusType,
     EngineFamilyType,
     ExportSourceTypeType,
     FailoverStatusType,
     IAMAuthModeType,
-    LocalWriteForwardingStatusType,
     ReplicaModeType,
     SourceTypeType,
     TargetHealthReasonType,
     TargetRoleType,
     TargetStateType,
     TargetTypeType,
     WriteForwardingStatusType,
@@ -46,29 +45,31 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountQuotaTypeDef",
     "ResponseMetadataTypeDef",
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddRoleToDBInstanceMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AuthorizeDBSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "AvailableProcessorFeatureTypeDef",
-    "TimestampTypeDef",
+    "BacktrackDBClusterMessageRequestTypeDef",
     "BlueGreenDeploymentTaskTypeDef",
     "SwitchoverDetailTypeDef",
+    "TagOutputTypeDef",
     "CancelExportTaskMessageRequestTypeDef",
     "CertificateDetailsTypeDef",
     "CertificateTypeDef",
     "CharacterSetTypeDef",
     "ClientGenerateDbAuthTokenRequestTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
@@ -79,15 +80,14 @@
     "ScalingConfigurationTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "ProcessorFeatureTypeDef",
     "DBProxyEndpointTypeDef",
     "UserAuthConfigTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "CustomDBEngineVersionAMITypeDef",
-    "RestoreWindowTypeDef",
     "DBClusterBacktrackTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
     "ParameterOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
@@ -95,28 +95,29 @@
     "MasterUserSecretTypeDef",
     "ScalingConfigurationInfoTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceAutomatedBackupsReplicationTypeDef",
+    "RestoreWindowTypeDef",
     "DBInstanceRoleTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
+    "ProcessorFeatureOutputTypeDef",
     "TargetHealthTypeDef",
     "UserAuthConfigInfoTypeDef",
     "EC2SecurityGroupTypeDef",
     "IPRangeTypeDef",
     "DBSnapshotAttributeTypeDef",
     "DeleteBlueGreenDeploymentRequestRequestTypeDef",
     "DeleteCustomDBEngineVersionMessageRequestTypeDef",
-    "DeleteDBClusterAutomatedBackupMessageRequestTypeDef",
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceAutomatedBackupMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBParameterGroupMessageRequestTypeDef",
@@ -147,25 +148,26 @@
     "GlobalClusterMemberTypeDef",
     "MinimumEngineVersionPerAllowedValueTypeDef",
     "ModifyActivityStreamRequestRequestTypeDef",
     "ModifyCertificatesMessageRequestTypeDef",
     "ModifyCurrentDBClusterCapacityMessageRequestTypeDef",
     "ModifyCustomDBEngineVersionMessageRequestTypeDef",
     "ModifyDBClusterEndpointMessageRequestTypeDef",
+    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBProxyEndpointRequestRequestTypeDef",
     "ModifyDBSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBSnapshotMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "OptionSettingTypeDef",
     "OptionVersionTypeDef",
+    "OptionSettingOutputTypeDef",
     "OutpostTypeDef",
-    "ParameterTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "PromoteReadReplicaMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBClusterMessageRequestTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RecurringChargeTypeDef",
@@ -185,22 +187,22 @@
     "StopActivityStreamRequestRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
     "StopDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef",
     "StopDBInstanceMessageRequestTypeDef",
     "SwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     "SwitchoverReadReplicaMessageRequestTypeDef",
     "AccountAttributesMessageTypeDef",
-    "DBClusterBacktrackResponseTypeDef",
+    "DBClusterBacktrackResponseMetadataTypeDef",
     "DBClusterCapacityInfoTypeDef",
-    "DBClusterEndpointResponseTypeDef",
+    "DBClusterEndpointResponseMetadataTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DBParameterGroupNameMessageTypeDef",
     "DownloadDBLogFilePortionDetailsTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "ExportTaskResponseTypeDef",
+    "ExportTaskResponseMetadataTypeDef",
     "ModifyActivityStreamResponseTypeDef",
     "StartActivityStreamResponseTypeDef",
     "StopActivityStreamResponseTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EventSubscriptionsMessageTypeDef",
@@ -220,20 +222,19 @@
     "CreateDBParameterGroupMessageRequestTypeDef",
     "CreateDBProxyEndpointRequestRequestTypeDef",
     "CreateDBSecurityGroupMessageRequestTypeDef",
     "CreateDBSnapshotMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateOptionGroupMessageRequestTypeDef",
-    "DBClusterSnapshotTypeDef",
     "PurchaseReservedDBInstancesOfferingMessageRequestTypeDef",
-    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
-    "BacktrackDBClusterMessageRequestTypeDef",
     "BlueGreenDeploymentTypeDef",
+    "DBClusterSnapshotTypeDef",
+    "TagListMessageTypeDef",
     "CertificateMessageTypeDef",
     "ModifyCertificatesResultTypeDef",
     "ClusterPendingModifiedValuesTypeDef",
     "DBProxyTargetGroupTypeDef",
     "ModifyDBProxyTargetGroupRequestRequestTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
@@ -244,43 +245,41 @@
     "CreateDBClusterMessageRequestTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromS3MessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
     "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBInstanceReadReplicaMessageRequestTypeDef",
-    "DBSnapshotTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
-    "PendingModifiedValuesTypeDef",
     "RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef",
     "RestoreDBInstanceFromS3MessageRequestTypeDef",
     "RestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     "CreateDBProxyEndpointResponseTypeDef",
     "DeleteDBProxyEndpointResponseTypeDef",
     "DescribeDBProxyEndpointsResponseTypeDef",
     "ModifyDBProxyEndpointResponseTypeDef",
     "CreateDBProxyRequestRequestTypeDef",
     "ModifyDBProxyRequestRequestTypeDef",
-    "DBClusterAutomatedBackupTypeDef",
     "DBClusterBacktrackMessageTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
-    "DBEngineVersionResponseTypeDef",
+    "DBEngineVersionResponseMetadataTypeDef",
     "DBEngineVersionTypeDef",
     "DBInstanceAutomatedBackupTypeDef",
+    "DBSnapshotTypeDef",
+    "PendingModifiedValuesTypeDef",
     "DBProxyTargetTypeDef",
     "DBProxyTypeDef",
     "DBSecurityGroupTypeDef",
     "DBSnapshotAttributesResultTypeDef",
     "DescribeBlueGreenDeploymentsRequestRequestTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
-    "DescribeDBClusterAutomatedBackupsMessageRequestTypeDef",
     "DescribeDBClusterBacktracksMessageRequestTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
@@ -357,51 +356,52 @@
     "DescribeDBSnapshotsMessageDBSnapshotDeletedWaitTypeDef",
     "DescribeDBLogFilesResponseTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "ExportTasksMessageTypeDef",
     "GlobalClusterTypeDef",
     "OptionGroupOptionSettingTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "OptionConfigurationTypeDef",
     "OptionTypeDef",
     "SubnetTypeDef",
-    "ParameterUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
     "ReservedDBInstanceTypeDef",
     "ReservedDBInstancesOfferingTypeDef",
     "SourceRegionMessageTypeDef",
-    "CopyDBClusterSnapshotResultTypeDef",
-    "CreateDBClusterSnapshotResultTypeDef",
-    "DBClusterSnapshotMessageTypeDef",
-    "DeleteDBClusterSnapshotResultTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "CreateBlueGreenDeploymentResponseTypeDef",
     "DeleteBlueGreenDeploymentResponseTypeDef",
     "DescribeBlueGreenDeploymentsResponseTypeDef",
     "SwitchoverBlueGreenDeploymentResponseTypeDef",
+    "CopyDBClusterSnapshotResultTypeDef",
+    "CreateDBClusterSnapshotResultTypeDef",
+    "DBClusterSnapshotMessageTypeDef",
+    "DeleteDBClusterSnapshotResultTypeDef",
     "DBClusterTypeDef",
     "DescribeDBProxyTargetGroupsResponseTypeDef",
     "ModifyDBProxyTargetGroupResponseTypeDef",
-    "CopyDBSnapshotResultTypeDef",
-    "CreateDBSnapshotResultTypeDef",
-    "DBSnapshotMessageTypeDef",
-    "DeleteDBSnapshotResultTypeDef",
-    "ModifyDBSnapshotResultTypeDef",
-    "DBClusterAutomatedBackupMessageTypeDef",
-    "DeleteDBClusterAutomatedBackupResultTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "DBEngineVersionMessageTypeDef",
     "DBInstanceAutomatedBackupMessageTypeDef",
     "DeleteDBInstanceAutomatedBackupResultTypeDef",
     "StartDBInstanceAutomatedBackupsReplicationResultTypeDef",
     "StopDBInstanceAutomatedBackupsReplicationResultTypeDef",
+    "CopyDBSnapshotResultTypeDef",
+    "CreateDBSnapshotResultTypeDef",
+    "DBSnapshotMessageTypeDef",
+    "DeleteDBSnapshotResultTypeDef",
+    "ModifyDBSnapshotResultTypeDef",
     "DescribeDBProxyTargetsResponseTypeDef",
     "RegisterDBProxyTargetsResponseTypeDef",
     "CreateDBProxyResponseTypeDef",
     "DeleteDBProxyResponseTypeDef",
     "DescribeDBProxiesResponseTypeDef",
     "ModifyDBProxyResponseTypeDef",
     "AuthorizeDBSecurityGroupIngressResultTypeDef",
@@ -416,18 +416,14 @@
     "GlobalClustersMessageTypeDef",
     "ModifyGlobalClusterResultTypeDef",
     "RemoveFromGlobalClusterResultTypeDef",
     "OptionGroupOptionTypeDef",
     "ModifyOptionGroupMessageRequestTypeDef",
     "OptionGroupTypeDef",
     "DBSubnetGroupTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "ApplyPendingMaintenanceActionResultTypeDef",
     "PendingMaintenanceActionsMessageTypeDef",
     "ValidDBInstanceModificationsMessageTypeDef",
     "PurchaseReservedDBInstancesOfferingResultTypeDef",
     "ReservedDBInstanceMessageTypeDef",
     "ReservedDBInstancesOfferingMessageTypeDef",
     "CreateDBClusterResultTypeDef",
@@ -470,15 +466,14 @@
 AccountQuotaTypeDef = TypedDict(
     "AccountQuotaTypeDef",
     {
         "AccountQuotaName": str,
         "Used": int,
         "Max": int,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -499,20 +494,22 @@
     "_OptionalAddRoleToDBClusterMessageRequestTypeDef",
     {
         "FeatureName": str,
     },
     total=False,
 )
 
+
 class AddRoleToDBClusterMessageRequestTypeDef(
     _RequiredAddRoleToDBClusterMessageRequestTypeDef,
     _OptionalAddRoleToDBClusterMessageRequestTypeDef,
 ):
     pass
 
+
 AddRoleToDBInstanceMessageRequestTypeDef = TypedDict(
     "AddRoleToDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "RoleArn": str,
         "FeatureName": str,
     },
@@ -536,15 +533,14 @@
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -574,56 +570,85 @@
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+
 class AuthorizeDBSecurityGroupIngressMessageRequestTypeDef(
     _RequiredAuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
     _OptionalAuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
+
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 AvailableProcessorFeatureTypeDef = TypedDict(
     "AvailableProcessorFeatureTypeDef",
     {
         "Name": str,
         "DefaultValue": str,
         "AllowedValues": str,
     },
+)
+
+_RequiredBacktrackDBClusterMessageRequestTypeDef = TypedDict(
+    "_RequiredBacktrackDBClusterMessageRequestTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "BacktrackTo": Union[datetime, str],
+    },
+)
+_OptionalBacktrackDBClusterMessageRequestTypeDef = TypedDict(
+    "_OptionalBacktrackDBClusterMessageRequestTypeDef",
+    {
+        "Force": bool,
+        "UseEarliestTimeOnPointInTimeUnavailable": bool,
+    },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
+
+class BacktrackDBClusterMessageRequestTypeDef(
+    _RequiredBacktrackDBClusterMessageRequestTypeDef,
+    _OptionalBacktrackDBClusterMessageRequestTypeDef,
+):
+    pass
+
+
 BlueGreenDeploymentTaskTypeDef = TypedDict(
     "BlueGreenDeploymentTaskTypeDef",
     {
         "Name": str,
         "Status": str,
     },
-    total=False,
 )
 
 SwitchoverDetailTypeDef = TypedDict(
     "SwitchoverDetailTypeDef",
     {
         "SourceMember": str,
         "TargetMember": str,
         "Status": str,
     },
-    total=False,
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
 )
 
 CancelExportTaskMessageRequestTypeDef = TypedDict(
     "CancelExportTaskMessageRequestTypeDef",
     {
         "ExportTaskIdentifier": str,
     },
@@ -631,39 +656,36 @@
 
 CertificateDetailsTypeDef = TypedDict(
     "CertificateDetailsTypeDef",
     {
         "CAIdentifier": str,
         "ValidTill": datetime,
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
         "CustomerOverride": bool,
         "CustomerOverrideValidTill": datetime,
     },
-    total=False,
 )
 
 CharacterSetTypeDef = TypedDict(
     "CharacterSetTypeDef",
     {
         "CharacterSetName": str,
         "CharacterSetDescription": str,
     },
-    total=False,
 )
 
 _RequiredClientGenerateDbAuthTokenRequestTypeDef = TypedDict(
     "_RequiredClientGenerateDbAuthTokenRequestTypeDef",
     {
         "DBHostname": str,
         "Port": int,
@@ -674,20 +696,22 @@
     "_OptionalClientGenerateDbAuthTokenRequestTypeDef",
     {
         "Region": Optional[str],
     },
     total=False,
 )
 
+
 class ClientGenerateDbAuthTokenRequestTypeDef(
     _RequiredClientGenerateDbAuthTokenRequestTypeDef,
     _OptionalClientGenerateDbAuthTokenRequestTypeDef,
 ):
     pass
 
+
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
     },
     total=False,
@@ -695,27 +719,25 @@
 
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
-    total=False,
 )
 
 ConnectionPoolConfigurationInfoTypeDef = TypedDict(
     "ConnectionPoolConfigurationInfoTypeDef",
     {
         "MaxConnectionsPercent": int,
         "MaxIdleConnectionsPercent": int,
         "ConnectionBorrowTimeout": int,
         "SessionPinningFilters": List[str],
         "InitQuery": str,
     },
-    total=False,
 )
 
 ConnectionPoolConfigurationTypeDef = TypedDict(
     "ConnectionPoolConfigurationTypeDef",
     {
         "MaxConnectionsPercent": int,
         "MaxIdleConnectionsPercent": int,
@@ -730,26 +752,24 @@
     "DBClusterParameterGroupTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBClusterParameterGroupArn": str,
     },
-    total=False,
 )
 
 DBParameterGroupTypeDef = TypedDict(
     "DBParameterGroupTypeDef",
     {
         "DBParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBParameterGroupArn": str,
     },
-    total=False,
 )
 
 ScalingConfigurationTypeDef = TypedDict(
     "ScalingConfigurationTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
@@ -790,15 +810,14 @@
         "VpcSecurityGroupIds": List[str],
         "VpcSubnetIds": List[str],
         "Endpoint": str,
         "CreatedDate": datetime,
         "TargetRole": DBProxyEndpointTargetRoleType,
         "IsDefault": bool,
     },
-    total=False,
 )
 
 UserAuthConfigTypeDef = TypedDict(
     "UserAuthConfigTypeDef",
     {
         "Description": str,
         "UserName": str,
@@ -826,37 +845,26 @@
 
 CustomDBEngineVersionAMITypeDef = TypedDict(
     "CustomDBEngineVersionAMITypeDef",
     {
         "ImageId": str,
         "Status": str,
     },
-    total=False,
-)
-
-RestoreWindowTypeDef = TypedDict(
-    "RestoreWindowTypeDef",
-    {
-        "EarliestTime": datetime,
-        "LatestTime": datetime,
-    },
-    total=False,
 )
 
 DBClusterBacktrackTypeDef = TypedDict(
     "DBClusterBacktrackTypeDef",
     {
         "DBClusterIdentifier": str,
         "BacktrackIdentifier": str,
         "BacktrackTo": datetime,
         "BacktrackedFrom": datetime,
         "BacktrackRequestCreationTime": datetime,
         "Status": str,
     },
-    total=False,
 )
 
 DBClusterEndpointTypeDef = TypedDict(
     "DBClusterEndpointTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
         "DBClusterIdentifier": str,
@@ -865,35 +873,32 @@
         "Status": str,
         "EndpointType": str,
         "CustomEndpointType": str,
         "StaticMembers": List[str],
         "ExcludedMembers": List[str],
         "DBClusterEndpointArn": str,
     },
-    total=False,
 )
 
 DBClusterMemberTypeDef = TypedDict(
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
     },
-    total=False,
 )
 
 DBClusterOptionGroupStatusTypeDef = TypedDict(
     "DBClusterOptionGroupStatusTypeDef",
     {
         "DBClusterOptionGroupName": str,
         "Status": str,
     },
-    total=False,
 )
 
 ParameterOutputTypeDef = TypedDict(
     "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
@@ -903,232 +908,225 @@
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
         "SupportedEngineModes": List[str],
     },
-    total=False,
 )
 
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
         "FeatureName": str,
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
 
 DomainMembershipTypeDef = TypedDict(
     "DomainMembershipTypeDef",
     {
         "Domain": str,
         "Status": str,
         "FQDN": str,
         "IAMRoleName": str,
         "OU": str,
         "AuthSecretArn": str,
         "DnsIps": List[str],
     },
-    total=False,
 )
 
 MasterUserSecretTypeDef = TypedDict(
     "MasterUserSecretTypeDef",
     {
         "SecretArn": str,
         "SecretStatus": str,
         "KmsKeyId": str,
     },
-    total=False,
 )
 
 ScalingConfigurationInfoTypeDef = TypedDict(
     "ScalingConfigurationInfoTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
         "AutoPause": bool,
         "SecondsUntilAutoPause": int,
         "TimeoutAction": str,
         "SecondsBeforeTimeout": int,
     },
-    total=False,
 )
 
 ServerlessV2ScalingConfigurationInfoTypeDef = TypedDict(
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     {
         "MinCapacity": float,
         "MaxCapacity": float,
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
 
 TimezoneTypeDef = TypedDict(
     "TimezoneTypeDef",
     {
         "TimezoneName": str,
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
         "SupportedEngineModes": List[str],
         "SupportsParallelQuery": bool,
         "SupportsGlobalDatabases": bool,
         "SupportsBabelfish": bool,
-        "SupportsLocalWriteForwarding": bool,
     },
-    total=False,
 )
 
 DBInstanceAutomatedBackupsReplicationTypeDef = TypedDict(
     "DBInstanceAutomatedBackupsReplicationTypeDef",
     {
         "DBInstanceAutomatedBackupsArn": str,
     },
-    total=False,
+)
+
+RestoreWindowTypeDef = TypedDict(
+    "RestoreWindowTypeDef",
+    {
+        "EarliestTime": datetime,
+        "LatestTime": datetime,
+    },
 )
 
 DBInstanceRoleTypeDef = TypedDict(
     "DBInstanceRoleTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
         "Status": str,
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
 
 DBParameterGroupStatusTypeDef = TypedDict(
     "DBParameterGroupStatusTypeDef",
     {
         "DBParameterGroupName": str,
         "ParameterApplyStatus": str,
     },
-    total=False,
 )
 
 DBSecurityGroupMembershipTypeDef = TypedDict(
     "DBSecurityGroupMembershipTypeDef",
     {
         "DBSecurityGroupName": str,
         "Status": str,
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
 
 OptionGroupMembershipTypeDef = TypedDict(
     "OptionGroupMembershipTypeDef",
     {
         "OptionGroupName": str,
         "Status": str,
     },
-    total=False,
+)
+
+ProcessorFeatureOutputTypeDef = TypedDict(
+    "ProcessorFeatureOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
 )
 
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetStateType,
         "Reason": TargetHealthReasonType,
         "Description": str,
     },
-    total=False,
 )
 
 UserAuthConfigInfoTypeDef = TypedDict(
     "UserAuthConfigInfoTypeDef",
     {
         "Description": str,
         "UserName": str,
         "AuthScheme": Literal["SECRETS"],
         "SecretArn": str,
         "IAMAuth": IAMAuthModeType,
         "ClientPasswordAuthType": ClientPasswordAuthTypeType,
     },
-    total=False,
 )
 
 EC2SecurityGroupTypeDef = TypedDict(
     "EC2SecurityGroupTypeDef",
     {
         "Status": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
-    total=False,
 )
 
 IPRangeTypeDef = TypedDict(
     "IPRangeTypeDef",
     {
         "Status": str,
         "CIDRIP": str,
     },
-    total=False,
 )
 
 DBSnapshotAttributeTypeDef = TypedDict(
     "DBSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
-    total=False,
 )
 
 _RequiredDeleteBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
     },
@@ -1137,35 +1135,30 @@
     "_OptionalDeleteBlueGreenDeploymentRequestRequestTypeDef",
     {
         "DeleteTarget": bool,
     },
     total=False,
 )
 
+
 class DeleteBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredDeleteBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalDeleteBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "DeleteCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
 
-DeleteDBClusterAutomatedBackupMessageRequestTypeDef = TypedDict(
-    "DeleteDBClusterAutomatedBackupMessageRequestTypeDef",
-    {
-        "DbClusterResourceId": str,
-    },
-)
-
 DeleteDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 
@@ -1176,24 +1169,25 @@
     },
 )
 _OptionalDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_OptionalDeleteDBClusterMessageRequestTypeDef",
     {
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
-        "DeleteAutomatedBackups": bool,
     },
     total=False,
 )
 
+
 class DeleteDBClusterMessageRequestTypeDef(
     _RequiredDeleteDBClusterMessageRequestTypeDef, _OptionalDeleteDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 DeleteDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 
@@ -1225,19 +1219,21 @@
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
         "DeleteAutomatedBackups": bool,
     },
     total=False,
 )
 
+
 class DeleteDBInstanceMessageRequestTypeDef(
     _RequiredDeleteDBInstanceMessageRequestTypeDef, _OptionalDeleteDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 DeleteDBParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBParameterGroupMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
     },
 )
 
@@ -1309,20 +1305,22 @@
         "TargetGroupName": str,
         "DBInstanceIdentifiers": Sequence[str],
         "DBClusterIdentifiers": Sequence[str],
     },
     total=False,
 )
 
+
 class DeregisterDBProxyTargetsRequestRequestTypeDef(
     _RequiredDeregisterDBProxyTargetsRequestRequestTypeDef,
     _OptionalDeregisterDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -1356,15 +1354,14 @@
 DescribeDBLogFilesDetailsTypeDef = TypedDict(
     "DescribeDBLogFilesDetailsTypeDef",
     {
         "LogFileName": str,
         "LastWritten": int,
         "Size": int,
     },
-    total=False,
 )
 
 DescribeDBSnapshotAttributesMessageRequestTypeDef = TypedDict(
     "DescribeDBSnapshotAttributesMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
@@ -1379,15 +1376,14 @@
 
 DoubleRangeTypeDef = TypedDict(
     "DoubleRangeTypeDef",
     {
         "From": float,
         "To": float,
     },
-    total=False,
 )
 
 _RequiredDownloadDBLogFilePortionMessageRequestTypeDef = TypedDict(
     "_RequiredDownloadDBLogFilePortionMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "LogFileName": str,
@@ -1398,40 +1394,40 @@
     {
         "Marker": str,
         "NumberOfLines": int,
     },
     total=False,
 )
 
+
 class DownloadDBLogFilePortionMessageRequestTypeDef(
     _RequiredDownloadDBLogFilePortionMessageRequestTypeDef,
     _OptionalDownloadDBLogFilePortionMessageRequestTypeDef,
 ):
     pass
 
+
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
 
 ExportTaskTypeDef = TypedDict(
     "ExportTaskTypeDef",
     {
         "ExportTaskIdentifier": str,
         "SourceArn": str,
@@ -1446,15 +1442,14 @@
         "Status": str,
         "PercentProgress": int,
         "TotalExtractedDataInGB": int,
         "FailureCause": str,
         "WarningMessage": str,
         "SourceType": ExportSourceTypeType,
     },
-    total=False,
 )
 
 _RequiredFailoverDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredFailoverDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -1463,19 +1458,21 @@
     "_OptionalFailoverDBClusterMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
     },
     total=False,
 )
 
+
 class FailoverDBClusterMessageRequestTypeDef(
     _RequiredFailoverDBClusterMessageRequestTypeDef, _OptionalFailoverDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 FailoverGlobalClusterMessageRequestTypeDef = TypedDict(
     "FailoverGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "TargetDbClusterIdentifier": str,
     },
 )
@@ -1483,35 +1480,32 @@
 FailoverStateTypeDef = TypedDict(
     "FailoverStateTypeDef",
     {
         "Status": FailoverStatusType,
         "FromDbClusterArn": str,
         "ToDbClusterArn": str,
     },
-    total=False,
 )
 
 GlobalClusterMemberTypeDef = TypedDict(
     "GlobalClusterMemberTypeDef",
     {
         "DBClusterArn": str,
         "Readers": List[str],
         "IsWriter": bool,
         "GlobalWriteForwardingStatus": WriteForwardingStatusType,
     },
-    total=False,
 )
 
 MinimumEngineVersionPerAllowedValueTypeDef = TypedDict(
     "MinimumEngineVersionPerAllowedValueTypeDef",
     {
         "AllowedValue": str,
         "MinimumEngineVersion": str,
     },
-    total=False,
 )
 
 ModifyActivityStreamRequestRequestTypeDef = TypedDict(
     "ModifyActivityStreamRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "AuditPolicyState": AuditPolicyStateType,
@@ -1540,20 +1534,22 @@
         "Capacity": int,
         "SecondsBeforeTimeout": int,
         "TimeoutAction": str,
     },
     total=False,
 )
 
+
 class ModifyCurrentDBClusterCapacityMessageRequestTypeDef(
     _RequiredModifyCurrentDBClusterCapacityMessageRequestTypeDef,
     _OptionalModifyCurrentDBClusterCapacityMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
@@ -1562,20 +1558,22 @@
     {
         "Description": str,
         "Status": CustomEngineVersionStatusType,
     },
     total=False,
 )
 
+
 class ModifyCustomDBEngineVersionMessageRequestTypeDef(
     _RequiredModifyCustomDBEngineVersionMessageRequestTypeDef,
     _OptionalModifyCustomDBEngineVersionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 _OptionalModifyDBClusterEndpointMessageRequestTypeDef = TypedDict(
@@ -1584,20 +1582,40 @@
         "EndpointType": str,
         "StaticMembers": Sequence[str],
         "ExcludedMembers": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBClusterEndpointMessageRequestTypeDef(
     _RequiredModifyDBClusterEndpointMessageRequestTypeDef,
     _OptionalModifyDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
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
+        "SupportedEngineModes": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1606,20 +1624,22 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBClusterSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBProxyEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyEndpointRequestRequestTypeDef",
     {
         "DBProxyEndpointName": str,
     },
 )
 _OptionalModifyDBProxyEndpointRequestRequestTypeDef = TypedDict(
@@ -1627,20 +1647,22 @@
     {
         "NewDBProxyEndpointName": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBProxyEndpointRequestRequestTypeDef(
     _RequiredModifyDBProxyEndpointRequestRequestTypeDef,
     _OptionalModifyDBProxyEndpointRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSnapshotAttributeMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1649,20 +1671,22 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSnapshotMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
 )
 _OptionalModifyDBSnapshotMessageRequestTypeDef = TypedDict(
@@ -1670,19 +1694,21 @@
     {
         "EngineVersion": str,
         "OptionGroupName": str,
     },
     total=False,
 )
 
+
 class ModifyDBSnapshotMessageRequestTypeDef(
     _RequiredModifyDBSnapshotMessageRequestTypeDef, _OptionalModifyDBSnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -1690,20 +1716,22 @@
     "_OptionalModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupDescription": str,
     },
     total=False,
 )
 
+
 class ModifyDBSubnetGroupMessageRequestTypeDef(
     _RequiredModifyDBSubnetGroupMessageRequestTypeDef,
     _OptionalModifyDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -1713,20 +1741,22 @@
         "SourceType": str,
         "EventCategories": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 ModifyGlobalClusterMessageRequestTypeDef = TypedDict(
     "ModifyGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "NewGlobalClusterIdentifier": str,
         "DeletionProtection": bool,
         "EngineVersion": str,
@@ -1753,54 +1783,48 @@
 
 OptionVersionTypeDef = TypedDict(
     "OptionVersionTypeDef",
     {
         "Version": str,
         "IsDefault": bool,
     },
-    total=False,
-)
-
-OutpostTypeDef = TypedDict(
-    "OutpostTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+OptionSettingOutputTypeDef = TypedDict(
+    "OptionSettingOutputTypeDef",
     {
-        "ParameterName": str,
-        "ParameterValue": str,
+        "Name": str,
+        "Value": str,
+        "DefaultValue": str,
         "Description": str,
-        "Source": str,
         "ApplyType": str,
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
-        "MinimumEngineVersion": str,
-        "ApplyMethod": ApplyMethodType,
-        "SupportedEngineModes": Sequence[str],
+        "IsCollection": bool,
+    },
+)
+
+OutpostTypeDef = TypedDict(
+    "OutpostTypeDef",
+    {
+        "Arn": str,
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
 
 PromoteReadReplicaDBClusterMessageRequestTypeDef = TypedDict(
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -1817,28 +1841,29 @@
     {
         "BackupRetentionPeriod": int,
         "PreferredBackupWindow": str,
     },
     total=False,
 )
 
+
 class PromoteReadReplicaMessageRequestTypeDef(
     _RequiredPromoteReadReplicaMessageRequestTypeDef,
     _OptionalPromoteReadReplicaMessageRequestTypeDef,
 ):
     pass
 
+
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "From": int,
         "To": int,
         "Step": int,
     },
-    total=False,
 )
 
 RebootDBClusterMessageRequestTypeDef = TypedDict(
     "RebootDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -1854,26 +1879,27 @@
     "_OptionalRebootDBInstanceMessageRequestTypeDef",
     {
         "ForceFailover": bool,
     },
     total=False,
 )
 
+
 class RebootDBInstanceMessageRequestTypeDef(
     _RequiredRebootDBInstanceMessageRequestTypeDef, _OptionalRebootDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
-    total=False,
 )
 
 _RequiredRegisterDBProxyTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDBProxyTargetsRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
@@ -1884,20 +1910,22 @@
         "TargetGroupName": str,
         "DBInstanceIdentifiers": Sequence[str],
         "DBClusterIdentifiers": Sequence[str],
     },
     total=False,
 )
 
+
 class RegisterDBProxyTargetsRequestRequestTypeDef(
     _RequiredRegisterDBProxyTargetsRequestRequestTypeDef,
     _OptionalRegisterDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 RemoveFromGlobalClusterMessageRequestTypeDef = TypedDict(
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "DbClusterIdentifier": str,
     },
     total=False,
@@ -1914,20 +1942,22 @@
     "_OptionalRemoveRoleFromDBClusterMessageRequestTypeDef",
     {
         "FeatureName": str,
     },
     total=False,
 )
 
+
 class RemoveRoleFromDBClusterMessageRequestTypeDef(
     _RequiredRemoveRoleFromDBClusterMessageRequestTypeDef,
     _OptionalRemoveRoleFromDBClusterMessageRequestTypeDef,
 ):
     pass
 
+
 RemoveRoleFromDBInstanceMessageRequestTypeDef = TypedDict(
     "RemoveRoleFromDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "RoleArn": str,
         "FeatureName": str,
     },
@@ -1962,29 +1992,30 @@
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+
 class RevokeDBSecurityGroupIngressMessageRequestTypeDef(
     _RequiredRevokeDBSecurityGroupIngressMessageRequestTypeDef,
     _OptionalRevokeDBSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
+
 SourceRegionTypeDef = TypedDict(
     "SourceRegionTypeDef",
     {
         "RegionName": str,
         "Endpoint": str,
         "Status": str,
         "SupportsDBInstanceAutomatedBackupsReplication": bool,
     },
-    total=False,
 )
 
 _RequiredStartActivityStreamRequestRequestTypeDef = TypedDict(
     "_RequiredStartActivityStreamRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Mode": ActivityStreamModeType,
@@ -1996,20 +2027,22 @@
     {
         "ApplyImmediately": bool,
         "EngineNativeAuditFieldsIncluded": bool,
     },
     total=False,
 )
 
+
 class StartActivityStreamRequestRequestTypeDef(
     _RequiredStartActivityStreamRequestRequestTypeDef,
     _OptionalStartActivityStreamRequestRequestTypeDef,
 ):
     pass
 
+
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -2026,20 +2059,22 @@
         "KmsKeyId": str,
         "PreSignedUrl": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class StartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef(
     _RequiredStartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
     _OptionalStartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
 ):
     pass
 
+
 StartDBInstanceMessageRequestTypeDef = TypedDict(
     "StartDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 
@@ -2058,39 +2093,43 @@
     {
         "S3Prefix": str,
         "ExportOnly": Sequence[str],
     },
     total=False,
 )
 
+
 class StartExportTaskMessageRequestTypeDef(
     _RequiredStartExportTaskMessageRequestTypeDef, _OptionalStartExportTaskMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredStopActivityStreamRequestRequestTypeDef = TypedDict(
     "_RequiredStopActivityStreamRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalStopActivityStreamRequestRequestTypeDef = TypedDict(
     "_OptionalStopActivityStreamRequestRequestTypeDef",
     {
         "ApplyImmediately": bool,
     },
     total=False,
 )
 
+
 class StopActivityStreamRequestRequestTypeDef(
     _RequiredStopActivityStreamRequestRequestTypeDef,
     _OptionalStopActivityStreamRequestRequestTypeDef,
 ):
     pass
 
+
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -2111,39 +2150,43 @@
     "_OptionalStopDBInstanceMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
     total=False,
 )
 
+
 class StopDBInstanceMessageRequestTypeDef(
     _RequiredStopDBInstanceMessageRequestTypeDef, _OptionalStopDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
     },
 )
 _OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     {
         "SwitchoverTimeout": int,
     },
     total=False,
 )
 
+
 class SwitchoverBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 SwitchoverReadReplicaMessageRequestTypeDef = TypedDict(
     "SwitchoverReadReplicaMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 
@@ -2151,16 +2194,16 @@
     "AccountAttributesMessageTypeDef",
     {
         "AccountQuotas": List[AccountQuotaTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DBClusterBacktrackResponseTypeDef = TypedDict(
-    "DBClusterBacktrackResponseTypeDef",
+DBClusterBacktrackResponseMetadataTypeDef = TypedDict(
+    "DBClusterBacktrackResponseMetadataTypeDef",
     {
         "DBClusterIdentifier": str,
         "BacktrackIdentifier": str,
         "BacktrackTo": datetime,
         "BacktrackedFrom": datetime,
         "BacktrackRequestCreationTime": datetime,
         "Status": str,
@@ -2176,16 +2219,16 @@
         "CurrentCapacity": int,
         "SecondsBeforeTimeout": int,
         "TimeoutAction": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DBClusterEndpointResponseTypeDef = TypedDict(
-    "DBClusterEndpointResponseTypeDef",
+DBClusterEndpointResponseMetadataTypeDef = TypedDict(
+    "DBClusterEndpointResponseMetadataTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
         "DBClusterIdentifier": str,
         "DBClusterEndpointResourceIdentifier": str,
         "Endpoint": str,
         "Status": str,
         "EndpointType": str,
@@ -2226,16 +2269,16 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ExportTaskResponseTypeDef = TypedDict(
-    "ExportTaskResponseTypeDef",
+ExportTaskResponseMetadataTypeDef = TypedDict(
+    "ExportTaskResponseMetadataTypeDef",
     {
         "ExportTaskIdentifier": str,
         "SourceArn": str,
         "ExportOnly": List[str],
         "SnapshotTime": datetime,
         "TaskStartTime": datetime,
         "TaskEndTime": datetime,
@@ -2358,20 +2401,22 @@
     "_OptionalCopyDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCopyDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBClusterSnapshotMessageRequestTypeDef",
     {
         "SourceDBClusterSnapshotIdentifier": str,
         "TargetDBClusterSnapshotIdentifier": str,
     },
 )
@@ -2383,20 +2428,22 @@
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CopyDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCopyDBParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBParameterGroupMessageRequestTypeDef",
     {
         "SourceDBParameterGroupIdentifier": str,
         "TargetDBParameterGroupIdentifier": str,
         "TargetDBParameterGroupDescription": str,
     },
@@ -2405,20 +2452,22 @@
     "_OptionalCopyDBParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyDBParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCopyDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBSnapshotMessageRequestTypeDef",
     {
         "SourceDBSnapshotIdentifier": str,
         "TargetDBSnapshotIdentifier": str,
     },
 )
@@ -2433,19 +2482,21 @@
         "TargetCustomAvailabilityZone": str,
         "CopyOptionGroup": bool,
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CopyDBSnapshotMessageRequestTypeDef(
     _RequiredCopyDBSnapshotMessageRequestTypeDef, _OptionalCopyDBSnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCopyOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCopyOptionGroupMessageRequestTypeDef",
     {
         "SourceOptionGroupIdentifier": str,
         "TargetOptionGroupIdentifier": str,
         "TargetOptionGroupDescription": str,
     },
@@ -2454,19 +2505,21 @@
     "_OptionalCopyOptionGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyOptionGroupMessageRequestTypeDef(
     _RequiredCopyOptionGroupMessageRequestTypeDef, _OptionalCopyOptionGroupMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentName": str,
         "Source": str,
     },
 )
@@ -2477,20 +2530,22 @@
         "TargetDBParameterGroupName": str,
         "TargetDBClusterParameterGroupName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredCreateBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalCreateBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
@@ -2504,20 +2559,22 @@
         "Description": str,
         "Manifest": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCustomDBEngineVersionMessageRequestTypeDef(
     _RequiredCreateCustomDBEngineVersionMessageRequestTypeDef,
     _OptionalCreateCustomDBEngineVersionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "EndpointType": str,
     },
@@ -2528,20 +2585,22 @@
         "StaticMembers": Sequence[str],
         "ExcludedMembers": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBClusterEndpointMessageRequestTypeDef(
     _RequiredCreateDBClusterEndpointMessageRequestTypeDef,
     _OptionalCreateDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -2550,20 +2609,22 @@
     "_OptionalCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterIdentifier": str,
     },
 )
@@ -2571,20 +2632,22 @@
     "_OptionalCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBParameterGroupMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -2593,20 +2656,22 @@
     "_OptionalCreateDBParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBProxyEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDBProxyEndpointRequestRequestTypeDef",
     {
         "DBProxyName": str,
         "DBProxyEndpointName": str,
         "VpcSubnetIds": Sequence[str],
     },
@@ -2617,20 +2682,22 @@
         "VpcSecurityGroupIds": Sequence[str],
         "TargetRole": DBProxyEndpointTargetRoleType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBProxyEndpointRequestRequestTypeDef(
     _RequiredCreateDBProxyEndpointRequestRequestTypeDef,
     _OptionalCreateDBProxyEndpointRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSecurityGroupMessageRequestTypeDef",
     {
         "DBSecurityGroupName": str,
         "DBSecurityGroupDescription": str,
     },
 )
@@ -2638,20 +2705,22 @@
     "_OptionalCreateDBSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBSecurityGroupMessageRequestTypeDef(
     _RequiredCreateDBSecurityGroupMessageRequestTypeDef,
     _OptionalCreateDBSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSnapshotMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "DBInstanceIdentifier": str,
     },
 )
@@ -2659,19 +2728,21 @@
     "_OptionalCreateDBSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBSnapshotMessageRequestTypeDef(
     _RequiredCreateDBSnapshotMessageRequestTypeDef, _OptionalCreateDBSnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -2680,20 +2751,22 @@
     "_OptionalCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBSubnetGroupMessageRequestTypeDef(
     _RequiredCreateDBSubnetGroupMessageRequestTypeDef,
     _OptionalCreateDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "SnsTopicArn": str,
     },
 )
@@ -2705,20 +2778,22 @@
         "SourceIds": Sequence[str],
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateOptionGroupMessageRequestTypeDef",
     {
         "OptionGroupName": str,
         "EngineName": str,
         "MajorEngineVersion": str,
         "OptionGroupDescription": str,
@@ -2728,50 +2803,20 @@
     "_OptionalCreateOptionGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateOptionGroupMessageRequestTypeDef(
     _RequiredCreateOptionGroupMessageRequestTypeDef, _OptionalCreateOptionGroupMessageRequestTypeDef
 ):
     pass
 
-DBClusterSnapshotTypeDef = TypedDict(
-    "DBClusterSnapshotTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "DBClusterSnapshotIdentifier": str,
-        "DBClusterIdentifier": str,
-        "SnapshotCreateTime": datetime,
-        "Engine": str,
-        "EngineMode": str,
-        "AllocatedStorage": int,
-        "Status": str,
-        "Port": int,
-        "VpcId": str,
-        "ClusterCreateTime": datetime,
-        "MasterUsername": str,
-        "EngineVersion": str,
-        "LicenseModel": str,
-        "SnapshotType": str,
-        "PercentProgress": int,
-        "StorageEncrypted": bool,
-        "KmsKeyId": str,
-        "DBClusterSnapshotArn": str,
-        "SourceDBClusterSnapshotArn": str,
-        "IAMDatabaseAuthenticationEnabled": bool,
-        "TagList": List[TagTypeDef],
-        "DBSystemId": str,
-        "StorageType": str,
-        "DbClusterResourceId": str,
-    },
-    total=False,
-)
 
 _RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef",
     {
         "ReservedDBInstancesOfferingId": str,
     },
 )
@@ -2781,27 +2826,21 @@
         "ReservedDBInstanceId": str,
         "DBInstanceCount": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PurchaseReservedDBInstancesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
 ):
     pass
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
@@ -2834,55 +2873,69 @@
         "SupportedNetworkTypes": List[str],
         "SupportsStorageThroughput": bool,
         "MinStorageThroughputPerDbInstance": int,
         "MaxStorageThroughputPerDbInstance": int,
         "MinStorageThroughputPerIops": float,
         "MaxStorageThroughputPerIops": float,
     },
-    total=False,
-)
-
-_RequiredBacktrackDBClusterMessageRequestTypeDef = TypedDict(
-    "_RequiredBacktrackDBClusterMessageRequestTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "BacktrackTo": TimestampTypeDef,
-    },
-)
-_OptionalBacktrackDBClusterMessageRequestTypeDef = TypedDict(
-    "_OptionalBacktrackDBClusterMessageRequestTypeDef",
-    {
-        "Force": bool,
-        "UseEarliestTimeOnPointInTimeUnavailable": bool,
-    },
-    total=False,
 )
 
-class BacktrackDBClusterMessageRequestTypeDef(
-    _RequiredBacktrackDBClusterMessageRequestTypeDef,
-    _OptionalBacktrackDBClusterMessageRequestTypeDef,
-):
-    pass
-
 BlueGreenDeploymentTypeDef = TypedDict(
     "BlueGreenDeploymentTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "BlueGreenDeploymentName": str,
         "Source": str,
         "Target": str,
         "SwitchoverDetails": List[SwitchoverDetailTypeDef],
         "Tasks": List[BlueGreenDeploymentTaskTypeDef],
         "Status": str,
         "StatusDetails": str,
         "CreateTime": datetime,
         "DeleteTime": datetime,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
+    },
+)
+
+DBClusterSnapshotTypeDef = TypedDict(
+    "DBClusterSnapshotTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "DBClusterSnapshotIdentifier": str,
+        "DBClusterIdentifier": str,
+        "SnapshotCreateTime": datetime,
+        "Engine": str,
+        "EngineMode": str,
+        "AllocatedStorage": int,
+        "Status": str,
+        "Port": int,
+        "VpcId": str,
+        "ClusterCreateTime": datetime,
+        "MasterUsername": str,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "SnapshotType": str,
+        "PercentProgress": int,
+        "StorageEncrypted": bool,
+        "KmsKeyId": str,
+        "DBClusterSnapshotArn": str,
+        "SourceDBClusterSnapshotArn": str,
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "TagList": List[TagOutputTypeDef],
+        "DBSystemId": str,
+        "StorageType": str,
+    },
+)
+
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
@@ -2907,30 +2960,28 @@
         "IAMDatabaseAuthenticationEnabled": bool,
         "EngineVersion": str,
         "BackupRetentionPeriod": int,
         "AllocatedStorage": int,
         "Iops": int,
         "StorageType": str,
     },
-    total=False,
 )
 
 DBProxyTargetGroupTypeDef = TypedDict(
     "DBProxyTargetGroupTypeDef",
     {
         "DBProxyName": str,
         "TargetGroupName": str,
         "TargetGroupArn": str,
         "IsDefault": bool,
         "Status": str,
         "ConnectionPoolConfig": ConnectionPoolConfigurationInfoTypeDef,
         "CreatedDate": datetime,
         "UpdatedDate": datetime,
     },
-    total=False,
 )
 
 _RequiredModifyDBProxyTargetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyTargetGroupRequestRequestTypeDef",
     {
         "TargetGroupName": str,
         "DBProxyName": str,
@@ -2941,20 +2992,22 @@
     {
         "ConnectionPoolConfig": ConnectionPoolConfigurationTypeDef,
         "NewName": str,
     },
     total=False,
 )
 
+
 class ModifyDBProxyTargetGroupRequestRequestTypeDef(
     _RequiredModifyDBProxyTargetGroupRequestRequestTypeDef,
     _OptionalModifyDBProxyTargetGroupRequestRequestTypeDef,
 ):
     pass
 
+
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3054,25 +3107,26 @@
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
         "DBSystemId": str,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
-        "EnableLocalWriteForwarding": bool,
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CreateDBClusterMessageRequestTypeDef(
     _RequiredCreateDBClusterMessageRequestTypeDef, _OptionalCreateDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalModifyDBClusterMessageRequestTypeDef = TypedDict(
@@ -3114,24 +3168,25 @@
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
         "ManageMasterUserPassword": bool,
         "RotateMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "EngineMode": str,
         "AllowEngineModeChange": bool,
-        "EnableLocalWriteForwarding": bool,
     },
     total=False,
 )
 
+
 class ModifyDBClusterMessageRequestTypeDef(
     _RequiredModifyDBClusterMessageRequestTypeDef, _OptionalModifyDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredRestoreDBClusterFromS3MessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromS3MessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Engine": str,
         "MasterUsername": str,
         "SourceEngine": str,
@@ -3172,20 +3227,22 @@
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "StorageType": str,
     },
     total=False,
 )
 
+
 class RestoreDBClusterFromS3MessageRequestTypeDef(
     _RequiredRestoreDBClusterFromS3MessageRequestTypeDef,
     _OptionalRestoreDBClusterFromS3MessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "Engine": str,
     },
@@ -3218,32 +3275,34 @@
         "PubliclyAccessible": bool,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
     },
     total=False,
 )
 
+
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
+        "SourceDBClusterIdentifier": str,
     },
 )
 _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "RestoreType": str,
-        "SourceDBClusterIdentifier": str,
-        "RestoreToTime": TimestampTypeDef,
+        "RestoreToTime": Union[datetime, str],
         "UseLatestRestorableTime": bool,
         "Port": int,
         "DBSubnetGroupName": str,
         "OptionGroupName": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
@@ -3259,25 +3318,26 @@
         "EngineMode": str,
         "DBClusterInstanceClass": str,
         "StorageType": str,
         "PubliclyAccessible": bool,
         "Iops": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
-        "SourceDbClusterResourceId": str,
     },
     total=False,
 )
 
+
 class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
     },
@@ -3342,19 +3402,21 @@
         "MasterUserSecretKmsKeyId": str,
         "CACertificateIdentifier": str,
         "DBSystemId": str,
     },
     total=False,
 )
 
+
 class CreateDBInstanceMessageRequestTypeDef(
     _RequiredCreateDBInstanceMessageRequestTypeDef, _OptionalCreateDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalCreateDBInstanceReadReplicaMessageRequestTypeDef = TypedDict(
@@ -3402,60 +3464,21 @@
         "AllocatedStorage": int,
         "SourceDBClusterIdentifier": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CreateDBInstanceReadReplicaMessageRequestTypeDef(
     _RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef,
     _OptionalCreateDBInstanceReadReplicaMessageRequestTypeDef,
 ):
     pass
 
-DBSnapshotTypeDef = TypedDict(
-    "DBSnapshotTypeDef",
-    {
-        "DBSnapshotIdentifier": str,
-        "DBInstanceIdentifier": str,
-        "SnapshotCreateTime": datetime,
-        "Engine": str,
-        "AllocatedStorage": int,
-        "Status": str,
-        "Port": int,
-        "AvailabilityZone": str,
-        "VpcId": str,
-        "InstanceCreateTime": datetime,
-        "MasterUsername": str,
-        "EngineVersion": str,
-        "LicenseModel": str,
-        "SnapshotType": str,
-        "Iops": int,
-        "OptionGroupName": str,
-        "PercentProgress": int,
-        "SourceRegion": str,
-        "SourceDBSnapshotIdentifier": str,
-        "StorageType": str,
-        "TdeCredentialArn": str,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "DBSnapshotArn": str,
-        "Timezone": str,
-        "IAMDatabaseAuthenticationEnabled": bool,
-        "ProcessorFeatures": List[ProcessorFeatureTypeDef],
-        "DbiResourceId": str,
-        "TagList": List[TagTypeDef],
-        "OriginalSnapshotCreateTime": datetime,
-        "SnapshotDatabaseTime": datetime,
-        "SnapshotTarget": str,
-        "StorageThroughput": int,
-        "DBSystemId": str,
-    },
-    total=False,
-)
 
 _RequiredModifyDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
@@ -3519,45 +3542,20 @@
         "RotateMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "Engine": str,
     },
     total=False,
 )
 
+
 class ModifyDBInstanceMessageRequestTypeDef(
     _RequiredModifyDBInstanceMessageRequestTypeDef, _OptionalModifyDBInstanceMessageRequestTypeDef
 ):
     pass
 
-PendingModifiedValuesTypeDef = TypedDict(
-    "PendingModifiedValuesTypeDef",
-    {
-        "DBInstanceClass": str,
-        "AllocatedStorage": int,
-        "MasterUserPassword": str,
-        "Port": int,
-        "BackupRetentionPeriod": int,
-        "MultiAZ": bool,
-        "EngineVersion": str,
-        "LicenseModel": str,
-        "Iops": int,
-        "DBInstanceIdentifier": str,
-        "StorageType": str,
-        "CACertificateIdentifier": str,
-        "DBSubnetGroupName": str,
-        "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
-        "ProcessorFeatures": List[ProcessorFeatureTypeDef],
-        "IAMDatabaseAuthenticationEnabled": bool,
-        "AutomationMode": AutomationModeType,
-        "ResumeFullAutomationModeTime": datetime,
-        "StorageThroughput": int,
-        "Engine": str,
-    },
-    total=False,
-)
 
 _RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
@@ -3602,20 +3600,22 @@
         "StorageThroughput": int,
         "DBClusterSnapshotIdentifier": str,
         "AllocatedStorage": int,
     },
     total=False,
 )
 
+
 class RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreDBInstanceFromS3MessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceFromS3MessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
         "SourceEngine": str,
@@ -3668,31 +3668,33 @@
         "StorageThroughput": int,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
     },
     total=False,
 )
 
+
 class RestoreDBInstanceFromS3MessageRequestTypeDef(
     _RequiredRestoreDBInstanceFromS3MessageRequestTypeDef,
     _OptionalRestoreDBInstanceFromS3MessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
     },
 )
 _OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
     "_OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     {
         "SourceDBInstanceIdentifier": str,
-        "RestoreTime": TimestampTypeDef,
+        "RestoreTime": Union[datetime, str],
         "UseLatestRestorableTime": bool,
         "DBInstanceClass": str,
         "Port": int,
         "AvailabilityZone": str,
         "DBSubnetGroupName": str,
         "MultiAZ": bool,
         "PubliclyAccessible": bool,
@@ -3729,20 +3731,22 @@
         "NetworkType": str,
         "StorageThroughput": int,
         "AllocatedStorage": int,
     },
     total=False,
 )
 
+
 class RestoreDBInstanceToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
+
 CreateDBProxyEndpointResponseTypeDef = TypedDict(
     "CreateDBProxyEndpointResponseTypeDef",
     {
         "DBProxyEndpoint": DBProxyEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3790,19 +3794,21 @@
         "IdleClientTimeout": int,
         "DebugLogging": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBProxyRequestRequestTypeDef(
     _RequiredCreateDBProxyRequestRequestTypeDef, _OptionalCreateDBProxyRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyDBProxyRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalModifyDBProxyRequestRequestTypeDef = TypedDict(
@@ -3815,48 +3821,20 @@
         "DebugLogging": bool,
         "RoleArn": str,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBProxyRequestRequestTypeDef(
     _RequiredModifyDBProxyRequestRequestTypeDef, _OptionalModifyDBProxyRequestRequestTypeDef
 ):
     pass
 
-DBClusterAutomatedBackupTypeDef = TypedDict(
-    "DBClusterAutomatedBackupTypeDef",
-    {
-        "Engine": str,
-        "VpcId": str,
-        "DBClusterAutomatedBackupsArn": str,
-        "DBClusterIdentifier": str,
-        "RestoreWindow": RestoreWindowTypeDef,
-        "MasterUsername": str,
-        "DbClusterResourceId": str,
-        "Region": str,
-        "LicenseModel": str,
-        "Status": str,
-        "IAMDatabaseAuthenticationEnabled": bool,
-        "ClusterCreateTime": datetime,
-        "StorageEncrypted": bool,
-        "AllocatedStorage": int,
-        "EngineVersion": str,
-        "DBClusterArn": str,
-        "BackupRetentionPeriod": int,
-        "EngineMode": str,
-        "AvailabilityZones": List[str],
-        "Port": int,
-        "KmsKeyId": str,
-        "StorageType": str,
-        "Iops": int,
-    },
-    total=False,
-)
 
 DBClusterBacktrackMessageTypeDef = TypedDict(
     "DBClusterBacktrackMessageTypeDef",
     {
         "Marker": str,
         "DBClusterBacktracks": List[DBClusterBacktrackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3893,28 +3871,26 @@
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
         "Parameters": List[ParameterOutputTypeDef],
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
-DBEngineVersionResponseTypeDef = TypedDict(
-    "DBEngineVersionResponseTypeDef",
+DBEngineVersionResponseMetadataTypeDef = TypedDict(
+    "DBEngineVersionResponseMetadataTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "DBEngineDescription": str,
         "DBEngineVersionDescription": str,
         "DefaultCharacterSet": CharacterSetTypeDef,
@@ -3934,20 +3910,19 @@
         "SupportsGlobalDatabases": bool,
         "MajorEngineVersion": str,
         "DatabaseInstallationFilesS3BucketName": str,
         "DatabaseInstallationFilesS3Prefix": str,
         "DBEngineVersionArn": str,
         "KMSKeyId": str,
         "CreateTime": datetime,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "SupportsBabelfish": bool,
         "CustomDBEngineVersionManifest": str,
         "SupportsCertificateRotationWithoutRestart": bool,
         "SupportedCACertificateIdentifiers": List[str],
-        "SupportsLocalWriteForwarding": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
@@ -3973,22 +3948,20 @@
         "SupportsGlobalDatabases": bool,
         "MajorEngineVersion": str,
         "DatabaseInstallationFilesS3BucketName": str,
         "DatabaseInstallationFilesS3Prefix": str,
         "DBEngineVersionArn": str,
         "KMSKeyId": str,
         "CreateTime": datetime,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "SupportsBabelfish": bool,
         "CustomDBEngineVersionManifest": str,
         "SupportsCertificateRotationWithoutRestart": bool,
         "SupportedCACertificateIdentifiers": List[str],
-        "SupportsLocalWriteForwarding": bool,
     },
-    total=False,
 )
 
 DBInstanceAutomatedBackupTypeDef = TypedDict(
     "DBInstanceAutomatedBackupTypeDef",
     {
         "DBInstanceArn": str,
         "DbiResourceId": str,
@@ -4017,30 +3990,94 @@
         "DBInstanceAutomatedBackupsArn": str,
         "DBInstanceAutomatedBackupsReplications": List[
             DBInstanceAutomatedBackupsReplicationTypeDef
         ],
         "BackupTarget": str,
         "StorageThroughput": int,
     },
-    total=False,
+)
+
+DBSnapshotTypeDef = TypedDict(
+    "DBSnapshotTypeDef",
+    {
+        "DBSnapshotIdentifier": str,
+        "DBInstanceIdentifier": str,
+        "SnapshotCreateTime": datetime,
+        "Engine": str,
+        "AllocatedStorage": int,
+        "Status": str,
+        "Port": int,
+        "AvailabilityZone": str,
+        "VpcId": str,
+        "InstanceCreateTime": datetime,
+        "MasterUsername": str,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "SnapshotType": str,
+        "Iops": int,
+        "OptionGroupName": str,
+        "PercentProgress": int,
+        "SourceRegion": str,
+        "SourceDBSnapshotIdentifier": str,
+        "StorageType": str,
+        "TdeCredentialArn": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "DBSnapshotArn": str,
+        "Timezone": str,
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "ProcessorFeatures": List[ProcessorFeatureOutputTypeDef],
+        "DbiResourceId": str,
+        "TagList": List[TagOutputTypeDef],
+        "OriginalSnapshotCreateTime": datetime,
+        "SnapshotDatabaseTime": datetime,
+        "SnapshotTarget": str,
+        "StorageThroughput": int,
+        "DBSystemId": str,
+    },
+)
+
+PendingModifiedValuesTypeDef = TypedDict(
+    "PendingModifiedValuesTypeDef",
+    {
+        "DBInstanceClass": str,
+        "AllocatedStorage": int,
+        "MasterUserPassword": str,
+        "Port": int,
+        "BackupRetentionPeriod": int,
+        "MultiAZ": bool,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "Iops": int,
+        "DBInstanceIdentifier": str,
+        "StorageType": str,
+        "CACertificateIdentifier": str,
+        "DBSubnetGroupName": str,
+        "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
+        "ProcessorFeatures": List[ProcessorFeatureOutputTypeDef],
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "AutomationMode": AutomationModeType,
+        "ResumeFullAutomationModeTime": datetime,
+        "StorageThroughput": int,
+        "Engine": str,
+    },
 )
 
 DBProxyTargetTypeDef = TypedDict(
     "DBProxyTargetTypeDef",
     {
         "TargetArn": str,
         "Endpoint": str,
         "TrackedClusterId": str,
         "RdsResourceId": str,
         "Port": int,
         "Type": TargetTypeType,
         "Role": TargetRoleType,
         "TargetHealth": TargetHealthTypeDef,
     },
-    total=False,
 )
 
 DBProxyTypeDef = TypedDict(
     "DBProxyTypeDef",
     {
         "DBProxyName": str,
         "DBProxyArn": str,
@@ -4054,38 +4091,35 @@
         "Endpoint": str,
         "RequireTLS": bool,
         "IdleClientTimeout": int,
         "DebugLogging": bool,
         "CreatedDate": datetime,
         "UpdatedDate": datetime,
     },
-    total=False,
 )
 
 DBSecurityGroupTypeDef = TypedDict(
     "DBSecurityGroupTypeDef",
     {
         "OwnerId": str,
         "DBSecurityGroupName": str,
         "DBSecurityGroupDescription": str,
         "VpcId": str,
         "EC2SecurityGroups": List[EC2SecurityGroupTypeDef],
         "IPRanges": List[IPRangeTypeDef],
         "DBSecurityGroupArn": str,
     },
-    total=False,
 )
 
 DBSnapshotAttributesResultTypeDef = TypedDict(
     "DBSnapshotAttributesResultTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "DBSnapshotAttributes": List[DBSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
 DescribeBlueGreenDeploymentsRequestRequestTypeDef = TypedDict(
     "DescribeBlueGreenDeploymentsRequestRequestTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
@@ -4102,26 +4136,14 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBClusterAutomatedBackupsMessageRequestTypeDef = TypedDict(
-    "DescribeDBClusterAutomatedBackupsMessageRequestTypeDef",
-    {
-        "DbClusterResourceId": str,
-        "DBClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
 _RequiredDescribeDBClusterBacktracksMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterBacktracksMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalDescribeDBClusterBacktracksMessageRequestTypeDef = TypedDict(
@@ -4131,20 +4153,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDBClusterBacktracksMessageRequestTypeDef(
     _RequiredDescribeDBClusterBacktracksMessageRequestTypeDef,
     _OptionalDescribeDBClusterBacktracksMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeDBClusterEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
@@ -4177,32 +4201,33 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
-        "DbClusterResourceId": str,
     },
     total=False,
 )
 
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
@@ -4271,20 +4296,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDBLogFilesMessageRequestTypeDef(
     _RequiredDescribeDBLogFilesMessageRequestTypeDef,
     _OptionalDescribeDBLogFilesMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -4305,20 +4332,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDBParametersMessageRequestTypeDef(
     _RequiredDescribeDBParametersMessageRequestTypeDef,
     _OptionalDescribeDBParametersMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeDBProxiesRequestRequestTypeDef = TypedDict(
     "DescribeDBProxiesRequestRequestTypeDef",
     {
         "DBProxyName": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4351,20 +4380,22 @@
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeDBProxyTargetGroupsRequestRequestTypeDef(
     _RequiredDescribeDBProxyTargetGroupsRequestRequestTypeDef,
     _OptionalDescribeDBProxyTargetGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDBProxyTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDBProxyTargetsRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalDescribeDBProxyTargetsRequestRequestTypeDef = TypedDict(
@@ -4374,20 +4405,22 @@
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeDBProxyTargetsRequestRequestTypeDef(
     _RequiredDescribeDBProxyTargetsRequestRequestTypeDef,
     _OptionalDescribeDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeDBSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSecurityGroupsMessageRequestTypeDef",
     {
         "DBSecurityGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -4434,20 +4467,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -4456,20 +4491,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
@@ -4487,16 +4524,16 @@
 )
 
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
         "Duration": int,
         "EventCategories": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
@@ -4539,20 +4576,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeOptionGroupOptionsMessageRequestTypeDef(
     _RequiredDescribeOptionGroupOptionsMessageRequestTypeDef,
     _OptionalDescribeOptionGroupOptionsMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeOptionGroupsMessageRequestTypeDef = TypedDict(
     "DescribeOptionGroupsMessageRequestTypeDef",
     {
         "OptionGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4579,20 +4618,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
+
 DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4655,20 +4696,22 @@
     "_OptionalListTagsForResourceMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class ListTagsForResourceMessageRequestTypeDef(
     _RequiredListTagsForResourceMessageRequestTypeDef,
     _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeBlueGreenDeploymentsRequestDescribeBlueGreenDeploymentsPaginateTypeDef = TypedDict(
     "DescribeBlueGreenDeploymentsRequestDescribeBlueGreenDeploymentsPaginateTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4697,20 +4740,22 @@
         "BacktrackIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef(
     _RequiredDescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef,
     _OptionalDescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4740,30 +4785,31 @@
         "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
     _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "IncludeShared": bool,
         "IncludePublic": bool,
-        "DbClusterResourceId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
     "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
@@ -4828,20 +4874,22 @@
         "FileSize": int,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef(
     _RequiredDescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef,
     _OptionalDescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4860,20 +4908,22 @@
         "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
     _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef = TypedDict(
     "DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef",
     {
         "DBProxyName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4903,20 +4953,22 @@
         "TargetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef(
     _RequiredDescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef,
     _OptionalDescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef = TypedDict(
@@ -4925,20 +4977,22 @@
         "TargetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef(
     _RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef,
     _OptionalDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef = TypedDict(
     "DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef",
     {
         "DBSecurityGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4981,20 +5035,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
@@ -5002,20 +5058,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
+
 DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5023,16 +5081,16 @@
 )
 
 DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
         "Duration": int,
         "EventCategories": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -5071,20 +5129,22 @@
         "MajorEngineVersion": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef(
     _RequiredDescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef,
     _OptionalDescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef,
 ):
     pass
 
+
 DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef = TypedDict(
     "DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef",
     {
         "OptionGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "EngineName": str,
         "MajorEngineVersion": str,
@@ -5109,20 +5169,22 @@
         "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
 ):
     pass
 
+
 DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
     TypedDict(
         "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
         {
             "ResourceIdentifier": str,
             "Filters": Sequence[FilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
@@ -5184,32 +5246,33 @@
     "_OptionalDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef(
     _RequiredDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef,
     _OptionalDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
-        "DbClusterResourceId": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef",
@@ -5218,15 +5281,14 @@
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
-        "DbClusterResourceId": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClustersMessageDBClusterAvailableWaitTypeDef = TypedDict(
     "DescribeDBClustersMessageDBClusterAvailableWaitTypeDef",
@@ -5375,32 +5437,92 @@
         "EngineVersion": str,
         "DatabaseName": str,
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
         "FailoverState": FailoverStateTypeDef,
     },
-    total=False,
 )
 
 OptionGroupOptionSettingTypeDef = TypedDict(
     "OptionGroupOptionSettingTypeDef",
     {
         "SettingName": str,
         "SettingDescription": str,
         "DefaultValue": str,
         "ApplyType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "IsRequired": bool,
         "MinimumEngineVersionPerAllowedValue": List[MinimumEngineVersionPerAllowedValueTypeDef],
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
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
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
+    total=False,
+)
+
+
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
+_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+    },
+)
+_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
     total=False,
 )
 
+
+class ResetDBParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
 _RequiredOptionConfigurationTypeDef = TypedDict(
     "_RequiredOptionConfigurationTypeDef",
     {
         "OptionName": str,
     },
 )
 _OptionalOptionConfigurationTypeDef = TypedDict(
@@ -5411,68 +5533,65 @@
         "DBSecurityGroupMemberships": Sequence[str],
         "VpcSecurityGroupMemberships": Sequence[str],
         "OptionSettings": Sequence[OptionSettingTypeDef],
     },
     total=False,
 )
 
+
 class OptionConfigurationTypeDef(
     _RequiredOptionConfigurationTypeDef, _OptionalOptionConfigurationTypeDef
 ):
     pass
 
+
 OptionTypeDef = TypedDict(
     "OptionTypeDef",
     {
         "OptionName": str,
         "OptionDescription": str,
         "Persistent": bool,
         "Permanent": bool,
         "Port": int,
         "OptionVersion": str,
-        "OptionSettings": List[OptionSettingTypeDef],
+        "OptionSettings": List[OptionSettingOutputTypeDef],
         "DBSecurityGroupMemberships": List[DBSecurityGroupMembershipTypeDef],
         "VpcSecurityGroupMemberships": List[VpcSecurityGroupMembershipTypeDef],
     },
-    total=False,
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetOutpost": OutpostTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
-ParameterUnionTypeDef = Union[ParameterTypeDef, ParameterOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
 )
 
 ValidStorageOptionsTypeDef = TypedDict(
     "ValidStorageOptionsTypeDef",
     {
         "StorageType": str,
         "StorageSize": List[RangeTypeDef],
         "ProvisionedIops": List[RangeTypeDef],
         "IopsToStorageRatio": List[DoubleRangeTypeDef],
         "SupportsStorageAutoscaling": bool,
         "ProvisionedStorageThroughput": List[RangeTypeDef],
         "StorageThroughputToIopsRatio": List[DoubleRangeTypeDef],
     },
-    total=False,
 )
 
 ReservedDBInstanceTypeDef = TypedDict(
     "ReservedDBInstanceTypeDef",
     {
         "ReservedDBInstanceId": str,
         "ReservedDBInstancesOfferingId": str,
@@ -5487,15 +5606,14 @@
         "OfferingType": str,
         "MultiAZ": bool,
         "State": str,
         "RecurringCharges": List[RecurringChargeTypeDef],
         "ReservedDBInstanceArn": str,
         "LeaseId": str,
     },
-    total=False,
 )
 
 ReservedDBInstancesOfferingTypeDef = TypedDict(
     "ReservedDBInstancesOfferingTypeDef",
     {
         "ReservedDBInstancesOfferingId": str,
         "DBInstanceClass": str,
@@ -5504,97 +5622,96 @@
         "UsagePrice": float,
         "CurrencyCode": str,
         "ProductDescription": str,
         "OfferingType": str,
         "MultiAZ": bool,
         "RecurringCharges": List[RecurringChargeTypeDef],
     },
-    total=False,
 )
 
 SourceRegionMessageTypeDef = TypedDict(
     "SourceRegionMessageTypeDef",
     {
         "Marker": str,
         "SourceRegions": List[SourceRegionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CopyDBClusterSnapshotResultTypeDef = TypedDict(
-    "CopyDBClusterSnapshotResultTypeDef",
+OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
+    "OrderableDBInstanceOptionsMessageTypeDef",
     {
-        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
+        "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
+        "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateDBClusterSnapshotResultTypeDef = TypedDict(
-    "CreateDBClusterSnapshotResultTypeDef",
+CreateBlueGreenDeploymentResponseTypeDef = TypedDict(
+    "CreateBlueGreenDeploymentResponseTypeDef",
     {
-        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
+        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DBClusterSnapshotMessageTypeDef = TypedDict(
-    "DBClusterSnapshotMessageTypeDef",
+DeleteBlueGreenDeploymentResponseTypeDef = TypedDict(
+    "DeleteBlueGreenDeploymentResponseTypeDef",
     {
-        "Marker": str,
-        "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
+        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteDBClusterSnapshotResultTypeDef = TypedDict(
-    "DeleteDBClusterSnapshotResultTypeDef",
+DescribeBlueGreenDeploymentsResponseTypeDef = TypedDict(
+    "DescribeBlueGreenDeploymentsResponseTypeDef",
     {
-        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
+        "BlueGreenDeployments": List[BlueGreenDeploymentTypeDef],
+        "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
-    "OrderableDBInstanceOptionsMessageTypeDef",
+SwitchoverBlueGreenDeploymentResponseTypeDef = TypedDict(
+    "SwitchoverBlueGreenDeploymentResponseTypeDef",
     {
-        "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
-        "Marker": str,
+        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateBlueGreenDeploymentResponseTypeDef = TypedDict(
-    "CreateBlueGreenDeploymentResponseTypeDef",
+CopyDBClusterSnapshotResultTypeDef = TypedDict(
+    "CopyDBClusterSnapshotResultTypeDef",
     {
-        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
+        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteBlueGreenDeploymentResponseTypeDef = TypedDict(
-    "DeleteBlueGreenDeploymentResponseTypeDef",
+CreateDBClusterSnapshotResultTypeDef = TypedDict(
+    "CreateDBClusterSnapshotResultTypeDef",
     {
-        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
+        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeBlueGreenDeploymentsResponseTypeDef = TypedDict(
-    "DescribeBlueGreenDeploymentsResponseTypeDef",
+DBClusterSnapshotMessageTypeDef = TypedDict(
+    "DBClusterSnapshotMessageTypeDef",
     {
-        "BlueGreenDeployments": List[BlueGreenDeploymentTypeDef],
         "Marker": str,
+        "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SwitchoverBlueGreenDeploymentResponseTypeDef = TypedDict(
-    "SwitchoverBlueGreenDeploymentResponseTypeDef",
+DeleteDBClusterSnapshotResultTypeDef = TypedDict(
+    "DeleteDBClusterSnapshotResultTypeDef",
     {
-        "BlueGreenDeployment": BlueGreenDeploymentTypeDef,
+        "DBClusterSnapshot": DBClusterSnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterTypeDef = TypedDict(
     "DBClusterTypeDef",
     {
@@ -5647,15 +5764,15 @@
         "ActivityStreamMode": ActivityStreamModeType,
         "ActivityStreamStatus": ActivityStreamStatusType,
         "ActivityStreamKmsKeyId": str,
         "ActivityStreamKinesisStreamName": str,
         "CopyTagsToSnapshot": bool,
         "CrossAccountClone": bool,
         "DomainMemberships": List[DomainMembershipTypeDef],
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "GlobalWriteForwardingStatus": WriteForwardingStatusType,
         "GlobalWriteForwardingRequested": bool,
         "PendingModifiedValues": ClusterPendingModifiedValuesTypeDef,
         "DBClusterInstanceClass": str,
         "StorageType": str,
         "Iops": int,
         "PubliclyAccessible": bool,
@@ -5666,17 +5783,15 @@
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationInfoTypeDef,
         "NetworkType": str,
         "DBSystemId": str,
         "MasterUserSecret": MasterUserSecretTypeDef,
         "IOOptimizedNextAllowedModificationTime": datetime,
-        "LocalWriteForwardingStatus": LocalWriteForwardingStatusType,
     },
-    total=False,
 )
 
 DescribeDBProxyTargetGroupsResponseTypeDef = TypedDict(
     "DescribeDBProxyTargetGroupsResponseTypeDef",
     {
         "TargetGroups": List[DBProxyTargetGroupTypeDef],
         "Marker": str,
@@ -5688,72 +5803,14 @@
     "ModifyDBProxyTargetGroupResponseTypeDef",
     {
         "DBProxyTargetGroup": DBProxyTargetGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CopyDBSnapshotResultTypeDef = TypedDict(
-    "CopyDBSnapshotResultTypeDef",
-    {
-        "DBSnapshot": DBSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDBSnapshotResultTypeDef = TypedDict(
-    "CreateDBSnapshotResultTypeDef",
-    {
-        "DBSnapshot": DBSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DBSnapshotMessageTypeDef = TypedDict(
-    "DBSnapshotMessageTypeDef",
-    {
-        "Marker": str,
-        "DBSnapshots": List[DBSnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDBSnapshotResultTypeDef = TypedDict(
-    "DeleteDBSnapshotResultTypeDef",
-    {
-        "DBSnapshot": DBSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyDBSnapshotResultTypeDef = TypedDict(
-    "ModifyDBSnapshotResultTypeDef",
-    {
-        "DBSnapshot": DBSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DBClusterAutomatedBackupMessageTypeDef = TypedDict(
-    "DBClusterAutomatedBackupMessageTypeDef",
-    {
-        "Marker": str,
-        "DBClusterAutomatedBackups": List[DBClusterAutomatedBackupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDBClusterAutomatedBackupResultTypeDef = TypedDict(
-    "DeleteDBClusterAutomatedBackupResultTypeDef",
-    {
-        "DBClusterAutomatedBackup": DBClusterAutomatedBackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5820,14 +5877,55 @@
     "StopDBInstanceAutomatedBackupsReplicationResultTypeDef",
     {
         "DBInstanceAutomatedBackup": DBInstanceAutomatedBackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CopyDBSnapshotResultTypeDef = TypedDict(
+    "CopyDBSnapshotResultTypeDef",
+    {
+        "DBSnapshot": DBSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDBSnapshotResultTypeDef = TypedDict(
+    "CreateDBSnapshotResultTypeDef",
+    {
+        "DBSnapshot": DBSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBSnapshotMessageTypeDef = TypedDict(
+    "DBSnapshotMessageTypeDef",
+    {
+        "Marker": str,
+        "DBSnapshots": List[DBSnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDBSnapshotResultTypeDef = TypedDict(
+    "DeleteDBSnapshotResultTypeDef",
+    {
+        "DBSnapshot": DBSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyDBSnapshotResultTypeDef = TypedDict(
+    "ModifyDBSnapshotResultTypeDef",
+    {
+        "DBSnapshot": DBSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeDBProxyTargetsResponseTypeDef = TypedDict(
     "DescribeDBProxyTargetsResponseTypeDef",
     {
         "Targets": List[DBProxyTargetTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5989,15 +6087,14 @@
         "RequiresAutoMinorEngineVersionUpgrade": bool,
         "VpcOnly": bool,
         "SupportsOptionVersionDowngrade": bool,
         "OptionGroupOptionSettings": List[OptionGroupOptionSettingTypeDef],
         "OptionGroupOptionVersions": List[OptionVersionTypeDef],
         "CopyableCrossAccount": bool,
     },
-    total=False,
 )
 
 _RequiredModifyOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyOptionGroupMessageRequestTypeDef",
     {
         "OptionGroupName": str,
     },
@@ -6008,19 +6105,21 @@
         "OptionsToInclude": Sequence[OptionConfigurationTypeDef],
         "OptionsToRemove": Sequence[str],
         "ApplyImmediately": bool,
     },
     total=False,
 )
 
+
 class ModifyOptionGroupMessageRequestTypeDef(
     _RequiredModifyOptionGroupMessageRequestTypeDef, _OptionalModifyOptionGroupMessageRequestTypeDef
 ):
     pass
 
+
 OptionGroupTypeDef = TypedDict(
     "OptionGroupTypeDef",
     {
         "OptionGroupName": str,
         "OptionGroupDescription": str,
         "EngineName": str,
         "MajorEngineVersion": str,
@@ -6028,89 +6127,29 @@
         "AllowsVpcAndNonVpcInstanceMemberships": bool,
         "VpcId": str,
         "OptionGroupArn": str,
         "SourceOptionGroup": str,
         "SourceAccountId": str,
         "CopyTimestamp": datetime,
     },
-    total=False,
 )
 
 DBSubnetGroupTypeDef = TypedDict(
     "DBSubnetGroupTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
         "SupportedNetworkTypes": List[str],
     },
-    total=False,
 )
 
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-)
-
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterUnionTypeDef],
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
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-    total=False,
-)
-
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-    },
-)
-_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-    total=False,
-)
-
-class ResetDBParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBParameterGroupMessageRequestTypeDef,
-):
-    pass
-
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6126,15 +6165,14 @@
 
 ValidDBInstanceModificationsMessageTypeDef = TypedDict(
     "ValidDBInstanceModificationsMessageTypeDef",
     {
         "Storage": List[ValidStorageOptionsTypeDef],
         "ValidProcessorFeatures": List[AvailableProcessorFeatureTypeDef],
     },
-    total=False,
 )
 
 PurchaseReservedDBInstancesOfferingResultTypeDef = TypedDict(
     "PurchaseReservedDBInstancesOfferingResultTypeDef",
     {
         "ReservedDBInstance": ReservedDBInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6361,20 +6399,20 @@
         "DBInstanceArn": str,
         "Timezone": str,
         "IAMDatabaseAuthenticationEnabled": bool,
         "PerformanceInsightsEnabled": bool,
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "EnabledCloudwatchLogsExports": List[str],
-        "ProcessorFeatures": List[ProcessorFeatureTypeDef],
+        "ProcessorFeatures": List[ProcessorFeatureOutputTypeDef],
         "DeletionProtection": bool,
         "AssociatedRoles": List[DBInstanceRoleTypeDef],
         "ListenerEndpoint": EndpointTypeDef,
         "MaxAllocatedStorage": int,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "DBInstanceAutomatedBackupsReplications": List[
             DBInstanceAutomatedBackupsReplicationTypeDef
         ],
         "CustomerOwnedIpEnabled": bool,
         "AwsBackupRecoveryPointArn": str,
         "ActivityStreamStatus": ActivityStreamStatusType,
         "ActivityStreamKmsKeyId": str,
@@ -6388,17 +6426,15 @@
         "NetworkType": str,
         "ActivityStreamPolicyStatus": ActivityStreamPolicyStatusType,
         "StorageThroughput": int,
         "DBSystemId": str,
         "MasterUserSecret": MasterUserSecretTypeDef,
         "CertificateDetails": CertificateDetailsTypeDef,
         "ReadReplicaSourceDBClusterIdentifier": str,
-        "PercentProgress": str,
     },
-    total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/waiter.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotAvailable.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/waiters/#dbclustersnapshotavailablewaiter)
         """
 
@@ -137,15 +136,14 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotDeleted.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/waiters/#dbclustersnapshotdeletedwaiter)
         """
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds/waiter.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotAvailable.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/waiters/#dbclustersnapshotavailablewaiter)
         """
 
@@ -133,15 +132,14 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotDeleted.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/waiters/#dbclustersnapshotdeletedwaiter)
         """
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds.egg-info/PKG-INFO` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.28.17
-Summary: Type annotations for boto3.RDS 1.28.17 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.9
+Summary: Type annotations for boto3.RDS 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rds type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 rds type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rds"></a>
 
 # mypy-boto3-rds
 
 [![PyPI - mypy-boto3-rds](https://img.shields.io/pypi/v/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rds?color=blue)](https://pypistats.org/packages/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
 [mypy-boto3-rds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/).
 
 See how it helps to find and fix potential bugs:
 
@@ -76,15 +76,15 @@
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
@@ -562,15 +562,14 @@
     DescribeReservedDBInstancesPaginatorName,
     DescribeSourceRegionsPaginatorName,
     DownloadDBLogFilePortionPaginatorName,
     EngineFamilyType,
     ExportSourceTypeType,
     FailoverStatusType,
     IAMAuthModeType,
-    LocalWriteForwardingStatusType,
     ReplicaModeType,
     SourceTypeType,
     TargetHealthReasonType,
     TargetRoleType,
     TargetStateType,
     TargetTypeType,
     WriteForwardingStatusType,
@@ -583,37 +582,38 @@
 )
 
 
 def check_value(value: ActivityStreamModeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_rds.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rds.type_defs import (
     AccountQuotaTypeDef,
     ResponseMetadataTypeDef,
     AddRoleToDBClusterMessageRequestTypeDef,
     AddRoleToDBInstanceMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     AvailableProcessorFeatureTypeDef,
-    TimestampTypeDef,
+    BacktrackDBClusterMessageRequestTypeDef,
     BlueGreenDeploymentTaskTypeDef,
     SwitchoverDetailTypeDef,
+    TagOutputTypeDef,
     CancelExportTaskMessageRequestTypeDef,
     CertificateDetailsTypeDef,
     CertificateTypeDef,
     CharacterSetTypeDef,
     ClientGenerateDbAuthTokenRequestTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
@@ -624,15 +624,14 @@
     ScalingConfigurationTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     ProcessorFeatureTypeDef,
     DBProxyEndpointTypeDef,
     UserAuthConfigTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     CustomDBEngineVersionAMITypeDef,
-    RestoreWindowTypeDef,
     DBClusterBacktrackTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
     ParameterOutputTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
@@ -640,28 +639,29 @@
     MasterUserSecretTypeDef,
     ScalingConfigurationInfoTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceAutomatedBackupsReplicationTypeDef,
+    RestoreWindowTypeDef,
     DBInstanceRoleTypeDef,
     DBInstanceStatusInfoTypeDef,
     DBParameterGroupStatusTypeDef,
     DBSecurityGroupMembershipTypeDef,
     EndpointTypeDef,
     OptionGroupMembershipTypeDef,
+    ProcessorFeatureOutputTypeDef,
     TargetHealthTypeDef,
     UserAuthConfigInfoTypeDef,
     EC2SecurityGroupTypeDef,
     IPRangeTypeDef,
     DBSnapshotAttributeTypeDef,
     DeleteBlueGreenDeploymentRequestRequestTypeDef,
     DeleteCustomDBEngineVersionMessageRequestTypeDef,
-    DeleteDBClusterAutomatedBackupMessageRequestTypeDef,
     DeleteDBClusterEndpointMessageRequestTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceAutomatedBackupMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBParameterGroupMessageRequestTypeDef,
@@ -692,25 +692,26 @@
     GlobalClusterMemberTypeDef,
     MinimumEngineVersionPerAllowedValueTypeDef,
     ModifyActivityStreamRequestRequestTypeDef,
     ModifyCertificatesMessageRequestTypeDef,
     ModifyCurrentDBClusterCapacityMessageRequestTypeDef,
     ModifyCustomDBEngineVersionMessageRequestTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBProxyEndpointRequestRequestTypeDef,
     ModifyDBSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSnapshotMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     OptionSettingTypeDef,
     OptionVersionTypeDef,
+    OptionSettingOutputTypeDef,
     OutpostTypeDef,
-    ParameterTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
     PromoteReadReplicaMessageRequestTypeDef,
     RangeTypeDef,
     RebootDBClusterMessageRequestTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RecurringChargeTypeDef,
@@ -730,22 +731,22 @@
     StopActivityStreamRequestRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     StopDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
     StopDBInstanceMessageRequestTypeDef,
     SwitchoverBlueGreenDeploymentRequestRequestTypeDef,
     SwitchoverReadReplicaMessageRequestTypeDef,
     AccountAttributesMessageTypeDef,
-    DBClusterBacktrackResponseTypeDef,
+    DBClusterBacktrackResponseMetadataTypeDef,
     DBClusterCapacityInfoTypeDef,
-    DBClusterEndpointResponseTypeDef,
+    DBClusterEndpointResponseMetadataTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DBParameterGroupNameMessageTypeDef,
     DownloadDBLogFilePortionDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
-    ExportTaskResponseTypeDef,
+    ExportTaskResponseMetadataTypeDef,
     ModifyActivityStreamResponseTypeDef,
     StartActivityStreamResponseTypeDef,
     StopActivityStreamResponseTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EventSubscriptionsMessageTypeDef,
@@ -765,20 +766,19 @@
     CreateDBParameterGroupMessageRequestTypeDef,
     CreateDBProxyEndpointRequestRequestTypeDef,
     CreateDBSecurityGroupMessageRequestTypeDef,
     CreateDBSnapshotMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateOptionGroupMessageRequestTypeDef,
-    DBClusterSnapshotTypeDef,
     PurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
-    BacktrackDBClusterMessageRequestTypeDef,
     BlueGreenDeploymentTypeDef,
+    DBClusterSnapshotTypeDef,
+    TagListMessageTypeDef,
     CertificateMessageTypeDef,
     ModifyCertificatesResultTypeDef,
     ClusterPendingModifiedValuesTypeDef,
     DBProxyTargetGroupTypeDef,
     ModifyDBProxyTargetGroupRequestRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -789,43 +789,41 @@
     CreateDBClusterMessageRequestTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromS3MessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBInstanceReadReplicaMessageRequestTypeDef,
-    DBSnapshotTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
-    PendingModifiedValuesTypeDef,
     RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
     RestoreDBInstanceFromS3MessageRequestTypeDef,
     RestoreDBInstanceToPointInTimeMessageRequestTypeDef,
     CreateDBProxyEndpointResponseTypeDef,
     DeleteDBProxyEndpointResponseTypeDef,
     DescribeDBProxyEndpointsResponseTypeDef,
     ModifyDBProxyEndpointResponseTypeDef,
     CreateDBProxyRequestRequestTypeDef,
     ModifyDBProxyRequestRequestTypeDef,
-    DBClusterAutomatedBackupTypeDef,
     DBClusterBacktrackMessageTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
-    DBEngineVersionResponseTypeDef,
+    DBEngineVersionResponseMetadataTypeDef,
     DBEngineVersionTypeDef,
     DBInstanceAutomatedBackupTypeDef,
+    DBSnapshotTypeDef,
+    PendingModifiedValuesTypeDef,
     DBProxyTargetTypeDef,
     DBProxyTypeDef,
     DBSecurityGroupTypeDef,
     DBSnapshotAttributesResultTypeDef,
     DescribeBlueGreenDeploymentsRequestRequestTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
-    DescribeDBClusterAutomatedBackupsMessageRequestTypeDef,
     DescribeDBClusterBacktracksMessageRequestTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
@@ -902,51 +900,52 @@
     DescribeDBSnapshotsMessageDBSnapshotDeletedWaitTypeDef,
     DescribeDBLogFilesResponseTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     ExportTasksMessageTypeDef,
     GlobalClusterTypeDef,
     OptionGroupOptionSettingTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ModifyDBParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBParameterGroupMessageRequestTypeDef,
     OptionConfigurationTypeDef,
     OptionTypeDef,
     SubnetTypeDef,
-    ParameterUnionTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
     ReservedDBInstanceTypeDef,
     ReservedDBInstancesOfferingTypeDef,
     SourceRegionMessageTypeDef,
-    CopyDBClusterSnapshotResultTypeDef,
-    CreateDBClusterSnapshotResultTypeDef,
-    DBClusterSnapshotMessageTypeDef,
-    DeleteDBClusterSnapshotResultTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     CreateBlueGreenDeploymentResponseTypeDef,
     DeleteBlueGreenDeploymentResponseTypeDef,
     DescribeBlueGreenDeploymentsResponseTypeDef,
     SwitchoverBlueGreenDeploymentResponseTypeDef,
+    CopyDBClusterSnapshotResultTypeDef,
+    CreateDBClusterSnapshotResultTypeDef,
+    DBClusterSnapshotMessageTypeDef,
+    DeleteDBClusterSnapshotResultTypeDef,
     DBClusterTypeDef,
     DescribeDBProxyTargetGroupsResponseTypeDef,
     ModifyDBProxyTargetGroupResponseTypeDef,
-    CopyDBSnapshotResultTypeDef,
-    CreateDBSnapshotResultTypeDef,
-    DBSnapshotMessageTypeDef,
-    DeleteDBSnapshotResultTypeDef,
-    ModifyDBSnapshotResultTypeDef,
-    DBClusterAutomatedBackupMessageTypeDef,
-    DeleteDBClusterAutomatedBackupResultTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
     DBEngineVersionMessageTypeDef,
     DBInstanceAutomatedBackupMessageTypeDef,
     DeleteDBInstanceAutomatedBackupResultTypeDef,
     StartDBInstanceAutomatedBackupsReplicationResultTypeDef,
     StopDBInstanceAutomatedBackupsReplicationResultTypeDef,
+    CopyDBSnapshotResultTypeDef,
+    CreateDBSnapshotResultTypeDef,
+    DBSnapshotMessageTypeDef,
+    DeleteDBSnapshotResultTypeDef,
+    ModifyDBSnapshotResultTypeDef,
     DescribeDBProxyTargetsResponseTypeDef,
     RegisterDBProxyTargetsResponseTypeDef,
     CreateDBProxyResponseTypeDef,
     DeleteDBProxyResponseTypeDef,
     DescribeDBProxiesResponseTypeDef,
     ModifyDBProxyResponseTypeDef,
     AuthorizeDBSecurityGroupIngressResultTypeDef,
@@ -961,18 +960,14 @@
     GlobalClustersMessageTypeDef,
     ModifyGlobalClusterResultTypeDef,
     RemoveFromGlobalClusterResultTypeDef,
     OptionGroupOptionTypeDef,
     ModifyOptionGroupMessageRequestTypeDef,
     OptionGroupTypeDef,
     DBSubnetGroupTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ModifyDBParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBParameterGroupMessageRequestTypeDef,
     ApplyPendingMaintenanceActionResultTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ValidDBInstanceModificationsMessageTypeDef,
     PurchaseReservedDBInstancesOfferingResultTypeDef,
     ReservedDBInstanceMessageTypeDef,
     ReservedDBInstancesOfferingMessageTypeDef,
     CreateDBClusterResultTypeDef,
@@ -1009,15 +1004,15 @@
     RestoreDBInstanceToPointInTimeResultTypeDef,
     StartDBInstanceResultTypeDef,
     StopDBInstanceResultTypeDef,
     SwitchoverReadReplicaResultTypeDef,
 )
 
 
-def get_value() -> AccountQuotaTypeDef:
+def get_structure() -> AccountQuotaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rds-1.28.17/mypy_boto3_rds.egg-info/SOURCES.txt` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.17/setup.py` & `mypy-boto3-rds-1.28.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rds",
-    version="1.28.17",
+    version="1.28.9",
     packages=["mypy_boto3_rds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RDS 1.28.17 service generated with mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.RDS 1.28.9 service generated with mypy-boto3-builder 7.15.1"
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
-    keywords="boto3 rds type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 rds type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_rds": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

