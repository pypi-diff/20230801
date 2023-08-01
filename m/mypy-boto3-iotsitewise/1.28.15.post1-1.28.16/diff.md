# Comparing `tmp/mypy-boto3-iotsitewise-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iotsitewise-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotsitewise-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:23 2023, max compression
+gzip compressed data, was "mypy-boto3-iotsitewise-1.28.16.tar", last modified: Tue Aug  1 11:37:02 2023, max compression
```

## Comparing `mypy-boto3-iotsitewise-1.28.15.post1.tar` & `mypy-boto3-iotsitewise-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.305196 mypy-boto3-iotsitewise-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28625 2023-07-29 10:03:23.305196 mypy-boto3-iotsitewise-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27116 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.285196 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62842 2023-07-29 09:48:07.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    62739 2023-07-29 09:48:07.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-29 09:48:08.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-29 09:48:08.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-07-29 09:48:07.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21879 2023-07-29 09:48:07.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   108938 2023-07-29 09:48:11.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   108730 2023-07-29 09:48:09.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-29 09:48:08.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-29 09:48:08.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.285196 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28625 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:23.305196 mypy-boto3-iotsitewise-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:48:04.000000 mypy-boto3-iotsitewise-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:02.964859 mypy-boto3-iotsitewise-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:50.000000 mypy-boto3-iotsitewise-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28766 2023-08-01 11:37:02.964859 mypy-boto3-iotsitewise-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27266 2023-08-01 11:20:50.000000 mypy-boto3-iotsitewise-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:02.956859 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-08-01 11:20:50.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-08-01 11:20:50.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 11:20:50.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62558 2023-08-01 11:20:51.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62455 2023-08-01 11:20:51.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-08-01 11:20:52.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-08-01 11:20:52.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-08-01 11:20:51.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-08-01 11:20:51.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:50.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   109310 2023-08-01 11:20:57.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109102 2023-08-01 11:20:53.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:50.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-08-01 11:20:51.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-08-01 11:20:51.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:02.964859 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28766 2023-08-01 11:37:02.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-01 11:37:02.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:02.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:02.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:02.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:37:02.000000 mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:02.964859 mypy-boto3-iotsitewise-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 11:20:50.000000 mypy-boto3-iotsitewise-1.28.16/setup.py
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/LICENSE` & `mypy-boto3-iotsitewise-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/PKG-INFO` & `mypy-boto3-iotsitewise-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsitewise
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTSiteWise 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotsitewise type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotsitewise type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsitewise)](https://pepy.tech/project/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
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
@@ -461,20 +461,20 @@
 )
 
 
 def check_value(value: AggregateTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotsitewise.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotsitewise.type_defs import (
     AggregatesTypeDef,
     AlarmsTypeDef,
     AssetErrorDetailsTypeDef,
     AssetHierarchyInfoTypeDef,
@@ -486,29 +486,28 @@
     VariantTypeDef,
     AssociateAssetsRequestRequestTypeDef,
     AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
     AttributeTypeDef,
     BatchAssociateProjectAssetsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDisassociateProjectAssetsRequestRequestTypeDef,
-    BatchGetAssetPropertyAggregatesEntryTypeDef,
+    TimestampTypeDef,
     BatchGetAssetPropertyAggregatesErrorEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueErrorEntryTypeDef,
     BatchGetAssetPropertyValueErrorInfoTypeDef,
-    BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorInfoTypeDef,
+    BlobTypeDef,
     ConfigurationErrorDetailsTypeDef,
     CreateAssetRequestRequestTypeDef,
     ErrorReportLocationTypeDef,
     FileTypeDef,
     CreateDashboardRequestRequestTypeDef,
-    ImageFileTypeDef,
     CreateProjectRequestRequestTypeDef,
     CsvOutputTypeDef,
     CsvTypeDef,
     CustomerManagedS3StorageTypeDef,
     DashboardSummaryTypeDef,
     DeleteAccessPolicyRequestRequestTypeDef,
     DeleteAssetModelRequestRequestTypeDef,
@@ -538,16 +537,14 @@
     DisassociateAssetsRequestRequestTypeDef,
     DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     VariableValueTypeDef,
     ForwardingConfigTypeDef,
     GreengrassTypeDef,
     GreengrassV2TypeDef,
     PaginatorConfigTypeDef,
-    GetAssetPropertyAggregatesRequestRequestTypeDef,
-    GetAssetPropertyValueHistoryRequestRequestTypeDef,
     GetAssetPropertyValueRequestRequestTypeDef,
     GetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
     GroupIdentityTypeDef,
     IAMRoleIdentityTypeDef,
     IAMUserIdentityTypeDef,
     UserIdentityTypeDef,
     JobSummaryTypeDef,
@@ -600,23 +597,24 @@
     DescribeGatewayCapabilityConfigurationResponseTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeTimeSeriesResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListProjectAssetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateGatewayCapabilityConfigurationResponseTypeDef,
-    BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+    BatchGetAssetPropertyAggregatesEntryTypeDef,
+    BatchGetAssetPropertyValueHistoryEntryTypeDef,
+    GetAssetPropertyAggregatesRequestRequestTypeDef,
+    GetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     BatchGetAssetPropertyValueRequestRequestTypeDef,
     BatchGetAssetPropertyValueSkippedEntryTypeDef,
-    BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
+    ImageFileTypeDef,
     ConfigurationStatusTypeDef,
-    CreatePortalRequestRequestTypeDef,
-    ImageTypeDef,
     FileFormatOutputTypeDef,
     FileFormatTypeDef,
     MultiLayerStorageTypeDef,
     ListDashboardsResponseTypeDef,
     DescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     DescribeAssetRequestAssetActiveWaitTypeDef,
@@ -662,17 +660,20 @@
     BatchPutAssetPropertyErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistorySuccessEntryTypeDef,
     BatchGetAssetPropertyValueSuccessEntryTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
+    BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+    BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
+    CreatePortalRequestRequestTypeDef,
+    ImageTypeDef,
     DescribeDefaultEncryptionConfigurationResponseTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
-    UpdatePortalRequestRequestTypeDef,
     JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     DescribeStorageConfigurationResponseTypeDef,
     PutStorageConfigurationRequestRequestTypeDef,
     PutStorageConfigurationResponseTypeDef,
     AssetModelStatusTypeDef,
     AssetStatusTypeDef,
@@ -694,16 +695,18 @@
     DescribeAccessPolicyResponseTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchPutAssetPropertyValueResponseTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
     BatchGetAssetPropertyValueResponseTypeDef,
     BatchPutAssetPropertyValueRequestRequestTypeDef,
+    UpdatePortalRequestRequestTypeDef,
     DescribeBulkImportJobResponseTypeDef,
     CreateBulkImportJobRequestRequestTypeDef,
+    JobConfigurationUnionTypeDef,
     AssetModelSummaryTypeDef,
     CreateAssetModelResponseTypeDef,
     DeleteAssetModelResponseTypeDef,
     UpdateAssetModelResponseTypeDef,
     AssetSummaryTypeDef,
     AssociatedAssetsSummaryTypeDef,
     CreateAssetResponseTypeDef,
@@ -724,22 +727,24 @@
     AssetModelPropertyDefinitionTypeDef,
     AssetModelPropertyTypeDef,
     AssetModelCompositeModelOutputTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
     CompositeModelPropertyTypeDef,
     AssetModelCompositeModelDefinitionTypeDef,
     AssetModelCompositeModelTypeDef,
+    AssetModelPropertyUnionTypeDef,
     DescribeAssetModelResponseTypeDef,
     DescribeAssetPropertyResponseTypeDef,
     CreateAssetModelRequestRequestTypeDef,
+    AssetModelCompositeModelUnionTypeDef,
     UpdateAssetModelRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregatesTypeDef:
+def get_value() -> AggregatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/README.md` & `mypy-boto3-iotsitewise-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsitewise)](https://pepy.tech/project/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
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
@@ -429,20 +429,20 @@
 )
 
 
 def check_value(value: AggregateTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotsitewise.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotsitewise.type_defs import (
     AggregatesTypeDef,
     AlarmsTypeDef,
     AssetErrorDetailsTypeDef,
     AssetHierarchyInfoTypeDef,
@@ -454,29 +454,28 @@
     VariantTypeDef,
     AssociateAssetsRequestRequestTypeDef,
     AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
     AttributeTypeDef,
     BatchAssociateProjectAssetsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDisassociateProjectAssetsRequestRequestTypeDef,
-    BatchGetAssetPropertyAggregatesEntryTypeDef,
+    TimestampTypeDef,
     BatchGetAssetPropertyAggregatesErrorEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueErrorEntryTypeDef,
     BatchGetAssetPropertyValueErrorInfoTypeDef,
-    BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorInfoTypeDef,
+    BlobTypeDef,
     ConfigurationErrorDetailsTypeDef,
     CreateAssetRequestRequestTypeDef,
     ErrorReportLocationTypeDef,
     FileTypeDef,
     CreateDashboardRequestRequestTypeDef,
-    ImageFileTypeDef,
     CreateProjectRequestRequestTypeDef,
     CsvOutputTypeDef,
     CsvTypeDef,
     CustomerManagedS3StorageTypeDef,
     DashboardSummaryTypeDef,
     DeleteAccessPolicyRequestRequestTypeDef,
     DeleteAssetModelRequestRequestTypeDef,
@@ -506,16 +505,14 @@
     DisassociateAssetsRequestRequestTypeDef,
     DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     VariableValueTypeDef,
     ForwardingConfigTypeDef,
     GreengrassTypeDef,
     GreengrassV2TypeDef,
     PaginatorConfigTypeDef,
-    GetAssetPropertyAggregatesRequestRequestTypeDef,
-    GetAssetPropertyValueHistoryRequestRequestTypeDef,
     GetAssetPropertyValueRequestRequestTypeDef,
     GetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
     GroupIdentityTypeDef,
     IAMRoleIdentityTypeDef,
     IAMUserIdentityTypeDef,
     UserIdentityTypeDef,
     JobSummaryTypeDef,
@@ -568,23 +565,24 @@
     DescribeGatewayCapabilityConfigurationResponseTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeTimeSeriesResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListProjectAssetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateGatewayCapabilityConfigurationResponseTypeDef,
-    BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+    BatchGetAssetPropertyAggregatesEntryTypeDef,
+    BatchGetAssetPropertyValueHistoryEntryTypeDef,
+    GetAssetPropertyAggregatesRequestRequestTypeDef,
+    GetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     BatchGetAssetPropertyValueRequestRequestTypeDef,
     BatchGetAssetPropertyValueSkippedEntryTypeDef,
-    BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
+    ImageFileTypeDef,
     ConfigurationStatusTypeDef,
-    CreatePortalRequestRequestTypeDef,
-    ImageTypeDef,
     FileFormatOutputTypeDef,
     FileFormatTypeDef,
     MultiLayerStorageTypeDef,
     ListDashboardsResponseTypeDef,
     DescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     DescribeAssetRequestAssetActiveWaitTypeDef,
@@ -630,17 +628,20 @@
     BatchPutAssetPropertyErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistorySuccessEntryTypeDef,
     BatchGetAssetPropertyValueSuccessEntryTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
+    BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+    BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
+    CreatePortalRequestRequestTypeDef,
+    ImageTypeDef,
     DescribeDefaultEncryptionConfigurationResponseTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
-    UpdatePortalRequestRequestTypeDef,
     JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     DescribeStorageConfigurationResponseTypeDef,
     PutStorageConfigurationRequestRequestTypeDef,
     PutStorageConfigurationResponseTypeDef,
     AssetModelStatusTypeDef,
     AssetStatusTypeDef,
@@ -662,16 +663,18 @@
     DescribeAccessPolicyResponseTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchPutAssetPropertyValueResponseTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
     BatchGetAssetPropertyValueResponseTypeDef,
     BatchPutAssetPropertyValueRequestRequestTypeDef,
+    UpdatePortalRequestRequestTypeDef,
     DescribeBulkImportJobResponseTypeDef,
     CreateBulkImportJobRequestRequestTypeDef,
+    JobConfigurationUnionTypeDef,
     AssetModelSummaryTypeDef,
     CreateAssetModelResponseTypeDef,
     DeleteAssetModelResponseTypeDef,
     UpdateAssetModelResponseTypeDef,
     AssetSummaryTypeDef,
     AssociatedAssetsSummaryTypeDef,
     CreateAssetResponseTypeDef,
@@ -692,22 +695,24 @@
     AssetModelPropertyDefinitionTypeDef,
     AssetModelPropertyTypeDef,
     AssetModelCompositeModelOutputTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
     CompositeModelPropertyTypeDef,
     AssetModelCompositeModelDefinitionTypeDef,
     AssetModelCompositeModelTypeDef,
+    AssetModelPropertyUnionTypeDef,
     DescribeAssetModelResponseTypeDef,
     DescribeAssetPropertyResponseTypeDef,
     CreateAssetModelRequestRequestTypeDef,
+    AssetModelCompositeModelUnionTypeDef,
     UpdateAssetModelRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregatesTypeDef:
+def get_value() -> AggregatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__init__.py` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__init__.pyi` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__main__.py` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTSiteWise 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTSiteWise 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise\nOther"
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

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/client.py` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iotsitewise.client import IoTSiteWiseClient
 
     session = Session()
     client: IoTSiteWiseClient = session.client("iotsitewise")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregateTypeType,
     AuthModeType,
     DisassociatedDataStorageStateType,
@@ -56,21 +55,19 @@
     ListProjectAssetsPaginator,
     ListProjectsPaginator,
     ListTimeSeriesPaginator,
 )
 from .type_defs import (
     AlarmsTypeDef,
     AssetModelCompositeModelDefinitionTypeDef,
-    AssetModelCompositeModelOutputTypeDef,
-    AssetModelCompositeModelTypeDef,
+    AssetModelCompositeModelUnionTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
     AssetModelHierarchyTypeDef,
     AssetModelPropertyDefinitionTypeDef,
-    AssetModelPropertyOutputTypeDef,
-    AssetModelPropertyTypeDef,
+    AssetModelPropertyUnionTypeDef,
     BatchAssociateProjectAssetsResponseTypeDef,
     BatchDisassociateProjectAssetsResponseTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
@@ -108,16 +105,15 @@
     GetAssetPropertyAggregatesResponseTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
     IdentityTypeDef,
     ImageFileTypeDef,
     ImageTypeDef,
-    JobConfigurationOutputTypeDef,
-    JobConfigurationTypeDef,
+    JobConfigurationUnionTypeDef,
     ListAccessPoliciesResponseTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
     ListAssetModelsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetsResponseTypeDef,
     ListAssociatedAssetsResponseTypeDef,
@@ -132,14 +128,15 @@
     LoggingOptionsTypeDef,
     MultiLayerStorageTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
     PutStorageConfigurationResponseTypeDef,
     ResourceTypeDef,
     RetentionPeriodTypeDef,
+    TimestampTypeDef,
     UpdateAssetModelResponseTypeDef,
     UpdateAssetResponseTypeDef,
     UpdateGatewayCapabilityConfigurationResponseTypeDef,
     UpdatePortalResponseTypeDef,
 )
 from .waiter import (
     AssetActiveWaiter,
@@ -359,15 +356,15 @@
     def create_bulk_import_job(
         self,
         *,
         jobName: str,
         jobRoleArn: str,
         files: Sequence[FileTypeDef],
         errorReportLocation: ErrorReportLocationTypeDef,
-        jobConfiguration: Union[JobConfigurationTypeDef, JobConfigurationOutputTypeDef]
+        jobConfiguration: JobConfigurationUnionTypeDef
     ) -> CreateBulkImportJobResponseTypeDef:
         """
         Defines a job to ingest data to IoT SiteWise from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_bulk_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/client/#create_bulk_import_job)
         """
@@ -676,16 +673,16 @@
         """
 
     def get_asset_property_aggregates(
         self,
         *,
         aggregateTypes: Sequence[AggregateTypeType],
         resolution: str,
-        startDate: Union[datetime, str],
-        endDate: Union[datetime, str],
+        startDate: TimestampTypeDef,
+        endDate: TimestampTypeDef,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -709,16 +706,16 @@
 
     def get_asset_property_value_history(
         self,
         *,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
-        startDate: Union[datetime, str] = ...,
-        endDate: Union[datetime, str] = ...,
+        startDate: TimestampTypeDef = ...,
+        endDate: TimestampTypeDef = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetAssetPropertyValueHistoryResponseTypeDef:
         """
         Gets the history of an asset property's values.
@@ -1025,21 +1022,17 @@
 
     def update_asset_model(
         self,
         *,
         assetModelId: str,
         assetModelName: str,
         assetModelDescription: str = ...,
-        assetModelProperties: Sequence[
-            Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
-        ] = ...,
+        assetModelProperties: Sequence[AssetModelPropertyUnionTypeDef] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyTypeDef] = ...,
-        assetModelCompositeModels: Sequence[
-            Union[AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef]
-        ] = ...,
+        assetModelCompositeModels: Sequence[AssetModelCompositeModelUnionTypeDef] = ...,
         clientToken: str = ...
     ) -> UpdateAssetModelResponseTypeDef:
         """
         Updates an asset model and all of the assets that were created from the model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/client/#update_asset_model)
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/client.pyi` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iotsitewise.client import IoTSiteWiseClient
 
     session = Session()
     client: IoTSiteWiseClient = session.client("iotsitewise")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregateTypeType,
     AuthModeType,
     DisassociatedDataStorageStateType,
@@ -56,21 +55,19 @@
     ListProjectAssetsPaginator,
     ListProjectsPaginator,
     ListTimeSeriesPaginator,
 )
 from .type_defs import (
     AlarmsTypeDef,
     AssetModelCompositeModelDefinitionTypeDef,
-    AssetModelCompositeModelOutputTypeDef,
-    AssetModelCompositeModelTypeDef,
+    AssetModelCompositeModelUnionTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
     AssetModelHierarchyTypeDef,
     AssetModelPropertyDefinitionTypeDef,
-    AssetModelPropertyOutputTypeDef,
-    AssetModelPropertyTypeDef,
+    AssetModelPropertyUnionTypeDef,
     BatchAssociateProjectAssetsResponseTypeDef,
     BatchDisassociateProjectAssetsResponseTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
@@ -108,16 +105,15 @@
     GetAssetPropertyAggregatesResponseTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
     IdentityTypeDef,
     ImageFileTypeDef,
     ImageTypeDef,
-    JobConfigurationOutputTypeDef,
-    JobConfigurationTypeDef,
+    JobConfigurationUnionTypeDef,
     ListAccessPoliciesResponseTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
     ListAssetModelsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetsResponseTypeDef,
     ListAssociatedAssetsResponseTypeDef,
@@ -132,14 +128,15 @@
     LoggingOptionsTypeDef,
     MultiLayerStorageTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
     PutStorageConfigurationResponseTypeDef,
     ResourceTypeDef,
     RetentionPeriodTypeDef,
+    TimestampTypeDef,
     UpdateAssetModelResponseTypeDef,
     UpdateAssetResponseTypeDef,
     UpdateGatewayCapabilityConfigurationResponseTypeDef,
     UpdatePortalResponseTypeDef,
 )
 from .waiter import (
     AssetActiveWaiter,
@@ -341,15 +338,15 @@
     def create_bulk_import_job(
         self,
         *,
         jobName: str,
         jobRoleArn: str,
         files: Sequence[FileTypeDef],
         errorReportLocation: ErrorReportLocationTypeDef,
-        jobConfiguration: Union[JobConfigurationTypeDef, JobConfigurationOutputTypeDef]
+        jobConfiguration: JobConfigurationUnionTypeDef
     ) -> CreateBulkImportJobResponseTypeDef:
         """
         Defines a job to ingest data to IoT SiteWise from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_bulk_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/client/#create_bulk_import_job)
         """
@@ -628,16 +625,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/client/#generate_presigned_url)
         """
     def get_asset_property_aggregates(
         self,
         *,
         aggregateTypes: Sequence[AggregateTypeType],
         resolution: str,
-        startDate: Union[datetime, str],
-        endDate: Union[datetime, str],
+        startDate: TimestampTypeDef,
+        endDate: TimestampTypeDef,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -659,16 +656,16 @@
         """
     def get_asset_property_value_history(
         self,
         *,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
-        startDate: Union[datetime, str] = ...,
-        endDate: Union[datetime, str] = ...,
+        startDate: TimestampTypeDef = ...,
+        endDate: TimestampTypeDef = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetAssetPropertyValueHistoryResponseTypeDef:
         """
         Gets the history of an asset property's values.
@@ -951,21 +948,17 @@
         """
     def update_asset_model(
         self,
         *,
         assetModelId: str,
         assetModelName: str,
         assetModelDescription: str = ...,
-        assetModelProperties: Sequence[
-            Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
-        ] = ...,
+        assetModelProperties: Sequence[AssetModelPropertyUnionTypeDef] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyTypeDef] = ...,
-        assetModelCompositeModels: Sequence[
-            Union[AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef]
-        ] = ...,
+        assetModelCompositeModels: Sequence[AssetModelCompositeModelUnionTypeDef] = ...,
         clientToken: str = ...
     ) -> UpdateAssetModelResponseTypeDef:
         """
         Updates an asset model and all of the assets that were created from the model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/client/#update_asset_model)
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/literals.py` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/literals.pyi` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/paginator.py` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,15 @@
     list_portals_paginator: ListPortalsPaginator = client.get_paginator("list_portals")
     list_project_assets_paginator: ListProjectAssetsPaginator = client.get_paginator("list_project_assets")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_time_series_paginator: ListTimeSeriesPaginator = client.get_paginator("list_time_series")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AggregateTypeType,
     IdentityTypeType,
     ListAssetModelPropertiesFilterType,
@@ -85,22 +84,22 @@
     ListDashboardsResponseTypeDef,
     ListGatewaysResponseTypeDef,
     ListPortalsResponseTypeDef,
     ListProjectAssetsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTimeSeriesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GetAssetPropertyAggregatesPaginator",
     "GetAssetPropertyValueHistoryPaginator",
     "GetInterpolatedAssetPropertyValuesPaginator",
     "ListAccessPoliciesPaginator",
     "ListAssetModelPropertiesPaginator",
     "ListAssetModelsPaginator",
@@ -113,75 +112,70 @@
     "ListGatewaysPaginator",
     "ListPortalsPaginator",
     "ListProjectAssetsPaginator",
     "ListProjectsPaginator",
     "ListTimeSeriesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetAssetPropertyAggregatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyaggregatespaginator)
     """
 
     def paginate(
         self,
         *,
         aggregateTypes: Sequence[AggregateTypeType],
         resolution: str,
-        startDate: Union[datetime, str],
-        endDate: Union[datetime, str],
+        startDate: TimestampTypeDef,
+        endDate: TimestampTypeDef,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAssetPropertyAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyaggregatespaginator)
         """
 
-
 class GetAssetPropertyValueHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyvaluehistorypaginator)
     """
 
     def paginate(
         self,
         *,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
-        startDate: Union[datetime, str] = ...,
-        endDate: Union[datetime, str] = ...,
+        startDate: TimestampTypeDef = ...,
+        endDate: TimestampTypeDef = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAssetPropertyValueHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyvaluehistorypaginator)
         """
 
-
 class GetInterpolatedAssetPropertyValuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getinterpolatedassetpropertyvaluespaginator)
     """
 
     def paginate(
@@ -201,15 +195,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInterpolatedAssetPropertyValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getinterpolatedassetpropertyvaluespaginator)
         """
 
-
 class ListAccessPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAccessPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listaccesspoliciespaginator)
     """
 
     def paginate(
@@ -223,15 +216,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAccessPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listaccesspoliciespaginator)
         """
 
-
 class ListAssetModelPropertiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModelProperties)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelpropertiespaginator)
     """
 
     def paginate(
@@ -242,30 +234,28 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetModelPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModelProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelpropertiespaginator)
         """
 
-
 class ListAssetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelspaginator)
         """
 
-
 class ListAssetPropertiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetProperties)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetpropertiespaginator)
     """
 
     def paginate(
@@ -276,15 +266,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetpropertiespaginator)
         """
 
-
 class ListAssetRelationshipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetRelationships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetrelationshipspaginator)
     """
 
     def paginate(
@@ -295,15 +284,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetRelationships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetrelationshipspaginator)
         """
 
-
 class ListAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetspaginator)
     """
 
     def paginate(
@@ -314,15 +302,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetspaginator)
         """
 
-
 class ListAssociatedAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssociatedAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassociatedassetspaginator)
     """
 
     def paginate(
@@ -334,15 +321,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssociatedAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassociatedassetspaginator)
         """
 
-
 class ListBulkImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListBulkImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listbulkimportjobspaginator)
     """
 
     def paginate(
@@ -352,90 +338,84 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBulkImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListBulkImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listbulkimportjobspaginator)
         """
 
-
 class ListDashboardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListDashboards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listdashboardspaginator)
     """
 
     def paginate(
         self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDashboardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListDashboards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listdashboardspaginator)
         """
 
-
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listgatewayspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewaysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listgatewayspaginator)
         """
 
-
 class ListPortalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListPortals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listportalspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPortalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListPortals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listportalspaginator)
         """
 
-
 class ListProjectAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjectAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectassetspaginator)
     """
 
     def paginate(
         self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjectAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectassetspaginator)
         """
 
-
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectspaginator)
     """
 
     def paginate(
         self, *, portalId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectspaginator)
         """
 
-
 class ListTimeSeriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListTimeSeries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listtimeseriespaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/paginator.pyi` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,15 @@
     list_portals_paginator: ListPortalsPaginator = client.get_paginator("list_portals")
     list_project_assets_paginator: ListProjectAssetsPaginator = client.get_paginator("list_project_assets")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_time_series_paginator: ListTimeSeriesPaginator = client.get_paginator("list_time_series")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AggregateTypeType,
     IdentityTypeType,
     ListAssetModelPropertiesFilterType,
@@ -85,21 +84,23 @@
     ListDashboardsResponseTypeDef,
     ListGatewaysResponseTypeDef,
     ListPortalsResponseTypeDef,
     ListProjectAssetsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTimeSeriesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "GetAssetPropertyAggregatesPaginator",
     "GetAssetPropertyValueHistoryPaginator",
     "GetInterpolatedAssetPropertyValuesPaginator",
     "ListAccessPoliciesPaginator",
     "ListAssetModelPropertiesPaginator",
     "ListAssetModelsPaginator",
@@ -112,70 +113,75 @@
     "ListGatewaysPaginator",
     "ListPortalsPaginator",
     "ListProjectAssetsPaginator",
     "ListProjectsPaginator",
     "ListTimeSeriesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetAssetPropertyAggregatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyaggregatespaginator)
     """
 
     def paginate(
         self,
         *,
         aggregateTypes: Sequence[AggregateTypeType],
         resolution: str,
-        startDate: Union[datetime, str],
-        endDate: Union[datetime, str],
+        startDate: TimestampTypeDef,
+        endDate: TimestampTypeDef,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAssetPropertyAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyaggregatespaginator)
         """
 
+
 class GetAssetPropertyValueHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyvaluehistorypaginator)
     """
 
     def paginate(
         self,
         *,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
-        startDate: Union[datetime, str] = ...,
-        endDate: Union[datetime, str] = ...,
+        startDate: TimestampTypeDef = ...,
+        endDate: TimestampTypeDef = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAssetPropertyValueHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyvaluehistorypaginator)
         """
 
+
 class GetInterpolatedAssetPropertyValuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getinterpolatedassetpropertyvaluespaginator)
     """
 
     def paginate(
@@ -195,14 +201,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInterpolatedAssetPropertyValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getinterpolatedassetpropertyvaluespaginator)
         """
 
