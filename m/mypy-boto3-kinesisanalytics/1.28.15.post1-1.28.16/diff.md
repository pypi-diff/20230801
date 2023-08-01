# Comparing `tmp/mypy-boto3-kinesisanalytics-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-kinesisanalytics-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisanalytics-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:28 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisanalytics-1.28.16.tar", last modified: Tue Aug  1 11:37:09 2023, max compression
```

## Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1.tar` & `mypy-boto3-kinesisanalytics-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:28.405223 mypy-boto3-kinesisanalytics-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-07-29 10:03:28.405223 mypy-boto3-kinesisanalytics-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:28.393223 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26473 2023-07-29 09:48:53.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26440 2023-07-29 09:48:53.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:28.405223 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:28.405223 mypy-boto3-kinesisanalytics-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:48:52.000000 mypy-boto3-kinesisanalytics-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.164846 mypy-boto3-kinesisanalytics-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:41.000000 mypy-boto3-kinesisanalytics-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-08-01 11:37:09.164846 mypy-boto3-kinesisanalytics-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-08-01 11:21:41.000000 mypy-boto3-kinesisanalytics-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.156846 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-01 11:21:41.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-01 11:21:41.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-01 11:21:41.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-08-01 11:21:42.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-08-01 11:21:41.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-08-01 11:21:42.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-08-01 11:21:42.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:41.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26531 2023-08-01 11:21:43.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26498 2023-08-01 11:21:42.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:41.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.164846 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-08-01 11:37:08.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 11:37:08.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:08.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:08.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:08.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:37:08.000000 mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:09.164846 mypy-boto3-kinesisanalytics-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 11:21:41.000000 mypy-boto3-kinesisanalytics-1.28.16/setup.py
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/LICENSE` & `mypy-boto3-kinesisanalytics-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/PKG-INFO` & `mypy-boto3-kinesisanalytics-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalytics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisAnalytics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesisanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesisanalytics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalytics)](https://pepy.tech/project/mypy-boto3-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[boto3.KinesisAnalytics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [mypy-boto3-kinesisanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/).
 
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
@@ -291,35 +291,35 @@
 )
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesisanalytics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
+    TimestampTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     InputParallelismTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
@@ -350,14 +350,15 @@
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
@@ -383,15 +384,15 @@
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     ApplicationUpdateTypeDef,
     DescribeApplicationResponseTypeDef,
     UpdateApplicationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/README.md` & `mypy-boto3-kinesisanalytics-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalytics)](https://pepy.tech/project/mypy-boto3-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[boto3.KinesisAnalytics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [mypy-boto3-kinesisanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/).
 
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
@@ -259,35 +259,35 @@
 )
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesisanalytics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
+    TimestampTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     InputParallelismTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
@@ -318,14 +318,15 @@
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
@@ -351,15 +352,15 @@
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     ApplicationUpdateTypeDef,
     DescribeApplicationResponseTypeDef,
     UpdateApplicationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/__main__.py` & `mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisAnalytics 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.KinesisAnalytics 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics\nOther"
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

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/client.py` & `mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_kinesisanalytics.client import KinesisAnalyticsClient
 
     session = Session()
     client: KinesisAnalyticsClient = session.client("kinesisanalytics")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     ApplicationUpdateTypeDef,
     CloudWatchLoggingOptionTypeDef,
     CreateApplicationResponseTypeDef,
@@ -30,14 +29,15 @@
     InputTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputTypeDef,
     ReferenceDataSourceTypeDef,
     S3ConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("KinesisAnalyticsClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -174,15 +174,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/client/#create_application)
         """
 
     def delete_application(
-        self, *, ApplicationName: str, CreateTimestamp: Union[datetime, str]
+        self, *, ApplicationName: str, CreateTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/client/#delete_application)
         """
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/client.pyi` & `mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_kinesisanalytics.client import KinesisAnalyticsClient
 
     session = Session()
     client: KinesisAnalyticsClient = session.client("kinesisanalytics")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     ApplicationUpdateTypeDef,
     CloudWatchLoggingOptionTypeDef,
     CreateApplicationResponseTypeDef,
@@ -30,14 +29,15 @@
     InputTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputTypeDef,
     ReferenceDataSourceTypeDef,
     S3ConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("KinesisAnalyticsClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -162,15 +162,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/client/#create_application)
         """
     def delete_application(
-        self, *, ApplicationName: str, CreateTimestamp: Union[datetime, str]
+        self, *, ApplicationName: str, CreateTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/client/#delete_application)
         """
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/literals.py` & `mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/literals.pyi` & `mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/type_defs.py` & `mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesisanalytics.type_defs import CloudWatchLoggingOptionTypeDef
 
-    data: CloudWatchLoggingOptionTypeDef = {...}
+    data: CloudWatchLoggingOptionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplicationStatusType, InputStartingPositionType, RecordFormatTypeType
@@ -31,15 +31,15 @@
     "CSVMappingParametersTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "InputParallelismTypeDef",
     "KinesisFirehoseInputDescriptionTypeDef",
     "KinesisStreamsInputDescriptionTypeDef",
@@ -70,14 +70,15 @@
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "DeleteApplicationRequestRequestTypeDef",
     "InputConfigurationTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
@@ -238,22 +239,15 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceId": str,
     },
 )
 
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CreateTimestamp": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 
@@ -577,14 +571,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteApplicationRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CreateTimestamp": TimestampTypeDef,
+    },
+)
+
 InputConfigurationTypeDef = TypedDict(
     "InputConfigurationTypeDef",
     {
         "Id": str,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics/type_defs.pyi` & `mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesisanalytics.type_defs import CloudWatchLoggingOptionTypeDef
 
-    data: CloudWatchLoggingOptionTypeDef = {...}
+    data: CloudWatchLoggingOptionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplicationStatusType, InputStartingPositionType, RecordFormatTypeType
@@ -30,15 +30,15 @@
     "CSVMappingParametersTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "InputParallelismTypeDef",
     "KinesisFirehoseInputDescriptionTypeDef",
     "KinesisStreamsInputDescriptionTypeDef",
@@ -69,14 +69,15 @@
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "DeleteApplicationRequestRequestTypeDef",
     "InputConfigurationTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
@@ -231,22 +232,15 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceId": str,
     },
 )
 
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CreateTimestamp": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 
@@ -568,14 +562,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteApplicationRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CreateTimestamp": TimestampTypeDef,
+    },
+)
+
 InputConfigurationTypeDef = TypedDict(
     "InputConfigurationTypeDef",
     {
         "Id": str,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO` & `mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalytics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisAnalytics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesisanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesisanalytics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalytics)](https://pepy.tech/project/mypy-boto3-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[boto3.KinesisAnalytics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [mypy-boto3-kinesisanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/).
 
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
@@ -291,35 +291,35 @@
 )
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesisanalytics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
+    TimestampTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     InputParallelismTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
@@ -350,14 +350,15 @@
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
@@ -383,15 +384,15 @@
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     ApplicationUpdateTypeDef,
     DescribeApplicationResponseTypeDef,
     UpdateApplicationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt` & `mypy-boto3-kinesisanalytics-1.28.16/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.15.post1/setup.py` & `mypy-boto3-kinesisanalytics-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisanalytics",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_kinesisanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisAnalytics 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.KinesisAnalytics 1.28.16 service generated with"
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
-    keywords="boto3 kinesisanalytics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 kinesisanalytics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_kinesisanalytics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

