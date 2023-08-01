# Comparing `tmp/mypy-boto3-firehose-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-firehose-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-firehose-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:09 2023, max compression
+gzip compressed data, was "mypy-boto3-firehose-1.28.16.tar", last modified: Tue Aug  1 11:36:49 2023, max compression
```

## Comparing `mypy-boto3-firehose-1.28.15.post1.tar` & `mypy-boto3-firehose-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.141153 mypy-boto3-firehose-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16623 2023-07-29 10:03:09.133154 mypy-boto3-firehose-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15126 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.121153 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48382 2023-07-29 09:45:26.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-07-29 09:45:25.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.133154 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16623 2023-07-29 10:03:08.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 10:03:08.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:08.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:08.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:08.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:08.000000 mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:09.141153 mypy-boto3-firehose-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:45:24.000000 mypy-boto3-firehose-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:49.120888 mypy-boto3-firehose-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:18:00.000000 mypy-boto3-firehose-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-08-01 11:36:49.112888 mypy-boto3-firehose-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-08-01 11:18:00.000000 mypy-boto3-firehose-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:49.112888 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 11:18:00.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 11:18:00.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:18:00.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-08-01 11:18:01.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-08-01 11:18:00.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-08-01 11:18:02.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-08-01 11:18:01.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:18:00.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48425 2023-08-01 11:18:04.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48374 2023-08-01 11:18:03.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:18:00.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:49.112888 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-08-01 11:36:48.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-01 11:36:48.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:48.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:36:48.000000 mypy-boto3-firehose-1.28.16/mypy_boto3_firehose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:49.120888 mypy-boto3-firehose-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:18:00.000000 mypy-boto3-firehose-1.28.16/setup.py
```

### Comparing `mypy-boto3-firehose-1.28.15.post1/LICENSE` & `mypy-boto3-firehose-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.15.post1/PKG-INFO` & `mypy-boto3-firehose-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-firehose
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Firehose 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Firehose 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 firehose type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 firehose type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-firehose)](https://pepy.tech/project/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -310,30 +310,31 @@
 )
 
 
 def check_value(value: AmazonOpenSearchServerlessS3BackupModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_firehose.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_firehose.type_defs import (
     AmazonOpenSearchServerlessBufferingHintsTypeDef,
     AmazonOpenSearchServerlessRetryOptionsTypeDef,
     CloudWatchLoggingOptionsTypeDef,
     VpcConfigurationTypeDef,
     VpcConfigurationDescriptionTypeDef,
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
+    BlobTypeDef,
     BufferingHintsTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     SchemaConfigurationTypeDef,
@@ -356,20 +357,20 @@
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
     OrcSerDeOutputTypeDef,
     OrcSerDeTypeDef,
     ParquetSerDeTypeDef,
     ProcessorParameterTypeDef,
-    RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
     RedshiftRetryOptionsTypeDef,
     SplunkRetryOptionsTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
+    RecordTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
     TagDeliveryStreamInputRequestTypeDef,
     CreateDeliveryStreamOutputTypeDef,
     ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamOutputTypeDef,
     PutRecordOutputTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
@@ -380,17 +381,17 @@
     HttpEndpointRequestConfigurationOutputTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
     SerializerOutputTypeDef,
     SerializerTypeDef,
     ProcessorOutputTypeDef,
     ProcessorTypeDef,
+    PutRecordBatchOutputTypeDef,
     PutRecordBatchInputRequestTypeDef,
     PutRecordInputRequestTypeDef,
-    PutRecordBatchOutputTypeDef,
     InputFormatConfigurationOutputTypeDef,
     InputFormatConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     S3DestinationDescriptionTypeDef,
     S3DestinationUpdateTypeDef,
     OutputFormatConfigurationOutputTypeDef,
     OutputFormatConfigurationTypeDef,
@@ -423,15 +424,15 @@
     CreateDeliveryStreamInputRequestTypeDef,
     UpdateDestinationInputRequestTypeDef,
     DeliveryStreamDescriptionTypeDef,
     DescribeDeliveryStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
+def get_value() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-firehose-1.28.15.post1/README.md` & `mypy-boto3-firehose-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-firehose)](https://pepy.tech/project/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -278,30 +278,31 @@
 )
 
 
 def check_value(value: AmazonOpenSearchServerlessS3BackupModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_firehose.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_firehose.type_defs import (
     AmazonOpenSearchServerlessBufferingHintsTypeDef,
     AmazonOpenSearchServerlessRetryOptionsTypeDef,
     CloudWatchLoggingOptionsTypeDef,
     VpcConfigurationTypeDef,
     VpcConfigurationDescriptionTypeDef,
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
+    BlobTypeDef,
     BufferingHintsTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     SchemaConfigurationTypeDef,
@@ -324,20 +325,20 @@
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
     OrcSerDeOutputTypeDef,
     OrcSerDeTypeDef,
     ParquetSerDeTypeDef,
     ProcessorParameterTypeDef,
-    RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
     RedshiftRetryOptionsTypeDef,
     SplunkRetryOptionsTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
+    RecordTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
     TagDeliveryStreamInputRequestTypeDef,
     CreateDeliveryStreamOutputTypeDef,
     ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamOutputTypeDef,
     PutRecordOutputTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
@@ -348,17 +349,17 @@
     HttpEndpointRequestConfigurationOutputTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
     SerializerOutputTypeDef,
     SerializerTypeDef,
     ProcessorOutputTypeDef,
     ProcessorTypeDef,
+    PutRecordBatchOutputTypeDef,
     PutRecordBatchInputRequestTypeDef,
     PutRecordInputRequestTypeDef,
-    PutRecordBatchOutputTypeDef,
     InputFormatConfigurationOutputTypeDef,
     InputFormatConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     S3DestinationDescriptionTypeDef,
     S3DestinationUpdateTypeDef,
     OutputFormatConfigurationOutputTypeDef,
     OutputFormatConfigurationTypeDef,
@@ -391,15 +392,15 @@
     CreateDeliveryStreamInputRequestTypeDef,
     UpdateDestinationInputRequestTypeDef,
     DeliveryStreamDescriptionTypeDef,
     DescribeDeliveryStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
+def get_value() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/client.py` & `mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/client.pyi` & `mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/literals.py` & `mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/literals.pyi` & `mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/type_defs.py` & `mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsTypeDef
 
-    data: AmazonOpenSearchServerlessBufferingHintsTypeDef = {...}
+    data: AmazonOpenSearchServerlessBufferingHintsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -57,14 +57,15 @@
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     "AmazonOpenSearchServerlessRetryOptionsTypeDef",
     "CloudWatchLoggingOptionsTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "AmazonopensearchserviceBufferingHintsTypeDef",
     "AmazonopensearchserviceRetryOptionsTypeDef",
+    "BlobTypeDef",
     "BufferingHintsTypeDef",
     "CopyCommandTypeDef",
     "DeliveryStreamEncryptionConfigurationInputTypeDef",
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "SchemaConfigurationTypeDef",
@@ -87,20 +88,20 @@
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
     "OrcSerDeOutputTypeDef",
     "OrcSerDeTypeDef",
     "ParquetSerDeTypeDef",
     "ProcessorParameterTypeDef",
-    "RecordTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
     "RedshiftRetryOptionsTypeDef",
     "SplunkRetryOptionsTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     "UntagDeliveryStreamInputRequestTypeDef",
+    "RecordTypeDef",
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
     "TagDeliveryStreamInputRequestTypeDef",
     "CreateDeliveryStreamOutputTypeDef",
     "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamOutputTypeDef",
     "PutRecordOutputTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
@@ -111,17 +112,17 @@
     "HttpEndpointRequestConfigurationOutputTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
     "SerializerOutputTypeDef",
     "SerializerTypeDef",
     "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
+    "PutRecordBatchOutputTypeDef",
     "PutRecordBatchInputRequestTypeDef",
     "PutRecordInputRequestTypeDef",
-    "PutRecordBatchOutputTypeDef",
     "InputFormatConfigurationOutputTypeDef",
     "InputFormatConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "S3DestinationDescriptionTypeDef",
     "S3DestinationUpdateTypeDef",
     "OutputFormatConfigurationOutputTypeDef",
     "OutputFormatConfigurationTypeDef",
@@ -216,14 +217,15 @@
     "AmazonopensearchserviceRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BufferingHintsTypeDef = TypedDict(
     "BufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
@@ -593,21 +595,14 @@
     "ProcessorParameterTypeDef",
     {
         "ParameterName": ProcessorParameterNameType,
         "ParameterValue": str,
     },
 )
 
-RecordTypeDef = TypedDict(
-    "RecordTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 PutRecordBatchResponseEntryTypeDef = TypedDict(
     "PutRecordBatchResponseEntryTypeDef",
     {
         "RecordId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -641,14 +636,21 @@
     "UntagDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "TagKeys": Sequence[str],
     },
 )
 
+RecordTypeDef = TypedDict(
+    "RecordTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+)
+
 _RequiredStartDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
     "_RequiredStartDeliveryStreamEncryptionInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
@@ -837,14 +839,24 @@
 )
 
 
 class ProcessorTypeDef(_RequiredProcessorTypeDef, _OptionalProcessorTypeDef):
     pass
 
 
+PutRecordBatchOutputTypeDef = TypedDict(
+    "PutRecordBatchOutputTypeDef",
+    {
+        "FailedPutCount": int,
+        "Encrypted": bool,
+        "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutRecordBatchInputRequestTypeDef = TypedDict(
     "PutRecordBatchInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Records": Sequence[RecordTypeDef],
     },
 )
@@ -853,24 +865,14 @@
     "PutRecordInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Record": RecordTypeDef,
     },
 )
 
