# Comparing `tmp/mypy-boto3-timestream-write-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-timestream-write-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-write-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:22 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-write-1.28.16.tar", last modified: Tue Aug  1 11:38:01 2023, max compression
```

## Comparing `mypy-boto3-timestream-write-1.28.15.post1.tar` & `mypy-boto3-timestream-write-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-07-29 10:00:51.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:01.180701 mypy-boto3-timestream-write-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-08-01 11:38:01.172701 mypy-boto3-timestream-write-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:01.164701 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-08-01 11:34:28.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23883 2023-08-01 11:34:28.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:01.172701 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-08-01 11:38:00.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 11:38:00.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:00.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:00.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:00.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:38:00.000000 mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:01.180701 mypy-boto3-timestream-write-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-01 11:34:27.000000 mypy-boto3-timestream-write-1.28.16/setup.py
```

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/LICENSE` & `mypy-boto3-timestream-write-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/PKG-INFO` & `mypy-boto3-timestream-write-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.TimestreamWrite 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.TimestreamWrite 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 timestream-write type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 timestream-write type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-write)](https://pepy.tech/project/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
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
@@ -298,20 +298,20 @@
 )
 
 
 def check_value(value: BatchLoadDataFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_timestream_write.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
@@ -363,30 +363,32 @@
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelOutputTypeDef,
     DataModelTypeDef,
+    SchemaUnionTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
     UpdateTableRequestRequestTypeDef,
     DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
     BatchLoadTaskDescriptionTypeDef,
     CreateBatchLoadTaskRequestRequestTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
 )
 
 
-def get_structure() -> BatchLoadProgressReportTypeDef:
+def get_value() -> BatchLoadProgressReportTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/README.md` & `mypy-boto3-timestream-write-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-write)](https://pepy.tech/project/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
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
@@ -266,20 +266,20 @@
 )
 
 
 def check_value(value: BatchLoadDataFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_timestream_write.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
@@ -331,30 +331,32 @@
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelOutputTypeDef,
     DataModelTypeDef,
+    SchemaUnionTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
     UpdateTableRequestRequestTypeDef,
     DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
     BatchLoadTaskDescriptionTypeDef,
     CreateBatchLoadTaskRequestRequestTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
 )
 
 
-def get_structure() -> BatchLoadProgressReportTypeDef:
+def get_value() -> BatchLoadProgressReportTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/client.py` & `mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,41 +9,39 @@
     from boto3.session import Session
     from mypy_boto3_timestream_write.client import TimestreamWriteClient
 
     session = Session()
     client: TimestreamWriteClient = session.client("timestream-write")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BatchLoadStatusType
 from .type_defs import (
     CreateBatchLoadTaskResponseTypeDef,
     CreateDatabaseResponseTypeDef,
     CreateTableResponseTypeDef,
-    DataModelConfigurationOutputTypeDef,
-    DataModelConfigurationTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeTableResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
-    SchemaOutputTypeDef,
-    SchemaTypeDef,
+    SchemaUnionTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -107,17 +105,15 @@
         self,
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
-        DataModelConfiguration: Union[
-            DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
-        ] = ...,
+        DataModelConfiguration: DataModelConfigurationUnionTypeDef = ...,
         RecordVersion: int = ...
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_batch_load_task)
@@ -137,15 +133,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...
+        Schema: SchemaUnionTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_table)
         """
@@ -293,15 +289,15 @@
     def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...
+        Schema: SchemaUnionTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#update_table)
```

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/client.pyi` & `mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,41 +9,39 @@
     from boto3.session import Session
     from mypy_boto3_timestream_write.client import TimestreamWriteClient
 
     session = Session()
     client: TimestreamWriteClient = session.client("timestream-write")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BatchLoadStatusType
 from .type_defs import (
     CreateBatchLoadTaskResponseTypeDef,
     CreateDatabaseResponseTypeDef,
     CreateTableResponseTypeDef,
-    DataModelConfigurationOutputTypeDef,
-    DataModelConfigurationTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeTableResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
-    SchemaOutputTypeDef,
-    SchemaTypeDef,
+    SchemaUnionTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -101,17 +99,15 @@
         self,
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
-        DataModelConfiguration: Union[
-            DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
-        ] = ...,
+        DataModelConfiguration: DataModelConfigurationUnionTypeDef = ...,
         RecordVersion: int = ...
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_batch_load_task)
@@ -129,15 +125,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...
+        Schema: SchemaUnionTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_table)
         """
@@ -269,15 +265,15 @@
     def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...
+        Schema: SchemaUnionTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#update_table)
```

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/literals.py` & `mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/literals.pyi` & `mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/type_defs.py` & `mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_timestream_write.type_defs import BatchLoadProgressReportTypeDef
 
-    data: BatchLoadProgressReportTypeDef = {...}
+    data: BatchLoadProgressReportTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
     PartitionKeyEnforcementLevelType,
     PartitionKeyTypeType,
     S3EncryptionOptionType,
@@ -89,25 +89,27 @@
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
     "DataModelOutputTypeDef",
     "DataModelTypeDef",
+    "SchemaUnionTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
     "BatchLoadTaskDescriptionTypeDef",
     "CreateBatchLoadTaskRequestRequestTypeDef",
+    "DataModelConfigurationUnionTypeDef",
     "DescribeBatchLoadTaskResponseTypeDef",
 )
 
 BatchLoadProgressReportTypeDef = TypedDict(
     "BatchLoadProgressReportTypeDef",
     {
         "RecordsProcessed": int,
@@ -800,14 +802,15 @@
 )
 
 
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
 
+SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -963,14 +966,17 @@
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
 
+DataModelConfigurationUnionTypeDef = Union[
+    DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
+]
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/type_defs.pyi` & `mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_timestream_write.type_defs import BatchLoadProgressReportTypeDef
 
-    data: BatchLoadProgressReportTypeDef = {...}
+    data: BatchLoadProgressReportTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
     PartitionKeyEnforcementLevelType,
     PartitionKeyTypeType,
     S3EncryptionOptionType,
@@ -88,25 +88,27 @@
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
     "DataModelOutputTypeDef",
     "DataModelTypeDef",
+    "SchemaUnionTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
     "BatchLoadTaskDescriptionTypeDef",
     "CreateBatchLoadTaskRequestRequestTypeDef",
+    "DataModelConfigurationUnionTypeDef",
     "DescribeBatchLoadTaskResponseTypeDef",
 )
 
 BatchLoadProgressReportTypeDef = TypedDict(
     "BatchLoadProgressReportTypeDef",
     {
         "RecordsProcessed": int,
@@ -769,14 +771,15 @@
     },
     total=False,
 )
 
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
+SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -926,14 +929,17 @@
 
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
+DataModelConfigurationUnionTypeDef = Union[
+    DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
+]
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/PKG-INFO` & `mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.TimestreamWrite 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.TimestreamWrite 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 timestream-write type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 timestream-write type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-write)](https://pepy.tech/project/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
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
@@ -298,20 +298,20 @@
 )
 
 
 def check_value(value: BatchLoadDataFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_timestream_write.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
@@ -363,30 +363,32 @@
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelOutputTypeDef,
     DataModelTypeDef,
+    SchemaUnionTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
     UpdateTableRequestRequestTypeDef,
     DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
     BatchLoadTaskDescriptionTypeDef,
     CreateBatchLoadTaskRequestRequestTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
 )
 
 
-def get_structure() -> BatchLoadProgressReportTypeDef:
+def get_value() -> BatchLoadProgressReportTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/SOURCES.txt` & `mypy-boto3-timestream-write-1.28.16/mypy_boto3_timestream_write.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15.post1/setup.py` & `mypy-boto3-timestream-write-1.28.16/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-write",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_timestream_write"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamWrite 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.TimestreamWrite 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 timestream-write type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 timestream-write type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_timestream_write": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

