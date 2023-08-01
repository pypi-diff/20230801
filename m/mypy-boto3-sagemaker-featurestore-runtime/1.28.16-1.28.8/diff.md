# Comparing `tmp/mypy-boto3-sagemaker-featurestore-runtime-1.28.16.tar.gz` & `tmp/mypy-boto3-sagemaker-featurestore-runtime-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-featurestore-runtime-1.28.16.tar", last modified: Tue Aug  1 11:37:45 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-featurestore-runtime-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16.tar` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.596753 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-08-01 11:37:45.592753 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.588753 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.592753 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:45.596753 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 11:32:00.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-20 19:47:15.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/setup.py
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/LICENSE` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/PKG-INFO` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-featurestore-runtime
-Version: 1.28.16
-Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.8
+Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-featurestore-runtime type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 sagemaker-featurestore-runtime type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-featurestore-runtime"></a>
 
 # mypy-boto3-sagemaker-featurestore-runtime
 
 [![PyPI - mypy-boto3-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-featurestore-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-featurestore-runtime)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
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
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -291,43 +291,43 @@
 )
 
 
 def check_value(value: DeletionModeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_sagemaker_featurestore_runtime.type_defs` module contains
-structures and shapes assembled to typed dictionaries and unions for additional
-type checking.
+structures and shapes assembled to typed dictionaries for additional type
+checking.
 
 ```python
 from mypy_boto3_sagemaker_featurestore_runtime.type_defs import (
     BatchGetRecordErrorTypeDef,
     BatchGetRecordIdentifierOutputTypeDef,
     BatchGetRecordIdentifierTypeDef,
     ResponseMetadataTypeDef,
-    FeatureValueTypeDef,
+    FeatureValueOutputTypeDef,
     DeleteRecordRequestRequestTypeDef,
+    FeatureValueTypeDef,
     GetRecordRequestRequestTypeDef,
     TtlDurationTypeDef,
-    BatchGetRecordIdentifierUnionTypeDef,
+    BatchGetRecordRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     BatchGetRecordResultDetailTypeDef,
     GetRecordResponseTypeDef,
     PutRecordRequestRequestTypeDef,
-    BatchGetRecordRequestRequestTypeDef,
     BatchGetRecordResponseTypeDef,
 )
 
 
-def get_value() -> BatchGetRecordErrorTypeDef:
+def get_structure() -> BatchGetRecordErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/README.md` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-featurestore-runtime"></a>
 
 # mypy-boto3-sagemaker-featurestore-runtime
 
 [![PyPI - mypy-boto3-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-featurestore-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-featurestore-runtime)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
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
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -259,43 +259,43 @@
 )
 
 
 def check_value(value: DeletionModeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_sagemaker_featurestore_runtime.type_defs` module contains
-structures and shapes assembled to typed dictionaries and unions for additional
-type checking.
+structures and shapes assembled to typed dictionaries for additional type
+checking.
 
 ```python
 from mypy_boto3_sagemaker_featurestore_runtime.type_defs import (
     BatchGetRecordErrorTypeDef,
     BatchGetRecordIdentifierOutputTypeDef,
     BatchGetRecordIdentifierTypeDef,
     ResponseMetadataTypeDef,
-    FeatureValueTypeDef,
+    FeatureValueOutputTypeDef,
     DeleteRecordRequestRequestTypeDef,
+    FeatureValueTypeDef,
     GetRecordRequestRequestTypeDef,
     TtlDurationTypeDef,
-    BatchGetRecordIdentifierUnionTypeDef,
+    BatchGetRecordRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     BatchGetRecordResultDetailTypeDef,
     GetRecordResponseTypeDef,
     PutRecordRequestRequestTypeDef,
-    BatchGetRecordRequestRequestTypeDef,
     BatchGetRecordResponseTypeDef,
 )
 
 
-def get_value() -> BatchGetRecordErrorTypeDef:
+def get_structure() -> BatchGetRecordErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/__init__.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/__main__.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.16\nVersion:        "
-        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8\nVersion:        "
+        " 1.28.8\nBuilder version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/client.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DeletionModeType, ExpirationTimeResponseType, TargetStoreType
 from .type_defs import (
-    BatchGetRecordIdentifierUnionTypeDef,
+    BatchGetRecordIdentifierTypeDef,
     BatchGetRecordResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FeatureValueTypeDef,
     GetRecordResponseTypeDef,
     TtlDurationTypeDef,
 )
 
@@ -63,15 +63,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#exceptions)
         """
 
     def batch_get_record(
         self,
         *,
-        Identifiers: Sequence[BatchGetRecordIdentifierUnionTypeDef],
+        Identifiers: Sequence[BatchGetRecordIdentifierTypeDef],
         ExpirationTimeResponse: ExpirationTimeResponseType = ...
     ) -> BatchGetRecordResponseTypeDef:
         """
         Retrieves a batch of `Records` from a `FeatureGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.batch_get_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#batch_get_record)
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/client.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DeletionModeType, ExpirationTimeResponseType, TargetStoreType
 from .type_defs import (
-    BatchGetRecordIdentifierUnionTypeDef,
+    BatchGetRecordIdentifierTypeDef,
     BatchGetRecordResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FeatureValueTypeDef,
     GetRecordResponseTypeDef,
     TtlDurationTypeDef,
 )
 
@@ -59,15 +59,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#exceptions)
         """
     def batch_get_record(
         self,
         *,
-        Identifiers: Sequence[BatchGetRecordIdentifierUnionTypeDef],
+        Identifiers: Sequence[BatchGetRecordIdentifierTypeDef],
         ExpirationTimeResponse: ExpirationTimeResponseType = ...
     ) -> BatchGetRecordResponseTypeDef:
         """
         Retrieves a batch of `Records` from a `FeatureGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.batch_get_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#batch_get_record)
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/literals.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,14 @@
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
@@ -237,15 +236,14 @@
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

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,14 @@
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
@@ -235,15 +234,14 @@
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

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_featurestore_runtime.type_defs import BatchGetRecordErrorTypeDef
 
-    data: BatchGetRecordErrorTypeDef = ...
+    data: BatchGetRecordErrorTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     DeletionModeType,
     ExpirationTimeResponseType,
     TargetStoreType,
     TtlDurationUnitType,
 )
@@ -28,59 +28,46 @@
 
 
 __all__ = (
     "BatchGetRecordErrorTypeDef",
     "BatchGetRecordIdentifierOutputTypeDef",
     "BatchGetRecordIdentifierTypeDef",
     "ResponseMetadataTypeDef",
-    "FeatureValueTypeDef",
+    "FeatureValueOutputTypeDef",
     "DeleteRecordRequestRequestTypeDef",
+    "FeatureValueTypeDef",
     "GetRecordRequestRequestTypeDef",
     "TtlDurationTypeDef",
-    "BatchGetRecordIdentifierUnionTypeDef",
+    "BatchGetRecordRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "BatchGetRecordResultDetailTypeDef",
     "GetRecordResponseTypeDef",
     "PutRecordRequestRequestTypeDef",
-    "BatchGetRecordRequestRequestTypeDef",
     "BatchGetRecordResponseTypeDef",
 )
 
 BatchGetRecordErrorTypeDef = TypedDict(
     "BatchGetRecordErrorTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_RequiredBatchGetRecordIdentifierOutputTypeDef",
+BatchGetRecordIdentifierOutputTypeDef = TypedDict(
+    "BatchGetRecordIdentifierOutputTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": List[str],
-    },
-)
-_OptionalBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_OptionalBatchGetRecordIdentifierOutputTypeDef",
-    {
         "FeatureNames": List[str],
     },
-    total=False,
 )
 
-
-class BatchGetRecordIdentifierOutputTypeDef(
-    _RequiredBatchGetRecordIdentifierOutputTypeDef, _OptionalBatchGetRecordIdentifierOutputTypeDef
-):
-    pass
-
-
 _RequiredBatchGetRecordIdentifierTypeDef = TypedDict(
     "_RequiredBatchGetRecordIdentifierTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": Sequence[str],
     },
 )
@@ -106,16 +93,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-FeatureValueTypeDef = TypedDict(
-    "FeatureValueTypeDef",
+FeatureValueOutputTypeDef = TypedDict(
+    "FeatureValueOutputTypeDef",
     {
         "FeatureName": str,
         "ValueAsString": str,
     },
 )
 
 _RequiredDeleteRecordRequestRequestTypeDef = TypedDict(
@@ -138,14 +125,22 @@
 
 class DeleteRecordRequestRequestTypeDef(
     _RequiredDeleteRecordRequestRequestTypeDef, _OptionalDeleteRecordRequestRequestTypeDef
 ):
     pass
 
 
+FeatureValueTypeDef = TypedDict(
+    "FeatureValueTypeDef",
+    {
+        "FeatureName": str,
+        "ValueAsString": str,
+    },
+)
+
 _RequiredGetRecordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecordRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
     },
 )
@@ -169,51 +164,56 @@
     "TtlDurationTypeDef",
     {
         "Unit": TtlDurationUnitType,
         "Value": int,
     },
 )
 
-BatchGetRecordIdentifierUnionTypeDef = Union[
-    BatchGetRecordIdentifierTypeDef, BatchGetRecordIdentifierOutputTypeDef
-]
+_RequiredBatchGetRecordRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetRecordRequestRequestTypeDef",
+    {
+        "Identifiers": Sequence[BatchGetRecordIdentifierTypeDef],
+    },
+)
+_OptionalBatchGetRecordRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetRecordRequestRequestTypeDef",
+    {
+        "ExpirationTimeResponse": ExpirationTimeResponseType,
+    },
+    total=False,
+)
+
+
+class BatchGetRecordRequestRequestTypeDef(
+    _RequiredBatchGetRecordRequestRequestTypeDef, _OptionalBatchGetRecordRequestRequestTypeDef
+):
+    pass
+
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_RequiredBatchGetRecordResultDetailTypeDef",
+BatchGetRecordResultDetailTypeDef = TypedDict(
+    "BatchGetRecordResultDetailTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
-        "Record": List[FeatureValueTypeDef],
-    },
-)
-_OptionalBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_OptionalBatchGetRecordResultDetailTypeDef",
-    {
+        "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
     },
-    total=False,
 )
 
-
-class BatchGetRecordResultDetailTypeDef(
-    _RequiredBatchGetRecordResultDetailTypeDef, _OptionalBatchGetRecordResultDetailTypeDef
-):
-    pass
-
-
 GetRecordResponseTypeDef = TypedDict(
     "GetRecordResponseTypeDef",
     {
-        "Record": List[FeatureValueTypeDef],
+        "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecordRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecordRequestRequestTypeDef",
@@ -234,35 +234,14 @@
 
 class PutRecordRequestRequestTypeDef(
     _RequiredPutRecordRequestRequestTypeDef, _OptionalPutRecordRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredBatchGetRecordRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetRecordRequestRequestTypeDef",
-    {
-        "Identifiers": Sequence[BatchGetRecordIdentifierUnionTypeDef],
-    },
-)
-_OptionalBatchGetRecordRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetRecordRequestRequestTypeDef",
-    {
-        "ExpirationTimeResponse": ExpirationTimeResponseType,
-    },
-    total=False,
-)
-
-
-class BatchGetRecordRequestRequestTypeDef(
-    _RequiredBatchGetRecordRequestRequestTypeDef, _OptionalBatchGetRecordRequestRequestTypeDef
-):
-    pass
-
-
 BatchGetRecordResponseTypeDef = TypedDict(
     "BatchGetRecordResponseTypeDef",
     {
         "Records": List[BatchGetRecordResultDetailTypeDef],
         "Errors": List[BatchGetRecordErrorTypeDef],
         "UnprocessedIdentifiers": List[BatchGetRecordIdentifierOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_featurestore_runtime.type_defs import BatchGetRecordErrorTypeDef
 
-    data: BatchGetRecordErrorTypeDef = ...
+    data: BatchGetRecordErrorTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     DeletionModeType,
     ExpirationTimeResponseType,
     TargetStoreType,
     TtlDurationUnitType,
 )
@@ -27,57 +27,46 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchGetRecordErrorTypeDef",
     "BatchGetRecordIdentifierOutputTypeDef",
     "BatchGetRecordIdentifierTypeDef",
     "ResponseMetadataTypeDef",
-    "FeatureValueTypeDef",
+    "FeatureValueOutputTypeDef",
     "DeleteRecordRequestRequestTypeDef",
+    "FeatureValueTypeDef",
     "GetRecordRequestRequestTypeDef",
     "TtlDurationTypeDef",
-    "BatchGetRecordIdentifierUnionTypeDef",
+    "BatchGetRecordRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "BatchGetRecordResultDetailTypeDef",
     "GetRecordResponseTypeDef",
     "PutRecordRequestRequestTypeDef",
-    "BatchGetRecordRequestRequestTypeDef",
     "BatchGetRecordResponseTypeDef",
 )
 
 BatchGetRecordErrorTypeDef = TypedDict(
     "BatchGetRecordErrorTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_RequiredBatchGetRecordIdentifierOutputTypeDef",
+BatchGetRecordIdentifierOutputTypeDef = TypedDict(
+    "BatchGetRecordIdentifierOutputTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": List[str],
-    },
-)
-_OptionalBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_OptionalBatchGetRecordIdentifierOutputTypeDef",
-    {
         "FeatureNames": List[str],
     },
-    total=False,
 )
 
-class BatchGetRecordIdentifierOutputTypeDef(
-    _RequiredBatchGetRecordIdentifierOutputTypeDef, _OptionalBatchGetRecordIdentifierOutputTypeDef
-):
-    pass
-
 _RequiredBatchGetRecordIdentifierTypeDef = TypedDict(
     "_RequiredBatchGetRecordIdentifierTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": Sequence[str],
     },
 )
@@ -101,16 +90,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-FeatureValueTypeDef = TypedDict(
-    "FeatureValueTypeDef",
+FeatureValueOutputTypeDef = TypedDict(
+    "FeatureValueOutputTypeDef",
     {
         "FeatureName": str,
         "ValueAsString": str,
     },
 )
 
 _RequiredDeleteRecordRequestRequestTypeDef = TypedDict(
@@ -131,14 +120,22 @@
 )
 
 class DeleteRecordRequestRequestTypeDef(
     _RequiredDeleteRecordRequestRequestTypeDef, _OptionalDeleteRecordRequestRequestTypeDef
 ):
     pass
 
+FeatureValueTypeDef = TypedDict(
+    "FeatureValueTypeDef",
+    {
+        "FeatureName": str,
+        "ValueAsString": str,
+    },
+)
+
 _RequiredGetRecordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecordRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
     },
 )
@@ -160,49 +157,54 @@
     "TtlDurationTypeDef",
     {
         "Unit": TtlDurationUnitType,
         "Value": int,
     },
 )
 
-BatchGetRecordIdentifierUnionTypeDef = Union[
-    BatchGetRecordIdentifierTypeDef, BatchGetRecordIdentifierOutputTypeDef
-]
+_RequiredBatchGetRecordRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetRecordRequestRequestTypeDef",
+    {
+        "Identifiers": Sequence[BatchGetRecordIdentifierTypeDef],
+    },
+)
+_OptionalBatchGetRecordRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetRecordRequestRequestTypeDef",
+    {
+        "ExpirationTimeResponse": ExpirationTimeResponseType,
+    },
+    total=False,
+)
+
+class BatchGetRecordRequestRequestTypeDef(
+    _RequiredBatchGetRecordRequestRequestTypeDef, _OptionalBatchGetRecordRequestRequestTypeDef
+):
+    pass
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_RequiredBatchGetRecordResultDetailTypeDef",
+BatchGetRecordResultDetailTypeDef = TypedDict(
+    "BatchGetRecordResultDetailTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
-        "Record": List[FeatureValueTypeDef],
-    },
-)
-_OptionalBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_OptionalBatchGetRecordResultDetailTypeDef",
-    {
+        "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
     },
-    total=False,
 )
 
-class BatchGetRecordResultDetailTypeDef(
-    _RequiredBatchGetRecordResultDetailTypeDef, _OptionalBatchGetRecordResultDetailTypeDef
-):
-    pass
-
 GetRecordResponseTypeDef = TypedDict(
     "GetRecordResponseTypeDef",
     {
-        "Record": List[FeatureValueTypeDef],
+        "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecordRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecordRequestRequestTypeDef",
@@ -221,33 +223,14 @@
 )
 
 class PutRecordRequestRequestTypeDef(
     _RequiredPutRecordRequestRequestTypeDef, _OptionalPutRecordRequestRequestTypeDef
 ):
     pass
 
-_RequiredBatchGetRecordRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetRecordRequestRequestTypeDef",
-    {
-        "Identifiers": Sequence[BatchGetRecordIdentifierUnionTypeDef],
-    },
-)
-_OptionalBatchGetRecordRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetRecordRequestRequestTypeDef",
-    {
-        "ExpirationTimeResponse": ExpirationTimeResponseType,
-    },
-    total=False,
-)
-
-class BatchGetRecordRequestRequestTypeDef(
-    _RequiredBatchGetRecordRequestRequestTypeDef, _OptionalBatchGetRecordRequestRequestTypeDef
-):
-    pass
-
 BatchGetRecordResponseTypeDef = TypedDict(
     "BatchGetRecordResponseTypeDef",
     {
         "Records": List[BatchGetRecordResultDetailTypeDef],
         "Errors": List[BatchGetRecordErrorTypeDef],
         "UnprocessedIdentifiers": List[BatchGetRecordIdentifierOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-featurestore-runtime
-Version: 1.28.16
-Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.8
+Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-featurestore-runtime type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 sagemaker-featurestore-runtime type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-featurestore-runtime"></a>
 
 # mypy-boto3-sagemaker-featurestore-runtime
 
 [![PyPI - mypy-boto3-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-featurestore-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-featurestore-runtime)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
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
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -291,43 +291,43 @@
 )
 
 
 def check_value(value: DeletionModeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_sagemaker_featurestore_runtime.type_defs` module contains
-structures and shapes assembled to typed dictionaries and unions for additional
-type checking.
+structures and shapes assembled to typed dictionaries for additional type
+checking.
 
 ```python
 from mypy_boto3_sagemaker_featurestore_runtime.type_defs import (
     BatchGetRecordErrorTypeDef,
     BatchGetRecordIdentifierOutputTypeDef,
     BatchGetRecordIdentifierTypeDef,
     ResponseMetadataTypeDef,
-    FeatureValueTypeDef,
+    FeatureValueOutputTypeDef,
     DeleteRecordRequestRequestTypeDef,
+    FeatureValueTypeDef,
     GetRecordRequestRequestTypeDef,
     TtlDurationTypeDef,
-    BatchGetRecordIdentifierUnionTypeDef,
+    BatchGetRecordRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     BatchGetRecordResultDetailTypeDef,
     GetRecordResponseTypeDef,
     PutRecordRequestRequestTypeDef,
-    BatchGetRecordRequestRequestTypeDef,
     BatchGetRecordResponseTypeDef,
 )
 
 
-def get_value() -> BatchGetRecordErrorTypeDef:
+def get_structure() -> BatchGetRecordErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.16/setup.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-featurestore-runtime",
-    version="1.28.16",
+    version="1.28.8",
     packages=["mypy_boto3_sagemaker_featurestore_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.16 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -35,15 +35,16 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords=(
-        "boto3 sagemaker-featurestore-runtime type-annotations botocore mypy typeshed autocomplete"
+        "boto3 sagemaker-featurestore-runtime type-annotations boto3-stubs mypy typeshed"
+        " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sagemaker_featurestore_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
```

