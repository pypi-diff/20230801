# Comparing `tmp/mypy-boto3-cognito-sync-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-cognito-sync-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-sync-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:48 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-sync-1.28.16.tar", last modified: Tue Aug  1 11:36:29 2023, max compression
```

## Comparing `mypy-boto3-cognito-sync-1.28.15.post1.tar` & `mypy-boto3-cognito-sync-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.821078 mypy-boto3-cognito-sync-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-29 10:02:48.817078 mypy-boto3-cognito-sync-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.809078 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-07-29 09:41:08.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.817078 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-29 10:02:48.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:02:48.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:48.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:48.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:48.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:02:48.000000 mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:48.821078 mypy-boto3-cognito-sync-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-29 09:41:06.000000 mypy-boto3-cognito-sync-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:29.212923 mypy-boto3-cognito-sync-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:38.000000 mypy-boto3-cognito-sync-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-08-01 11:36:29.200923 mypy-boto3-cognito-sync-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-08-01 11:13:38.000000 mypy-boto3-cognito-sync-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:29.200923 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 11:13:38.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 11:13:38.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-01 11:13:38.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-08-01 11:13:39.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-08-01 11:13:39.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-08-01 11:13:39.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-08-01 11:13:39.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:38.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-08-01 11:13:39.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-08-01 11:13:39.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:38.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:29.200923 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-08-01 11:36:28.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 11:36:29.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:28.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:28.000000 mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:29.212923 mypy-boto3-cognito-sync-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:13:38.000000 mypy-boto3-cognito-sync-1.28.16/setup.py
```

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/LICENSE` & `mypy-boto3-cognito-sync-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/PKG-INFO` & `mypy-boto3-cognito-sync-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-sync
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CognitoSync 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CognitoSync 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cognito-sync type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cognito-sync type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-sync)](https://pepy.tech/project/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
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
@@ -291,20 +291,20 @@
 )
 
 
 def check_value(value: BulkPublishStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
@@ -319,15 +319,15 @@
     GetIdentityPoolConfigurationRequestRequestTypeDef,
     PushSyncOutputTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
     PushSyncTypeDef,
-    RecordPatchTypeDef,
+    TimestampTypeDef,
     RegisterDeviceRequestRequestTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
     BulkPublishResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
@@ -339,20 +339,22 @@
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     ListRecordsResponseTypeDef,
     UpdateRecordsResponseTypeDef,
+    PushSyncUnionTypeDef,
     SetIdentityPoolConfigurationRequestRequestTypeDef,
+    RecordPatchTypeDef,
     UpdateRecordsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BulkPublishRequestRequestTypeDef:
+def get_value() -> BulkPublishRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/README.md` & `mypy-boto3-cognito-sync-1.28.16/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-sync)](https://pepy.tech/project/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
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
@@ -259,20 +259,20 @@
 )
 
 
 def check_value(value: BulkPublishStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
@@ -287,15 +287,15 @@
     GetIdentityPoolConfigurationRequestRequestTypeDef,
     PushSyncOutputTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
     PushSyncTypeDef,
-    RecordPatchTypeDef,
+    TimestampTypeDef,
     RegisterDeviceRequestRequestTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
     BulkPublishResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
@@ -307,20 +307,22 @@
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     ListRecordsResponseTypeDef,
     UpdateRecordsResponseTypeDef,
+    PushSyncUnionTypeDef,
     SetIdentityPoolConfigurationRequestRequestTypeDef,
+    RecordPatchTypeDef,
     UpdateRecordsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BulkPublishRequestRequestTypeDef:
+def get_value() -> BulkPublishRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/__main__.py` & `mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoSync 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CognitoSync 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync\nOther"
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

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/client.py` & `mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_cognito_sync.client import CognitoSyncClient
 
     session = Session()
     client: CognitoSyncClient = session.client("cognito-sync")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PlatformType
 from .type_defs import (
     BulkPublishResponseTypeDef,
     CognitoStreamsTypeDef,
@@ -28,16 +28,15 @@
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     ListRecordsResponseTypeDef,
-    PushSyncOutputTypeDef,
-    PushSyncTypeDef,
+    PushSyncUnionTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceResponseTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     UpdateRecordsResponseTypeDef,
 )
 
 __all__ = ("CognitoSyncClient",)
@@ -253,15 +252,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/client/#set_cognito_events)
         """
 
     def set_identity_pool_configuration(
         self,
         *,
         IdentityPoolId: str,
-        PushSync: Union[PushSyncTypeDef, PushSyncOutputTypeDef] = ...,
+        PushSync: PushSyncUnionTypeDef = ...,
         CognitoStreams: CognitoStreamsTypeDef = ...
     ) -> SetIdentityPoolConfigurationResponseTypeDef:
         """
         Sets the necessary configuration for push sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_identity_pool_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/client/#set_identity_pool_configuration)
```

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/client.pyi` & `mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_cognito_sync.client import CognitoSyncClient
 
     session = Session()
     client: CognitoSyncClient = session.client("cognito-sync")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PlatformType
 from .type_defs import (
     BulkPublishResponseTypeDef,
     CognitoStreamsTypeDef,
@@ -28,16 +28,15 @@
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     ListRecordsResponseTypeDef,
-    PushSyncOutputTypeDef,
-    PushSyncTypeDef,
+    PushSyncUnionTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceResponseTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     UpdateRecordsResponseTypeDef,
 )
 
 __all__ = ("CognitoSyncClient",)