+
 class ListAccessPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAccessPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listaccesspoliciespaginator)
     """
 
     def paginate(
@@ -216,14 +223,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAccessPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listaccesspoliciespaginator)
         """
 
+
 class ListAssetModelPropertiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModelProperties)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelpropertiespaginator)
     """
 
     def paginate(
@@ -234,28 +242,30 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetModelPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModelProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelpropertiespaginator)
         """
 
+
 class ListAssetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelspaginator)
         """
 
+
 class ListAssetPropertiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetProperties)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetpropertiespaginator)
     """
 
     def paginate(
@@ -266,14 +276,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetpropertiespaginator)
         """
 
+
 class ListAssetRelationshipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetRelationships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetrelationshipspaginator)
     """
 
     def paginate(
@@ -284,14 +295,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetRelationships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetrelationshipspaginator)
         """
 
+
 class ListAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetspaginator)
     """
 
     def paginate(
@@ -302,14 +314,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetspaginator)
         """
 
+
 class ListAssociatedAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssociatedAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassociatedassetspaginator)
     """
 
     def paginate(
@@ -321,14 +334,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssociatedAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassociatedassetspaginator)
         """
 
+
 class ListBulkImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListBulkImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listbulkimportjobspaginator)
     """
 
     def paginate(
@@ -338,84 +352,90 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBulkImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListBulkImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listbulkimportjobspaginator)
         """
 
+
 class ListDashboardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListDashboards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listdashboardspaginator)
     """
 
     def paginate(
         self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDashboardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListDashboards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listdashboardspaginator)
         """
 
+
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listgatewayspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewaysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listgatewayspaginator)
         """
 
