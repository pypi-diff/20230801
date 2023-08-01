# Comparing `tmp/mypy-boto3-iotanalytics-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iotanalytics-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotanalytics-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:20 2023, max compression
+gzip compressed data, was "mypy-boto3-iotanalytics-1.28.16.tar", last modified: Tue Aug  1 11:36:59 2023, max compression
```

## Comparing `mypy-boto3-iotanalytics-1.28.15.post1.tar` & `mypy-boto3-iotanalytics-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.025182 mypy-boto3-iotanalytics-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-07-29 10:03:20.025182 mypy-boto3-iotanalytics-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.017182 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27092 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51718 2023-07-29 09:47:52.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51637 2023-07-29 09:47:51.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.025182 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:20.025182 mypy-boto3-iotanalytics-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.860866 mypy-boto3-iotanalytics-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19335 2023-08-01 11:36:59.852866 mypy-boto3-iotanalytics-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.848866 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26290 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26244 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-08-01 11:20:33.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52398 2023-08-01 11:20:34.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-08-01 11:20:33.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.852866 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19335 2023-08-01 11:36:59.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:36:59.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:59.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:59.000000 mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:59.860866 mypy-boto3-iotanalytics-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:20:32.000000 mypy-boto3-iotanalytics-1.28.16/setup.py
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/LICENSE` & `mypy-boto3-iotanalytics-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/PKG-INFO` & `mypy-boto3-iotanalytics-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotanalytics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTAnalytics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotanalytics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotanalytics)](https://pepy.tech/project/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
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
@@ -335,28 +335,28 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotanalytics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
     AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
-    MessageTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
     CustomerManagedChannelS3StorageSummaryTypeDef,
     RetentionPeriodTypeDef,
@@ -395,37 +395,35 @@
     DeviceShadowEnrichActivityTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
     GlueConfigurationTypeDef,
     LambdaActivityTypeDef,
     PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListDatasetContentsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListDatastoresRequestRequestTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MathActivityTypeDef,
     OutputFileUriValueTypeDef,
     RemoveAttributesActivityOutputTypeDef,
     SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    SampleChannelDataRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreatePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
-    StartPipelineReprocessingRequestRequestTypeDef,
+    MessageTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
     ChannelStorageOutputTypeDef,
     ChannelStorageTypeDef,
     ChannelStorageSummaryTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
@@ -442,23 +440,28 @@
     DatastorePartitionTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    ListDatasetContentsRequestRequestTypeDef,
+    SampleChannelDataRequestRequestTypeDef,
+    StartPipelineReprocessingRequestRequestTypeDef,
     VariableTypeDef,
     PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
+    BatchPutMessageRequestRequestTypeDef,
     ChannelTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ChannelSummaryTypeDef,
     ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
@@ -470,41 +473,46 @@
     LateDataRuleTypeDef,
     SqlQueryDatasetActionOutputTypeDef,
     SqlQueryDatasetActionTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
     ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
     PipelineTypeDef,
-    CreatePipelineRequestRequestTypeDef,
+    PipelineActivityUnionTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ListChannelsResponseTypeDef,
     FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
+    DatastoreStorageUnionTypeDef,
     DatastoreSummaryTypeDef,
+    DatastorePartitionsUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
+    CreatePipelineRequestRequestTypeDef,
+    UpdatePipelineRequestRequestTypeDef,
     DatastoreTypeDef,
     CreateDatastoreRequestRequestTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
     ListDatastoresResponseTypeDef,
     DatasetTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    UpdateDatasetRequestRequestTypeDef,
+    DatasetActionUnionTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    UpdateDatasetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddAttributesActivityOutputTypeDef:
+def get_value() -> AddAttributesActivityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/README.md` & `mypy-boto3-iotanalytics-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotanalytics)](https://pepy.tech/project/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
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
@@ -303,28 +303,28 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotanalytics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
     AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
-    MessageTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
     CustomerManagedChannelS3StorageSummaryTypeDef,
     RetentionPeriodTypeDef,
@@ -363,37 +363,35 @@
     DeviceShadowEnrichActivityTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
     GlueConfigurationTypeDef,
     LambdaActivityTypeDef,
     PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListDatasetContentsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListDatastoresRequestRequestTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MathActivityTypeDef,
     OutputFileUriValueTypeDef,
     RemoveAttributesActivityOutputTypeDef,
     SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    SampleChannelDataRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreatePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
-    StartPipelineReprocessingRequestRequestTypeDef,
+    MessageTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
     ChannelStorageOutputTypeDef,
     ChannelStorageTypeDef,
     ChannelStorageSummaryTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
@@ -410,23 +408,28 @@
     DatastorePartitionTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    ListDatasetContentsRequestRequestTypeDef,
+    SampleChannelDataRequestRequestTypeDef,
+    StartPipelineReprocessingRequestRequestTypeDef,
     VariableTypeDef,
     PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
+    BatchPutMessageRequestRequestTypeDef,
     ChannelTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ChannelSummaryTypeDef,
     ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
@@ -438,41 +441,46 @@
     LateDataRuleTypeDef,
     SqlQueryDatasetActionOutputTypeDef,
     SqlQueryDatasetActionTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
     ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
     PipelineTypeDef,
-    CreatePipelineRequestRequestTypeDef,
+    PipelineActivityUnionTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ListChannelsResponseTypeDef,
     FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
+    DatastoreStorageUnionTypeDef,
     DatastoreSummaryTypeDef,
+    DatastorePartitionsUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
+    CreatePipelineRequestRequestTypeDef,
+    UpdatePipelineRequestRequestTypeDef,
     DatastoreTypeDef,
     CreateDatastoreRequestRequestTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
     ListDatastoresResponseTypeDef,
     DatasetTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    UpdateDatasetRequestRequestTypeDef,
+    DatasetActionUnionTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    UpdateDatasetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddAttributesActivityOutputTypeDef:
+def get_value() -> AddAttributesActivityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__init__.py` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__init__.pyi` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__main__.py` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTAnalytics 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTAnalytics 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics\nOther"
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

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/client.py` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,70 +10,64 @@
     from mypy_boto3_iotanalytics.client import IoTAnalyticsClient
 
     session = Session()
     client: IoTAnalyticsClient = session.client("iotanalytics")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     ListChannelsPaginator,
     ListDatasetContentsPaginator,
     ListDatasetsPaginator,
     ListDatastoresPaginator,
     ListPipelinesPaginator,
 )
 from .type_defs import (
     BatchPutMessageResponseTypeDef,
+    BlobTypeDef,
     ChannelMessagesTypeDef,
-    ChannelStorageOutputTypeDef,
-    ChannelStorageTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     CreatePipelineResponseTypeDef,
-    DatasetActionOutputTypeDef,
-    DatasetActionTypeDef,
+    DatasetActionUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetTriggerTypeDef,
-    DatastorePartitionsOutputTypeDef,
-    DatastorePartitionsTypeDef,
-    DatastoreStorageOutputTypeDef,
-    DatastoreStorageTypeDef,
+    DatastorePartitionsUnionTypeDef,
+    DatastoreStorageUnionTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     DescribePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileFormatConfigurationOutputTypeDef,
-    FileFormatConfigurationTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     GetDatasetContentResponseTypeDef,
     LateDataRuleTypeDef,
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingOptionsTypeDef,
     MessageTypeDef,
-    PipelineActivityOutputTypeDef,
-    PipelineActivityTypeDef,
+    PipelineActivityUnionTypeDef,
     RetentionPeriodTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     VersioningConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -154,30 +148,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#close)
         """
 
     def create_channel(
         self,
         *,
         channelName: str,
-        channelStorage: Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef] = ...,
+        channelStorage: ChannelStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_channel)
         """
 
     def create_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
+        actions: Sequence[DatasetActionUnionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
@@ -199,36 +193,32 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_dataset_content)
         """
 
     def create_datastore(
         self,
         *,
         datastoreName: str,
-        datastoreStorage: Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef] = ...,
+        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        fileFormatConfiguration: Union[
-            FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
-        ] = ...,
-        datastorePartitions: Union[
-            DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
-        ] = ...
+        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...,
+        datastorePartitions: DatastorePartitionsUnionTypeDef = ...
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_datastore)
         """
 
     def create_pipeline(
         self,
         *,
         pipelineName: str,
-        pipelineActivities: Sequence[Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]],
+        pipelineActivities: Sequence[PipelineActivityUnionTypeDef],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_pipeline)
@@ -356,16 +346,16 @@
 
     def list_dataset_contents(
         self,
         *,
         datasetName: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        scheduledOnOrAfter: Union[datetime, str] = ...,
-        scheduledBefore: Union[datetime, str] = ...
+        scheduledOnOrAfter: TimestampTypeDef = ...,
+        scheduledBefore: TimestampTypeDef = ...
     ) -> ListDatasetContentsResponseTypeDef:
         """
         Lists information about dataset contents that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.list_dataset_contents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#list_dataset_contents)
         """
