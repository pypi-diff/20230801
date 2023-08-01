# Comparing `tmp/mypy-boto3-kinesis-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-kinesis-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:26 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-1.28.16.tar", last modified: Tue Aug  1 11:37:06 2023, max compression
```

## Comparing `mypy-boto3-kinesis-1.28.15.post1.tar` & `mypy-boto3-kinesis-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.965216 mypy-boto3-kinesis-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:47.000000 mypy-boto3-kinesis-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16885 2023-07-29 10:03:26.957217 mypy-boto3-kinesis-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-07-29 09:48:47.000000 mypy-boto3-kinesis-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.949216 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-29 09:48:47.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-29 09:48:47.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:48:47.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24849 2023-07-29 09:48:48.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-07-29 09:48:47.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-07-29 09:48:48.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-29 09:48:48.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-29 09:48:48.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-29 09:48:48.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:47.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31886 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31825 2023-07-29 09:48:48.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:47.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-29 09:48:48.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-29 09:48:48.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.957217 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16885 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:26.965216 mypy-boto3-kinesis-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:48:47.000000 mypy-boto3-kinesis-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.960851 mypy-boto3-kinesis-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-08-01 11:37:06.960851 mypy-boto3-kinesis-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.952851 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24761 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-08-01 11:21:35.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-08-01 11:21:35.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31935 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31874 2023-08-01 11:21:35.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.960851 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:06.960851 mypy-boto3-kinesis-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:21:34.000000 mypy-boto3-kinesis-1.28.16/setup.py
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/LICENSE` & `mypy-boto3-kinesis-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.15.post1/PKG-INFO` & `mypy-boto3-kinesis-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Kinesis 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Kinesis 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesis type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesis type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis)](https://pepy.tech/project/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
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
@@ -354,24 +354,25 @@
 )
 
 
 def check_value(value: ConsumerStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesis.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesis.type_defs import (
     AddTagsToStreamInputRequestTypeDef,
+    BlobTypeDef,
     HashKeyRangeTypeDef,
     ConsumerDescriptionTypeDef,
     ConsumerTypeDef,
     StreamModeDetailsTypeDef,
     DecreaseStreamRetentionPeriodInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     DeregisterStreamConsumerInputRequestTypeDef,
@@ -382,81 +383,82 @@
     WaiterConfigTypeDef,
     DescribeStreamSummaryInputRequestTypeDef,
     DisableEnhancedMonitoringInputRequestTypeDef,
     EnableEnhancedMonitoringInputRequestTypeDef,
     EnhancedMetricsTypeDef,
     GetRecordsInputRequestTypeDef,
     RecordTypeDef,
-    GetShardIteratorInputRequestTypeDef,
+    TimestampTypeDef,
     IncreaseStreamRetentionPeriodInputRequestTypeDef,
     InternalFailureExceptionTypeDef,
     KMSAccessDeniedExceptionTypeDef,
     KMSDisabledExceptionTypeDef,
     KMSInvalidStateExceptionTypeDef,
     KMSNotFoundExceptionTypeDef,
     KMSOptInRequiredTypeDef,
     KMSThrottlingExceptionTypeDef,
-    ShardFilterTypeDef,
-    ListStreamConsumersInputRequestTypeDef,
     ListStreamsInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     TagTypeDef,
     MergeShardsInputRequestTypeDef,
-    PutRecordInputRequestTypeDef,
-    PutRecordsRequestEntryTypeDef,
     PutRecordsResultEntryTypeDef,
     RegisterStreamConsumerInputRequestTypeDef,
     RemoveTagsFromStreamInputRequestTypeDef,
     ResourceInUseExceptionTypeDef,
     ResourceNotFoundExceptionTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
-    StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
     UpdateShardCountInputRequestTypeDef,
+    PutRecordInputRequestTypeDef,
+    PutRecordsRequestEntryTypeDef,
     ChildShardTypeDef,
     CreateStreamInputRequestTypeDef,
     StreamSummaryTypeDef,
     UpdateStreamModeInputRequestTypeDef,
     DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EnhancedMonitoringOutputTypeDef,
     GetShardIteratorOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
     PutRecordOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
     UpdateShardCountOutputTypeDef,
     DescribeStreamInputDescribeStreamPaginateTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
     StreamDescriptionSummaryTypeDef,
-    ListShardsInputListShardsPaginateTypeDef,
-    ListShardsInputRequestTypeDef,
+    GetShardIteratorInputRequestTypeDef,
+    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    ListStreamConsumersInputRequestTypeDef,
+    ShardFilterTypeDef,
+    StartingPositionTypeDef,
     ListTagsForStreamOutputTypeDef,
-    PutRecordsInputRequestTypeDef,
     PutRecordsOutputTypeDef,
     ShardTypeDef,
-    SubscribeToShardInputRequestTypeDef,
+    PutRecordsInputRequestTypeDef,
     GetRecordsOutputTypeDef,
     SubscribeToShardEventTypeDef,
     ListStreamsOutputTypeDef,
     DescribeStreamSummaryOutputTypeDef,
+    ListShardsInputListShardsPaginateTypeDef,
+    ListShardsInputRequestTypeDef,
+    SubscribeToShardInputRequestTypeDef,
     ListShardsOutputTypeDef,
     StreamDescriptionTypeDef,
     SubscribeToShardEventStreamTypeDef,
     DescribeStreamOutputTypeDef,
     SubscribeToShardOutputTypeDef,
 )
 
 
-def get_structure() -> AddTagsToStreamInputRequestTypeDef:
+def get_value() -> AddTagsToStreamInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/README.md` & `mypy-boto3-kinesis-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis)](https://pepy.tech/project/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
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
@@ -322,24 +322,25 @@
 )
 
 
 def check_value(value: ConsumerStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesis.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesis.type_defs import (
     AddTagsToStreamInputRequestTypeDef,
+    BlobTypeDef,
     HashKeyRangeTypeDef,
     ConsumerDescriptionTypeDef,
     ConsumerTypeDef,
     StreamModeDetailsTypeDef,
     DecreaseStreamRetentionPeriodInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     DeregisterStreamConsumerInputRequestTypeDef,
@@ -350,81 +351,82 @@
     WaiterConfigTypeDef,
     DescribeStreamSummaryInputRequestTypeDef,
     DisableEnhancedMonitoringInputRequestTypeDef,
     EnableEnhancedMonitoringInputRequestTypeDef,
     EnhancedMetricsTypeDef,
     GetRecordsInputRequestTypeDef,
     RecordTypeDef,
-    GetShardIteratorInputRequestTypeDef,
+    TimestampTypeDef,
     IncreaseStreamRetentionPeriodInputRequestTypeDef,
     InternalFailureExceptionTypeDef,
     KMSAccessDeniedExceptionTypeDef,
     KMSDisabledExceptionTypeDef,
     KMSInvalidStateExceptionTypeDef,
     KMSNotFoundExceptionTypeDef,
     KMSOptInRequiredTypeDef,
     KMSThrottlingExceptionTypeDef,
-    ShardFilterTypeDef,
-    ListStreamConsumersInputRequestTypeDef,
     ListStreamsInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     TagTypeDef,
     MergeShardsInputRequestTypeDef,
-    PutRecordInputRequestTypeDef,
-    PutRecordsRequestEntryTypeDef,
     PutRecordsResultEntryTypeDef,
     RegisterStreamConsumerInputRequestTypeDef,
     RemoveTagsFromStreamInputRequestTypeDef,
     ResourceInUseExceptionTypeDef,
     ResourceNotFoundExceptionTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
-    StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
     UpdateShardCountInputRequestTypeDef,
+    PutRecordInputRequestTypeDef,
+    PutRecordsRequestEntryTypeDef,
     ChildShardTypeDef,
     CreateStreamInputRequestTypeDef,
     StreamSummaryTypeDef,
     UpdateStreamModeInputRequestTypeDef,
     DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EnhancedMonitoringOutputTypeDef,
     GetShardIteratorOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
     PutRecordOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
     UpdateShardCountOutputTypeDef,
     DescribeStreamInputDescribeStreamPaginateTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
     StreamDescriptionSummaryTypeDef,
-    ListShardsInputListShardsPaginateTypeDef,
-    ListShardsInputRequestTypeDef,
+    GetShardIteratorInputRequestTypeDef,
+    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    ListStreamConsumersInputRequestTypeDef,
+    ShardFilterTypeDef,
+    StartingPositionTypeDef,
     ListTagsForStreamOutputTypeDef,
-    PutRecordsInputRequestTypeDef,
     PutRecordsOutputTypeDef,
     ShardTypeDef,
-    SubscribeToShardInputRequestTypeDef,
+    PutRecordsInputRequestTypeDef,
     GetRecordsOutputTypeDef,
     SubscribeToShardEventTypeDef,
     ListStreamsOutputTypeDef,
     DescribeStreamSummaryOutputTypeDef,
+    ListShardsInputListShardsPaginateTypeDef,
+    ListShardsInputRequestTypeDef,
+    SubscribeToShardInputRequestTypeDef,
     ListShardsOutputTypeDef,
     StreamDescriptionTypeDef,
     SubscribeToShardEventStreamTypeDef,
     DescribeStreamOutputTypeDef,
     SubscribeToShardOutputTypeDef,
 )
 
 
-def get_structure() -> AddTagsToStreamInputRequestTypeDef:
+def get_value() -> AddTagsToStreamInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/__init__.py` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/__init__.pyi` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/__main__.py` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kinesis 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Kinesis 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis\nOther"
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

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/client.py` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,27 @@
     from mypy_boto3_kinesis.client import KinesisClient
 
     session = Session()
     client: KinesisClient = session.client("kinesis")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import EncryptionTypeType, MetricsNameType, ShardIteratorTypeType
 from .paginator import (
     DescribeStreamPaginator,
     ListShardsPaginator,
     ListStreamConsumersPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
     DescribeStreamOutputTypeDef,
     DescribeStreamSummaryOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EnhancedMonitoringOutputTypeDef,
     GetRecordsOutputTypeDef,
@@ -44,14 +43,15 @@
     PutRecordsOutputTypeDef,
     PutRecordsRequestEntryTypeDef,
     RegisterStreamConsumerOutputTypeDef,
     ShardFilterTypeDef,
     StartingPositionTypeDef,
     StreamModeDetailsTypeDef,
     SubscribeToShardOutputTypeDef,
+    TimestampTypeDef,
     UpdateShardCountOutputTypeDef,
 )
 from .waiter import StreamExistsWaiter, StreamNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -277,15 +277,15 @@
     def get_shard_iterator(
         self,
         *,
         ShardId: str,
         ShardIteratorType: ShardIteratorTypeType,
         StreamName: str = ...,
         StartingSequenceNumber: str = ...,
-        Timestamp: Union[datetime, str] = ...,
+        Timestamp: TimestampTypeDef = ...,
         StreamARN: str = ...
     ) -> GetShardIteratorOutputTypeDef:
         """
         Gets an Amazon Kinesis shard iterator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.get_shard_iterator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/client/#get_shard_iterator)
@@ -305,15 +305,15 @@
     def list_shards(
         self,
         *,
         StreamName: str = ...,
         NextToken: str = ...,
         ExclusiveStartShardId: str = ...,
         MaxResults: int = ...,
-        StreamCreationTimestamp: Union[datetime, str] = ...,
+        StreamCreationTimestamp: TimestampTypeDef = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...
     ) -> ListShardsOutputTypeDef:
         """
         Lists the shards in a stream and provides information about each shard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_shards)
