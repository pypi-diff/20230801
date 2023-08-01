# Comparing `tmp/mypy-boto3-dynamodb-1.28.15.post2.tar.gz` & `tmp/mypy-boto3-dynamodb-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodb-1.28.15.post2.tar", last modified: Sat Jul 29 10:02:59 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodb-1.28.16.tar", last modified: Tue Aug  1 11:36:39 2023, max compression
```

## Comparing `mypy-boto3-dynamodb-1.28.15.post2.tar` & `mypy-boto3-dynamodb-1.28.16.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.365115 mypy-boto3-dynamodb-1.28.15.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-07-29 10:02:59.365115 mypy-boto3-dynamodb-1.28.15.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24487 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.361115 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53762 2023-07-29 09:42:58.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53695 2023-07-29 09:42:58.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26844 2023-07-29 09:42:58.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-07-29 09:42:58.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   122126 2023-07-29 09:43:03.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   121987 2023-07-29 09:43:02.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.365115 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:59.365115 mypy-boto3-dynamodb-1.28.15.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.404906 mypy-boto3-dynamodb-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26276 2023-08-01 11:36:39.400906 mypy-boto3-dynamodb-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.396906 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48027 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-08-01 11:15:32.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   105178 2023-08-01 11:15:36.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105039 2023-08-01 11:15:34.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.400906 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26276 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:39.404906 mypy-boto3-dynamodb-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/setup.py
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/LICENSE` & `mypy-boto3-dynamodb-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/PKG-INFO` & `mypy-boto3-dynamodb-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.28.15.post2
-Summary: Type annotations for boto3.DynamoDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DynamoDB 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 dynamodb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 dynamodb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
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
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -79,15 +79,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -472,33 +472,35 @@
 )
 
 
 def check_value(value: AttributeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
     ResponseMetadataTypeDef,
     ArchivalSummaryTypeDef,
     AttributeDefinitionTypeDef,
     AttributeValueTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTypeDef,
+    TableAttributeValueTypeDef,
     BillingModeSummaryTypeDef,
     CapacityTypeDef,
+    ConditionBaseImportTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
     ContributorInsightsSummaryTypeDef,
     CreateBackupInputRequestTypeDef,
     KeySchemaElementTypeDef,
     ProjectionTypeDef,
     ProvisionedThroughputTypeDef,
     ReplicaTypeDef,
@@ -528,22 +530,20 @@
     KinesisDataStreamDestinationTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
     ExportSummaryTypeDef,
-    ExportTableToPointInTimeInputRequestTypeDef,
-    GetItemInputTableGetItemTypeDef,
+    TimestampTypeDef,
     ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
     ListTablesInputRequestTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
@@ -562,39 +562,26 @@
     ListTablesOutputTypeDef,
     ProvisionedThroughputDescriptionResponseTypeDef,
     RestoreSummaryResponseTypeDef,
     SSEDescriptionResponseTypeDef,
     StreamSpecificationResponseTypeDef,
     TableClassSummaryResponseTypeDef,
     UpdateContributorInsightsOutputTypeDef,
-    AttributeValueUpdateTypeDef,
+    UniversalAttributeValueTypeDef,
+    AutoScalingPolicyDescriptionTypeDef,
+    AutoScalingPolicyUpdateTypeDef,
+    CreateBackupOutputTypeDef,
+    ListBackupsOutputTypeDef,
     BatchStatementErrorTypeDef,
-    BatchStatementRequestTypeDef,
-    ConditionCheckTypeDef,
-    ConditionTypeDef,
     DeleteRequestOutputTypeDef,
-    DeleteRequestTypeDef,
-    DeleteTypeDef,
-    ExecuteStatementInputRequestTypeDef,
-    ExpectedAttributeValueTypeDef,
-    GetItemInputRequestTypeDef,
-    GetTypeDef,
+    GetItemInputTableGetItemTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
     KeysAndAttributesOutputTypeDef,
-    KeysAndAttributesTypeDef,
-    ParameterizedStatementTypeDef,
     PutRequestOutputTypeDef,
-    PutRequestTypeDef,
-    PutTypeDef,
-    UpdateTypeDef,
-    AutoScalingPolicyDescriptionTypeDef,
-    AutoScalingPolicyUpdateTypeDef,
-    CreateBackupOutputTypeDef,
-    ListBackupsOutputTypeDef,
     ConsumedCapacityTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
     GlobalSecondaryIndexTypeDef,
     SourceTableDetailsTypeDef,
@@ -613,49 +600,47 @@
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
+    ExportTableToPointInTimeInputRequestTypeDef,
+    ListBackupsInputRequestTypeDef,
     GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexOutputTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
     ImportSummaryTypeDef,
     ListBackupsInputListBackupsPaginateTypeDef,
     ListTablesInputListTablesPaginateTypeDef,
     ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
-    BatchStatementResponseTypeDef,
-    BatchExecuteStatementInputRequestTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    QueryInputRequestTypeDef,
-    QueryInputTableQueryTypeDef,
-    ScanInputRequestTypeDef,
-    ScanInputScanPaginateTypeDef,
-    ScanInputTableScanTypeDef,
-    DeleteItemInputRequestTypeDef,
-    DeleteItemInputTableDeleteItemTypeDef,
-    PutItemInputRequestTypeDef,
-    PutItemInputTablePutItemTypeDef,
-    UpdateItemInputRequestTypeDef,
-    UpdateItemInputTableUpdateItemTypeDef,
-    TransactGetItemTypeDef,
-    BatchGetItemInputRequestTypeDef,
-    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    ExecuteTransactionInputRequestTypeDef,
-    WriteRequestOutputTypeDef,
-    WriteRequestTypeDef,
-    TransactWriteItemTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchStatementRequestTypeDef,
+    ConditionCheckTypeDef,
+    ConditionTypeDef,
+    DeleteRequestTypeDef,
+    DeleteTypeDef,
+    ExecuteStatementInputRequestTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemInputRequestTypeDef,
+    GetTypeDef,
+    KeysAndAttributesTypeDef,
+    ParameterizedStatementTypeDef,
+    PutRequestTypeDef,
+    PutTypeDef,
+    UpdateTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
+    BatchStatementResponseTypeDef,
+    WriteRequestOutputTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
@@ -667,40 +652,62 @@
     UpdateContinuousBackupsOutputTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     ListGlobalTablesOutputTypeDef,
     ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
+    InputFormatOptionsUnionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
-    CreateTableInputRequestTypeDef,
-    CreateTableInputServiceResourceCreateTableTypeDef,
-    RestoreTableFromBackupInputRequestTypeDef,
-    RestoreTableToPointInTimeInputRequestTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     TableCreationParametersOutputTypeDef,
     SourceTableFeatureDetailsTypeDef,
     ListImportsOutputTypeDef,
-    BatchExecuteStatementOutputTypeDef,
-    TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemOutputTypeDef,
-    BatchWriteItemInputRequestTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    TransactWriteItemsInputRequestTypeDef,
+    BatchExecuteStatementInputRequestTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    QueryInputRequestTypeDef,
+    QueryInputTableQueryTypeDef,
+    ScanInputRequestTypeDef,
+    ScanInputScanPaginateTypeDef,
+    ScanInputTableScanTypeDef,
+    DeleteItemInputRequestTypeDef,
+    DeleteItemInputTableDeleteItemTypeDef,
+    PutItemInputRequestTypeDef,
+    PutItemInputTablePutItemTypeDef,
+    UpdateItemInputRequestTypeDef,
+    UpdateItemInputTableUpdateItemTypeDef,
+    TransactGetItemTypeDef,
+    KeysAndAttributesUnionTypeDef,
+    ExecuteTransactionInputRequestTypeDef,
+    WriteRequestTypeDef,
+    TransactWriteItemTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
+    BatchExecuteStatementOutputTypeDef,
+    BatchWriteItemOutputTypeDef,
     ImportTableInputRequestTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
     ReplicationGroupUpdateTypeDef,
+    CreateTableInputRequestTypeDef,
+    CreateTableInputServiceResourceCreateTableTypeDef,
+    RestoreTableFromBackupInputRequestTypeDef,
+    RestoreTableToPointInTimeInputRequestTypeDef,
     ImportTableDescriptionTypeDef,
+    TableCreationParametersUnionTypeDef,
     BackupDescriptionTypeDef,
+    TransactGetItemsInputRequestTypeDef,
+    BatchGetItemInputRequestTypeDef,
+    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    WriteRequestUnionTypeDef,
+    TransactWriteItemsInputRequestTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
@@ -712,25 +719,27 @@
     UpdateTableOutputTypeDef,
     UpdateTableInputRequestTypeDef,
     UpdateTableInputTableUpdateTypeDef,
     DescribeImportOutputTypeDef,
     ImportTableOutputTypeDef,
     DeleteBackupOutputTypeDef,
     DescribeBackupOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/README.md` & `mypy-boto3-dynamodb-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
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
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -47,15 +47,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -440,33 +440,35 @@
 )
 
 
 def check_value(value: AttributeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
     ResponseMetadataTypeDef,
     ArchivalSummaryTypeDef,
     AttributeDefinitionTypeDef,
     AttributeValueTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTypeDef,
+    TableAttributeValueTypeDef,
     BillingModeSummaryTypeDef,
     CapacityTypeDef,
+    ConditionBaseImportTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
     ContributorInsightsSummaryTypeDef,
     CreateBackupInputRequestTypeDef,
     KeySchemaElementTypeDef,
     ProjectionTypeDef,
     ProvisionedThroughputTypeDef,
     ReplicaTypeDef,
@@ -496,22 +498,20 @@
     KinesisDataStreamDestinationTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
     ExportSummaryTypeDef,
-    ExportTableToPointInTimeInputRequestTypeDef,
-    GetItemInputTableGetItemTypeDef,
+    TimestampTypeDef,
     ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
     ListTablesInputRequestTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
@@ -530,39 +530,26 @@
     ListTablesOutputTypeDef,
     ProvisionedThroughputDescriptionResponseTypeDef,
     RestoreSummaryResponseTypeDef,
     SSEDescriptionResponseTypeDef,
     StreamSpecificationResponseTypeDef,
     TableClassSummaryResponseTypeDef,
     UpdateContributorInsightsOutputTypeDef,
-    AttributeValueUpdateTypeDef,
+    UniversalAttributeValueTypeDef,
+    AutoScalingPolicyDescriptionTypeDef,
+    AutoScalingPolicyUpdateTypeDef,
+    CreateBackupOutputTypeDef,
+    ListBackupsOutputTypeDef,
     BatchStatementErrorTypeDef,
-    BatchStatementRequestTypeDef,
-    ConditionCheckTypeDef,
-    ConditionTypeDef,
     DeleteRequestOutputTypeDef,
-    DeleteRequestTypeDef,
-    DeleteTypeDef,
-    ExecuteStatementInputRequestTypeDef,
-    ExpectedAttributeValueTypeDef,
-    GetItemInputRequestTypeDef,
-    GetTypeDef,
+    GetItemInputTableGetItemTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
     KeysAndAttributesOutputTypeDef,
-    KeysAndAttributesTypeDef,
-    ParameterizedStatementTypeDef,
     PutRequestOutputTypeDef,
-    PutRequestTypeDef,
-    PutTypeDef,
-    UpdateTypeDef,
-    AutoScalingPolicyDescriptionTypeDef,
-    AutoScalingPolicyUpdateTypeDef,
-    CreateBackupOutputTypeDef,
-    ListBackupsOutputTypeDef,
     ConsumedCapacityTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
     GlobalSecondaryIndexTypeDef,
     SourceTableDetailsTypeDef,
@@ -581,49 +568,47 @@
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
+    ExportTableToPointInTimeInputRequestTypeDef,
+    ListBackupsInputRequestTypeDef,
     GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexOutputTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
     ImportSummaryTypeDef,
     ListBackupsInputListBackupsPaginateTypeDef,
     ListTablesInputListTablesPaginateTypeDef,
     ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
-    BatchStatementResponseTypeDef,
-    BatchExecuteStatementInputRequestTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    QueryInputRequestTypeDef,
-    QueryInputTableQueryTypeDef,
-    ScanInputRequestTypeDef,
-    ScanInputScanPaginateTypeDef,
-    ScanInputTableScanTypeDef,
-    DeleteItemInputRequestTypeDef,
-    DeleteItemInputTableDeleteItemTypeDef,
-    PutItemInputRequestTypeDef,
-    PutItemInputTablePutItemTypeDef,
-    UpdateItemInputRequestTypeDef,
-    UpdateItemInputTableUpdateItemTypeDef,
-    TransactGetItemTypeDef,
-    BatchGetItemInputRequestTypeDef,
-    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    ExecuteTransactionInputRequestTypeDef,
-    WriteRequestOutputTypeDef,
-    WriteRequestTypeDef,
-    TransactWriteItemTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchStatementRequestTypeDef,
+    ConditionCheckTypeDef,
+    ConditionTypeDef,
+    DeleteRequestTypeDef,
+    DeleteTypeDef,
+    ExecuteStatementInputRequestTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemInputRequestTypeDef,
+    GetTypeDef,
+    KeysAndAttributesTypeDef,
+    ParameterizedStatementTypeDef,
+    PutRequestTypeDef,
+    PutTypeDef,
+    UpdateTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
+    BatchStatementResponseTypeDef,
+    WriteRequestOutputTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
@@ -635,40 +620,62 @@
     UpdateContinuousBackupsOutputTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     ListGlobalTablesOutputTypeDef,
     ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
+    InputFormatOptionsUnionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
-    CreateTableInputRequestTypeDef,
-    CreateTableInputServiceResourceCreateTableTypeDef,
-    RestoreTableFromBackupInputRequestTypeDef,
-    RestoreTableToPointInTimeInputRequestTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     TableCreationParametersOutputTypeDef,
     SourceTableFeatureDetailsTypeDef,
     ListImportsOutputTypeDef,
-    BatchExecuteStatementOutputTypeDef,
-    TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemOutputTypeDef,
-    BatchWriteItemInputRequestTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    TransactWriteItemsInputRequestTypeDef,
+    BatchExecuteStatementInputRequestTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    QueryInputRequestTypeDef,
+    QueryInputTableQueryTypeDef,
+    ScanInputRequestTypeDef,
+    ScanInputScanPaginateTypeDef,
+    ScanInputTableScanTypeDef,
+    DeleteItemInputRequestTypeDef,
+    DeleteItemInputTableDeleteItemTypeDef,
+    PutItemInputRequestTypeDef,
+    PutItemInputTablePutItemTypeDef,
+    UpdateItemInputRequestTypeDef,
+    UpdateItemInputTableUpdateItemTypeDef,
+    TransactGetItemTypeDef,
+    KeysAndAttributesUnionTypeDef,
+    ExecuteTransactionInputRequestTypeDef,
+    WriteRequestTypeDef,
+    TransactWriteItemTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
+    BatchExecuteStatementOutputTypeDef,
+    BatchWriteItemOutputTypeDef,
     ImportTableInputRequestTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
     ReplicationGroupUpdateTypeDef,
+    CreateTableInputRequestTypeDef,
+    CreateTableInputServiceResourceCreateTableTypeDef,
+    RestoreTableFromBackupInputRequestTypeDef,
+    RestoreTableToPointInTimeInputRequestTypeDef,
     ImportTableDescriptionTypeDef,
+    TableCreationParametersUnionTypeDef,
     BackupDescriptionTypeDef,
+    TransactGetItemsInputRequestTypeDef,
+    BatchGetItemInputRequestTypeDef,
+    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    WriteRequestUnionTypeDef,
+    TransactWriteItemsInputRequestTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
@@ -680,25 +687,27 @@
     UpdateTableOutputTypeDef,
     UpdateTableInputRequestTypeDef,
     UpdateTableInputTableUpdateTypeDef,
     DescribeImportOutputTypeDef,
     ImportTableOutputTypeDef,
     DeleteBackupOutputTypeDef,
     DescribeBackupOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__init__.py` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__init__.pyi` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__main__.py` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.28.15\nVersion:         1.28.15.post2\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.DynamoDB 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post2")
+    print("1.28.16")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/client.py` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,15 @@
     from mypy_boto3_dynamodb.client import DynamoDBClient
 
     session = Session()
     client: DynamoDBClient = session.client("dynamodb")
     ```
 """
 import sys
-from datetime import datetime
-from decimal import Decimal
-from typing import Any, Dict, Mapping, Sequence, Set, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BackupTypeFilterType,
     BillingModeType,
     ConditionalOperatorType,
@@ -41,15 +39,14 @@
     ListTablesPaginator,
     ListTagsOfResourcePaginator,
     QueryPaginator,
     ScanPaginator,
 )
 from .type_defs import (
     AttributeDefinitionTypeDef,
-    AttributeValueTypeDef,
     AttributeValueUpdateTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     BatchStatementRequestTypeDef,
     BatchWriteItemOutputTypeDef,
     ConditionTypeDef,
@@ -75,23 +72,20 @@
     EmptyResponseMetadataTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     ExpectedAttributeValueTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     GetItemOutputTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
-    GlobalSecondaryIndexOutputTypeDef,
-    GlobalSecondaryIndexTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ImportTableOutputTypeDef,
-    InputFormatOptionsOutputTypeDef,
-    InputFormatOptionsTypeDef,
-    KeysAndAttributesOutputTypeDef,
-    KeysAndAttributesTypeDef,
+    InputFormatOptionsUnionTypeDef,
+    KeysAndAttributesUnionTypeDef,
     KeySchemaElementTypeDef,
     KinesisStreamingDestinationOutputTypeDef,
     ListBackupsOutputTypeDef,
     ListContributorInsightsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
@@ -110,32 +104,32 @@
     ReplicaUpdateTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     S3BucketSourceTypeDef,
     ScanOutputTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
-    TableCreationParametersOutputTypeDef,
-    TableCreationParametersTypeDef,
+    TableCreationParametersUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimeToLiveSpecificationTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactGetItemTypeDef,
     TransactWriteItemsOutputTypeDef,
     TransactWriteItemTypeDef,
+    UniversalAttributeValueTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateItemOutputTypeDef,
     UpdateTableOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
     UpdateTimeToLiveOutputTypeDef,
-    WriteRequestOutputTypeDef,
-    WriteRequestTypeDef,
+    WriteRequestUnionTypeDef,
 )
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -217,29 +211,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#batch_execute_statement)
         """
 
     def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, Union[KeysAndAttributesTypeDef, KeysAndAttributesOutputTypeDef]],
+        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_get_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#batch_get_item)
         """
 
     def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[Union[WriteRequestTypeDef, WriteRequestOutputTypeDef]]],
+        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
     ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
@@ -284,17 +278,15 @@
     def create_table(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
         KeySchema: Sequence[KeySchemaElementTypeDef],
         LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
@@ -314,61 +306,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#delete_backup)
         """
 
     def delete_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#delete_item)
@@ -522,33 +476,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#enable_kinesis_streaming_destination)
         """
 
     def execute_statement(
         self,
         *,
         Statement: str,
-        Parameters: Sequence[
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ] = ...,
+        Parameters: Sequence[UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         Limit: int = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> ExecuteStatementOutputTypeDef:
         """
@@ -575,15 +511,15 @@
         """
 
     def export_table_to_point_in_time(
         self,
         *,
         TableArn: str,
         S3Bucket: str,
-        ExportTime: Union[datetime, str] = ...,
+        ExportTime: TimestampTypeDef = ...,
         ClientToken: str = ...,
         S3BucketOwner: str = ...,
         S3Prefix: str = ...,
         S3SseAlgorithm: S3SseAlgorithmType = ...,
         S3SseKmsKeyId: str = ...,
         ExportFormat: ExportFormatType = ...
     ) -> ExportTableToPointInTimeOutputTypeDef:
@@ -608,34 +544,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#generate_presigned_url)
         """
 
     def get_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
     ) -> GetItemOutputTypeDef:
         """
@@ -647,35 +564,33 @@
         """
 
     def import_table(
         self,
         *,
         S3BucketSource: S3BucketSourceTypeDef,
         InputFormat: InputFormatType,
-        TableCreationParameters: Union[
-            TableCreationParametersTypeDef, TableCreationParametersOutputTypeDef
-        ],
+        TableCreationParameters: TableCreationParametersUnionTypeDef,
         ClientToken: str = ...,
-        InputFormatOptions: Union[InputFormatOptionsTypeDef, InputFormatOptionsOutputTypeDef] = ...,
+        InputFormatOptions: InputFormatOptionsUnionTypeDef = ...,
         InputCompressionType: InputCompressionTypeType = ...
     ) -> ImportTableOutputTypeDef:
         """
         Imports table data from an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.import_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#import_table)
         """
 
     def list_backups(
         self,
         *,
         TableName: str = ...,
         Limit: int = ...,
-        TimeRangeLowerBound: Union[datetime, str] = ...,
-        TimeRangeUpperBound: Union[datetime, str] = ...,
+        TimeRangeLowerBound: TimestampTypeDef = ...,
+        TimeRangeUpperBound: TimestampTypeDef = ...,
         ExclusiveStartBackupArn: str = ...,
         BackupType: BackupTypeFilterType = ...
     ) -> ListBackupsOutputTypeDef:
         """
         List backups associated with an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_backups)
@@ -744,61 +659,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#list_tags_of_resource)
         """
 
     def put_item(
         self,
         *,
         TableName: str,
-        Item: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Item: Mapping[str, UniversalAttributeValueTypeDef],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#put_item)
@@ -813,59 +690,21 @@
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
         KeyConditions: Mapping[str, ConditionTypeDef] = ...,
         QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#query)
@@ -873,17 +712,15 @@
 
     def restore_table_from_backup(
         self,
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
@@ -894,19 +731,17 @@
     def restore_table_to_point_in_time(
         self,
         *,
         TargetTableName: str,
         SourceTableArn: str = ...,
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
-        RestoreDateTime: Union[datetime, str] = ...,
+        RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and `LatestRestorableDateTime`.
@@ -921,60 +756,22 @@
         TableName: str,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
         ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...
     ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.scan)
@@ -1089,63 +886,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#update_global_table_settings)
         """
 
     def update_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/client.pyi` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,15 @@
     from mypy_boto3_dynamodb.client import DynamoDBClient
 
     session = Session()
     client: DynamoDBClient = session.client("dynamodb")
     ```
 """
 import sys
-from datetime import datetime
-from decimal import Decimal
-from typing import Any, Dict, Mapping, Sequence, Set, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BackupTypeFilterType,
     BillingModeType,
     ConditionalOperatorType,
@@ -41,15 +39,14 @@
     ListTablesPaginator,
     ListTagsOfResourcePaginator,
     QueryPaginator,
     ScanPaginator,
 )
 from .type_defs import (
     AttributeDefinitionTypeDef,
-    AttributeValueTypeDef,
     AttributeValueUpdateTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     BatchStatementRequestTypeDef,
     BatchWriteItemOutputTypeDef,
     ConditionTypeDef,
@@ -75,23 +72,20 @@
     EmptyResponseMetadataTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     ExpectedAttributeValueTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     GetItemOutputTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
-    GlobalSecondaryIndexOutputTypeDef,
-    GlobalSecondaryIndexTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ImportTableOutputTypeDef,
-    InputFormatOptionsOutputTypeDef,
-    InputFormatOptionsTypeDef,
-    KeysAndAttributesOutputTypeDef,
-    KeysAndAttributesTypeDef,
+    InputFormatOptionsUnionTypeDef,
+    KeysAndAttributesUnionTypeDef,
     KeySchemaElementTypeDef,
     KinesisStreamingDestinationOutputTypeDef,
     ListBackupsOutputTypeDef,
     ListContributorInsightsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
@@ -110,32 +104,32 @@
     ReplicaUpdateTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     S3BucketSourceTypeDef,
     ScanOutputTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
-    TableCreationParametersOutputTypeDef,
-    TableCreationParametersTypeDef,
+    TableCreationParametersUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimeToLiveSpecificationTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactGetItemTypeDef,
     TransactWriteItemsOutputTypeDef,
     TransactWriteItemTypeDef,
+    UniversalAttributeValueTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateItemOutputTypeDef,
     UpdateTableOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
     UpdateTimeToLiveOutputTypeDef,
-    WriteRequestOutputTypeDef,
-    WriteRequestTypeDef,
+    WriteRequestUnionTypeDef,
 )
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -211,28 +205,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#batch_execute_statement)
         """
     def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, Union[KeysAndAttributesTypeDef, KeysAndAttributesOutputTypeDef]],
+        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_get_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#batch_get_item)
         """
     def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[Union[WriteRequestTypeDef, WriteRequestOutputTypeDef]]],
+        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
     ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
@@ -272,17 +266,15 @@
     def create_table(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
         KeySchema: Sequence[KeySchemaElementTypeDef],
         LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
@@ -300,61 +292,23 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#delete_backup)
         """
     def delete_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#delete_item)
@@ -491,33 +445,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.enable_kinesis_streaming_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#enable_kinesis_streaming_destination)
         """
     def execute_statement(
         self,
         *,
         Statement: str,
-        Parameters: Sequence[
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ] = ...,
+        Parameters: Sequence[UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         Limit: int = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> ExecuteStatementOutputTypeDef:
         """
@@ -542,15 +478,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#execute_transaction)
         """
     def export_table_to_point_in_time(
         self,
         *,
         TableArn: str,
         S3Bucket: str,
-        ExportTime: Union[datetime, str] = ...,
+        ExportTime: TimestampTypeDef = ...,
         ClientToken: str = ...,
         S3BucketOwner: str = ...,
         S3Prefix: str = ...,
         S3SseAlgorithm: S3SseAlgorithmType = ...,
         S3SseKmsKeyId: str = ...,
         ExportFormat: ExportFormatType = ...
     ) -> ExportTableToPointInTimeOutputTypeDef:
@@ -573,34 +509,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#generate_presigned_url)
         """
     def get_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
     ) -> GetItemOutputTypeDef:
         """
@@ -611,34 +528,32 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#get_item)
         """
     def import_table(
         self,
         *,
         S3BucketSource: S3BucketSourceTypeDef,
         InputFormat: InputFormatType,
-        TableCreationParameters: Union[
-            TableCreationParametersTypeDef, TableCreationParametersOutputTypeDef
-        ],
+        TableCreationParameters: TableCreationParametersUnionTypeDef,
         ClientToken: str = ...,
-        InputFormatOptions: Union[InputFormatOptionsTypeDef, InputFormatOptionsOutputTypeDef] = ...,
+        InputFormatOptions: InputFormatOptionsUnionTypeDef = ...,
         InputCompressionType: InputCompressionTypeType = ...
     ) -> ImportTableOutputTypeDef:
         """
         Imports table data from an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.import_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#import_table)
         """
     def list_backups(
         self,
         *,
         TableName: str = ...,
         Limit: int = ...,
-        TimeRangeLowerBound: Union[datetime, str] = ...,
-        TimeRangeUpperBound: Union[datetime, str] = ...,
+        TimeRangeLowerBound: TimestampTypeDef = ...,
+        TimeRangeUpperBound: TimestampTypeDef = ...,
         ExclusiveStartBackupArn: str = ...,
         BackupType: BackupTypeFilterType = ...
     ) -> ListBackupsOutputTypeDef:
         """
         List backups associated with an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_backups)
@@ -700,61 +615,23 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_tags_of_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#list_tags_of_resource)
         """
     def put_item(
         self,
         *,
         TableName: str,
-        Item: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Item: Mapping[str, UniversalAttributeValueTypeDef],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#put_item)
@@ -768,76 +645,36 @@
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
         KeyConditions: Mapping[str, ConditionTypeDef] = ...,
         QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#query)
         """
     def restore_table_from_backup(
         self,
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
@@ -847,19 +684,17 @@
     def restore_table_to_point_in_time(
         self,
         *,
         TargetTableName: str,
         SourceTableArn: str = ...,
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
-        RestoreDateTime: Union[datetime, str] = ...,
+        RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and `LatestRestorableDateTime`.
@@ -873,60 +708,22 @@
         TableName: str,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
         ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...
     ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.scan)
@@ -1032,63 +829,25 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_global_table_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#update_global_table_settings)
         """
     def update_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/literals.py` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/literals.pyi` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/paginator.py` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     list_backups_paginator: ListBackupsPaginator = client.get_paginator("list_backups")
     list_tables_paginator: ListTablesPaginator = client.get_paginator("list_tables")
     list_tags_of_resource_paginator: ListTagsOfResourcePaginator = client.get_paginator("list_tags_of_resource")
     query_paginator: QueryPaginator = client.get_paginator("query")
     scan_paginator: ScanPaginator = client.get_paginator("scan")
     ```
 """
-from datetime import datetime
-from decimal import Decimal
-from typing import Any, Generic, Iterator, Mapping, Sequence, Set, TypeVar, Union
+from typing import Generic, Iterator, Mapping, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     BackupTypeFilterType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
@@ -43,14 +41,16 @@
     ConditionTypeDef,
     ListBackupsOutputTypeDef,
     ListTablesOutputTypeDef,
     ListTagsOfResourceOutputTypeDef,
     PaginatorConfigTypeDef,
     QueryOutputTypeDef,
     ScanOutputTypeDef,
+    TableAttributeValueTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
     "QueryPaginator",
@@ -74,16 +74,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
     """
 
     def paginate(
         self,
         *,
         TableName: str = ...,
-        TimeRangeLowerBound: Union[datetime, str] = ...,
-        TimeRangeUpperBound: Union[datetime, str] = ...,
+        TimeRangeLowerBound: TimestampTypeDef = ...,
+        TimeRangeUpperBound: TimestampTypeDef = ...,
         BackupType: BackupTypeFilterType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
         """
@@ -138,33 +138,15 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
@@ -186,33 +168,15 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/paginator.pyi` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/paginator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     list_backups_paginator: ListBackupsPaginator = client.get_paginator("list_backups")
     list_tables_paginator: ListTablesPaginator = client.get_paginator("list_tables")
     list_tags_of_resource_paginator: ListTagsOfResourcePaginator = client.get_paginator("list_tags_of_resource")
     query_paginator: QueryPaginator = client.get_paginator("query")
     scan_paginator: ScanPaginator = client.get_paginator("scan")
     ```
 """
-from datetime import datetime
-from decimal import Decimal
-from typing import Any, Generic, Iterator, Mapping, Sequence, Set, TypeVar, Union
+from typing import Generic, Iterator, Mapping, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     BackupTypeFilterType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
@@ -43,14 +41,16 @@
     ConditionTypeDef,
     ListBackupsOutputTypeDef,
     ListTablesOutputTypeDef,
     ListTagsOfResourceOutputTypeDef,
     PaginatorConfigTypeDef,
     QueryOutputTypeDef,
     ScanOutputTypeDef,
+    TableAttributeValueTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
     "QueryPaginator",
@@ -71,16 +71,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
     """
 
     def paginate(
         self,
         *,
         TableName: str = ...,
-        TimeRangeLowerBound: Union[datetime, str] = ...,
-        TimeRangeUpperBound: Union[datetime, str] = ...,
+        TimeRangeLowerBound: TimestampTypeDef = ...,
+        TimeRangeUpperBound: TimestampTypeDef = ...,
         BackupType: BackupTypeFilterType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
         """
@@ -132,33 +132,15 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
@@ -179,33 +161,15 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/type_defs.py` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -68,16 +68,18 @@
     "ArchivalSummaryTypeDef",
     "AttributeDefinitionTypeDef",
     "AttributeValueTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTypeDef",
+    "TableAttributeValueTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityTypeDef",
+    "ConditionBaseImportTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
     "KeySchemaElementTypeDef",
     "ProjectionTypeDef",
     "ProvisionedThroughputTypeDef",
     "ReplicaTypeDef",
@@ -107,22 +109,20 @@
     "KinesisDataStreamDestinationTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
     "ExportSummaryTypeDef",
-    "ExportTableToPointInTimeInputRequestTypeDef",
-    "GetItemInputTableGetItemTypeDef",
+    "TimestampTypeDef",
     "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
     "ListTablesInputRequestTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
@@ -141,39 +141,26 @@
     "ListTablesOutputTypeDef",
     "ProvisionedThroughputDescriptionResponseTypeDef",
     "RestoreSummaryResponseTypeDef",
     "SSEDescriptionResponseTypeDef",
     "StreamSpecificationResponseTypeDef",
     "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
-    "AttributeValueUpdateTypeDef",
+    "UniversalAttributeValueTypeDef",
+    "AutoScalingPolicyDescriptionTypeDef",
+    "AutoScalingPolicyUpdateTypeDef",
+    "CreateBackupOutputTypeDef",
+    "ListBackupsOutputTypeDef",
     "BatchStatementErrorTypeDef",
-    "BatchStatementRequestTypeDef",
-    "ConditionCheckTypeDef",
-    "ConditionTypeDef",
     "DeleteRequestOutputTypeDef",
-    "DeleteRequestTypeDef",
-    "DeleteTypeDef",
-    "ExecuteStatementInputRequestTypeDef",
-    "ExpectedAttributeValueTypeDef",
-    "GetItemInputRequestTypeDef",
-    "GetTypeDef",
+    "GetItemInputTableGetItemTypeDef",
     "ItemCollectionMetricsTypeDef",
     "ItemResponseTypeDef",
     "KeysAndAttributesOutputTypeDef",
-    "KeysAndAttributesTypeDef",
-    "ParameterizedStatementTypeDef",
     "PutRequestOutputTypeDef",
-    "PutRequestTypeDef",
-    "PutTypeDef",
-    "UpdateTypeDef",
-    "AutoScalingPolicyDescriptionTypeDef",
-    "AutoScalingPolicyUpdateTypeDef",
-    "CreateBackupOutputTypeDef",
-    "ListBackupsOutputTypeDef",
     "ConsumedCapacityTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
     "GlobalSecondaryIndexTypeDef",
     "SourceTableDetailsTypeDef",
@@ -192,49 +179,47 @@
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
+    "ExportTableToPointInTimeInputRequestTypeDef",
+    "ListBackupsInputRequestTypeDef",
     "GlobalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexOutputTypeDef",
     "LocalSecondaryIndexDescriptionTypeDef",
     "LocalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
     "ImportSummaryTypeDef",
     "ListBackupsInputListBackupsPaginateTypeDef",
     "ListTablesInputListTablesPaginateTypeDef",
     "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
     "UpdateTimeToLiveOutputTypeDef",
-    "BatchStatementResponseTypeDef",
-    "BatchExecuteStatementInputRequestTypeDef",
-    "QueryInputQueryPaginateTypeDef",
-    "QueryInputRequestTypeDef",
-    "QueryInputTableQueryTypeDef",
-    "ScanInputRequestTypeDef",
-    "ScanInputScanPaginateTypeDef",
-    "ScanInputTableScanTypeDef",
-    "DeleteItemInputRequestTypeDef",
-    "DeleteItemInputTableDeleteItemTypeDef",
-    "PutItemInputRequestTypeDef",
-    "PutItemInputTablePutItemTypeDef",
-    "UpdateItemInputRequestTypeDef",
-    "UpdateItemInputTableUpdateItemTypeDef",
-    "TransactGetItemTypeDef",
-    "BatchGetItemInputRequestTypeDef",
-    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    "ExecuteTransactionInputRequestTypeDef",
-    "WriteRequestOutputTypeDef",
-    "WriteRequestTypeDef",
-    "TransactWriteItemTypeDef",
+    "AttributeValueUpdateTypeDef",
+    "BatchStatementRequestTypeDef",
+    "ConditionCheckTypeDef",
+    "ConditionTypeDef",
+    "DeleteRequestTypeDef",
+    "DeleteTypeDef",
+    "ExecuteStatementInputRequestTypeDef",
+    "ExpectedAttributeValueTypeDef",
+    "GetItemInputRequestTypeDef",
+    "GetTypeDef",
+    "KeysAndAttributesTypeDef",
+    "ParameterizedStatementTypeDef",
+    "PutRequestTypeDef",
+    "PutTypeDef",
+    "UpdateTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
+    "BatchStatementResponseTypeDef",
+    "WriteRequestOutputTypeDef",
     "BatchGetItemOutputTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
     "GetItemOutputTypeDef",
     "PutItemOutputTypeDef",
     "QueryOutputTypeDef",
@@ -246,40 +231,62 @@
     "UpdateContinuousBackupsOutputTypeDef",
     "TableCreationParametersTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
     "ListGlobalTablesOutputTypeDef",
     "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
+    "InputFormatOptionsUnionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
-    "CreateTableInputRequestTypeDef",
-    "CreateTableInputServiceResourceCreateTableTypeDef",
-    "RestoreTableFromBackupInputRequestTypeDef",
-    "RestoreTableToPointInTimeInputRequestTypeDef",
+    "GlobalSecondaryIndexUnionTypeDef",
     "TableCreationParametersOutputTypeDef",
     "SourceTableFeatureDetailsTypeDef",
     "ListImportsOutputTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
-    "TransactGetItemsInputRequestTypeDef",
-    "BatchWriteItemOutputTypeDef",
-    "BatchWriteItemInputRequestTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
-    "TransactWriteItemsInputRequestTypeDef",
+    "BatchExecuteStatementInputRequestTypeDef",
+    "QueryInputQueryPaginateTypeDef",
+    "QueryInputRequestTypeDef",
+    "QueryInputTableQueryTypeDef",
+    "ScanInputRequestTypeDef",
+    "ScanInputScanPaginateTypeDef",
+    "ScanInputTableScanTypeDef",
+    "DeleteItemInputRequestTypeDef",
+    "DeleteItemInputTableDeleteItemTypeDef",
+    "PutItemInputRequestTypeDef",
+    "PutItemInputTablePutItemTypeDef",
+    "UpdateItemInputRequestTypeDef",
+    "UpdateItemInputTableUpdateItemTypeDef",
+    "TransactGetItemTypeDef",
+    "KeysAndAttributesUnionTypeDef",
+    "ExecuteTransactionInputRequestTypeDef",
+    "WriteRequestTypeDef",
+    "TransactWriteItemTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
+    "BatchWriteItemOutputTypeDef",
     "ImportTableInputRequestTypeDef",
     "GlobalTableDescriptionTypeDef",
     "TableDescriptionTypeDef",
     "ReplicationGroupUpdateTypeDef",
+    "CreateTableInputRequestTypeDef",
+    "CreateTableInputServiceResourceCreateTableTypeDef",
+    "RestoreTableFromBackupInputRequestTypeDef",
+    "RestoreTableToPointInTimeInputRequestTypeDef",
     "ImportTableDescriptionTypeDef",
+    "TableCreationParametersUnionTypeDef",
     "BackupDescriptionTypeDef",
+    "TransactGetItemsInputRequestTypeDef",
+    "BatchGetItemInputRequestTypeDef",
+    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    "WriteRequestUnionTypeDef",
+    "TransactWriteItemsInputRequestTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
@@ -291,14 +298,16 @@
     "UpdateTableOutputTypeDef",
     "UpdateTableInputRequestTypeDef",
     "UpdateTableInputTableUpdateTypeDef",
     "DescribeImportOutputTypeDef",
     "ImportTableOutputTypeDef",
     "DeleteBackupOutputTypeDef",
     "DescribeBackupOutputTypeDef",
+    "BatchWriteItemInputRequestTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
@@ -435,14 +444,30 @@
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
     total=False,
 )
 