@@ -415,48 +405,45 @@
         Sets or updates the IoT Analytics logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.put_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#put_logging_options)
         """
 
     def run_pipeline_activity(
-        self,
-        *,
-        pipelineActivity: Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef],
-        payloads: Sequence[Union[str, bytes, IO[Any], StreamingBody]]
+        self, *, pipelineActivity: PipelineActivityUnionTypeDef, payloads: Sequence[BlobTypeDef]
     ) -> RunPipelineActivityResponseTypeDef:
         """
         Simulates the results of running a pipeline activity on a message payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.run_pipeline_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#run_pipeline_activity)
         """
 
     def sample_channel_data(
         self,
         *,
         channelName: str,
         maxMessages: int = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...
     ) -> SampleChannelDataResponseTypeDef:
         """
         Retrieves a sample of messages from the specified channel ingested during the
         specified timeframe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.sample_channel_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#sample_channel_data)
         """
 
     def start_pipeline_reprocessing(
         self,
         *,
         pipelineName: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         channelMessages: ChannelMessagesTypeDef = ...
     ) -> StartPipelineReprocessingResponseTypeDef:
         """
         Starts the reprocessing of raw message data through the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.start_pipeline_reprocessing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#start_pipeline_reprocessing)
@@ -478,29 +465,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#untag_resource)
         """
 
     def update_channel(
         self,
         *,
         channelName: str,
-        channelStorage: Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef] = ...,
+        channelStorage: ChannelStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_channel)
         """
 
     def update_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
+        actions: Sequence[DatasetActionUnionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -511,31 +498,26 @@
         """
 
     def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        datastoreStorage: Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef] = ...,
-        fileFormatConfiguration: Union[
-            FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
-        ] = ...
+        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
+        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_datastore)
         """
 
     def update_pipeline(
-        self,
-        *,
-        pipelineName: str,
-        pipelineActivities: Sequence[Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]]
+        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityUnionTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_pipeline)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/client.pyi` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,70 +10,64 @@
     from mypy_boto3_iotanalytics.client import IoTAnalyticsClient
 
     session = Session()
     client: IoTAnalyticsClient = session.client("iotanalytics")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import (
     ListChannelsPaginator,
     ListDatasetContentsPaginator,
     ListDatasetsPaginator,
     ListDatastoresPaginator,
     ListPipelinesPaginator,
 )
 from .type_defs import (
     BatchPutMessageResponseTypeDef,
+    BlobTypeDef,
     ChannelMessagesTypeDef,
-    ChannelStorageOutputTypeDef,
-    ChannelStorageTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     CreatePipelineResponseTypeDef,
-    DatasetActionOutputTypeDef,
-    DatasetActionTypeDef,
+    DatasetActionUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetTriggerTypeDef,
-    DatastorePartitionsOutputTypeDef,
-    DatastorePartitionsTypeDef,
-    DatastoreStorageOutputTypeDef,
-    DatastoreStorageTypeDef,
+    DatastorePartitionsUnionTypeDef,
+    DatastoreStorageUnionTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     DescribePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileFormatConfigurationOutputTypeDef,
-    FileFormatConfigurationTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     GetDatasetContentResponseTypeDef,
     LateDataRuleTypeDef,
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingOptionsTypeDef,
     MessageTypeDef,
-    PipelineActivityOutputTypeDef,
-    PipelineActivityTypeDef,
+    PipelineActivityUnionTypeDef,
     RetentionPeriodTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     VersioningConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -145,29 +139,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#close)
         """
     def create_channel(
         self,
         *,
         channelName: str,
-        channelStorage: Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef] = ...,
+        channelStorage: ChannelStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_channel)
         """
     def create_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
+        actions: Sequence[DatasetActionUnionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
@@ -187,35 +181,31 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_dataset_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_dataset_content)
         """
     def create_datastore(
         self,
         *,
         datastoreName: str,
-        datastoreStorage: Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef] = ...,
+        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        fileFormatConfiguration: Union[
-            FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
-        ] = ...,
-        datastorePartitions: Union[
-            DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
-        ] = ...
+        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...,
+        datastorePartitions: DatastorePartitionsUnionTypeDef = ...
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_datastore)
         """
     def create_pipeline(
         self,
         *,
         pipelineName: str,
-        pipelineActivities: Sequence[Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]],
+        pipelineActivities: Sequence[PipelineActivityUnionTypeDef],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_pipeline)
@@ -329,16 +319,16 @@
         """
     def list_dataset_contents(
         self,
         *,
         datasetName: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        scheduledOnOrAfter: Union[datetime, str] = ...,
-        scheduledBefore: Union[datetime, str] = ...
+        scheduledOnOrAfter: TimestampTypeDef = ...,
+        scheduledBefore: TimestampTypeDef = ...
     ) -> ListDatasetContentsResponseTypeDef:
         """
         Lists information about dataset contents that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.list_dataset_contents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#list_dataset_contents)
         """
@@ -382,46 +372,43 @@
         """
         Sets or updates the IoT Analytics logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.put_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#put_logging_options)
         """
     def run_pipeline_activity(
-        self,
-        *,
-        pipelineActivity: Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef],
-        payloads: Sequence[Union[str, bytes, IO[Any], StreamingBody]]
+        self, *, pipelineActivity: PipelineActivityUnionTypeDef, payloads: Sequence[BlobTypeDef]
     ) -> RunPipelineActivityResponseTypeDef:
         """
         Simulates the results of running a pipeline activity on a message payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.run_pipeline_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#run_pipeline_activity)
         """
     def sample_channel_data(
         self,
         *,
         channelName: str,
         maxMessages: int = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...
     ) -> SampleChannelDataResponseTypeDef:
         """
         Retrieves a sample of messages from the specified channel ingested during the
         specified timeframe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.sample_channel_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#sample_channel_data)
         """
     def start_pipeline_reprocessing(
         self,
         *,
         pipelineName: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         channelMessages: ChannelMessagesTypeDef = ...
     ) -> StartPipelineReprocessingResponseTypeDef:
         """
         Starts the reprocessing of raw message data through the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.start_pipeline_reprocessing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#start_pipeline_reprocessing)
@@ -440,28 +427,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#untag_resource)
         """
     def update_channel(
         self,
         *,
         channelName: str,
-        channelStorage: Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef] = ...,
+        channelStorage: ChannelStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_channel)
         """
     def update_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
+        actions: Sequence[DatasetActionUnionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -471,30 +458,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_dataset)
         """
     def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        datastoreStorage: Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef] = ...,
-        fileFormatConfiguration: Union[
-            FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
-        ] = ...
+        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
+        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_datastore)
         """
     def update_pipeline(
-        self,
-        *,
-        pipelineName: str,
-        pipelineActivities: Sequence[Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]]
+        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityUnionTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_pipeline)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/literals.py` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/literals.pyi` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/paginator.py` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,26 +23,26 @@
     list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
     list_dataset_contents_paginator: ListDatasetContentsPaginator = client.get_paginator("list_dataset_contents")
     list_datasets_paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
     list_datastores_paginator: ListDatastoresPaginator = client.get_paginator("list_datastores")
     list_pipelines_paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListChannelsPaginator",
     "ListDatasetContentsPaginator",
     "ListDatasetsPaginator",
     "ListDatastoresPaginator",
