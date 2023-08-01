# Comparing `tmp/mypy-boto3-rds-1.28.16.post1.tar.gz` & `tmp/mypy-boto3-rds-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rds-1.28.16.post1.tar", last modified: Tue Aug  1 11:37:37 2023, max compression
+gzip compressed data, was "mypy-boto3-rds-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-rds-1.28.16.post1.tar` & `mypy-boto3-rds-1.28.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:37.780777 mypy-boto3-rds-1.28.16.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:29:43.000000 mypy-boto3-rds-1.28.16.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41404 2023-08-01 11:37:37.772777 mypy-boto3-rds-1.28.16.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39930 2023-08-01 11:29:43.000000 mypy-boto3-rds-1.28.16.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:37.760777 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-08-01 11:29:43.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-08-01 11:29:43.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:29:43.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144250 2023-08-01 11:29:45.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   144057 2023-08-01 11:29:44.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-08-01 11:29:46.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-08-01 11:29:45.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    45225 2023-08-01 11:29:45.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    45188 2023-08-01 11:29:45.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:29:43.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   192136 2023-08-01 11:29:54.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   191959 2023-08-01 11:29:48.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 11:29:43.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-08-01 11:29:45.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-08-01 11:29:45.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:37.772777 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41404 2023-08-01 11:37:37.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:37:37.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:37.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:37.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:37.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:37.000000 mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:37.780777 mypy-boto3-rds-1.28.16.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-01 11:29:43.000000 mypy-boto3-rds-1.28.16.post1/setup.py
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