@@ -233,15 +232,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_cognito_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/client/#set_cognito_events)
         """
     def set_identity_pool_configuration(
         self,
         *,
         IdentityPoolId: str,
-        PushSync: Union[PushSyncTypeDef, PushSyncOutputTypeDef] = ...,
+        PushSync: PushSyncUnionTypeDef = ...,
         CognitoStreams: CognitoStreamsTypeDef = ...
     ) -> SetIdentityPoolConfigurationResponseTypeDef:
         """
         Sets the necessary configuration for push sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_identity_pool_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/client/#set_identity_pool_configuration)
```

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/literals.py` & `mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/literals.pyi` & `mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/type_defs.py` & `mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cognito_sync.type_defs import BulkPublishRequestRequestTypeDef
 
-    data: BulkPublishRequestRequestTypeDef = {...}
+    data: BulkPublishRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import BulkPublishStatusType, OperationType, PlatformType, StreamingStatusType
@@ -39,15 +39,15 @@
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     "PushSyncOutputTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
     "PushSyncTypeDef",
-    "RecordPatchTypeDef",
+    "TimestampTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
     "BulkPublishResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetBulkPublishDetailsResponseTypeDef",
@@ -59,15 +59,17 @@
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
     "SetIdentityPoolConfigurationResponseTypeDef",
     "ListRecordsResponseTypeDef",
     "UpdateRecordsResponseTypeDef",
+    "PushSyncUnionTypeDef",
     "SetIdentityPoolConfigurationRequestRequestTypeDef",
+    "RecordPatchTypeDef",
     "UpdateRecordsRequestRequestTypeDef",
 )
 
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
@@ -271,36 +273,15 @@
     {
         "ApplicationArns": Sequence[str],
         "RoleArn": str,
     },
     total=False,
 )
 
-_RequiredRecordPatchTypeDef = TypedDict(
-    "_RequiredRecordPatchTypeDef",
-    {
-        "Op": OperationType,
-        "Key": str,
-        "SyncCount": int,
-    },
-)
-_OptionalRecordPatchTypeDef = TypedDict(
-    "_OptionalRecordPatchTypeDef",
-    {
-        "Value": str,
-        "DeviceLastModifiedDate": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class RecordPatchTypeDef(_RequiredRecordPatchTypeDef, _OptionalRecordPatchTypeDef):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 RegisterDeviceRequestRequestTypeDef = TypedDict(
     "RegisterDeviceRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "Platform": PlatformType,
         "Token": str,
@@ -471,14 +452,15 @@
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PushSyncUnionTypeDef = Union[PushSyncTypeDef, PushSyncOutputTypeDef]
 _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
@@ -494,14 +476,36 @@
 class SetIdentityPoolConfigurationRequestRequestTypeDef(
     _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
     _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredRecordPatchTypeDef = TypedDict(
+    "_RequiredRecordPatchTypeDef",
+    {
+        "Op": OperationType,
+        "Key": str,
+        "SyncCount": int,
+    },
+)
+_OptionalRecordPatchTypeDef = TypedDict(
+    "_OptionalRecordPatchTypeDef",
+    {
+        "Value": str,
+        "DeviceLastModifiedDate": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class RecordPatchTypeDef(_RequiredRecordPatchTypeDef, _OptionalRecordPatchTypeDef):
+    pass
+
+
 _RequiredUpdateRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecordsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "SyncSessionToken": str,
```

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync/type_defs.pyi` & `mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cognito_sync.type_defs import BulkPublishRequestRequestTypeDef
 