@@ -81,16 +81,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
     """
 
     def paginate(
         self,
         *,
         datasetName: str,
-        scheduledOnOrAfter: Union[datetime, str] = ...,
-        scheduledBefore: Union[datetime, str] = ...,
+        scheduledOnOrAfter: TimestampTypeDef = ...,
+        scheduledBefore: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/paginator.pyi` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -23,26 +23,26 @@
     list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
     list_dataset_contents_paginator: ListDatasetContentsPaginator = client.get_paginator("list_dataset_contents")
     list_datasets_paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
     list_datastores_paginator: ListDatastoresPaginator = client.get_paginator("list_datastores")
     list_pipelines_paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListChannelsPaginator",
     "ListDatasetContentsPaginator",
     "ListDatasetsPaginator",
     "ListDatastoresPaginator",
@@ -77,16 +77,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
     """
 
     def paginate(
         self,
         *,
         datasetName: str,
-        scheduledOnOrAfter: Union[datetime, str] = ...,
-        scheduledBefore: Union[datetime, str] = ...,
+        scheduledOnOrAfter: TimestampTypeDef = ...,
+        scheduledBefore: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/type_defs.py` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotanalytics.type_defs import AddAttributesActivityOutputTypeDef
 
-    data: AddAttributesActivityOutputTypeDef = {...}
+    data: AddAttributesActivityOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -33,21 +33,20 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
-    "MessageTypeDef",
     "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     "RetentionPeriodTypeDef",
@@ -86,37 +85,35 @@
     "DeviceShadowEnrichActivityTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
     "GlueConfigurationTypeDef",
     "LambdaActivityTypeDef",
     "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListDatasetContentsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MathActivityTypeDef",
     "OutputFileUriValueTypeDef",
     "RemoveAttributesActivityOutputTypeDef",
     "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
-    "SampleChannelDataRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "BatchPutMessageRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "CreateDatasetContentResponseTypeDef",
     "CreatePipelineResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
-    "StartPipelineReprocessingRequestRequestTypeDef",
+    "MessageTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
     "ChannelStorageOutputTypeDef",
     "ChannelStorageTypeDef",
     "ChannelStorageSummaryTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
@@ -133,23 +130,28 @@
     "DatastorePartitionTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    "ListDatasetContentsRequestRequestTypeDef",
+    "SampleChannelDataRequestRequestTypeDef",
+    "StartPipelineReprocessingRequestRequestTypeDef",
     "VariableTypeDef",
     "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
+    "BatchPutMessageRequestRequestTypeDef",
     "ChannelTypeDef",
+    "ChannelStorageUnionTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ChannelSummaryTypeDef",
     "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
@@ -161,37 +163,42 @@
     "LateDataRuleTypeDef",
     "SqlQueryDatasetActionOutputTypeDef",
     "SqlQueryDatasetActionTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
     "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
     "PipelineTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
+    "PipelineActivityUnionTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
-    "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "FileFormatConfigurationOutputTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
+    "DatastoreStorageUnionTypeDef",
     "DatastoreSummaryTypeDef",
+    "DatastorePartitionsUnionTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
     "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
+    "UpdatePipelineRequestRequestTypeDef",
     "DatastoreTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
+    "FileFormatConfigurationUnionTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
     "ListDatastoresResponseTypeDef",
     "DatasetTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "UpdateDatasetRequestRequestTypeDef",
+    "DatasetActionUnionTypeDef",
     "DescribeDatastoreResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
 )
 
 _RequiredAddAttributesActivityOutputTypeDef = TypedDict(
     "_RequiredAddAttributesActivityOutputTypeDef",
     {
         "name": str,
         "attributes": Dict[str, str],
@@ -201,21 +208,19 @@
     "_OptionalAddAttributesActivityOutputTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class AddAttributesActivityOutputTypeDef(
     _RequiredAddAttributesActivityOutputTypeDef, _OptionalAddAttributesActivityOutputTypeDef
 ):
     pass
 
-
 _RequiredAddAttributesActivityTypeDef = TypedDict(
     "_RequiredAddAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
 )
@@ -223,50 +228,41 @@
     "_OptionalAddAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class AddAttributesActivityTypeDef(
     _RequiredAddAttributesActivityTypeDef, _OptionalAddAttributesActivityTypeDef
 ):
     pass
 
-
 BatchPutMessageErrorEntryTypeDef = TypedDict(
     "BatchPutMessageErrorEntryTypeDef",
     {
         "messageId": str,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-MessageTypeDef = TypedDict(
-    "MessageTypeDef",
-    {
-        "messageId": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "CancelPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
         "reprocessingId": str,
     },
 )
@@ -282,19 +278,17 @@
     "_OptionalChannelActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class ChannelActivityTypeDef(_RequiredChannelActivityTypeDef, _OptionalChannelActivityTypeDef):
     pass
 
-
 ChannelMessagesTypeDef = TypedDict(
     "ChannelMessagesTypeDef",
     {
         "s3Paths": Sequence[str],
     },
     total=False,
 )
@@ -319,21 +313,19 @@
     "_OptionalCustomerManagedChannelS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
-
 class CustomerManagedChannelS3StorageTypeDef(
     _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
-
 CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -383,22 +375,20 @@
     "_OptionalCreateDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
-
 class CreateDatasetContentRequestRequestTypeDef(
     _RequiredCreateDatasetContentRequestRequestTypeDef,
     _OptionalCreateDatasetContentRequestRequestTypeDef,
 ):
     pass
 
-
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "unlimited": bool,
         "maxVersions": int,
     },
     total=False,
@@ -425,22 +415,20 @@
     "_OptionalCustomerManagedDatastoreS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
-
 class CustomerManagedDatastoreS3StorageTypeDef(
     _RequiredCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
-
 DatasetActionSummaryTypeDef = TypedDict(
     "DatasetActionSummaryTypeDef",
     {
         "actionName": str,
         "actionType": DatasetActionTypeType,
     },
     total=False,
@@ -521,22 +509,20 @@
     "_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
-
 class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(
     _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
-
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "attributeName": str,
     },
 )
 
@@ -550,21 +536,19 @@
     "_OptionalTimestampPartitionTypeDef",
     {
         "timestampFormat": str,
     },
     total=False,
 )
 
-
 class TimestampPartitionTypeDef(
     _RequiredTimestampPartitionTypeDef, _OptionalTimestampPartitionTypeDef
 ):
     pass
 
-
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 
@@ -578,22 +562,20 @@
     "_OptionalDeleteDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
-
 class DeleteDatasetContentRequestRequestTypeDef(
     _RequiredDeleteDatasetContentRequestRequestTypeDef,
     _OptionalDeleteDatasetContentRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -636,21 +618,19 @@
     "_OptionalDescribeChannelRequestRequestTypeDef",
     {
         "includeStatistics": bool,
     },
     total=False,
 )
 
-
 class DescribeChannelRequestRequestTypeDef(
     _RequiredDescribeChannelRequestRequestTypeDef, _OptionalDescribeChannelRequestRequestTypeDef
 ):
     pass
 
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -664,21 +644,19 @@
     "_OptionalDescribeDatastoreRequestRequestTypeDef",
     {
         "includeStatistics": bool,
     },
     total=False,
 )
 
-
 class DescribeDatastoreRequestRequestTypeDef(
     _RequiredDescribeDatastoreRequestRequestTypeDef, _OptionalDescribeDatastoreRequestRequestTypeDef
 ):
     pass
 
-
 LoggingOptionsTypeDef = TypedDict(
     "LoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": Literal["ERROR"],
         "enabled": bool,
     },
@@ -704,21 +682,19 @@
     "_OptionalDeviceRegistryEnrichActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class DeviceRegistryEnrichActivityTypeDef(
     _RequiredDeviceRegistryEnrichActivityTypeDef, _OptionalDeviceRegistryEnrichActivityTypeDef
 ):
     pass
 
-
 _RequiredDeviceShadowEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceShadowEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -728,21 +704,19 @@
     "_OptionalDeviceShadowEnrichActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class DeviceShadowEnrichActivityTypeDef(
     _RequiredDeviceShadowEnrichActivityTypeDef, _OptionalDeviceShadowEnrichActivityTypeDef
 ):
     pass
 
-
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
 )
@@ -750,40 +724,36 @@
     "_OptionalFilterActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class FilterActivityTypeDef(_RequiredFilterActivityTypeDef, _OptionalFilterActivityTypeDef):
     pass
 
-
 _RequiredGetDatasetContentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDatasetContentRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalGetDatasetContentRequestRequestTypeDef = TypedDict(
     "_OptionalGetDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
-
 class GetDatasetContentRequestRequestTypeDef(
     _RequiredGetDatasetContentRequestRequestTypeDef, _OptionalGetDatasetContentRequestRequestTypeDef
 ):
     pass
 
-
 GlueConfigurationTypeDef = TypedDict(
     "GlueConfigurationTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
@@ -800,19 +770,17 @@
     "_OptionalLambdaActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class LambdaActivityTypeDef(_RequiredLambdaActivityTypeDef, _OptionalLambdaActivityTypeDef):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -824,39 +792,15 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestRequestTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class ListDatasetContentsRequestRequestTypeDef(
-    _RequiredListDatasetContentsRequestRequestTypeDef,
-    _OptionalListDatasetContentsRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -899,19 +843,17 @@
     "_OptionalMathActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class MathActivityTypeDef(_RequiredMathActivityTypeDef, _OptionalMathActivityTypeDef):
     pass
 
-
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
     },
 )
 
@@ -926,21 +868,19 @@
     "_OptionalRemoveAttributesActivityOutputTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class RemoveAttributesActivityOutputTypeDef(
     _RequiredRemoveAttributesActivityOutputTypeDef, _OptionalRemoveAttributesActivityOutputTypeDef
 ):
     pass
 
-
 _RequiredSelectAttributesActivityOutputTypeDef = TypedDict(
     "_RequiredSelectAttributesActivityOutputTypeDef",
     {
         "name": str,
         "attributes": List[str],
     },
 )
@@ -948,21 +888,19 @@
     "_OptionalSelectAttributesActivityOutputTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class SelectAttributesActivityOutputTypeDef(
     _RequiredSelectAttributesActivityOutputTypeDef, _OptionalSelectAttributesActivityOutputTypeDef
 ):
     pass
 
-
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -970,21 +908,19 @@
     "_OptionalRemoveAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class RemoveAttributesActivityTypeDef(
     _RequiredRemoveAttributesActivityTypeDef, _OptionalRemoveAttributesActivityTypeDef
 ):
     pass
 
-
 _RequiredSelectAttributesActivityTypeDef = TypedDict(
     "_RequiredSelectAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -992,70 +928,37 @@
     "_OptionalSelectAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class SelectAttributesActivityTypeDef(
     _RequiredSelectAttributesActivityTypeDef, _OptionalSelectAttributesActivityTypeDef
 ):
     pass
 
-
 ReprocessingSummaryTypeDef = TypedDict(
     "ReprocessingSummaryTypeDef",
     {
         "id": str,
         "status": ReprocessingStatusType,
         "creationTime": datetime,
     },
     total=False,
 )
 
-_RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
-    "_RequiredSampleChannelDataRequestRequestTypeDef",
-    {
-        "channelName": str,
-    },
-)
-_OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
-    "_OptionalSampleChannelDataRequestRequestTypeDef",
-    {
-        "maxMessages": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class SampleChannelDataRequestRequestTypeDef(
-    _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
-):
-    pass
-
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-BatchPutMessageRequestRequestTypeDef = TypedDict(
-    "BatchPutMessageRequestRequestTypeDef",
-    {
-        "channelName": str,
-        "messages": Sequence[MessageTypeDef],
-    },
-)
-
 BatchPutMessageResponseTypeDef = TypedDict(
     "BatchPutMessageResponseTypeDef",
     {
         "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1105,38 +1008,22 @@
     "StartPipelineReprocessingResponseTypeDef",
     {
         "reprocessingId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPipelineReprocessingRequestRequestTypeDef",
+MessageTypeDef = TypedDict(
+    "MessageTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "channelMessages": ChannelMessagesTypeDef,
+        "messageId": str,
+        "payload": BlobTypeDef,
     },
-    total=False,
 )
 
-
-class StartPipelineReprocessingRequestRequestTypeDef(
-    _RequiredStartPipelineReprocessingRequestRequestTypeDef,
-    _OptionalStartPipelineReprocessingRequestRequestTypeDef,
-):
-    pass
-
-
 ChannelStatisticsTypeDef = TypedDict(
     "ChannelStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
 )
@@ -1336,77 +1223,139 @@
     "_OptionalS3DestinationConfigurationTypeDef",
     {
         "glueConfiguration": GlueConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
-
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
     "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
     "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     {
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
+        "scheduledOnOrAfter": TimestampTypeDef,
+        "scheduledBefore": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
     _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
 ):
     pass
 
-
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+_RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "datasetName": str,
+    },
+)
+_OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+        "scheduledOnOrAfter": TimestampTypeDef,
+        "scheduledBefore": TimestampTypeDef,
     },
     total=False,
 )
 
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+class ListDatasetContentsRequestRequestTypeDef(
+    _RequiredListDatasetContentsRequestRequestTypeDef,
+    _OptionalListDatasetContentsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
+    "_RequiredSampleChannelDataRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "channelName": str,
+    },
+)
+_OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
+    "_OptionalSampleChannelDataRequestRequestTypeDef",
+    {
+        "maxMessages": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
     total=False,
 )
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+class SampleChannelDataRequestRequestTypeDef(
+    _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
+):
+    pass
+
+_RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "pipelineName": str,
+    },
+)
+_OptionalStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPipelineReprocessingRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "channelMessages": ChannelMessagesTypeDef,
     },
     total=False,
 )
 
+class StartPipelineReprocessingRequestRequestTypeDef(
+    _RequiredStartPipelineReprocessingRequestRequestTypeDef,
+    _OptionalStartPipelineReprocessingRequestRequestTypeDef,
+):
+    pass
+
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalVariableTypeDef = TypedDict(
@@ -1416,19 +1365,17 @@
         "doubleValue": float,
         "datasetContentVersionValue": DatasetContentVersionValueTypeDef,
         "outputFileUriValue": OutputFileUriValueTypeDef,
     },
     total=False,
 )
 
-
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
-
 PipelineActivityOutputTypeDef = TypedDict(
     "PipelineActivityOutputTypeDef",
     {
         "channel": ChannelActivityTypeDef,
         "lambda": LambdaActivityTypeDef,
         "datastore": DatastoreActivityTypeDef,
         "addAttributes": AddAttributesActivityOutputTypeDef,
@@ -1466,14 +1413,22 @@
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
+BatchPutMessageRequestRequestTypeDef = TypedDict(
+    "BatchPutMessageRequestRequestTypeDef",
+    {
+        "channelName": str,
+        "messages": Sequence[MessageTypeDef],
+    },
+)
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "name": str,
         "storage": ChannelStorageOutputTypeDef,
         "arn": str,
         "status": ChannelStatusType,
@@ -1481,14 +1436,15 @@
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
+ChannelStorageUnionTypeDef = Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef]
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalCreateChannelRequestRequestTypeDef = TypedDict(
@@ -1497,21 +1453,19 @@
         "channelStorage": ChannelStorageTypeDef,
         "retentionPeriod": RetentionPeriodTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
@@ -1519,21 +1473,19 @@
     {
         "channelStorage": ChannelStorageTypeDef,
         "retentionPeriod": RetentionPeriodTypeDef,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "channelName": str,
         "channelStorage": ChannelStorageSummaryTypeDef,
         "status": ChannelStatusType,
         "creationTime": datetime,
@@ -1637,61 +1589,55 @@
     "_OptionalLateDataRuleTypeDef",
     {
         "ruleName": str,
     },
     total=False,
 )
 
-
 class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
     pass
 
-
 _RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionOutputTypeDef",
     {
         "sqlQuery": str,
     },
 )
 _OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
     "_OptionalSqlQueryDatasetActionOutputTypeDef",
     {
         "filters": List[QueryFilterTypeDef],
     },
     total=False,
 )
 
-
 class SqlQueryDatasetActionOutputTypeDef(
     _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
 ):
     pass
 
-
 _RequiredSqlQueryDatasetActionTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionTypeDef",
     {
         "sqlQuery": str,
     },
 )
 _OptionalSqlQueryDatasetActionTypeDef = TypedDict(
     "_OptionalSqlQueryDatasetActionTypeDef",
     {
         "filters": Sequence[QueryFilterTypeDef],
     },
     total=False,
 )
 
-
 class SqlQueryDatasetActionTypeDef(
     _RequiredSqlQueryDatasetActionTypeDef, _OptionalSqlQueryDatasetActionTypeDef
 ):
     pass
 
-
 DatasetContentDeliveryDestinationTypeDef = TypedDict(
     "DatasetContentDeliveryDestinationTypeDef",
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
@@ -1709,21 +1655,19 @@
     "_OptionalContainerDatasetActionOutputTypeDef",
     {
         "variables": List[VariableTypeDef],
     },
     total=False,
 )
 
-
 class ContainerDatasetActionOutputTypeDef(
     _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
 ):
     pass
 
-
 _RequiredContainerDatasetActionTypeDef = TypedDict(
     "_RequiredContainerDatasetActionTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
         "resourceConfiguration": ResourceConfigurationTypeDef,
     },
@@ -1732,73 +1676,38 @@
     "_OptionalContainerDatasetActionTypeDef",
     {
         "variables": Sequence[VariableTypeDef],
     },
     total=False,
 )
 
-
 class ContainerDatasetActionTypeDef(
     _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
 ):
     pass
 
-
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "name": str,
         "arn": str,
         "activities": List[PipelineActivityOutputTypeDef],
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePipelineRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[
-            Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
-        ],
-    },
-)
-_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePipelineRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreatePipelineRequestRequestTypeDef(
-    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
-):
-    pass
-
-
+PipelineActivityUnionTypeDef = Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
 RunPipelineActivityRequestRequestTypeDef = TypedDict(
     "RunPipelineActivityRequestRequestTypeDef",
     {
         "pipelineActivity": PipelineActivityTypeDef,
-        "payloads": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-)
-
-UpdatePipelineRequestRequestTypeDef = TypedDict(
-    "UpdatePipelineRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[
-            Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
-        ],
+        "payloads": Sequence[BlobTypeDef],
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
@@ -1848,14 +1757,15 @@
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DatastoreStorageUnionTypeDef = Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef]
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
         "datastoreStorage": DatastoreStorageSummaryTypeDef,
         "status": DatastoreStatusType,
         "creationTime": datetime,
@@ -1863,35 +1773,36 @@
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
         "datastorePartitions": DatastorePartitionsOutputTypeDef,
     },
     total=False,
 )
 
+DatastorePartitionsUnionTypeDef = Union[
+    DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
+]
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_OptionalDatasetContentDeliveryRuleTypeDef",
     {
         "entryName": str,
     },
     total=False,
 )
 
-
 class DatasetContentDeliveryRuleTypeDef(
     _RequiredDatasetContentDeliveryRuleTypeDef, _OptionalDatasetContentDeliveryRuleTypeDef
 ):
     pass
 
-
 DatasetActionOutputTypeDef = TypedDict(
     "DatasetActionOutputTypeDef",
     {
         "actionName": str,
         "queryAction": SqlQueryDatasetActionOutputTypeDef,
         "containerAction": ContainerDatasetActionOutputTypeDef,
     },
@@ -1912,14 +1823,42 @@
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePipelineRequestRequestTypeDef",
+    {
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
+    },
+)
+_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePipelineRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreatePipelineRequestRequestTypeDef(
+    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
+):
+    pass
+
+UpdatePipelineRequestRequestTypeDef = TypedDict(
+    "UpdatePipelineRequestRequestTypeDef",
+    {
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
+    },
+)
+
 DatastoreTypeDef = TypedDict(
     "DatastoreTypeDef",
     {
         "name": str,
         "storage": DatastoreStorageOutputTypeDef,
         "arn": str,
         "status": DatastoreStatusType,
@@ -1947,21 +1886,22 @@
         "tags": Sequence[TagTypeDef],
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
         "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
-
 class CreateDatastoreRequestRequestTypeDef(
     _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
 ):
     pass
 
-
+FileFormatConfigurationUnionTypeDef = Union[
+    FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
+]
 _RequiredUpdateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalUpdateDatastoreRequestRequestTypeDef = TypedDict(
@@ -1970,21 +1910,19 @@
         "retentionPeriod": RetentionPeriodTypeDef,
         "datastoreStorage": DatastoreStorageTypeDef,
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDatastoreRequestRequestTypeDef(
     _RequiredUpdateDatastoreRequestRequestTypeDef, _OptionalUpdateDatastoreRequestRequestTypeDef
 ):
     pass
 
-
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2004,19 +1942,37 @@
         "retentionPeriod": RetentionPeriodTypeDef,
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "lateDataRules": List[LateDataRuleTypeDef],
     },
     total=False,
 )
 
+DatasetActionUnionTypeDef = Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]
+DescribeDatastoreResponseTypeDef = TypedDict(
+    "DescribeDatastoreResponseTypeDef",
+    {
+        "datastore": DatastoreTypeDef,
+        "statistics": DatastoreStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
+        "actions": Sequence[DatasetActionUnionTypeDef],
     },
 )
 _OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -2024,56 +1980,35 @@
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "tags": Sequence[TagTypeDef],
         "lateDataRules": Sequence[LateDataRuleTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
+        "actions": Sequence[DatasetActionUnionTypeDef],
     },
 )
 _OptionalUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
         "retentionPeriod": RetentionPeriodTypeDef,
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "lateDataRules": Sequence[LateDataRuleTypeDef],
     },
     total=False,
 )
 
-
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
-
-
-DescribeDatastoreResponseTypeDef = TypedDict(
-    "DescribeDatastoreResponseTypeDef",
-    {
-        "datastore": DatastoreTypeDef,
-        "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/type_defs.pyi` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotanalytics.type_defs import AddAttributesActivityOutputTypeDef
 
-    data: AddAttributesActivityOutputTypeDef = {...}
+    data: AddAttributesActivityOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -33,20 +33,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
-    "MessageTypeDef",
     "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     "RetentionPeriodTypeDef",
@@ -85,37 +86,35 @@
     "DeviceShadowEnrichActivityTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
     "GlueConfigurationTypeDef",
     "LambdaActivityTypeDef",
     "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListDatasetContentsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MathActivityTypeDef",
     "OutputFileUriValueTypeDef",
     "RemoveAttributesActivityOutputTypeDef",
     "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
-    "SampleChannelDataRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "BatchPutMessageRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "CreateDatasetContentResponseTypeDef",
     "CreatePipelineResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
-    "StartPipelineReprocessingRequestRequestTypeDef",
+    "MessageTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
     "ChannelStorageOutputTypeDef",
     "ChannelStorageTypeDef",
     "ChannelStorageSummaryTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
@@ -132,23 +131,28 @@
     "DatastorePartitionTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    "ListDatasetContentsRequestRequestTypeDef",
+    "SampleChannelDataRequestRequestTypeDef",
+    "StartPipelineReprocessingRequestRequestTypeDef",
     "VariableTypeDef",
     "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
+    "BatchPutMessageRequestRequestTypeDef",
     "ChannelTypeDef",
+    "ChannelStorageUnionTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ChannelSummaryTypeDef",
     "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
@@ -160,37 +164,42 @@
     "LateDataRuleTypeDef",
     "SqlQueryDatasetActionOutputTypeDef",
     "SqlQueryDatasetActionTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
     "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
     "PipelineTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
+    "PipelineActivityUnionTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
-    "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "FileFormatConfigurationOutputTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
+    "DatastoreStorageUnionTypeDef",
     "DatastoreSummaryTypeDef",
+    "DatastorePartitionsUnionTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
     "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
+    "UpdatePipelineRequestRequestTypeDef",
     "DatastoreTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
+    "FileFormatConfigurationUnionTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
     "ListDatastoresResponseTypeDef",
     "DatasetTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "UpdateDatasetRequestRequestTypeDef",
+    "DatasetActionUnionTypeDef",
     "DescribeDatastoreResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
 )
 
 _RequiredAddAttributesActivityOutputTypeDef = TypedDict(
     "_RequiredAddAttributesActivityOutputTypeDef",
     {
         "name": str,
         "attributes": Dict[str, str],
@@ -200,19 +209,21 @@
     "_OptionalAddAttributesActivityOutputTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class AddAttributesActivityOutputTypeDef(
     _RequiredAddAttributesActivityOutputTypeDef, _OptionalAddAttributesActivityOutputTypeDef
 ):
     pass
 
+
 _RequiredAddAttributesActivityTypeDef = TypedDict(
     "_RequiredAddAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
 )
@@ -220,48 +231,43 @@
     "_OptionalAddAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class AddAttributesActivityTypeDef(
     _RequiredAddAttributesActivityTypeDef, _OptionalAddAttributesActivityTypeDef
 ):
     pass
 