@@ -322,15 +322,15 @@
 
     def list_stream_consumers(
         self,
         *,
         StreamARN: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StreamCreationTimestamp: Union[datetime, str] = ...
+        StreamCreationTimestamp: TimestampTypeDef = ...
     ) -> ListStreamConsumersOutputTypeDef:
         """
         Lists the consumers registered to receive data from a stream using enhanced fan-
         out, and provides information about each consumer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_stream_consumers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/client/#list_stream_consumers)
@@ -376,15 +376,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.merge_shards)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/client/#merge_shards)
         """
 
     def put_record(
         self,
         *,
-        Data: Union[str, bytes, IO[Any], StreamingBody],
+        Data: BlobTypeDef,
         PartitionKey: str,
         StreamName: str = ...,
         ExplicitHashKey: str = ...,
         SequenceNumberForOrdering: str = ...,
         StreamARN: str = ...
     ) -> PutRecordOutputTypeDef:
         """
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/client.pyi` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,27 @@
     from mypy_boto3_kinesis.client import KinesisClient
 
     session = Session()
     client: KinesisClient = session.client("kinesis")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import EncryptionTypeType, MetricsNameType, ShardIteratorTypeType
 from .paginator import (
     DescribeStreamPaginator,
     ListShardsPaginator,
     ListStreamConsumersPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
     DescribeStreamOutputTypeDef,
     DescribeStreamSummaryOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EnhancedMonitoringOutputTypeDef,
     GetRecordsOutputTypeDef,
@@ -44,14 +43,15 @@
     PutRecordsOutputTypeDef,
     PutRecordsRequestEntryTypeDef,
     RegisterStreamConsumerOutputTypeDef,
     ShardFilterTypeDef,
     StartingPositionTypeDef,
     StreamModeDetailsTypeDef,
     SubscribeToShardOutputTypeDef,
+    TimestampTypeDef,
     UpdateShardCountOutputTypeDef,
 )
 from .waiter import StreamExistsWaiter, StreamNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -257,15 +257,15 @@
     def get_shard_iterator(
         self,
         *,
         ShardId: str,
         ShardIteratorType: ShardIteratorTypeType,
         StreamName: str = ...,
         StartingSequenceNumber: str = ...,
-        Timestamp: Union[datetime, str] = ...,
+        Timestamp: TimestampTypeDef = ...,
         StreamARN: str = ...
     ) -> GetShardIteratorOutputTypeDef:
         """
         Gets an Amazon Kinesis shard iterator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.get_shard_iterator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/client/#get_shard_iterator)
