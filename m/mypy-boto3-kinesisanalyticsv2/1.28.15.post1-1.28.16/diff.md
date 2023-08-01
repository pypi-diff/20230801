# Comparing `tmp/mypy-boto3-kinesisanalyticsv2-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-kinesisanalyticsv2-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisanalyticsv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:28 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisanalyticsv2-1.28.16.tar", last modified: Tue Aug  1 11:37:09 2023, max compression
```

## Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1.tar` & `mypy-boto3-kinesisanalyticsv2-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:28.741225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-29 10:03:28.741225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:28.729225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27553 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27513 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-29 09:48:57.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-29 09:48:57.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69775 2023-07-29 09:48:58.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69672 2023-07-29 09:48:58.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:28.741225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:28.741225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.288846 mypy-boto3-kinesisanalyticsv2-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-08-01 11:37:09.280846 mypy-boto3-kinesisanalyticsv2-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19804 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.272846 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27530 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27490 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69844 2023-08-01 11:21:46.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69741 2023-08-01 11:21:45.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.280846 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-08-01 11:37:09.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-01 11:37:09.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:09.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 11:37:09.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:09.288846 mypy-boto3-kinesisanalyticsv2-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-01 11:21:43.000000 mypy-boto3-kinesisanalyticsv2-1.28.16/setup.py
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/LICENSE` & `mypy-boto3-kinesisanalyticsv2-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/PKG-INFO` & `mypy-boto3-kinesisanalyticsv2-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalyticsv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesisanalyticsv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesisanalyticsv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalyticsv2)](https://pepy.tech/project/mypy-boto3-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalyticsV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[boto3.KinesisAnalyticsV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
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
@@ -331,20 +331,20 @@
 )
 
 
 def check_value(value: ApplicationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesisanalyticsv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesisanalyticsv2.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
@@ -354,14 +354,15 @@
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
+    BlobTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
@@ -373,16 +374,15 @@
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteApplicationSnapshotRequestRequestTypeDef,
+    TimestampTypeDef,
     DeleteApplicationVpcConfigurationRequestRequestTypeDef,
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
@@ -455,14 +455,16 @@
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
+    DeleteApplicationSnapshotRequestRequestTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
     ListApplicationSnapshotsResponseTypeDef,
     SqlRunConfigurationTypeDef,
     EnvironmentPropertiesTypeDef,
@@ -523,15 +525,15 @@
     DescribeApplicationResponseTypeDef,
     DescribeApplicationVersionResponseTypeDef,
     RollbackApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/README.md` & `mypy-boto3-kinesisanalyticsv2-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalyticsv2)](https://pepy.tech/project/mypy-boto3-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalyticsV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[boto3.KinesisAnalyticsV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
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
@@ -299,20 +299,20 @@
 )
 
 
 def check_value(value: ApplicationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesisanalyticsv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesisanalyticsv2.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
@@ -322,14 +322,15 @@
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
+    BlobTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
@@ -341,16 +342,15 @@
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteApplicationSnapshotRequestRequestTypeDef,
+    TimestampTypeDef,
     DeleteApplicationVpcConfigurationRequestRequestTypeDef,
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
@@ -423,14 +423,16 @@
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
+    DeleteApplicationSnapshotRequestRequestTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
     ListApplicationSnapshotsResponseTypeDef,
     SqlRunConfigurationTypeDef,
     EnvironmentPropertiesTypeDef,
@@ -491,15 +493,15 @@
     DescribeApplicationResponseTypeDef,
     DescribeApplicationVersionResponseTypeDef,
     RollbackApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__init__.py` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__init__.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__main__.py` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisAnalyticsV2 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.KinesisAnalyticsV2 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2\nOther"
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

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/client.py` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_kinesisanalyticsv2.client import KinesisAnalyticsV2Client
 
     session = Session()
     client: KinesisAnalyticsV2Client = session.client("kinesisanalyticsv2")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ApplicationModeType, RuntimeEnvironmentType, UrlTypeType
 from .paginator import ListApplicationSnapshotsPaginator, ListApplicationsPaginator
 from .type_defs import (
     AddApplicationCloudWatchLoggingOptionResponseTypeDef,
@@ -54,14 +53,15 @@
     OutputTypeDef,
     ReferenceDataSourceTypeDef,
     RollbackApplicationResponseTypeDef,
     RunConfigurationTypeDef,
     RunConfigurationUpdateTypeDef,
     S3ConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -254,15 +254,15 @@
         Creates a snapshot of the application's state data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.create_application_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/client/#create_application_snapshot)
         """
 
     def delete_application(
-        self, *, ApplicationName: str, CreateTimestamp: Union[datetime, str]
+        self, *, ApplicationName: str, CreateTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         Deletes the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/client/#delete_application)
         """
@@ -316,15 +316,15 @@
         """
 
     def delete_application_snapshot(
         self,
         *,
         ApplicationName: str,
         SnapshotName: str,
-        SnapshotCreationTimestamp: Union[datetime, str]
+        SnapshotCreationTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         Deletes a snapshot of application state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/client/#delete_application_snapshot)
         """
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/client.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_kinesisanalyticsv2.client import KinesisAnalyticsV2Client
 
     session = Session()
     client: KinesisAnalyticsV2Client = session.client("kinesisanalyticsv2")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ApplicationModeType, RuntimeEnvironmentType, UrlTypeType
 from .paginator import ListApplicationSnapshotsPaginator, ListApplicationsPaginator
 from .type_defs import (
     AddApplicationCloudWatchLoggingOptionResponseTypeDef,
@@ -54,14 +53,15 @@
     OutputTypeDef,
     ReferenceDataSourceTypeDef,
     RollbackApplicationResponseTypeDef,
     RunConfigurationTypeDef,
     RunConfigurationUpdateTypeDef,
     S3ConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -238,15 +238,15 @@
         """
         Creates a snapshot of the application's state data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.create_application_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/client/#create_application_snapshot)
         """
     def delete_application(
-        self, *, ApplicationName: str, CreateTimestamp: Union[datetime, str]
+        self, *, ApplicationName: str, CreateTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         Deletes the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/client/#delete_application)
         """
@@ -295,15 +295,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/client/#delete_application_reference_data_source)
         """
     def delete_application_snapshot(
         self,
         *,
         ApplicationName: str,
         SnapshotName: str,
-        SnapshotCreationTimestamp: Union[datetime, str]
+        SnapshotCreationTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         Deletes a snapshot of application state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/client/#delete_application_snapshot)
         """
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/literals.py` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/literals.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/paginator.py` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/paginator.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/type_defs.py` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesisanalyticsv2.type_defs import CloudWatchLoggingOptionTypeDef
 
-    data: CloudWatchLoggingOptionTypeDef = {...}
+    data: CloudWatchLoggingOptionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -50,14 +50,15 @@
     "ApplicationSnapshotConfigurationUpdateTypeDef",
     "VpcConfigurationUpdateTypeDef",
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
     "ApplicationRestoreConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
+    "BlobTypeDef",
     "CSVMappingParametersTypeDef",
     "GlueDataCatalogConfigurationDescriptionTypeDef",
     "GlueDataCatalogConfigurationTypeDef",
     "GlueDataCatalogConfigurationUpdateTypeDef",
     "CheckpointConfigurationDescriptionTypeDef",
     "CheckpointConfigurationTypeDef",
     "CheckpointConfigurationUpdateTypeDef",
@@ -69,16 +70,15 @@
     "TagTypeDef",
     "CreateApplicationSnapshotRequestRequestTypeDef",
     "MavenReferenceTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationRequestRequestTypeDef",
-    "DeleteApplicationSnapshotRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DeleteApplicationVpcConfigurationRequestRequestTypeDef",
     "S3ContentBaseLocationDescriptionTypeDef",
     "S3ContentBaseLocationTypeDef",
     "S3ContentBaseLocationUpdateTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
@@ -151,14 +151,16 @@
     "CodeContentDescriptionTypeDef",
     "CodeContentTypeDef",
     "CodeContentUpdateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomArtifactConfigurationDescriptionTypeDef",
     "CustomArtifactConfigurationTypeDef",
+    "DeleteApplicationRequestRequestTypeDef",
+    "DeleteApplicationSnapshotRequestRequestTypeDef",
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
     "ListApplicationSnapshotsResponseTypeDef",
     "SqlRunConfigurationTypeDef",
     "EnvironmentPropertiesTypeDef",
@@ -389,14 +391,15 @@
     "ApplicationVersionSummaryTypeDef",
     {
         "ApplicationVersionId": int,
         "ApplicationStatus": ApplicationStatusType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -649,31 +652,15 @@
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
-DeleteApplicationSnapshotRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationSnapshotRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "SnapshotName": str,
-        "SnapshotCreationTimestamp": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "VpcConfigurationId": str,
     },
 )
@@ -1558,25 +1545,25 @@
     total=False,
 )
 
 CodeContentTypeDef = TypedDict(
     "CodeContentTypeDef",
     {
         "TextContent": str,
-        "ZipFileContent": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFileContent": BlobTypeDef,
         "S3ContentLocation": S3ContentLocationTypeDef,
     },
     total=False,
 )
 
 CodeContentUpdateTypeDef = TypedDict(
     "CodeContentUpdateTypeDef",
     {
         "TextContentUpdate": str,
-        "ZipFileContentUpdate": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFileContentUpdate": BlobTypeDef,
         "S3ContentLocationUpdate": S3ContentLocationUpdateTypeDef,
     },
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
@@ -1622,14 +1609,31 @@
 
 class CustomArtifactConfigurationTypeDef(
     _RequiredCustomArtifactConfigurationTypeDef, _OptionalCustomArtifactConfigurationTypeDef
 ):
     pass
 
 
+DeleteApplicationRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CreateTimestamp": TimestampTypeDef,
+    },
+)
+
+DeleteApplicationSnapshotRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationSnapshotRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "SnapshotName": str,
+        "SnapshotCreationTimestamp": TimestampTypeDef,
+    },
+)
+
 DeployAsApplicationConfigurationDescriptionTypeDef = TypedDict(
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     {
         "S3ContentLocationDescription": S3ContentBaseLocationDescriptionTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/type_defs.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesisanalyticsv2.type_defs import CloudWatchLoggingOptionTypeDef
 
-    data: CloudWatchLoggingOptionTypeDef = {...}
+    data: CloudWatchLoggingOptionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -49,14 +49,15 @@
     "ApplicationSnapshotConfigurationUpdateTypeDef",
     "VpcConfigurationUpdateTypeDef",
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
     "ApplicationRestoreConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
+    "BlobTypeDef",
     "CSVMappingParametersTypeDef",
     "GlueDataCatalogConfigurationDescriptionTypeDef",
     "GlueDataCatalogConfigurationTypeDef",
     "GlueDataCatalogConfigurationUpdateTypeDef",
     "CheckpointConfigurationDescriptionTypeDef",
     "CheckpointConfigurationTypeDef",
     "CheckpointConfigurationUpdateTypeDef",
@@ -68,16 +69,15 @@
     "TagTypeDef",
     "CreateApplicationSnapshotRequestRequestTypeDef",
     "MavenReferenceTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationRequestRequestTypeDef",
-    "DeleteApplicationSnapshotRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DeleteApplicationVpcConfigurationRequestRequestTypeDef",
     "S3ContentBaseLocationDescriptionTypeDef",
     "S3ContentBaseLocationTypeDef",
     "S3ContentBaseLocationUpdateTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
@@ -150,14 +150,16 @@
     "CodeContentDescriptionTypeDef",
     "CodeContentTypeDef",
     "CodeContentUpdateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomArtifactConfigurationDescriptionTypeDef",
     "CustomArtifactConfigurationTypeDef",
+    "DeleteApplicationRequestRequestTypeDef",
+    "DeleteApplicationSnapshotRequestRequestTypeDef",
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
     "ListApplicationSnapshotsResponseTypeDef",
     "SqlRunConfigurationTypeDef",
     "EnvironmentPropertiesTypeDef",
@@ -380,14 +382,15 @@
     "ApplicationVersionSummaryTypeDef",
     {
         "ApplicationVersionId": int,
         "ApplicationStatus": ApplicationStatusType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -626,31 +629,15 @@
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
-DeleteApplicationSnapshotRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationSnapshotRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "SnapshotName": str,
-        "SnapshotCreationTimestamp": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "VpcConfigurationId": str,
     },
 )
@@ -1495,25 +1482,25 @@
     total=False,
 )
 
 CodeContentTypeDef = TypedDict(
     "CodeContentTypeDef",
     {
         "TextContent": str,
-        "ZipFileContent": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFileContent": BlobTypeDef,
         "S3ContentLocation": S3ContentLocationTypeDef,
     },
     total=False,
 )
 
 CodeContentUpdateTypeDef = TypedDict(
     "CodeContentUpdateTypeDef",
     {
         "TextContentUpdate": str,
-        "ZipFileContentUpdate": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFileContentUpdate": BlobTypeDef,
         "S3ContentLocationUpdate": S3ContentLocationUpdateTypeDef,
     },
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
@@ -1557,14 +1544,31 @@
 )
 
 class CustomArtifactConfigurationTypeDef(
     _RequiredCustomArtifactConfigurationTypeDef, _OptionalCustomArtifactConfigurationTypeDef
 ):
     pass
 
+DeleteApplicationRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CreateTimestamp": TimestampTypeDef,
+    },
+)
+
+DeleteApplicationSnapshotRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationSnapshotRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "SnapshotName": str,
+        "SnapshotCreationTimestamp": TimestampTypeDef,
+    },
+)
+
 DeployAsApplicationConfigurationDescriptionTypeDef = TypedDict(
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     {
         "S3ContentLocationDescription": S3ContentBaseLocationDescriptionTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalyticsv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesisanalyticsv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesisanalyticsv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalyticsv2)](https://pepy.tech/project/mypy-boto3-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalyticsV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[boto3.KinesisAnalyticsV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
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
@@ -331,20 +331,20 @@
 )
 
 
 def check_value(value: ApplicationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesisanalyticsv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesisanalyticsv2.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
@@ -354,14 +354,15 @@
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
+    BlobTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
@@ -373,16 +374,15 @@
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteApplicationSnapshotRequestRequestTypeDef,
+    TimestampTypeDef,
     DeleteApplicationVpcConfigurationRequestRequestTypeDef,
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
@@ -455,14 +455,16 @@
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
+    DeleteApplicationSnapshotRequestRequestTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
     ListApplicationSnapshotsResponseTypeDef,
     SqlRunConfigurationTypeDef,
     EnvironmentPropertiesTypeDef,
@@ -523,15 +525,15 @@
     DescribeApplicationResponseTypeDef,
     DescribeApplicationVersionResponseTypeDef,
     RollbackApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt` & `mypy-boto3-kinesisanalyticsv2-1.28.16/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/setup.py` & `mypy-boto3-kinesisanalyticsv2-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisanalyticsv2",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_kinesisanalyticsv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.KinesisAnalyticsV2 1.28.16 service generated with"
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
-    keywords="boto3 kinesisanalyticsv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 kinesisanalyticsv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_kinesisanalyticsv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/"
```