+
 BatchPutMessageErrorEntryTypeDef = TypedDict(
     "BatchPutMessageErrorEntryTypeDef",
     {
         "messageId": str,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-MessageTypeDef = TypedDict(
-    "MessageTypeDef",
-    {
-        "messageId": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "CancelPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
         "reprocessingId": str,
     },
 )
@@ -277,17 +283,19 @@
     "_OptionalChannelActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class ChannelActivityTypeDef(_RequiredChannelActivityTypeDef, _OptionalChannelActivityTypeDef):
     pass
 
+
 ChannelMessagesTypeDef = TypedDict(
     "ChannelMessagesTypeDef",
     {
         "s3Paths": Sequence[str],
     },
     total=False,
 )
@@ -312,19 +320,21 @@
     "_OptionalCustomerManagedChannelS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
+
 class CustomerManagedChannelS3StorageTypeDef(
     _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
+
 CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -374,20 +384,22 @@
     "_OptionalCreateDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
+
 class CreateDatasetContentRequestRequestTypeDef(
     _RequiredCreateDatasetContentRequestRequestTypeDef,
     _OptionalCreateDatasetContentRequestRequestTypeDef,
 ):
     pass
 
+
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "unlimited": bool,
         "maxVersions": int,
     },
     total=False,
@@ -414,20 +426,22 @@
     "_OptionalCustomerManagedDatastoreS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
+
 class CustomerManagedDatastoreS3StorageTypeDef(
     _RequiredCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
+
 DatasetActionSummaryTypeDef = TypedDict(
     "DatasetActionSummaryTypeDef",
     {
         "actionName": str,
         "actionType": DatasetActionTypeType,
     },
     total=False,
@@ -508,20 +522,22 @@
     "_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
+
 class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(
     _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
+
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "attributeName": str,
     },
 )
 
@@ -535,19 +551,21 @@
     "_OptionalTimestampPartitionTypeDef",
     {
         "timestampFormat": str,
     },
     total=False,
 )
 
+
 class TimestampPartitionTypeDef(
     _RequiredTimestampPartitionTypeDef, _OptionalTimestampPartitionTypeDef
 ):
     pass
 
+
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 
@@ -561,20 +579,22 @@
     "_OptionalDeleteDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
+
 class DeleteDatasetContentRequestRequestTypeDef(
     _RequiredDeleteDatasetContentRequestRequestTypeDef,
     _OptionalDeleteDatasetContentRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -617,19 +637,21 @@
     "_OptionalDescribeChannelRequestRequestTypeDef",
     {
         "includeStatistics": bool,
     },
     total=False,
 )
 
+
 class DescribeChannelRequestRequestTypeDef(
     _RequiredDescribeChannelRequestRequestTypeDef, _OptionalDescribeChannelRequestRequestTypeDef
 ):
     pass
 
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -643,19 +665,21 @@
     "_OptionalDescribeDatastoreRequestRequestTypeDef",
     {
         "includeStatistics": bool,
     },
     total=False,
 )
 
+
 class DescribeDatastoreRequestRequestTypeDef(
     _RequiredDescribeDatastoreRequestRequestTypeDef, _OptionalDescribeDatastoreRequestRequestTypeDef
 ):
     pass
 
+
 LoggingOptionsTypeDef = TypedDict(
     "LoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": Literal["ERROR"],
         "enabled": bool,
     },
@@ -681,19 +705,21 @@
     "_OptionalDeviceRegistryEnrichActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class DeviceRegistryEnrichActivityTypeDef(
     _RequiredDeviceRegistryEnrichActivityTypeDef, _OptionalDeviceRegistryEnrichActivityTypeDef
 ):
     pass
 