@@ -283,15 +283,15 @@
     def list_shards(
         self,
         *,
         StreamName: str = ...,
         NextToken: str = ...,
         ExclusiveStartShardId: str = ...,
         MaxResults: int = ...,
-        StreamCreationTimestamp: Union[datetime, str] = ...,
+        StreamCreationTimestamp: TimestampTypeDef = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...
     ) -> ListShardsOutputTypeDef:
         """
         Lists the shards in a stream and provides information about each shard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_shards)
@@ -299,15 +299,15 @@
         """
     def list_stream_consumers(
         self,
         *,
         StreamARN: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StreamCreationTimestamp: Union[datetime, str] = ...
+        StreamCreationTimestamp: TimestampTypeDef = ...
     ) -> ListStreamConsumersOutputTypeDef:
         """
         Lists the consumers registered to receive data from a stream using enhanced fan-
         out, and provides information about each consumer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_stream_consumers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/client/#list_stream_consumers)
@@ -349,15 +349,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.merge_shards)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/client/#merge_shards)
         """
     def put_record(
         self,
         *,
-        Data: Union[str, bytes, IO[Any], StreamingBody],
+        Data: BlobTypeDef,
         PartitionKey: str,
         StreamName: str = ...,
         ExplicitHashKey: str = ...,
         SequenceNumberForOrdering: str = ...,
         StreamARN: str = ...
     ) -> PutRecordOutputTypeDef:
         """
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/literals.py` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/literals.pyi` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/paginator.py` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
     describe_stream_paginator: DescribeStreamPaginator = client.get_paginator("describe_stream")
     list_shards_paginator: ListShardsPaginator = client.get_paginator("list_shards")
     list_stream_consumers_paginator: ListStreamConsumersPaginator = client.get_paginator("list_stream_consumers")
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeStreamOutputTypeDef,
     ListShardsOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
     ListStreamsOutputTypeDef,
     PaginatorConfigTypeDef,
     ShardFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeStreamPaginator",
     "ListShardsPaginator",
     "ListStreamConsumersPaginator",
     "ListStreamsPaginator",
@@ -83,15 +83,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartShardId: str = ...,
-        StreamCreationTimestamp: Union[datetime, str] = ...,
+        StreamCreationTimestamp: TimestampTypeDef = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListShardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListShards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#listshardspaginator)
@@ -104,15 +104,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamconsumerspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamARN: str,
-        StreamCreationTimestamp: Union[datetime, str] = ...,
+        StreamCreationTimestamp: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamConsumersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreamConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamconsumerspaginator)
         """
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/paginator.pyi` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
     describe_stream_paginator: DescribeStreamPaginator = client.get_paginator("describe_stream")
     list_shards_paginator: ListShardsPaginator = client.get_paginator("list_shards")
     list_stream_consumers_paginator: ListStreamConsumersPaginator = client.get_paginator("list_stream_consumers")
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeStreamOutputTypeDef,
     ListShardsOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
     ListStreamsOutputTypeDef,
     PaginatorConfigTypeDef,
     ShardFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeStreamPaginator",
     "ListShardsPaginator",
     "ListStreamConsumersPaginator",
     "ListStreamsPaginator",
@@ -79,15 +79,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartShardId: str = ...,
-        StreamCreationTimestamp: Union[datetime, str] = ...,
+        StreamCreationTimestamp: TimestampTypeDef = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListShardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListShards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#listshardspaginator)
@@ -99,15 +99,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamconsumerspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamARN: str,
-        StreamCreationTimestamp: Union[datetime, str] = ...,
+        StreamCreationTimestamp: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamConsumersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreamConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamconsumerspaginator)
         """
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/type_defs.py` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesis.type_defs import AddTagsToStreamInputRequestTypeDef
 
-    data: AddTagsToStreamInputRequestTypeDef = {...}
+    data: AddTagsToStreamInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.eventstream import EventStream
@@ -36,14 +36,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddTagsToStreamInputRequestTypeDef",
+    "BlobTypeDef",
     "HashKeyRangeTypeDef",
     "ConsumerDescriptionTypeDef",
     "ConsumerTypeDef",
     "StreamModeDetailsTypeDef",
     "DecreaseStreamRetentionPeriodInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "DeregisterStreamConsumerInputRequestTypeDef",
@@ -54,72 +55,73 @@
     "WaiterConfigTypeDef",
     "DescribeStreamSummaryInputRequestTypeDef",
     "DisableEnhancedMonitoringInputRequestTypeDef",
     "EnableEnhancedMonitoringInputRequestTypeDef",
     "EnhancedMetricsTypeDef",
     "GetRecordsInputRequestTypeDef",
     "RecordTypeDef",
-    "GetShardIteratorInputRequestTypeDef",
+    "TimestampTypeDef",
     "IncreaseStreamRetentionPeriodInputRequestTypeDef",
     "InternalFailureExceptionTypeDef",
     "KMSAccessDeniedExceptionTypeDef",
     "KMSDisabledExceptionTypeDef",
     "KMSInvalidStateExceptionTypeDef",
     "KMSNotFoundExceptionTypeDef",
     "KMSOptInRequiredTypeDef",
     "KMSThrottlingExceptionTypeDef",
-    "ShardFilterTypeDef",
-    "ListStreamConsumersInputRequestTypeDef",
     "ListStreamsInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "TagTypeDef",
     "MergeShardsInputRequestTypeDef",
-    "PutRecordInputRequestTypeDef",
-    "PutRecordsRequestEntryTypeDef",
     "PutRecordsResultEntryTypeDef",
     "RegisterStreamConsumerInputRequestTypeDef",
     "RemoveTagsFromStreamInputRequestTypeDef",
     "ResourceInUseExceptionTypeDef",
     "ResourceNotFoundExceptionTypeDef",
     "SequenceNumberRangeTypeDef",
     "SplitShardInputRequestTypeDef",
     "StartStreamEncryptionInputRequestTypeDef",
-    "StartingPositionTypeDef",
     "StopStreamEncryptionInputRequestTypeDef",
     "UpdateShardCountInputRequestTypeDef",
+    "PutRecordInputRequestTypeDef",
+    "PutRecordsRequestEntryTypeDef",
     "ChildShardTypeDef",
     "CreateStreamInputRequestTypeDef",
     "StreamSummaryTypeDef",
     "UpdateStreamModeInputRequestTypeDef",
     "DescribeLimitsOutputTypeDef",
     "DescribeStreamConsumerOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnhancedMonitoringOutputTypeDef",
     "GetShardIteratorOutputTypeDef",
     "ListStreamConsumersOutputTypeDef",
     "PutRecordOutputTypeDef",
     "RegisterStreamConsumerOutputTypeDef",
     "UpdateShardCountOutputTypeDef",
     "DescribeStreamInputDescribeStreamPaginateTypeDef",
-    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "DescribeStreamInputStreamExistsWaitTypeDef",
     "DescribeStreamInputStreamNotExistsWaitTypeDef",
     "StreamDescriptionSummaryTypeDef",
-    "ListShardsInputListShardsPaginateTypeDef",
-    "ListShardsInputRequestTypeDef",
+    "GetShardIteratorInputRequestTypeDef",
+    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    "ListStreamConsumersInputRequestTypeDef",
+    "ShardFilterTypeDef",
+    "StartingPositionTypeDef",
     "ListTagsForStreamOutputTypeDef",
-    "PutRecordsInputRequestTypeDef",
     "PutRecordsOutputTypeDef",
     "ShardTypeDef",
-    "SubscribeToShardInputRequestTypeDef",
+    "PutRecordsInputRequestTypeDef",
     "GetRecordsOutputTypeDef",
     "SubscribeToShardEventTypeDef",
     "ListStreamsOutputTypeDef",
     "DescribeStreamSummaryOutputTypeDef",