+
 class ListPortalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListPortals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listportalspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPortalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListPortals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listportalspaginator)
         """
 
+
 class ListProjectAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjectAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectassetspaginator)
     """
 
     def paginate(
         self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjectAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectassetspaginator)
         """
 
+
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectspaginator)
     """
 
     def paginate(
         self, *, portalId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectspaginator)
         """
 
+
 class ListTimeSeriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListTimeSeries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listtimeseriespaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/type_defs.py` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotsitewise.type_defs import AggregatesTypeDef
 
-    data: AggregatesTypeDef = {...}
+    data: AggregatesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -79,29 +79,28 @@
     "VariantTypeDef",
     "AssociateAssetsRequestRequestTypeDef",
     "AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
     "AttributeTypeDef",
     "BatchAssociateProjectAssetsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDisassociateProjectAssetsRequestRequestTypeDef",
-    "BatchGetAssetPropertyAggregatesEntryTypeDef",
+    "TimestampTypeDef",
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorInfoTypeDef",
     "BatchGetAssetPropertyValueEntryTypeDef",
     "BatchGetAssetPropertyValueErrorEntryTypeDef",
     "BatchGetAssetPropertyValueErrorInfoTypeDef",
-    "BatchGetAssetPropertyValueHistoryEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryErrorInfoTypeDef",
+    "BlobTypeDef",
     "ConfigurationErrorDetailsTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "ErrorReportLocationTypeDef",
     "FileTypeDef",
     "CreateDashboardRequestRequestTypeDef",
-    "ImageFileTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "CsvOutputTypeDef",
     "CsvTypeDef",
     "CustomerManagedS3StorageTypeDef",
     "DashboardSummaryTypeDef",
     "DeleteAccessPolicyRequestRequestTypeDef",
     "DeleteAssetModelRequestRequestTypeDef",
@@ -131,16 +130,14 @@
     "DisassociateAssetsRequestRequestTypeDef",
     "DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
     "VariableValueTypeDef",
     "ForwardingConfigTypeDef",
     "GreengrassTypeDef",
     "GreengrassV2TypeDef",
     "PaginatorConfigTypeDef",
-    "GetAssetPropertyAggregatesRequestRequestTypeDef",
-    "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "GetAssetPropertyValueRequestRequestTypeDef",
     "GetInterpolatedAssetPropertyValuesRequestRequestTypeDef",
     "GroupIdentityTypeDef",
     "IAMRoleIdentityTypeDef",
     "IAMUserIdentityTypeDef",
     "UserIdentityTypeDef",
     "JobSummaryTypeDef",
@@ -193,23 +190,24 @@
     "DescribeGatewayCapabilityConfigurationResponseTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeTimeSeriesResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListProjectAssetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateGatewayCapabilityConfigurationResponseTypeDef",
-    "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+    "BatchGetAssetPropertyAggregatesEntryTypeDef",
+    "BatchGetAssetPropertyValueHistoryEntryTypeDef",
+    "GetAssetPropertyAggregatesRequestRequestTypeDef",
+    "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueRequestRequestTypeDef",
     "BatchGetAssetPropertyValueSkippedEntryTypeDef",
-    "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
+    "ImageFileTypeDef",
     "ConfigurationStatusTypeDef",
-    "CreatePortalRequestRequestTypeDef",
-    "ImageTypeDef",
     "FileFormatOutputTypeDef",
     "FileFormatTypeDef",
     "MultiLayerStorageTypeDef",
     "ListDashboardsResponseTypeDef",
     "DescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     "DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     "DescribeAssetRequestAssetActiveWaitTypeDef",
@@ -255,17 +253,20 @@
     "BatchPutAssetPropertyErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     "BatchGetAssetPropertyValueSuccessEntryTypeDef",
     "GetAssetPropertyValueHistoryResponseTypeDef",
     "GetAssetPropertyValueResponseTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "GetInterpolatedAssetPropertyValuesResponseTypeDef",
+    "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+    "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
+    "CreatePortalRequestRequestTypeDef",
+    "ImageTypeDef",
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     "PutDefaultEncryptionConfigurationResponseTypeDef",
-    "UpdatePortalRequestRequestTypeDef",
     "JobConfigurationOutputTypeDef",
     "JobConfigurationTypeDef",
     "DescribeStorageConfigurationResponseTypeDef",
     "PutStorageConfigurationRequestRequestTypeDef",
     "PutStorageConfigurationResponseTypeDef",
     "AssetModelStatusTypeDef",
     "AssetStatusTypeDef",
@@ -287,16 +288,18 @@
     "DescribeAccessPolicyResponseTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     "BatchPutAssetPropertyValueResponseTypeDef",
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     "BatchGetAssetPropertyValueResponseTypeDef",
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
+    "UpdatePortalRequestRequestTypeDef",
     "DescribeBulkImportJobResponseTypeDef",
     "CreateBulkImportJobRequestRequestTypeDef",
+    "JobConfigurationUnionTypeDef",
     "AssetModelSummaryTypeDef",
     "CreateAssetModelResponseTypeDef",
     "DeleteAssetModelResponseTypeDef",
     "UpdateAssetModelResponseTypeDef",
     "AssetSummaryTypeDef",
     "AssociatedAssetsSummaryTypeDef",
     "CreateAssetResponseTypeDef",
@@ -317,17 +320,19 @@
     "AssetModelPropertyDefinitionTypeDef",
     "AssetModelPropertyTypeDef",
     "AssetModelCompositeModelOutputTypeDef",
     "ListAssetModelPropertiesResponseTypeDef",
     "CompositeModelPropertyTypeDef",
     "AssetModelCompositeModelDefinitionTypeDef",
     "AssetModelCompositeModelTypeDef",
+    "AssetModelPropertyUnionTypeDef",
     "DescribeAssetModelResponseTypeDef",
     "DescribeAssetPropertyResponseTypeDef",
     "CreateAssetModelRequestRequestTypeDef",
+    "AssetModelCompositeModelUnionTypeDef",
     "UpdateAssetModelRequestRequestTypeDef",
 )
 
 AggregatesTypeDef = TypedDict(
     "AggregatesTypeDef",
     {
         "average": float,
@@ -572,44 +577,15 @@
 class BatchDisassociateProjectAssetsRequestRequestTypeDef(
     _RequiredBatchDisassociateProjectAssetsRequestRequestTypeDef,
     _OptionalBatchDisassociateProjectAssetsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredBatchGetAssetPropertyAggregatesEntryTypeDef = TypedDict(
-    "_RequiredBatchGetAssetPropertyAggregatesEntryTypeDef",
-    {
-        "entryId": str,
-        "aggregateTypes": Sequence[AggregateTypeType],
-        "resolution": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-)
-_OptionalBatchGetAssetPropertyAggregatesEntryTypeDef = TypedDict(
-    "_OptionalBatchGetAssetPropertyAggregatesEntryTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-    },
-    total=False,
-)
-
-
-class BatchGetAssetPropertyAggregatesEntryTypeDef(
-    _RequiredBatchGetAssetPropertyAggregatesEntryTypeDef,
-    _OptionalBatchGetAssetPropertyAggregatesEntryTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 BatchGetAssetPropertyAggregatesErrorEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     {
         "errorCode": BatchGetAssetPropertyAggregatesErrorCodeType,
         "errorMessage": str,
         "entryId": str,
     },
@@ -659,42 +635,14 @@
     "BatchGetAssetPropertyValueErrorInfoTypeDef",
     {
         "errorCode": BatchGetAssetPropertyValueErrorCodeType,
         "errorTimestamp": datetime,
     },
 )
 
-_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
-    "_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef",
-    {
-        "entryId": str,
-    },
-)
-_OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
-    "_OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-    },
-    total=False,
-)
-
-
-class BatchGetAssetPropertyValueHistoryEntryTypeDef(
-    _RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef,
-    _OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef,
-):
-    pass
-
-
 BatchGetAssetPropertyValueHistoryErrorEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyValueHistoryErrorEntryTypeDef",
     {
         "errorCode": BatchGetAssetPropertyValueHistoryErrorCodeType,
         "errorMessage": str,
         "entryId": str,
     },
@@ -704,14 +652,15 @@
     "BatchGetAssetPropertyValueHistoryErrorInfoTypeDef",
     {
         "errorCode": BatchGetAssetPropertyValueHistoryErrorCodeType,
         "errorTimestamp": datetime,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConfigurationErrorDetailsTypeDef = TypedDict(
     "ConfigurationErrorDetailsTypeDef",
     {
         "code": ErrorCodeType,
         "message": str,
     },
 )
@@ -789,22 +738,14 @@
 
 class CreateDashboardRequestRequestTypeDef(
     _RequiredCreateDashboardRequestRequestTypeDef, _OptionalCreateDashboardRequestRequestTypeDef
 ):
     pass
 
 
-ImageFileTypeDef = TypedDict(
-    "ImageFileTypeDef",
-    {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-        "type": Literal["PNG"],
-    },
-)
-
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "portalId": str,
         "projectName": str,
     },
 )
@@ -1270,61 +1211,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef",
-    {
-        "aggregateTypes": Sequence[AggregateTypeType],
-        "resolution": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-)
-_OptionalGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetAssetPropertyAggregatesRequestRequestTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class GetAssetPropertyAggregatesRequestRequestTypeDef(
-    _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef,
-    _OptionalGetAssetPropertyAggregatesRequestRequestTypeDef,
-):
-    pass
-
-
-GetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
-    "GetAssetPropertyValueHistoryRequestRequestTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
 GetAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "GetAssetPropertyValueRequestRequestTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
     },
@@ -2158,37 +2052,119 @@
     {
         "capabilityNamespace": str,
         "capabilitySyncStatus": CapabilitySyncStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+_RequiredBatchGetAssetPropertyAggregatesEntryTypeDef = TypedDict(
+    "_RequiredBatchGetAssetPropertyAggregatesEntryTypeDef",
     {
-        "entries": Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
+        "entryId": str,
+        "aggregateTypes": Sequence[AggregateTypeType],
+        "resolution": str,
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
     },
 )
-_OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+_OptionalBatchGetAssetPropertyAggregatesEntryTypeDef = TypedDict(
+    "_OptionalBatchGetAssetPropertyAggregatesEntryTypeDef",
     {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+    },
+    total=False,
+)
+
+
+class BatchGetAssetPropertyAggregatesEntryTypeDef(
+    _RequiredBatchGetAssetPropertyAggregatesEntryTypeDef,
+    _OptionalBatchGetAssetPropertyAggregatesEntryTypeDef,
+):
+    pass
+
+
+_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
+    "_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef",
+    {
+        "entryId": str,
+    },
+)
+_OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
+    "_OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+    },
+    total=False,
+)
+
+
+class BatchGetAssetPropertyValueHistoryEntryTypeDef(
+    _RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef,
+    _OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef,
+):
+    pass
+
+
+_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef",
+    {
+        "aggregateTypes": Sequence[AggregateTypeType],
+        "resolution": str,
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+    },
+)
+_OptionalGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetAssetPropertyAggregatesRequestRequestTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
 
-class BatchGetAssetPropertyAggregatesRequestRequestTypeDef(
-    _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
-    _OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+class GetAssetPropertyAggregatesRequestRequestTypeDef(
+    _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef,
+    _OptionalGetAssetPropertyAggregatesRequestRequestTypeDef,
 ):
     pass
 
 
+GetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
+    "GetAssetPropertyValueHistoryRequestRequestTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
 _RequiredBatchGetAssetPropertyAggregatesSkippedEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     {
         "entryId": str,
         "completionStatus": BatchEntryCompletionStatusType,
     },
 )
@@ -2249,37 +2225,14 @@
 class BatchGetAssetPropertyValueSkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueSkippedEntryTypeDef,
 ):
     pass
 
 
-_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
-    {
-        "entries": Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],
-    },
-)
-_OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class BatchGetAssetPropertyValueHistoryRequestRequestTypeDef(
-    _RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
-    _OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     {
         "entryId": str,
         "completionStatus": BatchEntryCompletionStatusType,
     },
 )
@@ -2295,14 +2248,22 @@
 class BatchGetAssetPropertyValueHistorySkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
 ):
     pass
 
 
+ImageFileTypeDef = TypedDict(
+    "ImageFileTypeDef",
+    {
+        "data": BlobTypeDef,
+        "type": Literal["PNG"],
+    },
+)
+
 _RequiredConfigurationStatusTypeDef = TypedDict(
     "_RequiredConfigurationStatusTypeDef",
     {
         "state": ConfigurationStateType,
     },
 )
 _OptionalConfigurationStatusTypeDef = TypedDict(
@@ -2316,52 +2277,14 @@
 
 class ConfigurationStatusTypeDef(
     _RequiredConfigurationStatusTypeDef, _OptionalConfigurationStatusTypeDef
 ):
     pass
 
 
-_RequiredCreatePortalRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePortalRequestRequestTypeDef",
-    {
-        "portalName": str,
-        "portalContactEmail": str,
-        "roleArn": str,
-    },
-)
-_OptionalCreatePortalRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePortalRequestRequestTypeDef",
-    {
-        "portalDescription": str,
-        "clientToken": str,
-        "portalLogoImageFile": ImageFileTypeDef,
-        "tags": Mapping[str, str],
-        "portalAuthMode": AuthModeType,
-        "notificationSenderEmail": str,
-        "alarms": AlarmsTypeDef,
-    },
-    total=False,
-)
-
-
-class CreatePortalRequestRequestTypeDef(
-    _RequiredCreatePortalRequestRequestTypeDef, _OptionalCreatePortalRequestRequestTypeDef
-):
-    pass
-
-
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "id": str,
-        "file": ImageFileTypeDef,
-    },
-    total=False,
-)
-
 FileFormatOutputTypeDef = TypedDict(
     "FileFormatOutputTypeDef",
     {
         "csv": CsvOutputTypeDef,
     },
     total=False,
 )
@@ -2607,16 +2530,16 @@
 )
 
 _RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
     "_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     {
         "aggregateTypes": Sequence[AggregateTypeType],
         "resolution": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
     },
 )
 _OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
     "_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     {
         "assetId": str,
         "propertyId": str,
@@ -2638,16 +2561,16 @@
 
 GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
         "qualities": Sequence[QualityType],
         "timeOrdering": TimeOrderingType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
@@ -3126,62 +3049,118 @@
     {
         "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
-    "DescribeDefaultEncryptionConfigurationResponseTypeDef",
+_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
-        "encryptionType": EncryptionTypeType,
-        "kmsKeyArn": str,
-        "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "entries": Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
     },
 )
+_OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
 
-PutDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
-    "PutDefaultEncryptionConfigurationResponseTypeDef",
+
+class BatchGetAssetPropertyAggregatesRequestRequestTypeDef(
+    _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+    _OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     {
-        "encryptionType": EncryptionTypeType,
-        "kmsKeyArn": str,
-        "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "entries": Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],
+    },
+)
+_OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
     },
+    total=False,
 )
 
-_RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdatePortalRequestRequestTypeDef",
+
+class BatchGetAssetPropertyValueHistoryRequestRequestTypeDef(
+    _RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
+    _OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreatePortalRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePortalRequestRequestTypeDef",
     {
-        "portalId": str,
         "portalName": str,
         "portalContactEmail": str,
         "roleArn": str,
     },
 )
-_OptionalUpdatePortalRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdatePortalRequestRequestTypeDef",
+_OptionalCreatePortalRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePortalRequestRequestTypeDef",
     {
         "portalDescription": str,
-        "portalLogoImage": ImageTypeDef,
         "clientToken": str,
+        "portalLogoImageFile": ImageFileTypeDef,
+        "tags": Mapping[str, str],
+        "portalAuthMode": AuthModeType,
         "notificationSenderEmail": str,
         "alarms": AlarmsTypeDef,
     },
     total=False,
 )
 
 
-class UpdatePortalRequestRequestTypeDef(
-    _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
+class CreatePortalRequestRequestTypeDef(
+    _RequiredCreatePortalRequestRequestTypeDef, _OptionalCreatePortalRequestRequestTypeDef
 ):
     pass
 
 
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
+    {
+        "id": str,
+        "file": ImageFileTypeDef,
+    },
+    total=False,
+)
+
+DescribeDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
+    "DescribeDefaultEncryptionConfigurationResponseTypeDef",
+    {
+        "encryptionType": EncryptionTypeType,
+        "kmsKeyArn": str,
+        "configurationStatus": ConfigurationStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
+    "PutDefaultEncryptionConfigurationResponseTypeDef",
+    {
+        "encryptionType": EncryptionTypeType,
+        "kmsKeyArn": str,
+        "configurationStatus": ConfigurationStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 JobConfigurationOutputTypeDef = TypedDict(
     "JobConfigurationOutputTypeDef",
     {
         "fileFormat": FileFormatOutputTypeDef,
     },
 )
 
@@ -3636,14 +3615,42 @@
 BatchPutAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     {
         "entries": Sequence[PutAssetPropertyValueEntryTypeDef],
     },
 )
 
+_RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdatePortalRequestRequestTypeDef",
+    {
+        "portalId": str,
+        "portalName": str,
+        "portalContactEmail": str,
+        "roleArn": str,
+    },
+)
+_OptionalUpdatePortalRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdatePortalRequestRequestTypeDef",
+    {
+        "portalDescription": str,
+        "portalLogoImage": ImageTypeDef,
+        "clientToken": str,
+        "notificationSenderEmail": str,
+        "alarms": AlarmsTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdatePortalRequestRequestTypeDef(
+    _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
+):
+    pass
+
+
 DescribeBulkImportJobResponseTypeDef = TypedDict(
     "DescribeBulkImportJobResponseTypeDef",
     {
         "jobId": str,
         "jobName": str,
         "jobStatus": JobStatusType,
         "jobRoleArn": str,
@@ -3663,14 +3670,15 @@
         "jobRoleArn": str,
         "files": Sequence[FileTypeDef],
         "errorReportLocation": ErrorReportLocationTypeDef,
         "jobConfiguration": JobConfigurationTypeDef,
     },
 )
 
+JobConfigurationUnionTypeDef = Union[JobConfigurationTypeDef, JobConfigurationOutputTypeDef]
 AssetModelSummaryTypeDef = TypedDict(
     "AssetModelSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
@@ -4104,14 +4112,15 @@
 
 class AssetModelCompositeModelTypeDef(
     _RequiredAssetModelCompositeModelTypeDef, _OptionalAssetModelCompositeModelTypeDef
 ):
     pass
 
 
+AssetModelPropertyUnionTypeDef = Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
 DescribeAssetModelResponseTypeDef = TypedDict(
     "DescribeAssetModelResponseTypeDef",
     {
         "assetModelId": str,
         "assetModelArn": str,
         "assetModelName": str,
         "assetModelDescription": str,
@@ -4159,32 +4168,31 @@
 
 class CreateAssetModelRequestRequestTypeDef(
     _RequiredCreateAssetModelRequestRequestTypeDef, _OptionalCreateAssetModelRequestRequestTypeDef
 ):
     pass
 
 
+AssetModelCompositeModelUnionTypeDef = Union[
+    AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef
+]
 _RequiredUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelId": str,
         "assetModelName": str,
     },
 )
 _OptionalUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelDescription": str,
-        "assetModelProperties": Sequence[
-            Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
-        ],
+        "assetModelProperties": Sequence[AssetModelPropertyUnionTypeDef],
         "assetModelHierarchies": Sequence[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": Sequence[
-            Union[AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef]
-        ],
+        "assetModelCompositeModels": Sequence[AssetModelCompositeModelUnionTypeDef],
         "clientToken": str,
     },
     total=False,
 )
 
 
 class UpdateAssetModelRequestRequestTypeDef(
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/type_defs.pyi` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotsitewise.type_defs import AggregatesTypeDef
 
-    data: AggregatesTypeDef = {...}
+    data: AggregatesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -78,29 +78,28 @@
     "VariantTypeDef",
     "AssociateAssetsRequestRequestTypeDef",
     "AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
     "AttributeTypeDef",
     "BatchAssociateProjectAssetsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDisassociateProjectAssetsRequestRequestTypeDef",
-    "BatchGetAssetPropertyAggregatesEntryTypeDef",
+    "TimestampTypeDef",
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorInfoTypeDef",
     "BatchGetAssetPropertyValueEntryTypeDef",
     "BatchGetAssetPropertyValueErrorEntryTypeDef",
     "BatchGetAssetPropertyValueErrorInfoTypeDef",
-    "BatchGetAssetPropertyValueHistoryEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryErrorInfoTypeDef",
+    "BlobTypeDef",
     "ConfigurationErrorDetailsTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "ErrorReportLocationTypeDef",
     "FileTypeDef",
     "CreateDashboardRequestRequestTypeDef",
-    "ImageFileTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "CsvOutputTypeDef",
     "CsvTypeDef",
     "CustomerManagedS3StorageTypeDef",
     "DashboardSummaryTypeDef",
     "DeleteAccessPolicyRequestRequestTypeDef",
     "DeleteAssetModelRequestRequestTypeDef",
@@ -130,16 +129,14 @@
     "DisassociateAssetsRequestRequestTypeDef",
     "DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
     "VariableValueTypeDef",
     "ForwardingConfigTypeDef",
     "GreengrassTypeDef",
     "GreengrassV2TypeDef",
     "PaginatorConfigTypeDef",
-    "GetAssetPropertyAggregatesRequestRequestTypeDef",
-    "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "GetAssetPropertyValueRequestRequestTypeDef",
     "GetInterpolatedAssetPropertyValuesRequestRequestTypeDef",
     "GroupIdentityTypeDef",
     "IAMRoleIdentityTypeDef",
     "IAMUserIdentityTypeDef",
     "UserIdentityTypeDef",
     "JobSummaryTypeDef",
@@ -192,23 +189,24 @@
     "DescribeGatewayCapabilityConfigurationResponseTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeTimeSeriesResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListProjectAssetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateGatewayCapabilityConfigurationResponseTypeDef",
-    "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+    "BatchGetAssetPropertyAggregatesEntryTypeDef",
+    "BatchGetAssetPropertyValueHistoryEntryTypeDef",
+    "GetAssetPropertyAggregatesRequestRequestTypeDef",
+    "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueRequestRequestTypeDef",
     "BatchGetAssetPropertyValueSkippedEntryTypeDef",
-    "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
+    "ImageFileTypeDef",
     "ConfigurationStatusTypeDef",
-    "CreatePortalRequestRequestTypeDef",
-    "ImageTypeDef",
     "FileFormatOutputTypeDef",
     "FileFormatTypeDef",
     "MultiLayerStorageTypeDef",
     "ListDashboardsResponseTypeDef",
     "DescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     "DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     "DescribeAssetRequestAssetActiveWaitTypeDef",
@@ -254,17 +252,20 @@
     "BatchPutAssetPropertyErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     "BatchGetAssetPropertyValueSuccessEntryTypeDef",
     "GetAssetPropertyValueHistoryResponseTypeDef",
     "GetAssetPropertyValueResponseTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "GetInterpolatedAssetPropertyValuesResponseTypeDef",
+    "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+    "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
+    "CreatePortalRequestRequestTypeDef",
+    "ImageTypeDef",
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     "PutDefaultEncryptionConfigurationResponseTypeDef",
-    "UpdatePortalRequestRequestTypeDef",
     "JobConfigurationOutputTypeDef",
     "JobConfigurationTypeDef",
     "DescribeStorageConfigurationResponseTypeDef",
     "PutStorageConfigurationRequestRequestTypeDef",
     "PutStorageConfigurationResponseTypeDef",
     "AssetModelStatusTypeDef",
     "AssetStatusTypeDef",
@@ -286,16 +287,18 @@
     "DescribeAccessPolicyResponseTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     "BatchPutAssetPropertyValueResponseTypeDef",
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     "BatchGetAssetPropertyValueResponseTypeDef",
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
+    "UpdatePortalRequestRequestTypeDef",
     "DescribeBulkImportJobResponseTypeDef",
     "CreateBulkImportJobRequestRequestTypeDef",
+    "JobConfigurationUnionTypeDef",
     "AssetModelSummaryTypeDef",
     "CreateAssetModelResponseTypeDef",
     "DeleteAssetModelResponseTypeDef",
     "UpdateAssetModelResponseTypeDef",
     "AssetSummaryTypeDef",
     "AssociatedAssetsSummaryTypeDef",
     "CreateAssetResponseTypeDef",
@@ -316,17 +319,19 @@
     "AssetModelPropertyDefinitionTypeDef",
     "AssetModelPropertyTypeDef",
     "AssetModelCompositeModelOutputTypeDef",
     "ListAssetModelPropertiesResponseTypeDef",
     "CompositeModelPropertyTypeDef",
     "AssetModelCompositeModelDefinitionTypeDef",
     "AssetModelCompositeModelTypeDef",
+    "AssetModelPropertyUnionTypeDef",
     "DescribeAssetModelResponseTypeDef",
     "DescribeAssetPropertyResponseTypeDef",
     "CreateAssetModelRequestRequestTypeDef",
+    "AssetModelCompositeModelUnionTypeDef",
     "UpdateAssetModelRequestRequestTypeDef",
 )
 
 AggregatesTypeDef = TypedDict(
     "AggregatesTypeDef",
     {
         "average": float,
@@ -555,42 +560,15 @@
 
 class BatchDisassociateProjectAssetsRequestRequestTypeDef(
     _RequiredBatchDisassociateProjectAssetsRequestRequestTypeDef,
     _OptionalBatchDisassociateProjectAssetsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredBatchGetAssetPropertyAggregatesEntryTypeDef = TypedDict(
-    "_RequiredBatchGetAssetPropertyAggregatesEntryTypeDef",
-    {
-        "entryId": str,
-        "aggregateTypes": Sequence[AggregateTypeType],
-        "resolution": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-)
-_OptionalBatchGetAssetPropertyAggregatesEntryTypeDef = TypedDict(
-    "_OptionalBatchGetAssetPropertyAggregatesEntryTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-    },
-    total=False,
-)
-
-class BatchGetAssetPropertyAggregatesEntryTypeDef(
-    _RequiredBatchGetAssetPropertyAggregatesEntryTypeDef,
-    _OptionalBatchGetAssetPropertyAggregatesEntryTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 BatchGetAssetPropertyAggregatesErrorEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     {
         "errorCode": BatchGetAssetPropertyAggregatesErrorCodeType,
         "errorMessage": str,
         "entryId": str,
     },
@@ -638,40 +616,14 @@
     "BatchGetAssetPropertyValueErrorInfoTypeDef",
     {
         "errorCode": BatchGetAssetPropertyValueErrorCodeType,
         "errorTimestamp": datetime,
     },
 )
 
-_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
-    "_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef",
-    {
-        "entryId": str,
-    },
-)
-_OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
-    "_OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-    },
-    total=False,
-)
-
-class BatchGetAssetPropertyValueHistoryEntryTypeDef(
-    _RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef,
-    _OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef,
-):
-    pass
-
 BatchGetAssetPropertyValueHistoryErrorEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyValueHistoryErrorEntryTypeDef",
     {
         "errorCode": BatchGetAssetPropertyValueHistoryErrorCodeType,
         "errorMessage": str,
         "entryId": str,
     },
@@ -681,14 +633,15 @@
     "BatchGetAssetPropertyValueHistoryErrorInfoTypeDef",
     {
         "errorCode": BatchGetAssetPropertyValueHistoryErrorCodeType,
         "errorTimestamp": datetime,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConfigurationErrorDetailsTypeDef = TypedDict(
     "ConfigurationErrorDetailsTypeDef",
     {
         "code": ErrorCodeType,
         "message": str,
     },
 )
@@ -760,22 +713,14 @@
 )
 
 class CreateDashboardRequestRequestTypeDef(
     _RequiredCreateDashboardRequestRequestTypeDef, _OptionalCreateDashboardRequestRequestTypeDef
 ):
     pass
 
-ImageFileTypeDef = TypedDict(
-    "ImageFileTypeDef",
-    {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-        "type": Literal["PNG"],
-    },
-)
-
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "portalId": str,
         "projectName": str,
     },
 )
@@ -1215,59 +1160,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef",
-    {
-        "aggregateTypes": Sequence[AggregateTypeType],
-        "resolution": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-)
-_OptionalGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetAssetPropertyAggregatesRequestRequestTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class GetAssetPropertyAggregatesRequestRequestTypeDef(
-    _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef,
-    _OptionalGetAssetPropertyAggregatesRequestRequestTypeDef,
-):
-    pass
-
-GetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
-    "GetAssetPropertyValueHistoryRequestRequestTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
 GetAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "GetAssetPropertyValueRequestRequestTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
     },
@@ -2061,35 +1961,113 @@
     {
         "capabilityNamespace": str,
         "capabilitySyncStatus": CapabilitySyncStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+_RequiredBatchGetAssetPropertyAggregatesEntryTypeDef = TypedDict(
+    "_RequiredBatchGetAssetPropertyAggregatesEntryTypeDef",
     {
-        "entries": Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
+        "entryId": str,
+        "aggregateTypes": Sequence[AggregateTypeType],
+        "resolution": str,
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
     },
 )
-_OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+_OptionalBatchGetAssetPropertyAggregatesEntryTypeDef = TypedDict(
+    "_OptionalBatchGetAssetPropertyAggregatesEntryTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+    },
+    total=False,
+)
+
+class BatchGetAssetPropertyAggregatesEntryTypeDef(
+    _RequiredBatchGetAssetPropertyAggregatesEntryTypeDef,
+    _OptionalBatchGetAssetPropertyAggregatesEntryTypeDef,
+):
+    pass
+
+_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
+    "_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef",
+    {
+        "entryId": str,
+    },
+)
+_OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
+    "_OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+    },
+    total=False,
+)
+
+class BatchGetAssetPropertyValueHistoryEntryTypeDef(
+    _RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef,
+    _OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef,
+):
+    pass
+
+_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef",
+    {
+        "aggregateTypes": Sequence[AggregateTypeType],
+        "resolution": str,
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+    },
+)
+_OptionalGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-class BatchGetAssetPropertyAggregatesRequestRequestTypeDef(
-    _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
-    _OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+class GetAssetPropertyAggregatesRequestRequestTypeDef(
+    _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef,
+    _OptionalGetAssetPropertyAggregatesRequestRequestTypeDef,
 ):
     pass
 
+GetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
+    "GetAssetPropertyValueHistoryRequestRequestTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
 _RequiredBatchGetAssetPropertyAggregatesSkippedEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     {
         "entryId": str,
         "completionStatus": BatchEntryCompletionStatusType,
     },
 )
@@ -2144,35 +2122,14 @@
 
 class BatchGetAssetPropertyValueSkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueSkippedEntryTypeDef,
 ):
     pass
 
-_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
-    {
-        "entries": Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],
-    },
-)
-_OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class BatchGetAssetPropertyValueHistoryRequestRequestTypeDef(
-    _RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
-    _OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
-):
-    pass
-
 _RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     {
         "entryId": str,
         "completionStatus": BatchEntryCompletionStatusType,
     },
 )
@@ -2186,14 +2143,22 @@
 
 class BatchGetAssetPropertyValueHistorySkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
 ):
     pass
 
+ImageFileTypeDef = TypedDict(
+    "ImageFileTypeDef",
+    {
+        "data": BlobTypeDef,
+        "type": Literal["PNG"],
+    },
+)
+
 _RequiredConfigurationStatusTypeDef = TypedDict(
     "_RequiredConfigurationStatusTypeDef",
     {
         "state": ConfigurationStateType,
     },
 )
 _OptionalConfigurationStatusTypeDef = TypedDict(
@@ -2205,50 +2170,14 @@
 )
 
 class ConfigurationStatusTypeDef(
     _RequiredConfigurationStatusTypeDef, _OptionalConfigurationStatusTypeDef
 ):
     pass
 
-_RequiredCreatePortalRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePortalRequestRequestTypeDef",
-    {
-        "portalName": str,
-        "portalContactEmail": str,
-        "roleArn": str,
-    },
-)
-_OptionalCreatePortalRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePortalRequestRequestTypeDef",
-    {
-        "portalDescription": str,
-        "clientToken": str,
-        "portalLogoImageFile": ImageFileTypeDef,
-        "tags": Mapping[str, str],
-        "portalAuthMode": AuthModeType,
-        "notificationSenderEmail": str,
-        "alarms": AlarmsTypeDef,
-    },
-    total=False,
-)
-
-class CreatePortalRequestRequestTypeDef(
-    _RequiredCreatePortalRequestRequestTypeDef, _OptionalCreatePortalRequestRequestTypeDef
-):
-    pass
-
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "id": str,
-        "file": ImageFileTypeDef,
-    },
-    total=False,
-)
-
 FileFormatOutputTypeDef = TypedDict(
     "FileFormatOutputTypeDef",
     {
         "csv": CsvOutputTypeDef,
     },
     total=False,
 )
@@ -2478,16 +2407,16 @@
 )
 
 _RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
     "_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     {
         "aggregateTypes": Sequence[AggregateTypeType],
         "resolution": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
     },
 )
 _OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
     "_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     {
         "assetId": str,
         "propertyId": str,
@@ -2507,16 +2436,16 @@
 
 GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
+        "startDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
         "qualities": Sequence[QualityType],
         "timeOrdering": TimeOrderingType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
@@ -2971,60 +2900,112 @@
     {
         "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
-    "DescribeDefaultEncryptionConfigurationResponseTypeDef",
+_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
-        "encryptionType": EncryptionTypeType,
-        "kmsKeyArn": str,
-        "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "entries": Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
+    },
+)
+_OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
     },
+    total=False,
 )
 
-PutDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
-    "PutDefaultEncryptionConfigurationResponseTypeDef",
+class BatchGetAssetPropertyAggregatesRequestRequestTypeDef(
+    _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+    _OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+):
+    pass
+
+_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     {
-        "encryptionType": EncryptionTypeType,
-        "kmsKeyArn": str,
-        "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "entries": Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],
+    },
+)
+_OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
     },
+    total=False,
 )
 
-_RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdatePortalRequestRequestTypeDef",
+class BatchGetAssetPropertyValueHistoryRequestRequestTypeDef(
+    _RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
+    _OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreatePortalRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePortalRequestRequestTypeDef",
     {
-        "portalId": str,
         "portalName": str,
         "portalContactEmail": str,
         "roleArn": str,
     },
 )
-_OptionalUpdatePortalRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdatePortalRequestRequestTypeDef",
+_OptionalCreatePortalRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePortalRequestRequestTypeDef",
     {
         "portalDescription": str,
-        "portalLogoImage": ImageTypeDef,
         "clientToken": str,
+        "portalLogoImageFile": ImageFileTypeDef,
+        "tags": Mapping[str, str],
+        "portalAuthMode": AuthModeType,
         "notificationSenderEmail": str,
         "alarms": AlarmsTypeDef,
     },
     total=False,
 )
 
-class UpdatePortalRequestRequestTypeDef(
-    _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
+class CreatePortalRequestRequestTypeDef(
+    _RequiredCreatePortalRequestRequestTypeDef, _OptionalCreatePortalRequestRequestTypeDef
 ):
     pass
 
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
+    {
+        "id": str,
+        "file": ImageFileTypeDef,
+    },
+    total=False,
+)
+
+DescribeDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
+    "DescribeDefaultEncryptionConfigurationResponseTypeDef",
+    {
+        "encryptionType": EncryptionTypeType,
+        "kmsKeyArn": str,
+        "configurationStatus": ConfigurationStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
+    "PutDefaultEncryptionConfigurationResponseTypeDef",
+    {
+        "encryptionType": EncryptionTypeType,
+        "kmsKeyArn": str,
+        "configurationStatus": ConfigurationStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 JobConfigurationOutputTypeDef = TypedDict(
     "JobConfigurationOutputTypeDef",
     {
         "fileFormat": FileFormatOutputTypeDef,
     },
 )
 
@@ -3453,14 +3434,40 @@
 BatchPutAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     {
         "entries": Sequence[PutAssetPropertyValueEntryTypeDef],
     },
 )
 
+_RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdatePortalRequestRequestTypeDef",
+    {
+        "portalId": str,
+        "portalName": str,
+        "portalContactEmail": str,
+        "roleArn": str,
+    },
+)
+_OptionalUpdatePortalRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdatePortalRequestRequestTypeDef",
+    {
+        "portalDescription": str,
+        "portalLogoImage": ImageTypeDef,
+        "clientToken": str,
+        "notificationSenderEmail": str,
+        "alarms": AlarmsTypeDef,
+    },
+    total=False,
+)
+
+class UpdatePortalRequestRequestTypeDef(
+    _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
+):
+    pass
+
 DescribeBulkImportJobResponseTypeDef = TypedDict(
     "DescribeBulkImportJobResponseTypeDef",
     {
         "jobId": str,
         "jobName": str,
         "jobStatus": JobStatusType,
         "jobRoleArn": str,
@@ -3480,14 +3487,15 @@
         "jobRoleArn": str,
         "files": Sequence[FileTypeDef],
         "errorReportLocation": ErrorReportLocationTypeDef,
         "jobConfiguration": JobConfigurationTypeDef,
     },
 )
 
+JobConfigurationUnionTypeDef = Union[JobConfigurationTypeDef, JobConfigurationOutputTypeDef]
 AssetModelSummaryTypeDef = TypedDict(
     "AssetModelSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
@@ -3899,14 +3907,15 @@
 )
 
 class AssetModelCompositeModelTypeDef(
     _RequiredAssetModelCompositeModelTypeDef, _OptionalAssetModelCompositeModelTypeDef
 ):
     pass
 
+AssetModelPropertyUnionTypeDef = Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
 DescribeAssetModelResponseTypeDef = TypedDict(
     "DescribeAssetModelResponseTypeDef",
     {
         "assetModelId": str,
         "assetModelArn": str,
         "assetModelName": str,
         "assetModelDescription": str,
@@ -3952,32 +3961,31 @@
 )
 
 class CreateAssetModelRequestRequestTypeDef(
     _RequiredCreateAssetModelRequestRequestTypeDef, _OptionalCreateAssetModelRequestRequestTypeDef
 ):
     pass
 
+AssetModelCompositeModelUnionTypeDef = Union[
+    AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef
+]
 _RequiredUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelId": str,
         "assetModelName": str,
     },
 )
 _OptionalUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelDescription": str,
-        "assetModelProperties": Sequence[
-            Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
-        ],
+        "assetModelProperties": Sequence[AssetModelPropertyUnionTypeDef],
         "assetModelHierarchies": Sequence[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": Sequence[
-            Union[AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef]
-        ],
+        "assetModelCompositeModels": Sequence[AssetModelCompositeModelUnionTypeDef],
         "clientToken": str,
     },
     total=False,
 )
 
 class UpdateAssetModelRequestRequestTypeDef(
     _RequiredUpdateAssetModelRequestRequestTypeDef, _OptionalUpdateAssetModelRequestRequestTypeDef
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/waiter.py` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/waiter.pyi` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/PKG-INFO` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsitewise
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTSiteWise 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotsitewise type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotsitewise type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsitewise)](https://pepy.tech/project/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
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
@@ -461,20 +461,20 @@
 )
 
 
 def check_value(value: AggregateTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotsitewise.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotsitewise.type_defs import (
     AggregatesTypeDef,
     AlarmsTypeDef,
     AssetErrorDetailsTypeDef,
     AssetHierarchyInfoTypeDef,
@@ -486,29 +486,28 @@
     VariantTypeDef,
     AssociateAssetsRequestRequestTypeDef,
     AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
     AttributeTypeDef,
     BatchAssociateProjectAssetsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDisassociateProjectAssetsRequestRequestTypeDef,
-    BatchGetAssetPropertyAggregatesEntryTypeDef,
+    TimestampTypeDef,
     BatchGetAssetPropertyAggregatesErrorEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueErrorEntryTypeDef,
     BatchGetAssetPropertyValueErrorInfoTypeDef,
-    BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorInfoTypeDef,
+    BlobTypeDef,
     ConfigurationErrorDetailsTypeDef,
     CreateAssetRequestRequestTypeDef,
     ErrorReportLocationTypeDef,
     FileTypeDef,
     CreateDashboardRequestRequestTypeDef,
-    ImageFileTypeDef,
     CreateProjectRequestRequestTypeDef,
     CsvOutputTypeDef,
     CsvTypeDef,
     CustomerManagedS3StorageTypeDef,
     DashboardSummaryTypeDef,
     DeleteAccessPolicyRequestRequestTypeDef,
     DeleteAssetModelRequestRequestTypeDef,
@@ -538,16 +537,14 @@
     DisassociateAssetsRequestRequestTypeDef,
     DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     VariableValueTypeDef,
     ForwardingConfigTypeDef,
     GreengrassTypeDef,
     GreengrassV2TypeDef,
     PaginatorConfigTypeDef,
-    GetAssetPropertyAggregatesRequestRequestTypeDef,
-    GetAssetPropertyValueHistoryRequestRequestTypeDef,
     GetAssetPropertyValueRequestRequestTypeDef,
     GetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
     GroupIdentityTypeDef,
     IAMRoleIdentityTypeDef,
     IAMUserIdentityTypeDef,
     UserIdentityTypeDef,
     JobSummaryTypeDef,
@@ -600,23 +597,24 @@
     DescribeGatewayCapabilityConfigurationResponseTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeTimeSeriesResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListProjectAssetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateGatewayCapabilityConfigurationResponseTypeDef,
-    BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+    BatchGetAssetPropertyAggregatesEntryTypeDef,
+    BatchGetAssetPropertyValueHistoryEntryTypeDef,
+    GetAssetPropertyAggregatesRequestRequestTypeDef,
+    GetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     BatchGetAssetPropertyValueRequestRequestTypeDef,
     BatchGetAssetPropertyValueSkippedEntryTypeDef,
-    BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
+    ImageFileTypeDef,
     ConfigurationStatusTypeDef,
-    CreatePortalRequestRequestTypeDef,
-    ImageTypeDef,
     FileFormatOutputTypeDef,
     FileFormatTypeDef,
     MultiLayerStorageTypeDef,
     ListDashboardsResponseTypeDef,
     DescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     DescribeAssetRequestAssetActiveWaitTypeDef,
@@ -662,17 +660,20 @@
     BatchPutAssetPropertyErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistorySuccessEntryTypeDef,
     BatchGetAssetPropertyValueSuccessEntryTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
+    BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
+    BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
+    CreatePortalRequestRequestTypeDef,
+    ImageTypeDef,
     DescribeDefaultEncryptionConfigurationResponseTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
-    UpdatePortalRequestRequestTypeDef,
     JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     DescribeStorageConfigurationResponseTypeDef,
     PutStorageConfigurationRequestRequestTypeDef,
     PutStorageConfigurationResponseTypeDef,
     AssetModelStatusTypeDef,
     AssetStatusTypeDef,
@@ -694,16 +695,18 @@
     DescribeAccessPolicyResponseTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchPutAssetPropertyValueResponseTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
     BatchGetAssetPropertyValueResponseTypeDef,
     BatchPutAssetPropertyValueRequestRequestTypeDef,
+    UpdatePortalRequestRequestTypeDef,
     DescribeBulkImportJobResponseTypeDef,
     CreateBulkImportJobRequestRequestTypeDef,
+    JobConfigurationUnionTypeDef,
     AssetModelSummaryTypeDef,
     CreateAssetModelResponseTypeDef,
     DeleteAssetModelResponseTypeDef,
     UpdateAssetModelResponseTypeDef,
     AssetSummaryTypeDef,
     AssociatedAssetsSummaryTypeDef,
     CreateAssetResponseTypeDef,
@@ -724,22 +727,24 @@
     AssetModelPropertyDefinitionTypeDef,
     AssetModelPropertyTypeDef,
     AssetModelCompositeModelOutputTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
     CompositeModelPropertyTypeDef,
     AssetModelCompositeModelDefinitionTypeDef,
     AssetModelCompositeModelTypeDef,
+    AssetModelPropertyUnionTypeDef,
     DescribeAssetModelResponseTypeDef,
     DescribeAssetPropertyResponseTypeDef,
     CreateAssetModelRequestRequestTypeDef,
+    AssetModelCompositeModelUnionTypeDef,
     UpdateAssetModelRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregatesTypeDef:
+def get_value() -> AggregatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/SOURCES.txt` & `mypy-boto3-iotsitewise-1.28.16/mypy_boto3_iotsitewise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15.post1/setup.py` & `mypy-boto3-iotsitewise-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotsitewise",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iotsitewise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.IoTSiteWise 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 iotsitewise type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iotsitewise type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iotsitewise": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