-PutRecordBatchOutputTypeDef = TypedDict(
-    "PutRecordBatchOutputTypeDef",
-    {
-        "FailedPutCount": int,
-        "Encrypted": bool,
-        "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 InputFormatConfigurationOutputTypeDef = TypedDict(
     "InputFormatConfigurationOutputTypeDef",
     {
         "Deserializer": DeserializerOutputTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose/type_defs.pyi` & `mypy-boto3-firehose-1.28.16/mypy_boto3_firehose/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsTypeDef
 
-    data: AmazonOpenSearchServerlessBufferingHintsTypeDef = {...}
+    data: AmazonOpenSearchServerlessBufferingHintsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -56,14 +56,15 @@
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     "AmazonOpenSearchServerlessRetryOptionsTypeDef",
     "CloudWatchLoggingOptionsTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "AmazonopensearchserviceBufferingHintsTypeDef",
     "AmazonopensearchserviceRetryOptionsTypeDef",
+    "BlobTypeDef",
     "BufferingHintsTypeDef",
     "CopyCommandTypeDef",
     "DeliveryStreamEncryptionConfigurationInputTypeDef",
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "SchemaConfigurationTypeDef",
@@ -86,20 +87,20 @@
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
     "OrcSerDeOutputTypeDef",
     "OrcSerDeTypeDef",
     "ParquetSerDeTypeDef",
     "ProcessorParameterTypeDef",
-    "RecordTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
     "RedshiftRetryOptionsTypeDef",
     "SplunkRetryOptionsTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     "UntagDeliveryStreamInputRequestTypeDef",
+    "RecordTypeDef",
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
     "TagDeliveryStreamInputRequestTypeDef",
     "CreateDeliveryStreamOutputTypeDef",
     "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamOutputTypeDef",
     "PutRecordOutputTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
@@ -110,17 +111,17 @@
     "HttpEndpointRequestConfigurationOutputTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
     "SerializerOutputTypeDef",
     "SerializerTypeDef",
     "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
+    "PutRecordBatchOutputTypeDef",
     "PutRecordBatchInputRequestTypeDef",
     "PutRecordInputRequestTypeDef",
-    "PutRecordBatchOutputTypeDef",
     "InputFormatConfigurationOutputTypeDef",
     "InputFormatConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "S3DestinationDescriptionTypeDef",
     "S3DestinationUpdateTypeDef",
     "OutputFormatConfigurationOutputTypeDef",
     "OutputFormatConfigurationTypeDef",
@@ -215,14 +216,15 @@
     "AmazonopensearchserviceRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BufferingHintsTypeDef = TypedDict(
     "BufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
@@ -578,21 +580,14 @@
     "ProcessorParameterTypeDef",
     {
         "ParameterName": ProcessorParameterNameType,
         "ParameterValue": str,
     },
 )
 
-RecordTypeDef = TypedDict(
-    "RecordTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 PutRecordBatchResponseEntryTypeDef = TypedDict(
     "PutRecordBatchResponseEntryTypeDef",
     {
         "RecordId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -626,14 +621,21 @@
     "UntagDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "TagKeys": Sequence[str],
     },
 )
 
+RecordTypeDef = TypedDict(
+    "RecordTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+)
+
 _RequiredStartDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
     "_RequiredStartDeliveryStreamEncryptionInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
@@ -816,14 +818,24 @@
     },
     total=False,
 )
 
 class ProcessorTypeDef(_RequiredProcessorTypeDef, _OptionalProcessorTypeDef):
     pass
 
+PutRecordBatchOutputTypeDef = TypedDict(
+    "PutRecordBatchOutputTypeDef",
+    {
+        "FailedPutCount": int,
+        "Encrypted": bool,
+        "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutRecordBatchInputRequestTypeDef = TypedDict(
     "PutRecordBatchInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Records": Sequence[RecordTypeDef],
     },
 )
@@ -832,24 +844,14 @@
     "PutRecordInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Record": RecordTypeDef,
     },
 )
 