+
 _RequiredDeviceShadowEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceShadowEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -703,19 +729,21 @@
     "_OptionalDeviceShadowEnrichActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class DeviceShadowEnrichActivityTypeDef(
     _RequiredDeviceShadowEnrichActivityTypeDef, _OptionalDeviceShadowEnrichActivityTypeDef
 ):
     pass
 
+
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
 )
@@ -723,36 +751,40 @@
     "_OptionalFilterActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class FilterActivityTypeDef(_RequiredFilterActivityTypeDef, _OptionalFilterActivityTypeDef):
     pass
 
+
 _RequiredGetDatasetContentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDatasetContentRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalGetDatasetContentRequestRequestTypeDef = TypedDict(
     "_OptionalGetDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
+
 class GetDatasetContentRequestRequestTypeDef(
     _RequiredGetDatasetContentRequestRequestTypeDef, _OptionalGetDatasetContentRequestRequestTypeDef
 ):
     pass
 
+
 GlueConfigurationTypeDef = TypedDict(
     "GlueConfigurationTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
@@ -769,17 +801,19 @@
     "_OptionalLambdaActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class LambdaActivityTypeDef(_RequiredLambdaActivityTypeDef, _OptionalLambdaActivityTypeDef):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -791,37 +825,15 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestRequestTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-class ListDatasetContentsRequestRequestTypeDef(
-    _RequiredListDatasetContentsRequestRequestTypeDef,
-    _OptionalListDatasetContentsRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -864,17 +876,19 @@
     "_OptionalMathActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class MathActivityTypeDef(_RequiredMathActivityTypeDef, _OptionalMathActivityTypeDef):
     pass
 
+
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
     },
 )
 