+    "ListShardsInputListShardsPaginateTypeDef",
+    "ListShardsInputRequestTypeDef",
+    "SubscribeToShardInputRequestTypeDef",
     "ListShardsOutputTypeDef",
     "StreamDescriptionTypeDef",
     "SubscribeToShardEventStreamTypeDef",
     "DescribeStreamOutputTypeDef",
     "SubscribeToShardOutputTypeDef",
 )
 
@@ -141,14 +143,15 @@
 
 class AddTagsToStreamInputRequestTypeDef(
     _RequiredAddTagsToStreamInputRequestTypeDef, _OptionalAddTagsToStreamInputRequestTypeDef
 ):
     pass
 
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 HashKeyRangeTypeDef = TypedDict(
     "HashKeyRangeTypeDef",
     {
         "StartingHashKey": str,
         "EndingHashKey": str,
     },
 )
@@ -378,39 +381,15 @@
 )
 
 
 class RecordTypeDef(_RequiredRecordTypeDef, _OptionalRecordTypeDef):
     pass
 
 
-_RequiredGetShardIteratorInputRequestTypeDef = TypedDict(
-    "_RequiredGetShardIteratorInputRequestTypeDef",
-    {
-        "ShardId": str,
-        "ShardIteratorType": ShardIteratorTypeType,
-    },
-)
-_OptionalGetShardIteratorInputRequestTypeDef = TypedDict(
-    "_OptionalGetShardIteratorInputRequestTypeDef",
-    {
-        "StreamName": str,
-        "StartingSequenceNumber": str,
-        "Timestamp": Union[datetime, str],
-        "StreamARN": str,
-    },
-    total=False,
-)
-
-
-class GetShardIteratorInputRequestTypeDef(
-    _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
     "_RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef",
     {
         "RetentionPeriodHours": int,
     },
 )
 _OptionalIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
@@ -482,57 +461,14 @@
     "KMSThrottlingExceptionTypeDef",
     {
         "message": str,
     },
     total=False,
 )
 