-PutRecordBatchOutputTypeDef = TypedDict(
-    "PutRecordBatchOutputTypeDef",
-    {
-        "FailedPutCount": int,
-        "Encrypted": bool,
-        "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 InputFormatConfigurationOutputTypeDef = TypedDict(
     "InputFormatConfigurationOutputTypeDef",
     {
         "Deserializer": DeserializerOutputTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose.egg-info/PKG-INFO` & `mypy-boto3-firehose-1.28.16/mypy_boto3_firehose.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-firehose
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Firehose 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Firehose 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 firehose type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 firehose type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-firehose)](https://pepy.tech/project/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -310,30 +310,31 @@
 )
 
 
 def check_value(value: AmazonOpenSearchServerlessS3BackupModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_firehose.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_firehose.type_defs import (
     AmazonOpenSearchServerlessBufferingHintsTypeDef,
     AmazonOpenSearchServerlessRetryOptionsTypeDef,
     CloudWatchLoggingOptionsTypeDef,
     VpcConfigurationTypeDef,
     VpcConfigurationDescriptionTypeDef,
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
+    BlobTypeDef,
     BufferingHintsTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     SchemaConfigurationTypeDef,
@@ -356,20 +357,20 @@
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
     OrcSerDeOutputTypeDef,
     OrcSerDeTypeDef,
     ParquetSerDeTypeDef,
     ProcessorParameterTypeDef,
-    RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
     RedshiftRetryOptionsTypeDef,
     SplunkRetryOptionsTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
+    RecordTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
     TagDeliveryStreamInputRequestTypeDef,
     CreateDeliveryStreamOutputTypeDef,
     ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamOutputTypeDef,
     PutRecordOutputTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
@@ -380,17 +381,17 @@
     HttpEndpointRequestConfigurationOutputTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
     SerializerOutputTypeDef,
     SerializerTypeDef,
     ProcessorOutputTypeDef,
     ProcessorTypeDef,
+    PutRecordBatchOutputTypeDef,
     PutRecordBatchInputRequestTypeDef,
     PutRecordInputRequestTypeDef,
-    PutRecordBatchOutputTypeDef,
     InputFormatConfigurationOutputTypeDef,
     InputFormatConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     S3DestinationDescriptionTypeDef,
     S3DestinationUpdateTypeDef,
     OutputFormatConfigurationOutputTypeDef,
     OutputFormatConfigurationTypeDef,
@@ -423,15 +424,15 @@
     CreateDeliveryStreamInputRequestTypeDef,
     UpdateDestinationInputRequestTypeDef,
     DeliveryStreamDescriptionTypeDef,
     DescribeDeliveryStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
+def get_value() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-firehose-1.28.15.post1/mypy_boto3_firehose.egg-info/SOURCES.txt` & `mypy-boto3-firehose-1.28.16/mypy_boto3_firehose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.15.post1/setup.py` & `mypy-boto3-firehose-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-firehose",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_firehose"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Firehose 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Firehose 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 firehose type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 firehose type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_firehose": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