+TableAttributeValueTypeDef = Union[
+    bytes,
+    bytearray,
+    str,
+    int,
+    Decimal,
+    bool,
+    Set[int],
+    Set[Decimal],
+    Set[str],
+    Set[bytes],
+    Set[bytearray],
+    Sequence[Any],
+    Mapping[str, Any],
+    None,
+]
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
     total=False,
@@ -454,14 +479,15 @@
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
     total=False,
 )
 
+ConditionBaseImportTypeDef = Union[str, ConditionBase]
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
@@ -794,86 +820,15 @@
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
     total=False,
 )
 
-_RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_RequiredExportTableToPointInTimeInputRequestTypeDef",
-    {
-        "TableArn": str,
-        "S3Bucket": str,
-    },
-)
-_OptionalExportTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_OptionalExportTableToPointInTimeInputRequestTypeDef",
-    {
-        "ExportTime": Union[datetime, str],
-        "ClientToken": str,
-        "S3BucketOwner": str,
-        "S3Prefix": str,
-        "S3SseAlgorithm": S3SseAlgorithmType,
-        "S3SseKmsKeyId": str,
-        "ExportFormat": ExportFormatType,
-    },
-    total=False,
-)
-
-
-class ExportTableToPointInTimeInputRequestTypeDef(
-    _RequiredExportTableToPointInTimeInputRequestTypeDef,
-    _OptionalExportTableToPointInTimeInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredGetItemInputTableGetItemTypeDef = TypedDict(
-    "_RequiredGetItemInputTableGetItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalGetItemInputTableGetItemTypeDef = TypedDict(
-    "_OptionalGetItemInputTableGetItemTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class GetItemInputTableGetItemTypeDef(
-    _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ProjectionOutputTypeDef = TypedDict(
     "ProjectionOutputTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": List[str],
     },
     total=False,
@@ -925,27 +880,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListBackupsInputRequestTypeDef = TypedDict(
-    "ListBackupsInputRequestTypeDef",
-    {
-        "TableName": str,
-        "Limit": int,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "ExclusiveStartBackupArn": str,
-        "BackupType": BackupTypeFilterType,
-    },
-    total=False,
-)
-
 ListContributorInsightsInputRequestTypeDef = TypedDict(
     "ListContributorInsightsInputRequestTypeDef",
     {
         "TableName": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1221,477 +1163,145 @@
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttributeValueUpdateTypeDef = TypedDict(
-    "AttributeValueUpdateTypeDef",
-    {
-        "Value": Union[
-            AttributeValueTypeDef,
-            bytes,
-            bytearray,
-            str,
-            int,
-            Decimal,
-            bool,
-            Set[int],
-            Set[Decimal],
-            Set[str],
-            Set[bytes],
-            Set[bytearray],
-            Sequence[Any],
-            Mapping[str, Any],
-            None,
-        ],
-        "Action": AttributeActionType,
-    },
-    total=False,
-)
-
-BatchStatementErrorTypeDef = TypedDict(
-    "BatchStatementErrorTypeDef",
+UniversalAttributeValueTypeDef = Union[
+    AttributeValueTypeDef,
+    bytes,
+    bytearray,
+    str,
+    int,
+    Decimal,
+    bool,
+    Set[int],
+    Set[Decimal],
+    Set[str],
+    Set[bytes],
+    Set[bytearray],
+    Sequence[Any],
+    Mapping[str, Any],
+    None,
+]
+AutoScalingPolicyDescriptionTypeDef = TypedDict(
+    "AutoScalingPolicyDescriptionTypeDef",
     {
-        "Code": BatchStatementErrorCodeEnumType,
-        "Message": str,
-        "Item": Dict[str, AttributeValueTypeDef],
+        "PolicyName": str,
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
+        ),
     },
     total=False,
 )
 
-_RequiredBatchStatementRequestTypeDef = TypedDict(
-    "_RequiredBatchStatementRequestTypeDef",
+_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_RequiredAutoScalingPolicyUpdateTypeDef",
     {
-        "Statement": str,
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
+        ),
     },
 )
-_OptionalBatchStatementRequestTypeDef = TypedDict(
-    "_OptionalBatchStatementRequestTypeDef",
+_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_OptionalAutoScalingPolicyUpdateTypeDef",
     {
-        "Parameters": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
-        "ConsistentRead": bool,
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
+        "PolicyName": str,
     },
     total=False,
 )
 
 
-class BatchStatementRequestTypeDef(
-    _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
+class AutoScalingPolicyUpdateTypeDef(
+    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
 ):
     pass
 
 
-_RequiredConditionCheckTypeDef = TypedDict(
-    "_RequiredConditionCheckTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "TableName": str,
-        "ConditionExpression": str,
-    },
-)
-_OptionalConditionCheckTypeDef = TypedDict(
-    "_OptionalConditionCheckTypeDef",
+CreateBackupOutputTypeDef = TypedDict(
+    "CreateBackupOutputTypeDef",
     {
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
+        "BackupDetails": BackupDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
-    pass
-
-
-_RequiredConditionTypeDef = TypedDict(
-    "_RequiredConditionTypeDef",
+ListBackupsOutputTypeDef = TypedDict(
+    "ListBackupsOutputTypeDef",
     {
-        "ComparisonOperator": ComparisonOperatorType,
+        "BackupSummaries": List[BackupSummaryTypeDef],
+        "LastEvaluatedBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalConditionTypeDef = TypedDict(
-    "_OptionalConditionTypeDef",
+
+BatchStatementErrorTypeDef = TypedDict(
+    "BatchStatementErrorTypeDef",
     {
-        "AttributeValueList": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
+        "Code": BatchStatementErrorCodeEnumType,
+        "Message": str,
+        "Item": Dict[str, TableAttributeValueTypeDef],
     },
     total=False,
 )
 
-
-class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
-    pass
-
-
 DeleteRequestOutputTypeDef = TypedDict(
     "DeleteRequestOutputTypeDef",
     {
-        "Key": Dict[str, AttributeValueTypeDef],
-    },
-)
-
-DeleteRequestTypeDef = TypedDict(
-    "DeleteRequestTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-
-_RequiredDeleteTypeDef = TypedDict(
-    "_RequiredDeleteTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "TableName": str,
-    },
-)
-_OptionalDeleteTypeDef = TypedDict(
-    "_OptionalDeleteTypeDef",
-    {
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
-    pass
-
-
-_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
-    "_RequiredExecuteStatementInputRequestTypeDef",
-    {
-        "Statement": str,
-    },
-)
-_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
-    "_OptionalExecuteStatementInputRequestTypeDef",
-    {
-        "Parameters": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
-        "ConsistentRead": bool,
-        "NextToken": str,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "Limit": int,
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class ExecuteStatementInputRequestTypeDef(
-    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
-):
-    pass
-
-
-ExpectedAttributeValueTypeDef = TypedDict(
-    "ExpectedAttributeValueTypeDef",
-    {
-        "Value": Union[
-            AttributeValueTypeDef,
-            bytes,
-            bytearray,
-            str,
-            int,
-            Decimal,
-            bool,
-            Set[int],
-            Set[Decimal],
-            Set[str],
-            Set[bytes],
-            Set[bytearray],
-            Sequence[Any],
-            Mapping[str, Any],
-            None,
-        ],
-        "Exists": bool,
-        "ComparisonOperator": ComparisonOperatorType,
-        "AttributeValueList": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
+        "Key": Dict[str, TableAttributeValueTypeDef],
     },
-    total=False,
 )
 
-_RequiredGetItemInputRequestTypeDef = TypedDict(
-    "_RequiredGetItemInputRequestTypeDef",
+_RequiredGetItemInputTableGetItemTypeDef = TypedDict(
+    "_RequiredGetItemInputTableGetItemTypeDef",
     {
-        "TableName": str,
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalGetItemInputRequestTypeDef = TypedDict(
-    "_OptionalGetItemInputRequestTypeDef",
+_OptionalGetItemInputTableGetItemTypeDef = TypedDict(
+    "_OptionalGetItemInputTableGetItemTypeDef",
     {
         "AttributesToGet": Sequence[str],
         "ConsistentRead": bool,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
 
-class GetItemInputRequestTypeDef(
-    _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
+class GetItemInputTableGetItemTypeDef(
+    _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
 
-_RequiredGetTypeDef = TypedDict(
-    "_RequiredGetTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "TableName": str,
-    },
-)
-_OptionalGetTypeDef = TypedDict(
-    "_OptionalGetTypeDef",
-    {
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
-    pass
-
-
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
-        "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
+        "ItemCollectionKey": Dict[str, TableAttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
     total=False,
 )
 
 ItemResponseTypeDef = TypedDict(
     "ItemResponseTypeDef",
     {
-        "Item": Dict[str, AttributeValueTypeDef],
+        "Item": Dict[str, TableAttributeValueTypeDef],
     },
     total=False,
 )
 
 _RequiredKeysAndAttributesOutputTypeDef = TypedDict(
     "_RequiredKeysAndAttributesOutputTypeDef",
     {
-        "Keys": List[Dict[str, AttributeValueTypeDef]],
+        "Keys": List[Dict[str, TableAttributeValueTypeDef]],
     },
 )
 _OptionalKeysAndAttributesOutputTypeDef = TypedDict(
     "_OptionalKeysAndAttributesOutputTypeDef",
     {
         "AttributesToGet": List[str],
         "ConsistentRead": bool,
@@ -1704,303 +1314,18 @@
 
 class KeysAndAttributesOutputTypeDef(
     _RequiredKeysAndAttributesOutputTypeDef, _OptionalKeysAndAttributesOutputTypeDef
 ):
     pass
 
 
-_RequiredKeysAndAttributesTypeDef = TypedDict(
-    "_RequiredKeysAndAttributesTypeDef",
-    {
-        "Keys": Sequence[
-            Mapping[
-                str,
-                Union[
-                    AttributeValueTypeDef,
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
-    },
-)
-_OptionalKeysAndAttributesTypeDef = TypedDict(
-    "_OptionalKeysAndAttributesTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class KeysAndAttributesTypeDef(
-    _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
-):
-    pass
-
-
-_RequiredParameterizedStatementTypeDef = TypedDict(
-    "_RequiredParameterizedStatementTypeDef",
-    {
-        "Statement": str,
-    },
-)
-_OptionalParameterizedStatementTypeDef = TypedDict(
-    "_OptionalParameterizedStatementTypeDef",
-    {
-        "Parameters": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class ParameterizedStatementTypeDef(
-    _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
-):
-    pass
-
-
 PutRequestOutputTypeDef = TypedDict(
     "PutRequestOutputTypeDef",
     {
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-)
-
-PutRequestTypeDef = TypedDict(
-    "PutRequestTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-
-_RequiredPutTypeDef = TypedDict(
-    "_RequiredPutTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "TableName": str,
-    },
-)
-_OptionalPutTypeDef = TypedDict(
-    "_OptionalPutTypeDef",
-    {
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
-    pass
-
-
-_RequiredUpdateTypeDef = TypedDict(
-    "_RequiredUpdateTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "UpdateExpression": str,
-        "TableName": str,
-    },
-)
-_OptionalUpdateTypeDef = TypedDict(
-    "_OptionalUpdateTypeDef",
-    {
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
-    pass
-
-
-AutoScalingPolicyDescriptionTypeDef = TypedDict(
-    "AutoScalingPolicyDescriptionTypeDef",
-    {
-        "PolicyName": str,
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
-        ),
-    },
-    total=False,
-)
-
-_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_RequiredAutoScalingPolicyUpdateTypeDef",
-    {
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
-        ),
-    },
-)
-_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_OptionalAutoScalingPolicyUpdateTypeDef",
-    {
-        "PolicyName": str,
-    },
-    total=False,
-)
-
-
-class AutoScalingPolicyUpdateTypeDef(
-    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
-):
-    pass
-
-
-CreateBackupOutputTypeDef = TypedDict(
-    "CreateBackupOutputTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupsOutputTypeDef = TypedDict(
-    "ListBackupsOutputTypeDef",
-    {
-        "BackupSummaries": List[BackupSummaryTypeDef],
-        "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": Dict[str, TableAttributeValueTypeDef],
     },
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
@@ -2328,14 +1653,56 @@
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_RequiredExportTableToPointInTimeInputRequestTypeDef",
+    {
+        "TableArn": str,
+        "S3Bucket": str,
+    },
+)
+_OptionalExportTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_OptionalExportTableToPointInTimeInputRequestTypeDef",
+    {
+        "ExportTime": TimestampTypeDef,
+        "ClientToken": str,
+        "S3BucketOwner": str,
+        "S3Prefix": str,
+        "S3SseAlgorithm": S3SseAlgorithmType,
+        "S3SseKmsKeyId": str,
+        "ExportFormat": ExportFormatType,
+    },
+    total=False,
+)
+
+
+class ExportTableToPointInTimeInputRequestTypeDef(
+    _RequiredExportTableToPointInTimeInputRequestTypeDef,
+    _OptionalExportTableToPointInTimeInputRequestTypeDef,
+):
+    pass
+
+
+ListBackupsInputRequestTypeDef = TypedDict(
+    "ListBackupsInputRequestTypeDef",
+    {
+        "TableName": str,
+        "Limit": int,
+        "TimeRangeLowerBound": TimestampTypeDef,
+        "TimeRangeUpperBound": TimestampTypeDef,
+        "ExclusiveStartBackupArn": str,
+        "BackupType": BackupTypeFilterType,
+    },
+    total=False,
+)
+
 GlobalSecondaryIndexInfoTypeDef = TypedDict(
     "GlobalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
@@ -2420,16 +1787,16 @@
     total=False,
 )
 
 ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
     "ListBackupsInputListBackupsPaginateTypeDef",
     {
         "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
+        "TimeRangeLowerBound": TimestampTypeDef,
+        "TimeRangeUpperBound": TimestampTypeDef,
         "BackupType": BackupTypeFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTablesInputListTablesPaginateTypeDef = TypedDict(
@@ -2482,921 +1849,302 @@
     "UpdateTimeToLiveOutputTypeDef",
     {
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchStatementResponseTypeDef = TypedDict(
-    "BatchStatementResponseTypeDef",
+AttributeValueUpdateTypeDef = TypedDict(
+    "AttributeValueUpdateTypeDef",
     {
-        "Error": BatchStatementErrorTypeDef,
-        "TableName": str,
-        "Item": Dict[str, AttributeValueTypeDef],
+        "Value": UniversalAttributeValueTypeDef,
+        "Action": AttributeActionType,
     },
     total=False,
 )
 
-_RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
-    "_RequiredBatchExecuteStatementInputRequestTypeDef",
+_RequiredBatchStatementRequestTypeDef = TypedDict(
+    "_RequiredBatchStatementRequestTypeDef",
     {
-        "Statements": Sequence[BatchStatementRequestTypeDef],
+        "Statement": str,
     },
 )
-_OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
-    "_OptionalBatchExecuteStatementInputRequestTypeDef",
+_OptionalBatchStatementRequestTypeDef = TypedDict(
+    "_OptionalBatchStatementRequestTypeDef",
     {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "Parameters": Sequence[UniversalAttributeValueTypeDef],
+        "ConsistentRead": bool,
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class BatchExecuteStatementInputRequestTypeDef(
-    _RequiredBatchExecuteStatementInputRequestTypeDef,
-    _OptionalBatchExecuteStatementInputRequestTypeDef,
+class BatchStatementRequestTypeDef(
+    _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
     pass
 
 
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
+_RequiredConditionCheckTypeDef = TypedDict(
+    "_RequiredConditionCheckTypeDef",
     {
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "TableName": str,
+        "ConditionExpression": str,
     },
 )
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
+_OptionalConditionCheckTypeDef = TypedDict(
+    "_OptionalConditionCheckTypeDef",
     {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTypeDef],
-        "QueryFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
+class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
     pass
 
 
-_RequiredQueryInputRequestTypeDef = TypedDict(
-    "_RequiredQueryInputRequestTypeDef",
+_RequiredConditionTypeDef = TypedDict(
+    "_RequiredConditionTypeDef",
     {
-        "TableName": str,
+        "ComparisonOperator": ComparisonOperatorType,
     },
 )
-_OptionalQueryInputRequestTypeDef = TypedDict(
-    "_OptionalQueryInputRequestTypeDef",
+_OptionalConditionTypeDef = TypedDict(
+    "_OptionalConditionTypeDef",
     {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTypeDef],
-        "QueryFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
 
-class QueryInputRequestTypeDef(
-    _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
-):
+class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
     pass
 
 
-QueryInputTableQueryTypeDef = TypedDict(
-    "QueryInputTableQueryTypeDef",
+DeleteRequestTypeDef = TypedDict(
+    "DeleteRequestTypeDef",
     {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTypeDef],
-        "QueryFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": Union[str, ConditionBase],
-        "KeyConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
-    total=False,
 )
 
-_RequiredScanInputRequestTypeDef = TypedDict(
-    "_RequiredScanInputRequestTypeDef",
+_RequiredDeleteTypeDef = TypedDict(
+    "_RequiredDeleteTypeDef",
     {
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "TableName": str,
     },
 )
-_OptionalScanInputRequestTypeDef = TypedDict(
-    "_OptionalScanInputRequestTypeDef",
+_OptionalDeleteTypeDef = TypedDict(
+    "_OptionalDeleteTypeDef",
     {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
+        "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
+class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
 
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
+_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
+    "_RequiredExecuteStatementInputRequestTypeDef",
     {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Statement": str,
     },
-    total=False,
 )
-
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
-
-ScanInputTableScanTypeDef = TypedDict(
-    "ScanInputTableScanTypeDef",
+_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
+    "_OptionalExecuteStatementInputRequestTypeDef",
     {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
-    },
-    total=False,
-)
-
-_RequiredDeleteItemInputRequestTypeDef = TypedDict(
-    "_RequiredDeleteItemInputRequestTypeDef",
-    {
-        "TableName": str,
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalDeleteItemInputRequestTypeDef = TypedDict(
-    "_OptionalDeleteItemInputRequestTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
+        "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Limit": int,
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class DeleteItemInputRequestTypeDef(
-    _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
+class ExecuteStatementInputRequestTypeDef(
+    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
 
-_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
+ExpectedAttributeValueTypeDef = TypedDict(
+    "ExpectedAttributeValueTypeDef",
     {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
+        "Value": UniversalAttributeValueTypeDef,
+        "Exists": bool,
+        "ComparisonOperator": ComparisonOperatorType,
+        "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-
-class DeleteItemInputTableDeleteItemTypeDef(
-    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
-):
-    pass
-
-
-_RequiredPutItemInputRequestTypeDef = TypedDict(
-    "_RequiredPutItemInputRequestTypeDef",
+_RequiredGetItemInputRequestTypeDef = TypedDict(
+    "_RequiredGetItemInputRequestTypeDef",
     {
         "TableName": str,
-        "Item": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
-_OptionalPutItemInputRequestTypeDef = TypedDict(
-    "_OptionalPutItemInputRequestTypeDef",
+_OptionalGetItemInputRequestTypeDef = TypedDict(
+    "_OptionalGetItemInputRequestTypeDef",
     {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ReturnValues": ReturnValueType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionalOperator": ConditionalOperatorType,
-        "ConditionExpression": str,
+        "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class PutItemInputRequestTypeDef(
-    _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
+class GetItemInputRequestTypeDef(
+    _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
 ):
     pass
 
 
-_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
-    "_RequiredPutItemInputTablePutItemTypeDef",
+_RequiredGetTypeDef = TypedDict(
+    "_RequiredGetTypeDef",
     {
-        "Item": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
+        "TableName": str,
     },
 )
-_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
-    "_OptionalPutItemInputTablePutItemTypeDef",
+_OptionalGetTypeDef = TypedDict(
+    "_OptionalGetTypeDef",
     {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionalOperator": ConditionalOperatorType,
-        "ConditionExpression": Union[str, ConditionBase],
+        "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class PutItemInputTablePutItemTypeDef(
-    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
-):
+class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
     pass
 
 
-_RequiredUpdateItemInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateItemInputRequestTypeDef",
+_RequiredKeysAndAttributesTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesTypeDef",
     {
-        "TableName": str,
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Keys": Sequence[Mapping[str, UniversalAttributeValueTypeDef]],
     },
 )
-_OptionalUpdateItemInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateItemInputRequestTypeDef",
+_OptionalKeysAndAttributesTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesTypeDef",
     {
-        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "UpdateExpression": str,
-        "ConditionExpression": str,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class UpdateItemInputRequestTypeDef(
-    _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
+class KeysAndAttributesTypeDef(
+    _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
 ):
     pass
 
 
-_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
+_RequiredParameterizedStatementTypeDef = TypedDict(
+    "_RequiredParameterizedStatementTypeDef",
     {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Statement": str,
     },
 )
-_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
+_OptionalParameterizedStatementTypeDef = TypedDict(
+    "_OptionalParameterizedStatementTypeDef",
     {
-        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "UpdateExpression": str,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class UpdateItemInputTableUpdateItemTypeDef(
-    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+class ParameterizedStatementTypeDef(
+    _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
     pass
 
 
-TransactGetItemTypeDef = TypedDict(
-    "TransactGetItemTypeDef",
-    {
-        "Get": GetTypeDef,
-    },
-)
-
-_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputRequestTypeDef",
-    {
-        "RequestItems": Mapping[
-            str, Union[KeysAndAttributesTypeDef, KeysAndAttributesOutputTypeDef]
-        ],
-    },
-)
-_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputRequestTypeDef",
+PutRequestTypeDef = TypedDict(
+    "PutRequestTypeDef",
     {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
-    total=False,
 )
 
-
-class BatchGetItemInputRequestTypeDef(
-    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
-):
-    pass
-
-
-_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+_RequiredPutTypeDef = TypedDict(
+    "_RequiredPutTypeDef",
     {
-        "RequestItems": Mapping[
-            str, Union[KeysAndAttributesTypeDef, KeysAndAttributesOutputTypeDef]
-        ],
+        "Item": Mapping[str, UniversalAttributeValueTypeDef],
+        "TableName": str,
     },
 )
-_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+_OptionalPutTypeDef = TypedDict(
+    "_OptionalPutTypeDef",
     {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
-    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-):
+class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
     pass
 
 
-_RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
-    "_RequiredExecuteTransactionInputRequestTypeDef",
+_RequiredUpdateTypeDef = TypedDict(
+    "_RequiredUpdateTypeDef",
     {
-        "TransactStatements": Sequence[ParameterizedStatementTypeDef],
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
+        "UpdateExpression": str,
+        "TableName": str,
     },
 )
-_OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
-    "_OptionalExecuteTransactionInputRequestTypeDef",
+_OptionalUpdateTypeDef = TypedDict(
+    "_OptionalUpdateTypeDef",
     {
-        "ClientRequestToken": str,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class ExecuteTransactionInputRequestTypeDef(
-    _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
-):
+class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
     pass
 
 
-WriteRequestOutputTypeDef = TypedDict(
-    "WriteRequestOutputTypeDef",
-    {
-        "PutRequest": PutRequestOutputTypeDef,
-        "DeleteRequest": DeleteRequestOutputTypeDef,
-    },
-    total=False,
-)
-
-WriteRequestTypeDef = TypedDict(
-    "WriteRequestTypeDef",
-    {
-        "PutRequest": PutRequestTypeDef,
-        "DeleteRequest": DeleteRequestTypeDef,
-    },
-    total=False,
-)
-
-TransactWriteItemTypeDef = TypedDict(
-    "TransactWriteItemTypeDef",
-    {
-        "ConditionCheck": ConditionCheckTypeDef,
-        "Put": PutTypeDef,
-        "Delete": DeleteTypeDef,
-        "Update": UpdateTypeDef,
-    },
-    total=False,
-)
-
 AutoScalingSettingsDescriptionTypeDef = TypedDict(
     "AutoScalingSettingsDescriptionTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
@@ -3413,41 +2161,60 @@
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
+BatchStatementResponseTypeDef = TypedDict(
+    "BatchStatementResponseTypeDef",
+    {
+        "Error": BatchStatementErrorTypeDef,
+        "TableName": str,
+        "Item": Dict[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+WriteRequestOutputTypeDef = TypedDict(
+    "WriteRequestOutputTypeDef",
+    {
+        "PutRequest": PutRequestOutputTypeDef,
+        "DeleteRequest": DeleteRequestOutputTypeDef,
+    },
+    total=False,
+)
+
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
-        "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
+        "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
-        "Attributes": Dict[str, AttributeValueTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
-        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
@@ -3456,49 +2223,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
-        "Item": Dict[str, AttributeValueTypeDef],
+        "Item": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
-        "Attributes": Dict[str, AttributeValueTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
-        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
-        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
@@ -3517,15 +2284,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
-        "Attributes": Dict[str, AttributeValueTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
@@ -3651,309 +2418,509 @@
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
 
+InputFormatOptionsUnionTypeDef = Union[InputFormatOptionsTypeDef, InputFormatOptionsOutputTypeDef]
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
-_RequiredCreateTableInputRequestTypeDef = TypedDict(
-    "_RequiredCreateTableInputRequestTypeDef",
+GlobalSecondaryIndexUnionTypeDef = Union[
+    GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef
+]
+_RequiredTableCreationParametersOutputTypeDef = TypedDict(
+    "_RequiredTableCreationParametersOutputTypeDef",
     {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
     },
 )
-_OptionalCreateTableInputRequestTypeDef = TypedDict(
-    "_OptionalCreateTableInputRequestTypeDef",
+_OptionalTableCreationParametersOutputTypeDef = TypedDict(
+    "_OptionalTableCreationParametersOutputTypeDef",
     {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
-        "GlobalSecondaryIndexes": Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ],
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "StreamSpecification": StreamSpecificationTypeDef,
         "SSESpecification": SSESpecificationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
     },
     total=False,
 )
 
 
-class CreateTableInputRequestTypeDef(
-    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
+class TableCreationParametersOutputTypeDef(
+    _RequiredTableCreationParametersOutputTypeDef, _OptionalTableCreationParametersOutputTypeDef
 ):
     pass
 
 
-_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
+SourceTableFeatureDetailsTypeDef = TypedDict(
+    "SourceTableFeatureDetailsTypeDef",
     {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
+        "StreamDescription": StreamSpecificationTypeDef,
+        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
     },
+    total=False,
 )
-_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
     {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
-        "GlobalSecondaryIndexes": Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "ImportSummaryList": List[ImportSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
+    "_RequiredBatchExecuteStatementInputRequestTypeDef",
+    {
+        "Statements": Sequence[BatchStatementRequestTypeDef],
+    },
+)
+_OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
+    "_OptionalBatchExecuteStatementInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
 
-class CreateTableInputServiceResourceCreateTableTypeDef(
-    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
-    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
+class BatchExecuteStatementInputRequestTypeDef(
+    _RequiredBatchExecuteStatementInputRequestTypeDef,
+    _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
     {
-        "TargetTableName": str,
-        "BackupArn": str,
+        "TableName": str,
     },
 )
-_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
     {
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class RestoreTableFromBackupInputRequestTypeDef(
-    _RequiredRestoreTableFromBackupInputRequestTypeDef,
-    _OptionalRestoreTableFromBackupInputRequestTypeDef,
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
 ):
     pass
 
 
-_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
+_RequiredQueryInputRequestTypeDef = TypedDict(
+    "_RequiredQueryInputRequestTypeDef",
     {
-        "TargetTableName": str,
+        "TableName": str,
     },
 )
-_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
+_OptionalQueryInputRequestTypeDef = TypedDict(
+    "_OptionalQueryInputRequestTypeDef",
     {
-        "SourceTableArn": str,
-        "SourceTableName": str,
-        "UseLatestRestorableTime": bool,
-        "RestoreDateTime": Union[datetime, str],
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[
-            Union[GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef]
-        ],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ExclusiveStartKey": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
 
-class RestoreTableToPointInTimeInputRequestTypeDef(
-    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
-    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
+class QueryInputRequestTypeDef(
+    _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
 
-_RequiredTableCreationParametersOutputTypeDef = TypedDict(
-    "_RequiredTableCreationParametersOutputTypeDef",
+QueryInputTableQueryTypeDef = TypedDict(
+    "QueryInputTableQueryTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "KeyConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+_RequiredScanInputRequestTypeDef = TypedDict(
+    "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
-        "KeySchema": List[KeySchemaElementTypeDef],
     },
 )
-_OptionalTableCreationParametersOutputTypeDef = TypedDict(
-    "_OptionalTableCreationParametersOutputTypeDef",
+_OptionalScanInputRequestTypeDef = TypedDict(
+    "_OptionalScanInputRequestTypeDef",
     {
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ExclusiveStartKey": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ConsistentRead": bool,
     },
     total=False,
 )
 
 
-class TableCreationParametersOutputTypeDef(
-    _RequiredTableCreationParametersOutputTypeDef, _OptionalTableCreationParametersOutputTypeDef
-):
+class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
 
-SourceTableFeatureDetailsTypeDef = TypedDict(
-    "SourceTableFeatureDetailsTypeDef",
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
     {
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationTypeDef,
-        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+
+ScanInputTableScanTypeDef = TypedDict(
+    "ScanInputTableScanTypeDef",
     {
-        "ImportSummaryList": List[ImportSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
     },
+    total=False,
 )
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
+_RequiredDeleteItemInputRequestTypeDef = TypedDict(
+    "_RequiredDeleteItemInputRequestTypeDef",
     {
-        "Responses": List[BatchStatementResponseTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TableName": str,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
+    },
+)
+_OptionalDeleteItemInputRequestTypeDef = TypedDict(
+    "_OptionalDeleteItemInputRequestTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
+    total=False,
 )
 
-_RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
-    "_RequiredTransactGetItemsInputRequestTypeDef",
+
+class DeleteItemInputRequestTypeDef(
+    _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
+):
+    pass
+
+
+_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
     {
-        "TransactItems": Sequence[TransactGetItemTypeDef],
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalTransactGetItemsInputRequestTypeDef = TypedDict(
-    "_OptionalTransactGetItemsInputRequestTypeDef",
+_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
     {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class TransactGetItemsInputRequestTypeDef(
-    _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
+class DeleteItemInputTableDeleteItemTypeDef(
+    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
 ):
     pass
 
 
-BatchWriteItemOutputTypeDef = TypedDict(
-    "BatchWriteItemOutputTypeDef",
+_RequiredPutItemInputRequestTypeDef = TypedDict(
+    "_RequiredPutItemInputRequestTypeDef",
     {
-        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TableName": str,
+        "Item": Mapping[str, UniversalAttributeValueTypeDef],
+    },
+)
+_OptionalPutItemInputRequestTypeDef = TypedDict(
+    "_OptionalPutItemInputRequestTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionalOperator": ConditionalOperatorType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
+    total=False,
 )
 
-_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputRequestTypeDef",
+
+class PutItemInputRequestTypeDef(
+    _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
+):
+    pass
+
+
+_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
+    "_RequiredPutItemInputTablePutItemTypeDef",
     {
-        "RequestItems": Mapping[
-            str, Sequence[Union[WriteRequestTypeDef, WriteRequestOutputTypeDef]]
-        ],
+        "Item": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputRequestTypeDef",
+_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
+    "_OptionalPutItemInputTablePutItemTypeDef",
     {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionalOperator": ConditionalOperatorType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class BatchWriteItemInputRequestTypeDef(
-    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
+class PutItemInputTablePutItemTypeDef(
+    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
 ):
     pass
 
 
-_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+_RequiredUpdateItemInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateItemInputRequestTypeDef",
     {
-        "RequestItems": Mapping[
-            str, Sequence[Union[WriteRequestTypeDef, WriteRequestOutputTypeDef]]
-        ],
+        "TableName": str,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
-_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+_OptionalUpdateItemInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateItemInputRequestTypeDef",
     {
+        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "UpdateExpression": str,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
-    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+class UpdateItemInputRequestTypeDef(
+    _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
 
-_RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
-    "_RequiredTransactWriteItemsInputRequestTypeDef",
+_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
     {
-        "TransactItems": Sequence[TransactWriteItemTypeDef],
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
-    "_OptionalTransactWriteItemsInputRequestTypeDef",
+_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
     {
+        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "UpdateExpression": str,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
+    },
+    total=False,
+)
+
+
+class UpdateItemInputTableUpdateItemTypeDef(
+    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+):
+    pass
+
+
+TransactGetItemTypeDef = TypedDict(
+    "TransactGetItemTypeDef",
+    {
+        "Get": GetTypeDef,
+    },
+)
+
+KeysAndAttributesUnionTypeDef = Union[KeysAndAttributesTypeDef, KeysAndAttributesOutputTypeDef]
+_RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
+    "_RequiredExecuteTransactionInputRequestTypeDef",
+    {
+        "TransactStatements": Sequence[ParameterizedStatementTypeDef],
+    },
+)
+_OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
+    "_OptionalExecuteTransactionInputRequestTypeDef",
+    {
         "ClientRequestToken": str,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
 
-class TransactWriteItemsInputRequestTypeDef(
-    _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
+class ExecuteTransactionInputRequestTypeDef(
+    _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
 ):
     pass
 
 
+WriteRequestTypeDef = TypedDict(
+    "WriteRequestTypeDef",
+    {
+        "PutRequest": PutRequestTypeDef,
+        "DeleteRequest": DeleteRequestTypeDef,
+    },
+    total=False,
+)
+
+TransactWriteItemTypeDef = TypedDict(
+    "TransactWriteItemTypeDef",
+    {
+        "ConditionCheck": ConditionCheckTypeDef,
+        "Put": PutTypeDef,
+        "Delete": DeleteTypeDef,
+        "Update": UpdateTypeDef,
+    },
+    total=False,
+)
+
 ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
@@ -4047,14 +3014,33 @@
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
 
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
+    {
+        "Responses": List[BatchStatementResponseTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchWriteItemOutputTypeDef = TypedDict(
+    "BatchWriteItemOutputTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredImportTableInputRequestTypeDef = TypedDict(
     "_RequiredImportTableInputRequestTypeDef",
     {
         "S3BucketSource": S3BucketSourceTypeDef,
         "InputFormat": InputFormatType,
         "TableCreationParameters": TableCreationParametersTypeDef,
     },
@@ -4124,14 +3110,134 @@
         "Create": CreateReplicationGroupMemberActionTypeDef,
         "Update": UpdateReplicationGroupMemberActionTypeDef,
         "Delete": DeleteReplicationGroupMemberActionTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateTableInputRequestTypeDef = TypedDict(
+    "_RequiredCreateTableInputRequestTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputRequestTypeDef = TypedDict(
+    "_OptionalCreateTableInputRequestTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+
+class CreateTableInputRequestTypeDef(
+    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+
+class CreateTableInputServiceResourceCreateTableTypeDef(
+    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
+    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
+):
+    pass
+
+
+_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+        "BackupArn": str,
+    },
+)
+_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
+    },
+    total=False,
+)
+
+
+class RestoreTableFromBackupInputRequestTypeDef(
+    _RequiredRestoreTableFromBackupInputRequestTypeDef,
+    _OptionalRestoreTableFromBackupInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+    },
+)
+_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "SourceTableArn": str,
+        "SourceTableName": str,
+        "UseLatestRestorableTime": bool,
+        "RestoreDateTime": TimestampTypeDef,
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
+    },
+    total=False,
+)
+
+
+class RestoreTableToPointInTimeInputRequestTypeDef(
+    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
+    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
+):
+    pass
+
+
 ImportTableDescriptionTypeDef = TypedDict(
     "ImportTableDescriptionTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
         "TableId": str,
@@ -4150,24 +3256,115 @@
         "ImportedItemCount": int,
         "FailureCode": str,
         "FailureMessage": str,
     },
     total=False,
 )
 
+TableCreationParametersUnionTypeDef = Union[
+    TableCreationParametersTypeDef, TableCreationParametersOutputTypeDef
+]
 BackupDescriptionTypeDef = TypedDict(
     "BackupDescriptionTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
         "SourceTableDetails": SourceTableDetailsTypeDef,
         "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
+    "_RequiredTransactGetItemsInputRequestTypeDef",
+    {
+        "TransactItems": Sequence[TransactGetItemTypeDef],
+    },
+)
+_OptionalTransactGetItemsInputRequestTypeDef = TypedDict(
+    "_OptionalTransactGetItemsInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+
+class TransactGetItemsInputRequestTypeDef(
+    _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
+):
+    pass
+
+
+_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputRequestTypeDef",
+    {
+        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
+    },
+)
+_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+
+class BatchGetItemInputRequestTypeDef(
+    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
+):
+    pass
+
+
+_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
+    },
+)
+_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+
+class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
+    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+):
+    pass
+
+
+WriteRequestUnionTypeDef = Union[WriteRequestTypeDef, WriteRequestOutputTypeDef]
+_RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
+    "_RequiredTransactWriteItemsInputRequestTypeDef",
+    {
+        "TransactItems": Sequence[TransactWriteItemTypeDef],
+    },
+)
+_OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
+    "_OptionalTransactWriteItemsInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class TransactWriteItemsInputRequestTypeDef(
+    _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
+):
+    pass
+
+
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
@@ -4401,14 +3598,59 @@
     "DescribeBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputRequestTypeDef",
+    {
+        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
+    },
+)
+_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+    },
+    total=False,
+)
+
+
+class BatchWriteItemInputRequestTypeDef(
+    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
+):
+    pass
+
+
+_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
+    },
+)
+_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+    },
+    total=False,
+)
+
+
+class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
+    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+):
+    pass
+
+
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/waiter.py` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/waiter.pyi` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/PKG-INFO` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.28.15.post2
-Summary: Type annotations for boto3.DynamoDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DynamoDB 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 dynamodb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 dynamodb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
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
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -79,15 +79,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -472,33 +472,35 @@
 )
 
 
 def check_value(value: AttributeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
     ResponseMetadataTypeDef,
     ArchivalSummaryTypeDef,
     AttributeDefinitionTypeDef,
     AttributeValueTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTypeDef,
+    TableAttributeValueTypeDef,
     BillingModeSummaryTypeDef,
     CapacityTypeDef,
+    ConditionBaseImportTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
     ContributorInsightsSummaryTypeDef,
     CreateBackupInputRequestTypeDef,
     KeySchemaElementTypeDef,
     ProjectionTypeDef,
     ProvisionedThroughputTypeDef,
     ReplicaTypeDef,
@@ -528,22 +530,20 @@
     KinesisDataStreamDestinationTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
     ExportSummaryTypeDef,
-    ExportTableToPointInTimeInputRequestTypeDef,
-    GetItemInputTableGetItemTypeDef,
+    TimestampTypeDef,
     ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
     ListTablesInputRequestTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
@@ -562,39 +562,26 @@
     ListTablesOutputTypeDef,
     ProvisionedThroughputDescriptionResponseTypeDef,
     RestoreSummaryResponseTypeDef,
     SSEDescriptionResponseTypeDef,
     StreamSpecificationResponseTypeDef,
     TableClassSummaryResponseTypeDef,
     UpdateContributorInsightsOutputTypeDef,
-    AttributeValueUpdateTypeDef,
+    UniversalAttributeValueTypeDef,
+    AutoScalingPolicyDescriptionTypeDef,
+    AutoScalingPolicyUpdateTypeDef,
+    CreateBackupOutputTypeDef,
+    ListBackupsOutputTypeDef,
     BatchStatementErrorTypeDef,
-    BatchStatementRequestTypeDef,
-    ConditionCheckTypeDef,
-    ConditionTypeDef,
     DeleteRequestOutputTypeDef,
-    DeleteRequestTypeDef,
-    DeleteTypeDef,
-    ExecuteStatementInputRequestTypeDef,
-    ExpectedAttributeValueTypeDef,
-    GetItemInputRequestTypeDef,
-    GetTypeDef,
+    GetItemInputTableGetItemTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
     KeysAndAttributesOutputTypeDef,
-    KeysAndAttributesTypeDef,
-    ParameterizedStatementTypeDef,
     PutRequestOutputTypeDef,
-    PutRequestTypeDef,
-    PutTypeDef,
-    UpdateTypeDef,
-    AutoScalingPolicyDescriptionTypeDef,
-    AutoScalingPolicyUpdateTypeDef,
-    CreateBackupOutputTypeDef,
-    ListBackupsOutputTypeDef,
     ConsumedCapacityTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
     GlobalSecondaryIndexTypeDef,
     SourceTableDetailsTypeDef,
@@ -613,49 +600,47 @@
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
+    ExportTableToPointInTimeInputRequestTypeDef,
+    ListBackupsInputRequestTypeDef,
     GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexOutputTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
     ImportSummaryTypeDef,
     ListBackupsInputListBackupsPaginateTypeDef,
     ListTablesInputListTablesPaginateTypeDef,
     ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
-    BatchStatementResponseTypeDef,
-    BatchExecuteStatementInputRequestTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    QueryInputRequestTypeDef,
-    QueryInputTableQueryTypeDef,
-    ScanInputRequestTypeDef,
-    ScanInputScanPaginateTypeDef,
-    ScanInputTableScanTypeDef,
-    DeleteItemInputRequestTypeDef,
-    DeleteItemInputTableDeleteItemTypeDef,
-    PutItemInputRequestTypeDef,
-    PutItemInputTablePutItemTypeDef,
-    UpdateItemInputRequestTypeDef,
-    UpdateItemInputTableUpdateItemTypeDef,
-    TransactGetItemTypeDef,
-    BatchGetItemInputRequestTypeDef,
-    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    ExecuteTransactionInputRequestTypeDef,
-    WriteRequestOutputTypeDef,
-    WriteRequestTypeDef,
-    TransactWriteItemTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchStatementRequestTypeDef,
+    ConditionCheckTypeDef,
+    ConditionTypeDef,
+    DeleteRequestTypeDef,
+    DeleteTypeDef,
+    ExecuteStatementInputRequestTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemInputRequestTypeDef,
+    GetTypeDef,
+    KeysAndAttributesTypeDef,
+    ParameterizedStatementTypeDef,
+    PutRequestTypeDef,
+    PutTypeDef,
+    UpdateTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
+    BatchStatementResponseTypeDef,
+    WriteRequestOutputTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
@@ -667,40 +652,62 @@
     UpdateContinuousBackupsOutputTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     ListGlobalTablesOutputTypeDef,
     ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
+    InputFormatOptionsUnionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
-    CreateTableInputRequestTypeDef,
-    CreateTableInputServiceResourceCreateTableTypeDef,
-    RestoreTableFromBackupInputRequestTypeDef,
-    RestoreTableToPointInTimeInputRequestTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     TableCreationParametersOutputTypeDef,
     SourceTableFeatureDetailsTypeDef,
     ListImportsOutputTypeDef,
-    BatchExecuteStatementOutputTypeDef,
-    TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemOutputTypeDef,
-    BatchWriteItemInputRequestTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    TransactWriteItemsInputRequestTypeDef,
+    BatchExecuteStatementInputRequestTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    QueryInputRequestTypeDef,
+    QueryInputTableQueryTypeDef,
+    ScanInputRequestTypeDef,
+    ScanInputScanPaginateTypeDef,
+    ScanInputTableScanTypeDef,
+    DeleteItemInputRequestTypeDef,
+    DeleteItemInputTableDeleteItemTypeDef,
+    PutItemInputRequestTypeDef,
+    PutItemInputTablePutItemTypeDef,
+    UpdateItemInputRequestTypeDef,
+    UpdateItemInputTableUpdateItemTypeDef,
+    TransactGetItemTypeDef,
+    KeysAndAttributesUnionTypeDef,
+    ExecuteTransactionInputRequestTypeDef,
+    WriteRequestTypeDef,
+    TransactWriteItemTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
+    BatchExecuteStatementOutputTypeDef,
+    BatchWriteItemOutputTypeDef,
     ImportTableInputRequestTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
     ReplicationGroupUpdateTypeDef,
+    CreateTableInputRequestTypeDef,
+    CreateTableInputServiceResourceCreateTableTypeDef,
+    RestoreTableFromBackupInputRequestTypeDef,
+    RestoreTableToPointInTimeInputRequestTypeDef,
     ImportTableDescriptionTypeDef,
+    TableCreationParametersUnionTypeDef,
     BackupDescriptionTypeDef,
+    TransactGetItemsInputRequestTypeDef,
+    BatchGetItemInputRequestTypeDef,
+    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    WriteRequestUnionTypeDef,
+    TransactWriteItemsInputRequestTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
@@ -712,25 +719,27 @@
     UpdateTableOutputTypeDef,
     UpdateTableInputRequestTypeDef,
     UpdateTableInputTableUpdateTypeDef,
     DescribeImportOutputTypeDef,
     ImportTableOutputTypeDef,
     DeleteBackupOutputTypeDef,
     DescribeBackupOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post2/setup.py` & `mypy-boto3-dynamodb-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.28.15.post2",
+    version="1.28.16",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DynamoDB 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.DynamoDB 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 dynamodb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 dynamodb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_dynamodb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