@@ -889,19 +903,21 @@
     "_OptionalRemoveAttributesActivityOutputTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class RemoveAttributesActivityOutputTypeDef(
     _RequiredRemoveAttributesActivityOutputTypeDef, _OptionalRemoveAttributesActivityOutputTypeDef
 ):
     pass
 
+
 _RequiredSelectAttributesActivityOutputTypeDef = TypedDict(
     "_RequiredSelectAttributesActivityOutputTypeDef",
     {
         "name": str,
         "attributes": List[str],
     },
 )
@@ -909,19 +925,21 @@
     "_OptionalSelectAttributesActivityOutputTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class SelectAttributesActivityOutputTypeDef(
     _RequiredSelectAttributesActivityOutputTypeDef, _OptionalSelectAttributesActivityOutputTypeDef
 ):
     pass
 
+
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -929,19 +947,21 @@
     "_OptionalRemoveAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class RemoveAttributesActivityTypeDef(
     _RequiredRemoveAttributesActivityTypeDef, _OptionalRemoveAttributesActivityTypeDef
 ):
     pass
 
+
 _RequiredSelectAttributesActivityTypeDef = TypedDict(
     "_RequiredSelectAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -949,66 +969,39 @@
     "_OptionalSelectAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class SelectAttributesActivityTypeDef(
     _RequiredSelectAttributesActivityTypeDef, _OptionalSelectAttributesActivityTypeDef
 ):
     pass
 