-_RequiredShardFilterTypeDef = TypedDict(
-    "_RequiredShardFilterTypeDef",
-    {
-        "Type": ShardFilterTypeType,
-    },
-)
-_OptionalShardFilterTypeDef = TypedDict(
-    "_OptionalShardFilterTypeDef",
-    {
-        "ShardId": str,
-        "Timestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class ShardFilterTypeDef(_RequiredShardFilterTypeDef, _OptionalShardFilterTypeDef):
-    pass
-
-
-_RequiredListStreamConsumersInputRequestTypeDef = TypedDict(
-    "_RequiredListStreamConsumersInputRequestTypeDef",
-    {
-        "StreamARN": str,
-    },
-)
-_OptionalListStreamConsumersInputRequestTypeDef = TypedDict(
-    "_OptionalListStreamConsumersInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StreamCreationTimestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class ListStreamConsumersInputRequestTypeDef(
-    _RequiredListStreamConsumersInputRequestTypeDef, _OptionalListStreamConsumersInputRequestTypeDef
-):
-    pass
-
-
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
         "Limit": int,
         "ExclusiveStartStreamName": str,
         "NextToken": str,
     },
@@ -588,61 +524,14 @@
 
 class MergeShardsInputRequestTypeDef(
     _RequiredMergeShardsInputRequestTypeDef, _OptionalMergeShardsInputRequestTypeDef
 ):
     pass
 
 
-_RequiredPutRecordInputRequestTypeDef = TypedDict(
-    "_RequiredPutRecordInputRequestTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-        "PartitionKey": str,
-    },
-)
-_OptionalPutRecordInputRequestTypeDef = TypedDict(
-    "_OptionalPutRecordInputRequestTypeDef",
-    {
-        "StreamName": str,
-        "ExplicitHashKey": str,
-        "SequenceNumberForOrdering": str,
-        "StreamARN": str,
-    },
-    total=False,
-)
-
-
-class PutRecordInputRequestTypeDef(
-    _RequiredPutRecordInputRequestTypeDef, _OptionalPutRecordInputRequestTypeDef
-):
-    pass
-
-
-_RequiredPutRecordsRequestEntryTypeDef = TypedDict(
-    "_RequiredPutRecordsRequestEntryTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-        "PartitionKey": str,
-    },
-)
-_OptionalPutRecordsRequestEntryTypeDef = TypedDict(
-    "_OptionalPutRecordsRequestEntryTypeDef",
-    {
-        "ExplicitHashKey": str,
-    },
-    total=False,
-)
-
-
-class PutRecordsRequestEntryTypeDef(
-    _RequiredPutRecordsRequestEntryTypeDef, _OptionalPutRecordsRequestEntryTypeDef
-):
-    pass
-
-
 PutRecordsResultEntryTypeDef = TypedDict(
     "PutRecordsResultEntryTypeDef",
     {
         "SequenceNumber": str,
         "ShardId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
@@ -761,34 +650,14 @@
 class StartStreamEncryptionInputRequestTypeDef(
     _RequiredStartStreamEncryptionInputRequestTypeDef,
     _OptionalStartStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredStartingPositionTypeDef = TypedDict(
-    "_RequiredStartingPositionTypeDef",
-    {
-        "Type": ShardIteratorTypeType,
-    },
-)
-_OptionalStartingPositionTypeDef = TypedDict(
-    "_OptionalStartingPositionTypeDef",
-    {
-        "SequenceNumber": str,
-        "Timestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class StartingPositionTypeDef(_RequiredStartingPositionTypeDef, _OptionalStartingPositionTypeDef):
-    pass
-
-
 _RequiredStopStreamEncryptionInputRequestTypeDef = TypedDict(
     "_RequiredStopStreamEncryptionInputRequestTypeDef",
     {
         "EncryptionType": EncryptionTypeType,
         "KeyId": str,
     },
 )
@@ -828,14 +697,61 @@
 
 class UpdateShardCountInputRequestTypeDef(
     _RequiredUpdateShardCountInputRequestTypeDef, _OptionalUpdateShardCountInputRequestTypeDef
 ):
     pass
 
 
+_RequiredPutRecordInputRequestTypeDef = TypedDict(
+    "_RequiredPutRecordInputRequestTypeDef",
+    {
+        "Data": BlobTypeDef,
+        "PartitionKey": str,
+    },
+)
+_OptionalPutRecordInputRequestTypeDef = TypedDict(
+    "_OptionalPutRecordInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "ExplicitHashKey": str,
+        "SequenceNumberForOrdering": str,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+
+class PutRecordInputRequestTypeDef(
+    _RequiredPutRecordInputRequestTypeDef, _OptionalPutRecordInputRequestTypeDef
+):
+    pass
+
+
+_RequiredPutRecordsRequestEntryTypeDef = TypedDict(
+    "_RequiredPutRecordsRequestEntryTypeDef",
+    {
+        "Data": BlobTypeDef,
+        "PartitionKey": str,
+    },
+)
+_OptionalPutRecordsRequestEntryTypeDef = TypedDict(
+    "_OptionalPutRecordsRequestEntryTypeDef",
+    {
+        "ExplicitHashKey": str,
+    },
+    total=False,
+)
+
+
+class PutRecordsRequestEntryTypeDef(
+    _RequiredPutRecordsRequestEntryTypeDef, _OptionalPutRecordsRequestEntryTypeDef
+):
+    pass
+
+
 ChildShardTypeDef = TypedDict(
     "ChildShardTypeDef",
     {
         "ShardId": str,
         "ParentShards": List[str],
         "HashKeyRange": HashKeyRangeTypeDef,
     },
@@ -982,37 +898,14 @@
         "StreamName": str,
         "StreamARN": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamARN": str,
-    },
-)
-_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamCreationTimestamp": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
-    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-):
-    pass
-
-
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "ExclusiveStartStreamName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1068,72 +961,134 @@
 
 class StreamDescriptionSummaryTypeDef(
     _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
 ):
     pass
 
 
-ListShardsInputListShardsPaginateTypeDef = TypedDict(
-    "ListShardsInputListShardsPaginateTypeDef",
+_RequiredGetShardIteratorInputRequestTypeDef = TypedDict(
+    "_RequiredGetShardIteratorInputRequestTypeDef",
+    {
+        "ShardId": str,
+        "ShardIteratorType": ShardIteratorTypeType,
+    },
+)
+_OptionalGetShardIteratorInputRequestTypeDef = TypedDict(
+    "_OptionalGetShardIteratorInputRequestTypeDef",
     {
         "StreamName": str,
-        "ExclusiveStartShardId": str,
-        "StreamCreationTimestamp": Union[datetime, str],
-        "ShardFilter": ShardFilterTypeDef,
+        "StartingSequenceNumber": str,
+        "Timestamp": TimestampTypeDef,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+
+class GetShardIteratorInputRequestTypeDef(
+    _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
+):
+    pass
+
+
+_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
         "StreamARN": str,
+    },
+)
+_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamCreationTimestamp": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListShardsInputRequestTypeDef = TypedDict(
-    "ListShardsInputRequestTypeDef",
+
+class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
+    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStreamConsumersInputRequestTypeDef = TypedDict(
+    "_RequiredListStreamConsumersInputRequestTypeDef",
+    {
+        "StreamARN": str,
+    },
+)
+_OptionalListStreamConsumersInputRequestTypeDef = TypedDict(
+    "_OptionalListStreamConsumersInputRequestTypeDef",
     {
-        "StreamName": str,
         "NextToken": str,
-        "ExclusiveStartShardId": str,
         "MaxResults": int,
-        "StreamCreationTimestamp": Union[datetime, str],
-        "ShardFilter": ShardFilterTypeDef,
-        "StreamARN": str,
+        "StreamCreationTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-ListTagsForStreamOutputTypeDef = TypedDict(
-    "ListTagsForStreamOutputTypeDef",
+
+class ListStreamConsumersInputRequestTypeDef(
+    _RequiredListStreamConsumersInputRequestTypeDef, _OptionalListStreamConsumersInputRequestTypeDef
+):
+    pass
+
+
+_RequiredShardFilterTypeDef = TypedDict(
+    "_RequiredShardFilterTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "HasMoreTags": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Type": ShardFilterTypeType,
+    },
+)
+_OptionalShardFilterTypeDef = TypedDict(
+    "_OptionalShardFilterTypeDef",
+    {
+        "ShardId": str,
+        "Timestamp": TimestampTypeDef,
     },
+    total=False,
 )
 
-_RequiredPutRecordsInputRequestTypeDef = TypedDict(
-    "_RequiredPutRecordsInputRequestTypeDef",
+
+class ShardFilterTypeDef(_RequiredShardFilterTypeDef, _OptionalShardFilterTypeDef):
+    pass
+
+
+_RequiredStartingPositionTypeDef = TypedDict(
+    "_RequiredStartingPositionTypeDef",
     {
-        "Records": Sequence[PutRecordsRequestEntryTypeDef],
+        "Type": ShardIteratorTypeType,
     },
 )
-_OptionalPutRecordsInputRequestTypeDef = TypedDict(
-    "_OptionalPutRecordsInputRequestTypeDef",
+_OptionalStartingPositionTypeDef = TypedDict(
+    "_OptionalStartingPositionTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
+        "SequenceNumber": str,
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
 
-class PutRecordsInputRequestTypeDef(
-    _RequiredPutRecordsInputRequestTypeDef, _OptionalPutRecordsInputRequestTypeDef
-):
+class StartingPositionTypeDef(_RequiredStartingPositionTypeDef, _OptionalStartingPositionTypeDef):
     pass
 
 
+ListTagsForStreamOutputTypeDef = TypedDict(
+    "ListTagsForStreamOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "HasMoreTags": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutRecordsOutputTypeDef = TypedDict(
     "PutRecordsOutputTypeDef",
     {
         "FailedRecordCount": int,
         "Records": List[PutRecordsResultEntryTypeDef],
         "EncryptionType": EncryptionTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1158,23 +1113,36 @@
 )
 
 
 class ShardTypeDef(_RequiredShardTypeDef, _OptionalShardTypeDef):
     pass
 
 
-SubscribeToShardInputRequestTypeDef = TypedDict(
-    "SubscribeToShardInputRequestTypeDef",
+_RequiredPutRecordsInputRequestTypeDef = TypedDict(
+    "_RequiredPutRecordsInputRequestTypeDef",
     {
-        "ConsumerARN": str,
-        "ShardId": str,
-        "StartingPosition": StartingPositionTypeDef,
+        "Records": Sequence[PutRecordsRequestEntryTypeDef],
+    },
+)
+_OptionalPutRecordsInputRequestTypeDef = TypedDict(
+    "_OptionalPutRecordsInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
     },
+    total=False,
 )
 
+
+class PutRecordsInputRequestTypeDef(
+    _RequiredPutRecordsInputRequestTypeDef, _OptionalPutRecordsInputRequestTypeDef
+):
+    pass
+
+
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
         "MillisBehindLatest": int,
         "ChildShards": List[ChildShardTypeDef],
@@ -1220,14 +1188,50 @@
     "DescribeStreamSummaryOutputTypeDef",
     {
         "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListShardsInputListShardsPaginateTypeDef = TypedDict(
+    "ListShardsInputListShardsPaginateTypeDef",
+    {
+        "StreamName": str,
+        "ExclusiveStartShardId": str,
+        "StreamCreationTimestamp": TimestampTypeDef,
+        "ShardFilter": ShardFilterTypeDef,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListShardsInputRequestTypeDef = TypedDict(
+    "ListShardsInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "NextToken": str,
+        "ExclusiveStartShardId": str,
+        "MaxResults": int,
+        "StreamCreationTimestamp": TimestampTypeDef,
+        "ShardFilter": ShardFilterTypeDef,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+SubscribeToShardInputRequestTypeDef = TypedDict(
+    "SubscribeToShardInputRequestTypeDef",
+    {
+        "ConsumerARN": str,
+        "ShardId": str,
+        "StartingPosition": StartingPositionTypeDef,
+    },
+)
+
 ListShardsOutputTypeDef = TypedDict(
     "ListShardsOutputTypeDef",
     {
         "Shards": List[ShardTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/type_defs.pyi` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesis.type_defs import AddTagsToStreamInputRequestTypeDef
 
-    data: AddTagsToStreamInputRequestTypeDef = {...}
+    data: AddTagsToStreamInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.eventstream import EventStream
@@ -35,14 +35,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddTagsToStreamInputRequestTypeDef",
+    "BlobTypeDef",
     "HashKeyRangeTypeDef",
     "ConsumerDescriptionTypeDef",
     "ConsumerTypeDef",
     "StreamModeDetailsTypeDef",
     "DecreaseStreamRetentionPeriodInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "DeregisterStreamConsumerInputRequestTypeDef",
@@ -53,72 +54,73 @@
     "WaiterConfigTypeDef",
     "DescribeStreamSummaryInputRequestTypeDef",
     "DisableEnhancedMonitoringInputRequestTypeDef",
     "EnableEnhancedMonitoringInputRequestTypeDef",
     "EnhancedMetricsTypeDef",
     "GetRecordsInputRequestTypeDef",
     "RecordTypeDef",
-    "GetShardIteratorInputRequestTypeDef",
+    "TimestampTypeDef",
     "IncreaseStreamRetentionPeriodInputRequestTypeDef",
     "InternalFailureExceptionTypeDef",
     "KMSAccessDeniedExceptionTypeDef",
     "KMSDisabledExceptionTypeDef",
     "KMSInvalidStateExceptionTypeDef",
     "KMSNotFoundExceptionTypeDef",
     "KMSOptInRequiredTypeDef",
     "KMSThrottlingExceptionTypeDef",
-    "ShardFilterTypeDef",
-    "ListStreamConsumersInputRequestTypeDef",
     "ListStreamsInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "TagTypeDef",
     "MergeShardsInputRequestTypeDef",
-    "PutRecordInputRequestTypeDef",
-    "PutRecordsRequestEntryTypeDef",
     "PutRecordsResultEntryTypeDef",
     "RegisterStreamConsumerInputRequestTypeDef",
     "RemoveTagsFromStreamInputRequestTypeDef",
     "ResourceInUseExceptionTypeDef",
     "ResourceNotFoundExceptionTypeDef",
     "SequenceNumberRangeTypeDef",
     "SplitShardInputRequestTypeDef",
     "StartStreamEncryptionInputRequestTypeDef",
-    "StartingPositionTypeDef",
     "StopStreamEncryptionInputRequestTypeDef",
     "UpdateShardCountInputRequestTypeDef",
+    "PutRecordInputRequestTypeDef",
+    "PutRecordsRequestEntryTypeDef",
     "ChildShardTypeDef",
     "CreateStreamInputRequestTypeDef",
     "StreamSummaryTypeDef",
     "UpdateStreamModeInputRequestTypeDef",
     "DescribeLimitsOutputTypeDef",
     "DescribeStreamConsumerOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnhancedMonitoringOutputTypeDef",
     "GetShardIteratorOutputTypeDef",
     "ListStreamConsumersOutputTypeDef",
     "PutRecordOutputTypeDef",
     "RegisterStreamConsumerOutputTypeDef",
     "UpdateShardCountOutputTypeDef",
     "DescribeStreamInputDescribeStreamPaginateTypeDef",
-    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "DescribeStreamInputStreamExistsWaitTypeDef",
     "DescribeStreamInputStreamNotExistsWaitTypeDef",
     "StreamDescriptionSummaryTypeDef",
-    "ListShardsInputListShardsPaginateTypeDef",
-    "ListShardsInputRequestTypeDef",
+    "GetShardIteratorInputRequestTypeDef",
+    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    "ListStreamConsumersInputRequestTypeDef",
+    "ShardFilterTypeDef",
+    "StartingPositionTypeDef",
     "ListTagsForStreamOutputTypeDef",
-    "PutRecordsInputRequestTypeDef",
     "PutRecordsOutputTypeDef",
     "ShardTypeDef",
-    "SubscribeToShardInputRequestTypeDef",
+    "PutRecordsInputRequestTypeDef",
     "GetRecordsOutputTypeDef",
     "SubscribeToShardEventTypeDef",
     "ListStreamsOutputTypeDef",
     "DescribeStreamSummaryOutputTypeDef",
+    "ListShardsInputListShardsPaginateTypeDef",
+    "ListShardsInputRequestTypeDef",
+    "SubscribeToShardInputRequestTypeDef",
     "ListShardsOutputTypeDef",
     "StreamDescriptionTypeDef",
     "SubscribeToShardEventStreamTypeDef",
     "DescribeStreamOutputTypeDef",
     "SubscribeToShardOutputTypeDef",
 )
 
@@ -138,14 +140,15 @@
 )
 
 class AddTagsToStreamInputRequestTypeDef(
     _RequiredAddTagsToStreamInputRequestTypeDef, _OptionalAddTagsToStreamInputRequestTypeDef
 ):
     pass
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 HashKeyRangeTypeDef = TypedDict(
     "HashKeyRangeTypeDef",
     {
         "StartingHashKey": str,
         "EndingHashKey": str,
     },
 )
@@ -365,37 +368,15 @@
     },
     total=False,
 )
 
 class RecordTypeDef(_RequiredRecordTypeDef, _OptionalRecordTypeDef):
     pass
 
-_RequiredGetShardIteratorInputRequestTypeDef = TypedDict(
-    "_RequiredGetShardIteratorInputRequestTypeDef",
-    {
-        "ShardId": str,
-        "ShardIteratorType": ShardIteratorTypeType,
-    },
-)
-_OptionalGetShardIteratorInputRequestTypeDef = TypedDict(
-    "_OptionalGetShardIteratorInputRequestTypeDef",
-    {
-        "StreamName": str,
-        "StartingSequenceNumber": str,
-        "Timestamp": Union[datetime, str],
-        "StreamARN": str,
-    },
-    total=False,
-)
-
-class GetShardIteratorInputRequestTypeDef(
-    _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
     "_RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef",
     {
         "RetentionPeriodHours": int,
     },
 )
 _OptionalIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
@@ -465,53 +446,14 @@
     "KMSThrottlingExceptionTypeDef",
     {
         "message": str,
     },
     total=False,
 )
 
-_RequiredShardFilterTypeDef = TypedDict(
-    "_RequiredShardFilterTypeDef",
-    {
-        "Type": ShardFilterTypeType,
-    },
-)
-_OptionalShardFilterTypeDef = TypedDict(
-    "_OptionalShardFilterTypeDef",
-    {
-        "ShardId": str,
-        "Timestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-class ShardFilterTypeDef(_RequiredShardFilterTypeDef, _OptionalShardFilterTypeDef):
-    pass
-
-_RequiredListStreamConsumersInputRequestTypeDef = TypedDict(
-    "_RequiredListStreamConsumersInputRequestTypeDef",
-    {
-        "StreamARN": str,
-    },
-)
-_OptionalListStreamConsumersInputRequestTypeDef = TypedDict(
-    "_OptionalListStreamConsumersInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StreamCreationTimestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-class ListStreamConsumersInputRequestTypeDef(
-    _RequiredListStreamConsumersInputRequestTypeDef, _OptionalListStreamConsumersInputRequestTypeDef
-):
-    pass
-
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
         "Limit": int,
         "ExclusiveStartStreamName": str,
         "NextToken": str,
     },
@@ -563,57 +505,14 @@
 )
 
 class MergeShardsInputRequestTypeDef(
     _RequiredMergeShardsInputRequestTypeDef, _OptionalMergeShardsInputRequestTypeDef
 ):
     pass
 
-_RequiredPutRecordInputRequestTypeDef = TypedDict(
-    "_RequiredPutRecordInputRequestTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-        "PartitionKey": str,
-    },
-)
-_OptionalPutRecordInputRequestTypeDef = TypedDict(
-    "_OptionalPutRecordInputRequestTypeDef",
-    {
-        "StreamName": str,
-        "ExplicitHashKey": str,
-        "SequenceNumberForOrdering": str,
-        "StreamARN": str,
-    },
-    total=False,
-)
-
-class PutRecordInputRequestTypeDef(
-    _RequiredPutRecordInputRequestTypeDef, _OptionalPutRecordInputRequestTypeDef
-):
-    pass
-
-_RequiredPutRecordsRequestEntryTypeDef = TypedDict(
-    "_RequiredPutRecordsRequestEntryTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-        "PartitionKey": str,
-    },
-)
-_OptionalPutRecordsRequestEntryTypeDef = TypedDict(
-    "_OptionalPutRecordsRequestEntryTypeDef",
-    {
-        "ExplicitHashKey": str,
-    },
-    total=False,
-)
-
-class PutRecordsRequestEntryTypeDef(
-    _RequiredPutRecordsRequestEntryTypeDef, _OptionalPutRecordsRequestEntryTypeDef
-):
-    pass
-
 PutRecordsResultEntryTypeDef = TypedDict(
     "PutRecordsResultEntryTypeDef",
     {
         "SequenceNumber": str,
         "ShardId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
@@ -724,32 +623,14 @@
 
 class StartStreamEncryptionInputRequestTypeDef(
     _RequiredStartStreamEncryptionInputRequestTypeDef,
     _OptionalStartStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
-_RequiredStartingPositionTypeDef = TypedDict(
-    "_RequiredStartingPositionTypeDef",
-    {
-        "Type": ShardIteratorTypeType,
-    },
-)
-_OptionalStartingPositionTypeDef = TypedDict(
-    "_OptionalStartingPositionTypeDef",
-    {
-        "SequenceNumber": str,
-        "Timestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-class StartingPositionTypeDef(_RequiredStartingPositionTypeDef, _OptionalStartingPositionTypeDef):
-    pass
-
 _RequiredStopStreamEncryptionInputRequestTypeDef = TypedDict(
     "_RequiredStopStreamEncryptionInputRequestTypeDef",
     {
         "EncryptionType": EncryptionTypeType,
         "KeyId": str,
     },
 )
@@ -785,14 +666,57 @@
 )
 
 class UpdateShardCountInputRequestTypeDef(
     _RequiredUpdateShardCountInputRequestTypeDef, _OptionalUpdateShardCountInputRequestTypeDef
 ):
     pass
 
+_RequiredPutRecordInputRequestTypeDef = TypedDict(
+    "_RequiredPutRecordInputRequestTypeDef",
+    {
+        "Data": BlobTypeDef,
+        "PartitionKey": str,
+    },
+)
+_OptionalPutRecordInputRequestTypeDef = TypedDict(
+    "_OptionalPutRecordInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "ExplicitHashKey": str,
+        "SequenceNumberForOrdering": str,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+class PutRecordInputRequestTypeDef(
+    _RequiredPutRecordInputRequestTypeDef, _OptionalPutRecordInputRequestTypeDef
+):
+    pass
+
+_RequiredPutRecordsRequestEntryTypeDef = TypedDict(
+    "_RequiredPutRecordsRequestEntryTypeDef",
+    {
+        "Data": BlobTypeDef,
+        "PartitionKey": str,
+    },
+)
+_OptionalPutRecordsRequestEntryTypeDef = TypedDict(
+    "_OptionalPutRecordsRequestEntryTypeDef",
+    {
+        "ExplicitHashKey": str,
+    },
+    total=False,
+)
+
+class PutRecordsRequestEntryTypeDef(
+    _RequiredPutRecordsRequestEntryTypeDef, _OptionalPutRecordsRequestEntryTypeDef
+):
+    pass
+
 ChildShardTypeDef = TypedDict(
     "ChildShardTypeDef",
     {
         "ShardId": str,
         "ParentShards": List[str],
         "HashKeyRange": HashKeyRangeTypeDef,
     },
@@ -935,35 +859,14 @@
         "StreamName": str,
         "StreamARN": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamARN": str,
-    },
-)
-_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamCreationTimestamp": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
-    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-):
-    pass
-
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "ExclusiveStartStreamName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1017,70 +920,124 @@
 )
 
 class StreamDescriptionSummaryTypeDef(
     _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
 ):
     pass
 
-ListShardsInputListShardsPaginateTypeDef = TypedDict(
-    "ListShardsInputListShardsPaginateTypeDef",
+_RequiredGetShardIteratorInputRequestTypeDef = TypedDict(
+    "_RequiredGetShardIteratorInputRequestTypeDef",
+    {
+        "ShardId": str,
+        "ShardIteratorType": ShardIteratorTypeType,
+    },
+)
+_OptionalGetShardIteratorInputRequestTypeDef = TypedDict(
+    "_OptionalGetShardIteratorInputRequestTypeDef",
     {
         "StreamName": str,
-        "ExclusiveStartShardId": str,
-        "StreamCreationTimestamp": Union[datetime, str],
-        "ShardFilter": ShardFilterTypeDef,
+        "StartingSequenceNumber": str,
+        "Timestamp": TimestampTypeDef,
         "StreamARN": str,
+    },
+    total=False,
+)
+
+class GetShardIteratorInputRequestTypeDef(
+    _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
+):
+    pass
+
+_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamARN": str,
+    },
+)
+_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamCreationTimestamp": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListShardsInputRequestTypeDef = TypedDict(
-    "ListShardsInputRequestTypeDef",
+class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
+    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+):
+    pass
+
+_RequiredListStreamConsumersInputRequestTypeDef = TypedDict(
+    "_RequiredListStreamConsumersInputRequestTypeDef",
+    {
+        "StreamARN": str,
+    },
+)
+_OptionalListStreamConsumersInputRequestTypeDef = TypedDict(
+    "_OptionalListStreamConsumersInputRequestTypeDef",
     {
-        "StreamName": str,
         "NextToken": str,
-        "ExclusiveStartShardId": str,
         "MaxResults": int,
-        "StreamCreationTimestamp": Union[datetime, str],
-        "ShardFilter": ShardFilterTypeDef,
-        "StreamARN": str,
+        "StreamCreationTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-ListTagsForStreamOutputTypeDef = TypedDict(
-    "ListTagsForStreamOutputTypeDef",
+class ListStreamConsumersInputRequestTypeDef(
+    _RequiredListStreamConsumersInputRequestTypeDef, _OptionalListStreamConsumersInputRequestTypeDef
+):
+    pass
+
+_RequiredShardFilterTypeDef = TypedDict(
+    "_RequiredShardFilterTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "HasMoreTags": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Type": ShardFilterTypeType,
+    },
+)
+_OptionalShardFilterTypeDef = TypedDict(
+    "_OptionalShardFilterTypeDef",
+    {
+        "ShardId": str,
+        "Timestamp": TimestampTypeDef,
     },
+    total=False,
 )
 
-_RequiredPutRecordsInputRequestTypeDef = TypedDict(
-    "_RequiredPutRecordsInputRequestTypeDef",
+class ShardFilterTypeDef(_RequiredShardFilterTypeDef, _OptionalShardFilterTypeDef):
+    pass
+
+_RequiredStartingPositionTypeDef = TypedDict(
+    "_RequiredStartingPositionTypeDef",
     {
-        "Records": Sequence[PutRecordsRequestEntryTypeDef],
+        "Type": ShardIteratorTypeType,
     },
 )
-_OptionalPutRecordsInputRequestTypeDef = TypedDict(
-    "_OptionalPutRecordsInputRequestTypeDef",
+_OptionalStartingPositionTypeDef = TypedDict(
+    "_OptionalStartingPositionTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
+        "SequenceNumber": str,
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-class PutRecordsInputRequestTypeDef(
-    _RequiredPutRecordsInputRequestTypeDef, _OptionalPutRecordsInputRequestTypeDef
-):
+class StartingPositionTypeDef(_RequiredStartingPositionTypeDef, _OptionalStartingPositionTypeDef):
     pass
 
+ListTagsForStreamOutputTypeDef = TypedDict(
+    "ListTagsForStreamOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "HasMoreTags": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutRecordsOutputTypeDef = TypedDict(
     "PutRecordsOutputTypeDef",
     {
         "FailedRecordCount": int,
         "Records": List[PutRecordsResultEntryTypeDef],
         "EncryptionType": EncryptionTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1103,22 +1060,33 @@
     },
     total=False,
 )
 
 class ShardTypeDef(_RequiredShardTypeDef, _OptionalShardTypeDef):
     pass
 
-SubscribeToShardInputRequestTypeDef = TypedDict(
-    "SubscribeToShardInputRequestTypeDef",
+_RequiredPutRecordsInputRequestTypeDef = TypedDict(
+    "_RequiredPutRecordsInputRequestTypeDef",
     {
-        "ConsumerARN": str,
-        "ShardId": str,
-        "StartingPosition": StartingPositionTypeDef,
+        "Records": Sequence[PutRecordsRequestEntryTypeDef],
     },
 )
+_OptionalPutRecordsInputRequestTypeDef = TypedDict(
+    "_OptionalPutRecordsInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+class PutRecordsInputRequestTypeDef(
+    _RequiredPutRecordsInputRequestTypeDef, _OptionalPutRecordsInputRequestTypeDef
+):
+    pass
 
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
         "MillisBehindLatest": int,
@@ -1163,14 +1131,50 @@
     "DescribeStreamSummaryOutputTypeDef",
     {
         "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListShardsInputListShardsPaginateTypeDef = TypedDict(
+    "ListShardsInputListShardsPaginateTypeDef",
+    {
+        "StreamName": str,
+        "ExclusiveStartShardId": str,
+        "StreamCreationTimestamp": TimestampTypeDef,
+        "ShardFilter": ShardFilterTypeDef,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListShardsInputRequestTypeDef = TypedDict(
+    "ListShardsInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "NextToken": str,
+        "ExclusiveStartShardId": str,
+        "MaxResults": int,
+        "StreamCreationTimestamp": TimestampTypeDef,
+        "ShardFilter": ShardFilterTypeDef,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+SubscribeToShardInputRequestTypeDef = TypedDict(
+    "SubscribeToShardInputRequestTypeDef",
+    {
+        "ConsumerARN": str,
+        "ShardId": str,
+        "StartingPosition": StartingPositionTypeDef,
+    },
+)
+
 ListShardsOutputTypeDef = TypedDict(
     "ListShardsOutputTypeDef",
     {
         "Shards": List[ShardTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/waiter.py` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis/waiter.pyi` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis.egg-info/PKG-INFO` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Kinesis 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Kinesis 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesis type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesis type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis)](https://pepy.tech/project/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
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
@@ -354,24 +354,25 @@
 )
 
 
 def check_value(value: ConsumerStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesis.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesis.type_defs import (
     AddTagsToStreamInputRequestTypeDef,
+    BlobTypeDef,
     HashKeyRangeTypeDef,
     ConsumerDescriptionTypeDef,
     ConsumerTypeDef,
     StreamModeDetailsTypeDef,
     DecreaseStreamRetentionPeriodInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     DeregisterStreamConsumerInputRequestTypeDef,
@@ -382,81 +383,82 @@
     WaiterConfigTypeDef,
     DescribeStreamSummaryInputRequestTypeDef,
     DisableEnhancedMonitoringInputRequestTypeDef,
     EnableEnhancedMonitoringInputRequestTypeDef,
     EnhancedMetricsTypeDef,
     GetRecordsInputRequestTypeDef,
     RecordTypeDef,
-    GetShardIteratorInputRequestTypeDef,
+    TimestampTypeDef,
     IncreaseStreamRetentionPeriodInputRequestTypeDef,
     InternalFailureExceptionTypeDef,
     KMSAccessDeniedExceptionTypeDef,
     KMSDisabledExceptionTypeDef,
     KMSInvalidStateExceptionTypeDef,
     KMSNotFoundExceptionTypeDef,
     KMSOptInRequiredTypeDef,
     KMSThrottlingExceptionTypeDef,
-    ShardFilterTypeDef,
-    ListStreamConsumersInputRequestTypeDef,
     ListStreamsInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     TagTypeDef,
     MergeShardsInputRequestTypeDef,
-    PutRecordInputRequestTypeDef,
-    PutRecordsRequestEntryTypeDef,
     PutRecordsResultEntryTypeDef,
     RegisterStreamConsumerInputRequestTypeDef,
     RemoveTagsFromStreamInputRequestTypeDef,
     ResourceInUseExceptionTypeDef,
     ResourceNotFoundExceptionTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
-    StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
     UpdateShardCountInputRequestTypeDef,
+    PutRecordInputRequestTypeDef,
+    PutRecordsRequestEntryTypeDef,
     ChildShardTypeDef,
     CreateStreamInputRequestTypeDef,
     StreamSummaryTypeDef,
     UpdateStreamModeInputRequestTypeDef,
     DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EnhancedMonitoringOutputTypeDef,
     GetShardIteratorOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
     PutRecordOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
     UpdateShardCountOutputTypeDef,
     DescribeStreamInputDescribeStreamPaginateTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
     StreamDescriptionSummaryTypeDef,
-    ListShardsInputListShardsPaginateTypeDef,
-    ListShardsInputRequestTypeDef,
+    GetShardIteratorInputRequestTypeDef,
+    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    ListStreamConsumersInputRequestTypeDef,
+    ShardFilterTypeDef,
+    StartingPositionTypeDef,
     ListTagsForStreamOutputTypeDef,
-    PutRecordsInputRequestTypeDef,
     PutRecordsOutputTypeDef,
     ShardTypeDef,
-    SubscribeToShardInputRequestTypeDef,
+    PutRecordsInputRequestTypeDef,
     GetRecordsOutputTypeDef,
     SubscribeToShardEventTypeDef,
     ListStreamsOutputTypeDef,
     DescribeStreamSummaryOutputTypeDef,
+    ListShardsInputListShardsPaginateTypeDef,
+    ListShardsInputRequestTypeDef,
+    SubscribeToShardInputRequestTypeDef,
     ListShardsOutputTypeDef,
     StreamDescriptionTypeDef,
     SubscribeToShardEventStreamTypeDef,
     DescribeStreamOutputTypeDef,
     SubscribeToShardOutputTypeDef,
 )
 
 
-def get_structure() -> AddTagsToStreamInputRequestTypeDef:
+def get_value() -> AddTagsToStreamInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesis-1.28.15.post1/mypy_boto3_kinesis.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-1.28.16/mypy_boto3_kinesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.15.post1/setup.py` & `mypy-boto3-kinesis-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_kinesis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kinesis 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Kinesis 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 kinesis type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 kinesis type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_kinesis": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