### Comparing `mypy-boto3-rds-1.28.16.post1/LICENSE` & `mypy-boto3-rds-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.16.post1/PKG-INFO` & `mypy-boto3-rds-1.28.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.28.16.post1
-Summary: Type annotations for boto3.RDS 1.28.16 service generated with mypy-boto3-builder 7.17.1
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
-[boto3.RDS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
@@ -646,14 +646,15 @@
     RestoreWindowTypeDef,
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
@@ -691,25 +692,26 @@
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
@@ -729,22 +731,22 @@
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
@@ -764,20 +766,19 @@
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
@@ -788,17 +789,15 @@
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
@@ -806,17 +805,19 @@
     ModifyDBProxyRequestRequestTypeDef,
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
     DescribeDBClusterBacktracksMessageRequestTypeDef,
@@ -899,49 +900,52 @@
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
@@ -956,18 +960,14 @@
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
@@ -1004,15 +1004,15 @@
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

### Comparing `mypy-boto3-rds-1.28.16.post1/README.md` & `mypy-boto3-rds-1.28.9/README.md`

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
-[boto3.RDS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
@@ -614,14 +614,15 @@
     RestoreWindowTypeDef,
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
@@ -659,25 +660,26 @@
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
@@ -697,22 +699,22 @@
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
@@ -732,20 +734,19 @@
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
@@ -756,17 +757,15 @@
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
@@ -774,17 +773,19 @@
     ModifyDBProxyRequestRequestTypeDef,
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
     DescribeDBClusterBacktracksMessageRequestTypeDef,
@@ -867,49 +868,52 @@
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
@@ -924,18 +928,14 @@
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
@@ -972,15 +972,15 @@
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

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/__init__.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/__init__.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/__main__.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RDS 1.28.16\nVersion:         1.28.16.post1\nBuilder version:"
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
-    print("1.28.16.post1")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/client.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/client.py`

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
@@ -91,25 +92,25 @@
     CreateDBSecurityGroupResultTypeDef,
     CreateDBSnapshotResultTypeDef,
     CreateDBSubnetGroupResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateGlobalClusterResultTypeDef,
     CreateOptionGroupResultTypeDef,
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
@@ -136,15 +137,15 @@
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
@@ -160,15 +161,15 @@
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
@@ -195,15 +196,14 @@
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
@@ -446,18 +446,18 @@
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
 
@@ -465,15 +465,15 @@
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
@@ -595,15 +595,15 @@
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
 
@@ -655,15 +655,14 @@
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
@@ -674,15 +673,15 @@
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
@@ -999,15 +998,15 @@
 
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
 
@@ -1023,15 +1022,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_db_cluster)
         """
 
     def delete_db_cluster_endpoint(
         self, *, DBClusterEndpointIdentifier: str
-    ) -> DBClusterEndpointResponseTypeDef:
+    ) -> DBClusterEndpointResponseMetadataTypeDef:
         """
         Deletes a custom endpoint and removes it from an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_db_cluster_endpoint)
         """
 
@@ -1611,16 +1610,16 @@
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
@@ -1915,15 +1914,15 @@
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
 
@@ -1966,16 +1965,15 @@
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
@@ -1983,24 +1981,24 @@
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
@@ -2087,15 +2085,15 @@
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
@@ -2210,15 +2208,15 @@
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
@@ -2362,29 +2360,29 @@
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
@@ -2479,15 +2477,15 @@
 
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
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
@@ -2626,15 +2624,15 @@
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
@@ -2753,15 +2751,15 @@
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

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/client.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/client.pyi`

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
@@ -91,25 +92,25 @@
     CreateDBSecurityGroupResultTypeDef,
     CreateDBSnapshotResultTypeDef,
     CreateDBSubnetGroupResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateGlobalClusterResultTypeDef,
     CreateOptionGroupResultTypeDef,
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
@@ -136,15 +137,15 @@
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
@@ -160,15 +161,15 @@
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
@@ -195,15 +196,14 @@
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
@@ -435,32 +435,32 @@
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
@@ -574,15 +574,15 @@
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
@@ -633,15 +633,14 @@
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
@@ -651,15 +650,15 @@
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
@@ -961,15 +960,15 @@
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
@@ -983,15 +982,15 @@
         The DeleteDBCluster action deletes a previously provisioned DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#delete_db_cluster)
         """
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
@@ -1528,16 +1527,16 @@
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
@@ -1812,15 +1811,15 @@
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
@@ -1862,39 +1861,38 @@
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
@@ -1978,15 +1976,15 @@
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
@@ -2093,15 +2091,15 @@
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
@@ -2232,28 +2230,28 @@
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
@@ -2345,15 +2343,15 @@
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
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
@@ -2489,15 +2487,15 @@
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
@@ -2610,15 +2608,15 @@
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

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/literals.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/literals.py`

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
```

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/literals.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/literals.pyi`

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
```

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/paginator.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/paginator.py`

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
@@ -673,16 +673,16 @@
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

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/paginator.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/paginator.pyi`

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
@@ -646,16 +646,16 @@
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

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/type_defs.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/type_defs.py`

 * *Files 2% similar despite different names*

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
@@ -59,17 +58,18 @@
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
@@ -102,14 +102,15 @@
     "RestoreWindowTypeDef",
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
@@ -244,17 +245,15 @@
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
@@ -262,17 +261,19 @@
     "ModifyDBProxyRequestRequestTypeDef",
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
     "DescribeDBClusterBacktracksMessageRequestTypeDef",
@@ -355,49 +356,52 @@
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
@@ -412,18 +416,14 @@
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
@@ -466,15 +466,14 @@
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
@@ -534,15 +533,14 @@
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
@@ -585,45 +583,72 @@
 
 
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
@@ -697,27 +719,25 @@
 
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
@@ -732,26 +752,24 @@
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
@@ -792,15 +810,14 @@
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
@@ -828,28 +845,26 @@
 
 CustomDBEngineVersionAMITypeDef = TypedDict(
     "CustomDBEngineVersionAMITypeDef",
     {
         "ImageId": str,
         "Status": str,
     },
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
@@ -858,35 +873,32 @@
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
@@ -896,241 +908,225 @@
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
 )
 
 RestoreWindowTypeDef = TypedDict(
     "RestoreWindowTypeDef",
     {
         "EarliestTime": datetime,
         "LatestTime": datetime,
     },
-    total=False,
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
@@ -1358,15 +1354,14 @@
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
@@ -1381,15 +1376,14 @@
 
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
@@ -1414,28 +1408,26 @@
 
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
@@ -1450,15 +1442,14 @@
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
@@ -1489,35 +1480,32 @@
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
@@ -1602,14 +1590,32 @@
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
+
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1777,54 +1783,48 @@
 
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
@@ -1856,15 +1856,14 @@
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
@@ -1893,15 +1892,14 @@
 
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
@@ -2010,15 +2008,14 @@
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
@@ -2197,16 +2194,16 @@
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
@@ -2222,16 +2219,16 @@
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
@@ -2272,16 +2269,16 @@
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
@@ -2813,45 +2810,14 @@
 
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
@@ -2868,22 +2834,14 @@
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
-
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
@@ -2915,57 +2873,69 @@
         "SupportedNetworkTypes": List[str],
         "SupportsStorageThroughput": bool,
         "MinStorageThroughputPerDbInstance": int,
         "MaxStorageThroughputPerDbInstance": int,
         "MinStorageThroughputPerIops": float,
         "MaxStorageThroughputPerIops": float,
     },
-    total=False,
 )
 
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
-)
-
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
@@ -2990,30 +2960,28 @@
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
@@ -3139,15 +3107,14 @@
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
 
 
 class CreateDBClusterMessageRequestTypeDef(
@@ -3201,15 +3168,14 @@
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
 
 
 class ModifyDBClusterMessageRequestTypeDef(
     _RequiredModifyDBClusterMessageRequestTypeDef, _OptionalModifyDBClusterMessageRequestTypeDef
@@ -3328,15 +3294,15 @@
         "SourceDBClusterIdentifier": str,
     },
 )
 _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "RestoreType": str,
-        "RestoreToTime": TimestampTypeDef,
+        "RestoreToTime": Union[datetime, str],
         "UseLatestRestorableTime": bool,
         "Port": int,
         "DBSubnetGroupName": str,
         "OptionGroupName": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
@@ -3506,55 +3472,14 @@
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
-
 _RequiredModifyDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalModifyDBInstanceMessageRequestTypeDef = TypedDict(
@@ -3624,41 +3549,14 @@
 
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
-
 _RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef = TypedDict(
@@ -3788,15 +3686,15 @@
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
@@ -3973,28 +3871,26 @@
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
@@ -4014,20 +3910,19 @@
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
@@ -4053,22 +3948,20 @@
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
@@ -4097,30 +3990,94 @@
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
@@ -4134,38 +4091,35 @@
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
@@ -4570,16 +4524,16 @@
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
@@ -5127,16 +5081,16 @@
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
@@ -5483,32 +5437,92 @@
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
@@ -5535,54 +5549,49 @@
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
@@ -5597,15 +5606,14 @@
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
@@ -5614,97 +5622,96 @@
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
@@ -5757,15 +5764,15 @@
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
@@ -5776,17 +5783,15 @@
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
@@ -5798,55 +5803,14 @@
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
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5913,14 +5877,55 @@
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
@@ -6082,15 +6087,14 @@
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
@@ -6123,92 +6127,28 @@
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
 )
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
 
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6225,15 +6165,14 @@
 
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
@@ -6460,20 +6399,20 @@
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
@@ -6487,17 +6426,15 @@
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

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/type_defs.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/type_defs.pyi`

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
@@ -58,17 +57,18 @@
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
@@ -101,14 +101,15 @@
     "RestoreWindowTypeDef",
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
@@ -146,25 +147,26 @@
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
@@ -184,22 +186,22 @@
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
@@ -219,20 +221,19 @@
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
@@ -243,17 +244,15 @@
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
@@ -261,17 +260,19 @@
     "ModifyDBProxyRequestRequestTypeDef",
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
     "DescribeDBClusterBacktracksMessageRequestTypeDef",
@@ -354,49 +355,52 @@
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
@@ -411,18 +415,14 @@
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
@@ -465,15 +465,14 @@
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
@@ -531,15 +530,14 @@
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
@@ -580,45 +578,70 @@
     pass
 
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
@@ -626,39 +649,36 @@
 
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
@@ -690,27 +710,25 @@
 
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
@@ -725,26 +743,24 @@
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
@@ -785,15 +801,14 @@
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
@@ -821,28 +836,26 @@
 
 CustomDBEngineVersionAMITypeDef = TypedDict(
     "CustomDBEngineVersionAMITypeDef",
     {
         "ImageId": str,
         "Status": str,
     },
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
@@ -851,35 +864,32 @@
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
@@ -889,241 +899,225 @@
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
 )
 
 RestoreWindowTypeDef = TypedDict(
     "RestoreWindowTypeDef",
     {
         "EarliestTime": datetime,
         "LatestTime": datetime,
     },
-    total=False,
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
@@ -1343,15 +1337,14 @@
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
@@ -1366,15 +1359,14 @@
 
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
@@ -1397,28 +1389,26 @@
 
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
@@ -1433,15 +1423,14 @@
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
@@ -1470,35 +1459,32 @@
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
@@ -1577,14 +1563,32 @@
 
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
+
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1740,54 +1744,48 @@
 
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
@@ -1817,15 +1815,14 @@
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
@@ -1852,15 +1849,14 @@
 
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
@@ -1963,15 +1959,14 @@
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
@@ -2138,16 +2133,16 @@
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
@@ -2163,16 +2158,16 @@
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
@@ -2213,16 +2208,16 @@
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
@@ -2720,45 +2715,14 @@
 )
 
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
@@ -2773,22 +2737,14 @@
 
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
-
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
@@ -2820,55 +2776,69 @@
         "SupportedNetworkTypes": List[str],
         "SupportsStorageThroughput": bool,
         "MinStorageThroughputPerDbInstance": int,
         "MaxStorageThroughputPerDbInstance": int,
         "MinStorageThroughputPerIops": float,
         "MaxStorageThroughputPerIops": float,
     },
-    total=False,
 )
 
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
-)
-
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
@@ -2893,30 +2863,28 @@
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
@@ -3040,15 +3008,14 @@
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
 
 class CreateDBClusterMessageRequestTypeDef(
     _RequiredCreateDBClusterMessageRequestTypeDef, _OptionalCreateDBClusterMessageRequestTypeDef
@@ -3100,15 +3067,14 @@
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
 
 class ModifyDBClusterMessageRequestTypeDef(
     _RequiredModifyDBClusterMessageRequestTypeDef, _OptionalModifyDBClusterMessageRequestTypeDef
 ):
@@ -3221,15 +3187,15 @@
         "SourceDBClusterIdentifier": str,
     },
 )
 _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "RestoreType": str,
-        "RestoreToTime": TimestampTypeDef,
+        "RestoreToTime": Union[datetime, str],
         "UseLatestRestorableTime": bool,
         "Port": int,
         "DBSubnetGroupName": str,
         "OptionGroupName": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
@@ -3393,55 +3359,14 @@
 
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
-
 _RequiredModifyDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalModifyDBInstanceMessageRequestTypeDef = TypedDict(
@@ -3509,41 +3434,14 @@
 )
 
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
-
 _RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef = TypedDict(
@@ -3669,15 +3567,15 @@
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
@@ -3848,28 +3746,26 @@
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
@@ -3889,20 +3785,19 @@
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
@@ -3928,22 +3823,20 @@
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
@@ -3972,30 +3865,94 @@
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
@@ -4009,38 +3966,35 @@
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
@@ -4429,16 +4383,16 @@
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
@@ -4964,16 +4918,16 @@
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
@@ -5314,32 +5268,88 @@
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
@@ -5364,54 +5374,49 @@
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
@@ -5426,15 +5431,14 @@
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
@@ -5443,97 +5447,96 @@
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
@@ -5586,15 +5589,15 @@
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
@@ -5605,17 +5608,15 @@
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
@@ -5627,55 +5628,14 @@
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
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5742,14 +5702,55 @@
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
@@ -5911,15 +5912,14 @@
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
@@ -5950,89 +5950,29 @@
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
@@ -6048,15 +5988,14 @@
 
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
@@ -6283,20 +6222,20 @@
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
@@ -6310,17 +6249,15 @@
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

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/waiter.py` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds/waiter.pyi` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds.egg-info/PKG-INFO` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.28.16.post1
-Summary: Type annotations for boto3.RDS 1.28.16 service generated with mypy-boto3-builder 7.17.1
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
-[boto3.RDS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
@@ -646,14 +646,15 @@
     RestoreWindowTypeDef,
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
@@ -691,25 +692,26 @@
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
@@ -729,22 +731,22 @@
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
@@ -764,20 +766,19 @@
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
@@ -788,17 +789,15 @@
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
@@ -806,17 +805,19 @@
     ModifyDBProxyRequestRequestTypeDef,
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
     DescribeDBClusterBacktracksMessageRequestTypeDef,
@@ -899,49 +900,52 @@
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
@@ -956,18 +960,14 @@
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
@@ -1004,15 +1004,15 @@
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

### Comparing `mypy-boto3-rds-1.28.16.post1/mypy_boto3_rds.egg-info/SOURCES.txt` & `mypy-boto3-rds-1.28.9/mypy_boto3_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.28.16.post1/setup.py` & `mypy-boto3-rds-1.28.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rds",
-    version="1.28.16.post1",
+    version="1.28.9",
     packages=["mypy_boto3_rds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RDS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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