+
 ReprocessingSummaryTypeDef = TypedDict(
     "ReprocessingSummaryTypeDef",
     {
         "id": str,
         "status": ReprocessingStatusType,
         "creationTime": datetime,
     },
     total=False,
 )
 
-_RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
-    "_RequiredSampleChannelDataRequestRequestTypeDef",
-    {
-        "channelName": str,
-    },
-)
-_OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
-    "_OptionalSampleChannelDataRequestRequestTypeDef",
-    {
-        "maxMessages": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class SampleChannelDataRequestRequestTypeDef(
-    _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
-):
-    pass
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-BatchPutMessageRequestRequestTypeDef = TypedDict(
-    "BatchPutMessageRequestRequestTypeDef",
-    {
-        "channelName": str,
-        "messages": Sequence[MessageTypeDef],
-    },
-)
-
 BatchPutMessageResponseTypeDef = TypedDict(
     "BatchPutMessageResponseTypeDef",
     {
         "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1058,36 +1051,22 @@
     "StartPipelineReprocessingResponseTypeDef",
     {
         "reprocessingId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPipelineReprocessingRequestRequestTypeDef",
+MessageTypeDef = TypedDict(
+    "MessageTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "channelMessages": ChannelMessagesTypeDef,
+        "messageId": str,
+        "payload": BlobTypeDef,
     },
-    total=False,
 )
 
-class StartPipelineReprocessingRequestRequestTypeDef(
-    _RequiredStartPipelineReprocessingRequestRequestTypeDef,
-    _OptionalStartPipelineReprocessingRequestRequestTypeDef,
-):
-    pass
-
 ChannelStatisticsTypeDef = TypedDict(
     "ChannelStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
 )
@@ -1287,73 +1266,149 @@
     "_OptionalS3DestinationConfigurationTypeDef",
     {
         "glueConfiguration": GlueConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
+
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
     "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
     "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     {
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
+        "scheduledOnOrAfter": TimestampTypeDef,
+        "scheduledBefore": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
     _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
 ):
     pass
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+
+_RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "datasetName": str,
+    },
+)
+_OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+        "scheduledOnOrAfter": TimestampTypeDef,
+        "scheduledBefore": TimestampTypeDef,
     },
     total=False,
 )
 
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+
+class ListDatasetContentsRequestRequestTypeDef(
+    _RequiredListDatasetContentsRequestRequestTypeDef,
+    _OptionalListDatasetContentsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
+    "_RequiredSampleChannelDataRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "channelName": str,
+    },
+)
+_OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
+    "_OptionalSampleChannelDataRequestRequestTypeDef",
+    {
+        "maxMessages": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
     total=False,
 )
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+
+class SampleChannelDataRequestRequestTypeDef(
+    _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "pipelineName": str,
+    },
+)
+_OptionalStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPipelineReprocessingRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "channelMessages": ChannelMessagesTypeDef,
     },
     total=False,
 )
 
+
+class StartPipelineReprocessingRequestRequestTypeDef(
+    _RequiredStartPipelineReprocessingRequestRequestTypeDef,
+    _OptionalStartPipelineReprocessingRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalVariableTypeDef = TypedDict(
@@ -1363,17 +1418,19 @@
         "doubleValue": float,
         "datasetContentVersionValue": DatasetContentVersionValueTypeDef,
         "outputFileUriValue": OutputFileUriValueTypeDef,
     },
     total=False,
 )
 
+
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
+
 PipelineActivityOutputTypeDef = TypedDict(
     "PipelineActivityOutputTypeDef",
     {
         "channel": ChannelActivityTypeDef,
         "lambda": LambdaActivityTypeDef,
         "datastore": DatastoreActivityTypeDef,
         "addAttributes": AddAttributesActivityOutputTypeDef,
@@ -1411,14 +1468,22 @@
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
+BatchPutMessageRequestRequestTypeDef = TypedDict(
+    "BatchPutMessageRequestRequestTypeDef",
+    {
+        "channelName": str,
+        "messages": Sequence[MessageTypeDef],
+    },
+)
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "name": str,
         "storage": ChannelStorageOutputTypeDef,
         "arn": str,
         "status": ChannelStatusType,
@@ -1426,14 +1491,15 @@
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
+ChannelStorageUnionTypeDef = Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef]
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalCreateChannelRequestRequestTypeDef = TypedDict(
@@ -1442,19 +1508,21 @@
         "channelStorage": ChannelStorageTypeDef,
         "retentionPeriod": RetentionPeriodTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
@@ -1462,19 +1530,21 @@
     {
         "channelStorage": ChannelStorageTypeDef,
         "retentionPeriod": RetentionPeriodTypeDef,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "channelName": str,
         "channelStorage": ChannelStorageSummaryTypeDef,
         "status": ChannelStatusType,
         "creationTime": datetime,
@@ -1578,55 +1648,61 @@
     "_OptionalLateDataRuleTypeDef",
     {
         "ruleName": str,
     },
     total=False,
 )
 
+
 class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
     pass
 
+
 _RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionOutputTypeDef",
     {
         "sqlQuery": str,
     },
 )
 _OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
     "_OptionalSqlQueryDatasetActionOutputTypeDef",
     {
         "filters": List[QueryFilterTypeDef],
     },
     total=False,
 )
 
+
 class SqlQueryDatasetActionOutputTypeDef(
     _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
 ):
     pass
 
+
 _RequiredSqlQueryDatasetActionTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionTypeDef",
     {
         "sqlQuery": str,
     },
 )
 _OptionalSqlQueryDatasetActionTypeDef = TypedDict(
     "_OptionalSqlQueryDatasetActionTypeDef",
     {
         "filters": Sequence[QueryFilterTypeDef],
     },
     total=False,
 )
 
+
 class SqlQueryDatasetActionTypeDef(
     _RequiredSqlQueryDatasetActionTypeDef, _OptionalSqlQueryDatasetActionTypeDef
 ):
     pass
 