-    data: BulkPublishRequestRequestTypeDef = {...}
+    data: BulkPublishRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import BulkPublishStatusType, OperationType, PlatformType, StreamingStatusType
@@ -38,15 +38,15 @@
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     "PushSyncOutputTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
     "PushSyncTypeDef",
-    "RecordPatchTypeDef",
+    "TimestampTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
     "BulkPublishResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetBulkPublishDetailsResponseTypeDef",
@@ -58,15 +58,17 @@
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
     "SetIdentityPoolConfigurationResponseTypeDef",
     "ListRecordsResponseTypeDef",
     "UpdateRecordsResponseTypeDef",
+    "PushSyncUnionTypeDef",
     "SetIdentityPoolConfigurationRequestRequestTypeDef",
+    "RecordPatchTypeDef",
     "UpdateRecordsRequestRequestTypeDef",
 )
 
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
@@ -266,34 +268,15 @@
     {
         "ApplicationArns": Sequence[str],
         "RoleArn": str,
     },
     total=False,
 )
 
-_RequiredRecordPatchTypeDef = TypedDict(
-    "_RequiredRecordPatchTypeDef",
-    {
-        "Op": OperationType,
-        "Key": str,
-        "SyncCount": int,
-    },
-)
-_OptionalRecordPatchTypeDef = TypedDict(
-    "_OptionalRecordPatchTypeDef",
-    {
-        "Value": str,
-        "DeviceLastModifiedDate": Union[datetime, str],
-    },
-    total=False,
-)
-
-class RecordPatchTypeDef(_RequiredRecordPatchTypeDef, _OptionalRecordPatchTypeDef):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 RegisterDeviceRequestRequestTypeDef = TypedDict(
     "RegisterDeviceRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "Platform": PlatformType,
         "Token": str,
@@ -464,14 +447,15 @@
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PushSyncUnionTypeDef = Union[PushSyncTypeDef, PushSyncOutputTypeDef]
 _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
@@ -485,14 +469,34 @@
 
 class SetIdentityPoolConfigurationRequestRequestTypeDef(
     _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
     _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredRecordPatchTypeDef = TypedDict(
+    "_RequiredRecordPatchTypeDef",
+    {
+        "Op": OperationType,
+        "Key": str,
+        "SyncCount": int,
+    },
+)
+_OptionalRecordPatchTypeDef = TypedDict(
+    "_OptionalRecordPatchTypeDef",
+    {
+        "Value": str,
+        "DeviceLastModifiedDate": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class RecordPatchTypeDef(_RequiredRecordPatchTypeDef, _OptionalRecordPatchTypeDef):
+    pass
+
 _RequiredUpdateRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecordsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "SyncSessionToken": str,
```

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync.egg-info/PKG-INFO` & `mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-sync
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CognitoSync 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CognitoSync 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cognito-sync type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cognito-sync type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-sync)](https://pepy.tech/project/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
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
@@ -291,20 +291,20 @@
 )
 
 
 def check_value(value: BulkPublishStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
@@ -319,15 +319,15 @@
     GetIdentityPoolConfigurationRequestRequestTypeDef,
     PushSyncOutputTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
     PushSyncTypeDef,
-    RecordPatchTypeDef,
+    TimestampTypeDef,
     RegisterDeviceRequestRequestTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
     BulkPublishResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
@@ -339,20 +339,22 @@
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     ListRecordsResponseTypeDef,
     UpdateRecordsResponseTypeDef,
+    PushSyncUnionTypeDef,
     SetIdentityPoolConfigurationRequestRequestTypeDef,
+    RecordPatchTypeDef,
     UpdateRecordsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BulkPublishRequestRequestTypeDef:
+def get_value() -> BulkPublishRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/mypy_boto3_cognito_sync.egg-info/SOURCES.txt` & `mypy-boto3-cognito-sync-1.28.16/mypy_boto3_cognito_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.15.post1/setup.py` & `mypy-boto3-cognito-sync-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-sync",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_cognito_sync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoSync 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CognitoSync 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 cognito-sync type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 cognito-sync type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_cognito_sync": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