+
 DatasetContentDeliveryDestinationTypeDef = TypedDict(
     "DatasetContentDeliveryDestinationTypeDef",
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
@@ -1644,19 +1720,21 @@
     "_OptionalContainerDatasetActionOutputTypeDef",
     {
         "variables": List[VariableTypeDef],
     },
     total=False,
 )
 
+
 class ContainerDatasetActionOutputTypeDef(
     _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
 ):
     pass
 
+
 _RequiredContainerDatasetActionTypeDef = TypedDict(
     "_RequiredContainerDatasetActionTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
         "resourceConfiguration": ResourceConfigurationTypeDef,
     },
@@ -1665,69 +1743,40 @@
     "_OptionalContainerDatasetActionTypeDef",
     {
         "variables": Sequence[VariableTypeDef],
     },
     total=False,
 )
 
+
 class ContainerDatasetActionTypeDef(
     _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
 ):
     pass
 
+
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "name": str,
         "arn": str,
         "activities": List[PipelineActivityOutputTypeDef],
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePipelineRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[
-            Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
-        ],
-    },
-)
-_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePipelineRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreatePipelineRequestRequestTypeDef(
-    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
-):
-    pass
-
+PipelineActivityUnionTypeDef = Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
 RunPipelineActivityRequestRequestTypeDef = TypedDict(
     "RunPipelineActivityRequestRequestTypeDef",
     {
         "pipelineActivity": PipelineActivityTypeDef,
-        "payloads": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-)
-
-UpdatePipelineRequestRequestTypeDef = TypedDict(
-    "UpdatePipelineRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[
-            Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
-        ],
+        "payloads": Sequence[BlobTypeDef],
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
@@ -1777,14 +1826,15 @@
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DatastoreStorageUnionTypeDef = Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef]
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
         "datastoreStorage": DatastoreStorageSummaryTypeDef,
         "status": DatastoreStatusType,
         "creationTime": datetime,
@@ -1792,33 +1842,38 @@
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
         "datastorePartitions": DatastorePartitionsOutputTypeDef,
     },
     total=False,
 )
 
+DatastorePartitionsUnionTypeDef = Union[
+    DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
+]
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_OptionalDatasetContentDeliveryRuleTypeDef",
     {
         "entryName": str,
     },
     total=False,
 )
 
+
 class DatasetContentDeliveryRuleTypeDef(
     _RequiredDatasetContentDeliveryRuleTypeDef, _OptionalDatasetContentDeliveryRuleTypeDef
 ):
     pass
 
+
 DatasetActionOutputTypeDef = TypedDict(
     "DatasetActionOutputTypeDef",
     {
         "actionName": str,
         "queryAction": SqlQueryDatasetActionOutputTypeDef,
         "containerAction": ContainerDatasetActionOutputTypeDef,
     },
@@ -1839,14 +1894,44 @@
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePipelineRequestRequestTypeDef",
+    {
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
+    },
+)
+_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePipelineRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreatePipelineRequestRequestTypeDef(
+    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
+):
+    pass
+
+
+UpdatePipelineRequestRequestTypeDef = TypedDict(
+    "UpdatePipelineRequestRequestTypeDef",
+    {
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
+    },
+)
+
 DatastoreTypeDef = TypedDict(
     "DatastoreTypeDef",
     {
         "name": str,
         "storage": DatastoreStorageOutputTypeDef,
         "arn": str,
         "status": DatastoreStatusType,
@@ -1874,19 +1959,24 @@
         "tags": Sequence[TagTypeDef],
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
         "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
+
 class CreateDatastoreRequestRequestTypeDef(
     _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
 ):
     pass
 
+
+FileFormatConfigurationUnionTypeDef = Union[
+    FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
+]
 _RequiredUpdateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalUpdateDatastoreRequestRequestTypeDef = TypedDict(
@@ -1895,19 +1985,21 @@
         "retentionPeriod": RetentionPeriodTypeDef,
         "datastoreStorage": DatastoreStorageTypeDef,
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDatastoreRequestRequestTypeDef(
     _RequiredUpdateDatastoreRequestRequestTypeDef, _OptionalUpdateDatastoreRequestRequestTypeDef
 ):
     pass
 
+
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1927,19 +2019,37 @@
         "retentionPeriod": RetentionPeriodTypeDef,
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "lateDataRules": List[LateDataRuleTypeDef],
     },
     total=False,
 )
 
+DatasetActionUnionTypeDef = Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]
+DescribeDatastoreResponseTypeDef = TypedDict(
+    "DescribeDatastoreResponseTypeDef",
+    {
+        "datastore": DatastoreTypeDef,
+        "statistics": DatastoreStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
+        "actions": Sequence[DatasetActionUnionTypeDef],
     },
 )
 _OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -1947,52 +2057,38 @@
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "tags": Sequence[TagTypeDef],
         "lateDataRules": Sequence[LateDataRuleTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
+        "actions": Sequence[DatasetActionUnionTypeDef],
     },
 )
 _OptionalUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
         "retentionPeriod": RetentionPeriodTypeDef,
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "lateDataRules": Sequence[LateDataRuleTypeDef],
     },
     total=False,
 )
 
+
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
-
-DescribeDatastoreResponseTypeDef = TypedDict(
-    "DescribeDatastoreResponseTypeDef",
-    {
-        "datastore": DatastoreTypeDef,
-        "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/PKG-INFO` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotanalytics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTAnalytics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotanalytics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotanalytics)](https://pepy.tech/project/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
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
@@ -335,28 +335,28 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotanalytics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
     AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
-    MessageTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
     CustomerManagedChannelS3StorageSummaryTypeDef,
     RetentionPeriodTypeDef,
@@ -395,37 +395,35 @@
     DeviceShadowEnrichActivityTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
     GlueConfigurationTypeDef,
     LambdaActivityTypeDef,
     PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListDatasetContentsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListDatastoresRequestRequestTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MathActivityTypeDef,
     OutputFileUriValueTypeDef,
     RemoveAttributesActivityOutputTypeDef,
     SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    SampleChannelDataRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreatePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
-    StartPipelineReprocessingRequestRequestTypeDef,
+    MessageTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
     ChannelStorageOutputTypeDef,
     ChannelStorageTypeDef,
     ChannelStorageSummaryTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
@@ -442,23 +440,28 @@
     DatastorePartitionTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    ListDatasetContentsRequestRequestTypeDef,
+    SampleChannelDataRequestRequestTypeDef,
+    StartPipelineReprocessingRequestRequestTypeDef,
     VariableTypeDef,
     PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
+    BatchPutMessageRequestRequestTypeDef,
     ChannelTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ChannelSummaryTypeDef,
     ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
@@ -470,41 +473,46 @@
     LateDataRuleTypeDef,
     SqlQueryDatasetActionOutputTypeDef,
     SqlQueryDatasetActionTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
     ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
     PipelineTypeDef,
-    CreatePipelineRequestRequestTypeDef,
+    PipelineActivityUnionTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ListChannelsResponseTypeDef,
     FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
+    DatastoreStorageUnionTypeDef,
     DatastoreSummaryTypeDef,
+    DatastorePartitionsUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
+    CreatePipelineRequestRequestTypeDef,
+    UpdatePipelineRequestRequestTypeDef,
     DatastoreTypeDef,
     CreateDatastoreRequestRequestTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
     ListDatastoresResponseTypeDef,
     DatasetTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    UpdateDatasetRequestRequestTypeDef,
+    DatasetActionUnionTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    UpdateDatasetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddAttributesActivityOutputTypeDef:
+def get_value() -> AddAttributesActivityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/SOURCES.txt` & `mypy-boto3-iotanalytics-1.28.16/mypy_boto3_iotanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15.post1/setup.py` & `mypy-boto3-iotanalytics-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotanalytics",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iotanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.IoTAnalytics 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 iotanalytics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iotanalytics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iotanalytics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

