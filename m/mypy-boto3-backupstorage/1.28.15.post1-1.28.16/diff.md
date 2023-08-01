# Comparing `tmp/mypy-boto3-backupstorage-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-backupstorage-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backupstorage-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:36 2023, max compression
+gzip compressed data, was "mypy-boto3-backupstorage-1.28.16.tar", last modified: Tue Aug  1 11:36:18 2023, max compression
```

## Comparing `mypy-boto3-backupstorage-1.28.15.post1.tar` & `mypy-boto3-backupstorage-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:36.937031 mypy-boto3-backupstorage-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:59.000000 mypy-boto3-backupstorage-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-29 10:02:36.937031 mypy-boto3-backupstorage-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-29 09:38:59.000000 mypy-boto3-backupstorage-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:36.937031 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-29 09:38:59.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-29 09:38:59.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 09:38:59.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-29 09:39:00.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-07-29 09:39:00.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-29 09:39:00.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-29 09:39:00.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:59.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-29 09:39:00.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-29 09:39:00.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:59.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:36.937031 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-29 10:02:36.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-29 10:02:36.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:36.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:36.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:36.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:02:36.000000 mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:36.937031 mypy-boto3-backupstorage-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-29 09:38:59.000000 mypy-boto3-backupstorage-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.468940 mypy-boto3-backupstorage-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:32.000000 mypy-boto3-backupstorage-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-08-01 11:36:18.468940 mypy-boto3-backupstorage-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-08-01 11:11:32.000000 mypy-boto3-backupstorage-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.456940 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-01 11:11:32.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 11:11:32.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 11:11:32.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-08-01 11:11:33.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-08-01 11:11:33.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-08-01 11:11:33.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-08-01 11:11:33.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:32.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-08-01 11:11:33.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-08-01 11:11:33.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:32.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.468940 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-08-01 11:36:18.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 11:36:18.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:18.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:36:18.000000 mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:18.468940 mypy-boto3-backupstorage-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 11:11:32.000000 mypy-boto3-backupstorage-1.28.16/setup.py
```

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/LICENSE` & `mypy-boto3-backupstorage-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/PKG-INFO` & `mypy-boto3-backupstorage-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backupstorage
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.BackupStorage 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.BackupStorage 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 backupstorage type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 backupstorage type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backupstorage)](https://pepy.tech/project/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
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
@@ -289,48 +289,50 @@
 )
 
 
 def check_value(value: DataChecksumAlgorithmType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_backupstorage.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_backupstorage.type_defs import (
     BackupObjectTypeDef,
+    BlobTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
     ResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
     GetObjectMetadataInputRequestTypeDef,
     ListChunksInputRequestTypeDef,
-    ListObjectsInputRequestTypeDef,
+    TimestampTypeDef,
+    StartObjectInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
     PutChunkInputRequestTypeDef,
     PutObjectInputRequestTypeDef,
-    StartObjectInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChunkOutputTypeDef,
     GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
     ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
     PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
     StartObjectOutputTypeDef,
+    ListObjectsInputRequestTypeDef,
 )
 
 
-def get_structure() -> BackupObjectTypeDef:
+def get_value() -> BackupObjectTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/README.md` & `mypy-boto3-backupstorage-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backupstorage)](https://pepy.tech/project/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
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
@@ -257,48 +257,50 @@
 )
 
 
 def check_value(value: DataChecksumAlgorithmType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_backupstorage.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_backupstorage.type_defs import (
     BackupObjectTypeDef,
+    BlobTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
     ResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
     GetObjectMetadataInputRequestTypeDef,
     ListChunksInputRequestTypeDef,
-    ListObjectsInputRequestTypeDef,
+    TimestampTypeDef,
+    StartObjectInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
     PutChunkInputRequestTypeDef,
     PutObjectInputRequestTypeDef,
-    StartObjectInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChunkOutputTypeDef,
     GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
     ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
     PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
     StartObjectOutputTypeDef,
+    ListObjectsInputRequestTypeDef,
 )
 
 
-def get_structure() -> BackupObjectTypeDef:
+def get_value() -> BackupObjectTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/__main__.py` & `mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BackupStorage 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.BackupStorage 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage\nOther"
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

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/client.py` & `mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     from mypy_boto3_backupstorage.client import BackupStorageClient
 
     session = Session()
     client: BackupStorageClient = session.client("backupstorage")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .type_defs import (
+    BlobTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChunkOutputTypeDef,
     GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
     ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
     PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
     StartObjectOutputTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -151,16 +151,16 @@
         self,
         *,
         StorageJobId: str,
         StartingObjectName: str = ...,
         StartingObjectPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        CreatedBefore: Union[datetime, str] = ...,
-        CreatedAfter: Union[datetime, str] = ...
+        CreatedBefore: TimestampTypeDef = ...,
+        CreatedAfter: TimestampTypeDef = ...
     ) -> ListObjectsOutputTypeDef:
         """
         List all Objects in a given Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.list_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/client/#list_objects)
         """
@@ -169,15 +169,15 @@
         self,
         *,
         BackupJobId: str,
         UploadId: str,
         ObjectChecksum: str,
         ObjectChecksumAlgorithm: Literal["SUMMARY"],
         MetadataString: str = ...,
-        MetadataBlob: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        MetadataBlob: BlobTypeDef = ...,
         MetadataBlobLength: int = ...,
         MetadataBlobChecksum: str = ...,
         MetadataBlobChecksumAlgorithm: Literal["SHA256"] = ...
     ) -> NotifyObjectCompleteOutputTypeDef:
         """
         Complete upload See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backupstorage-2018-04-10/NotifyObjectComplete).
@@ -188,15 +188,15 @@
 
     def put_chunk(
         self,
         *,
         BackupJobId: str,
         UploadId: str,
         ChunkIndex: int,
-        Data: Union[str, bytes, IO[Any], StreamingBody],
+        Data: BlobTypeDef,
         Length: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"]
     ) -> PutChunkOutputTypeDef:
         """
         Upload chunk.
 
@@ -206,15 +206,15 @@
 
     def put_object(
         self,
         *,
         BackupJobId: str,
         ObjectName: str,
         MetadataString: str = ...,
-        InlineChunk: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        InlineChunk: BlobTypeDef = ...,
         InlineChunkLength: int = ...,
         InlineChunkChecksum: str = ...,
         InlineChunkChecksumAlgorithm: str = ...,
         ObjectChecksum: str = ...,
         ObjectChecksumAlgorithm: Literal["SUMMARY"] = ...,
         ThrowOnDuplicate: bool = ...
     ) -> PutObjectOutputTypeDef:
```

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/client.pyi` & `mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     from mypy_boto3_backupstorage.client import BackupStorageClient
 
     session = Session()
     client: BackupStorageClient = session.client("backupstorage")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .type_defs import (
+    BlobTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChunkOutputTypeDef,
     GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
     ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
     PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
     StartObjectOutputTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -139,16 +139,16 @@
         self,
         *,
         StorageJobId: str,
         StartingObjectName: str = ...,
         StartingObjectPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        CreatedBefore: Union[datetime, str] = ...,
-        CreatedAfter: Union[datetime, str] = ...
+        CreatedBefore: TimestampTypeDef = ...,
+        CreatedAfter: TimestampTypeDef = ...
     ) -> ListObjectsOutputTypeDef:
         """
         List all Objects in a given Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.list_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/client/#list_objects)
         """
@@ -156,15 +156,15 @@
         self,
         *,
         BackupJobId: str,
         UploadId: str,
         ObjectChecksum: str,
         ObjectChecksumAlgorithm: Literal["SUMMARY"],
         MetadataString: str = ...,
-        MetadataBlob: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        MetadataBlob: BlobTypeDef = ...,
         MetadataBlobLength: int = ...,
         MetadataBlobChecksum: str = ...,
         MetadataBlobChecksumAlgorithm: Literal["SHA256"] = ...
     ) -> NotifyObjectCompleteOutputTypeDef:
         """
         Complete upload See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backupstorage-2018-04-10/NotifyObjectComplete).
@@ -174,15 +174,15 @@
         """
     def put_chunk(
         self,
         *,
         BackupJobId: str,
         UploadId: str,
         ChunkIndex: int,
-        Data: Union[str, bytes, IO[Any], StreamingBody],
+        Data: BlobTypeDef,
         Length: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"]
     ) -> PutChunkOutputTypeDef:
         """
         Upload chunk.
 
@@ -191,15 +191,15 @@
         """
     def put_object(
         self,
         *,
         BackupJobId: str,
         ObjectName: str,
         MetadataString: str = ...,
-        InlineChunk: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        InlineChunk: BlobTypeDef = ...,
         InlineChunkLength: int = ...,
         InlineChunkChecksum: str = ...,
         InlineChunkChecksumAlgorithm: str = ...,
         ObjectChecksum: str = ...,
         ObjectChecksumAlgorithm: Literal["SUMMARY"] = ...,
         ThrowOnDuplicate: bool = ...
     ) -> PutObjectOutputTypeDef:
```

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/literals.py` & `mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/literals.pyi` & `mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/type_defs.py` & `mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_backupstorage.type_defs import BackupObjectTypeDef
 
-    data: BackupObjectTypeDef = {...}
+    data: BackupObjectTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
@@ -25,34 +25,36 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BackupObjectTypeDef",
+    "BlobTypeDef",
     "ChunkTypeDef",
     "DeleteObjectInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetChunkInputRequestTypeDef",
     "GetObjectMetadataInputRequestTypeDef",
     "ListChunksInputRequestTypeDef",
-    "ListObjectsInputRequestTypeDef",
+    "TimestampTypeDef",
+    "StartObjectInputRequestTypeDef",
     "NotifyObjectCompleteInputRequestTypeDef",
     "PutChunkInputRequestTypeDef",
     "PutObjectInputRequestTypeDef",
-    "StartObjectInputRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChunkOutputTypeDef",
     "GetObjectMetadataOutputTypeDef",
     "ListChunksOutputTypeDef",
     "ListObjectsOutputTypeDef",
     "NotifyObjectCompleteOutputTypeDef",
     "PutChunkOutputTypeDef",
     "PutObjectOutputTypeDef",
     "StartObjectOutputTypeDef",
+    "ListObjectsInputRequestTypeDef",
 )
 
 _RequiredBackupObjectTypeDef = TypedDict(
     "_RequiredBackupObjectTypeDef",
     {
         "Name": str,
         "ObjectChecksum": str,
@@ -70,14 +72,15 @@
 )
 
 
 class BackupObjectTypeDef(_RequiredBackupObjectTypeDef, _OptionalBackupObjectTypeDef):
     pass
 
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChunkTypeDef = TypedDict(
     "ChunkTypeDef",
     {
         "Index": int,
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
@@ -139,36 +142,33 @@
 
 class ListChunksInputRequestTypeDef(
     _RequiredListChunksInputRequestTypeDef, _OptionalListChunksInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListObjectsInputRequestTypeDef = TypedDict(
-    "_RequiredListObjectsInputRequestTypeDef",
+TimestampTypeDef = Union[datetime, str]
+_RequiredStartObjectInputRequestTypeDef = TypedDict(
+    "_RequiredStartObjectInputRequestTypeDef",
     {
-        "StorageJobId": str,
+        "BackupJobId": str,
+        "ObjectName": str,
     },
 )
-_OptionalListObjectsInputRequestTypeDef = TypedDict(
-    "_OptionalListObjectsInputRequestTypeDef",
+_OptionalStartObjectInputRequestTypeDef = TypedDict(
+    "_OptionalStartObjectInputRequestTypeDef",
     {
-        "StartingObjectName": str,
-        "StartingObjectPrefix": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
+        "ThrowOnDuplicate": bool,
     },
     total=False,
 )
 
 
-class ListObjectsInputRequestTypeDef(
-    _RequiredListObjectsInputRequestTypeDef, _OptionalListObjectsInputRequestTypeDef
+class StartObjectInputRequestTypeDef(
+    _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
 ):
     pass
 
 
 _RequiredNotifyObjectCompleteInputRequestTypeDef = TypedDict(
     "_RequiredNotifyObjectCompleteInputRequestTypeDef",
     {
@@ -178,15 +178,15 @@
         "ObjectChecksumAlgorithm": Literal["SUMMARY"],
     },
 )
 _OptionalNotifyObjectCompleteInputRequestTypeDef = TypedDict(
     "_OptionalNotifyObjectCompleteInputRequestTypeDef",
     {
         "MetadataString": str,
-        "MetadataBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "MetadataBlob": BlobTypeDef,
         "MetadataBlobLength": int,
         "MetadataBlobChecksum": str,
         "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
     },
     total=False,
 )
 
@@ -200,15 +200,15 @@
 
 PutChunkInputRequestTypeDef = TypedDict(
     "PutChunkInputRequestTypeDef",
     {
         "BackupJobId": str,
         "UploadId": str,
         "ChunkIndex": int,
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Data": BlobTypeDef,
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 
 _RequiredPutObjectInputRequestTypeDef = TypedDict(
@@ -218,15 +218,15 @@
         "ObjectName": str,
     },
 )
 _OptionalPutObjectInputRequestTypeDef = TypedDict(
     "_OptionalPutObjectInputRequestTypeDef",
     {
         "MetadataString": str,
-        "InlineChunk": Union[str, bytes, IO[Any], StreamingBody],
+        "InlineChunk": BlobTypeDef,
         "InlineChunkLength": int,
         "InlineChunkChecksum": str,
         "InlineChunkChecksumAlgorithm": str,
         "ObjectChecksum": str,
         "ObjectChecksumAlgorithm": Literal["SUMMARY"],
         "ThrowOnDuplicate": bool,
     },
@@ -236,36 +236,14 @@
 
 class PutObjectInputRequestTypeDef(
     _RequiredPutObjectInputRequestTypeDef, _OptionalPutObjectInputRequestTypeDef
 ):
     pass
 
 
-_RequiredStartObjectInputRequestTypeDef = TypedDict(
-    "_RequiredStartObjectInputRequestTypeDef",
-    {
-        "BackupJobId": str,
-        "ObjectName": str,
-    },
-)
-_OptionalStartObjectInputRequestTypeDef = TypedDict(
-    "_OptionalStartObjectInputRequestTypeDef",
-    {
-        "ThrowOnDuplicate": bool,
-    },
-    total=False,
-)
-
-
-class StartObjectInputRequestTypeDef(
-    _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
-):
-    pass
-
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -342,7 +320,32 @@
 StartObjectOutputTypeDef = TypedDict(
     "StartObjectOutputTypeDef",
     {
         "UploadId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredListObjectsInputRequestTypeDef = TypedDict(
+    "_RequiredListObjectsInputRequestTypeDef",
+    {
+        "StorageJobId": str,
+    },
+)
+_OptionalListObjectsInputRequestTypeDef = TypedDict(
+    "_OptionalListObjectsInputRequestTypeDef",
+    {
+        "StartingObjectName": str,
+        "StartingObjectPrefix": str,
+        "MaxResults": int,
+        "NextToken": str,
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class ListObjectsInputRequestTypeDef(
+    _RequiredListObjectsInputRequestTypeDef, _OptionalListObjectsInputRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage/type_defs.pyi` & `mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_backupstorage.type_defs import BackupObjectTypeDef
 
-    data: BackupObjectTypeDef = {...}
+    data: BackupObjectTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
@@ -24,34 +24,36 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BackupObjectTypeDef",
+    "BlobTypeDef",
     "ChunkTypeDef",
     "DeleteObjectInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetChunkInputRequestTypeDef",
     "GetObjectMetadataInputRequestTypeDef",
     "ListChunksInputRequestTypeDef",
-    "ListObjectsInputRequestTypeDef",
+    "TimestampTypeDef",
+    "StartObjectInputRequestTypeDef",
     "NotifyObjectCompleteInputRequestTypeDef",
     "PutChunkInputRequestTypeDef",
     "PutObjectInputRequestTypeDef",
-    "StartObjectInputRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChunkOutputTypeDef",
     "GetObjectMetadataOutputTypeDef",
     "ListChunksOutputTypeDef",
     "ListObjectsOutputTypeDef",
     "NotifyObjectCompleteOutputTypeDef",
     "PutChunkOutputTypeDef",
     "PutObjectOutputTypeDef",
     "StartObjectOutputTypeDef",
+    "ListObjectsInputRequestTypeDef",
 )
 
 _RequiredBackupObjectTypeDef = TypedDict(
     "_RequiredBackupObjectTypeDef",
     {
         "Name": str,
         "ObjectChecksum": str,
@@ -67,14 +69,15 @@
     },
     total=False,
 )
 
 class BackupObjectTypeDef(_RequiredBackupObjectTypeDef, _OptionalBackupObjectTypeDef):
     pass
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChunkTypeDef = TypedDict(
     "ChunkTypeDef",
     {
         "Index": int,
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
@@ -134,35 +137,32 @@
 )
 
 class ListChunksInputRequestTypeDef(
     _RequiredListChunksInputRequestTypeDef, _OptionalListChunksInputRequestTypeDef
 ):
     pass
 
-_RequiredListObjectsInputRequestTypeDef = TypedDict(
-    "_RequiredListObjectsInputRequestTypeDef",
+TimestampTypeDef = Union[datetime, str]
+_RequiredStartObjectInputRequestTypeDef = TypedDict(
+    "_RequiredStartObjectInputRequestTypeDef",
     {
-        "StorageJobId": str,
+        "BackupJobId": str,
+        "ObjectName": str,
     },
 )
-_OptionalListObjectsInputRequestTypeDef = TypedDict(
-    "_OptionalListObjectsInputRequestTypeDef",
+_OptionalStartObjectInputRequestTypeDef = TypedDict(
+    "_OptionalStartObjectInputRequestTypeDef",
     {
-        "StartingObjectName": str,
-        "StartingObjectPrefix": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
+        "ThrowOnDuplicate": bool,
     },
     total=False,
 )
 
-class ListObjectsInputRequestTypeDef(
-    _RequiredListObjectsInputRequestTypeDef, _OptionalListObjectsInputRequestTypeDef
+class StartObjectInputRequestTypeDef(
+    _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
 ):
     pass
 
 _RequiredNotifyObjectCompleteInputRequestTypeDef = TypedDict(
     "_RequiredNotifyObjectCompleteInputRequestTypeDef",
     {
         "BackupJobId": str,
@@ -171,15 +171,15 @@
         "ObjectChecksumAlgorithm": Literal["SUMMARY"],
     },
 )
 _OptionalNotifyObjectCompleteInputRequestTypeDef = TypedDict(
     "_OptionalNotifyObjectCompleteInputRequestTypeDef",
     {
         "MetadataString": str,
-        "MetadataBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "MetadataBlob": BlobTypeDef,
         "MetadataBlobLength": int,
         "MetadataBlobChecksum": str,
         "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
     },
     total=False,
 )
 
@@ -191,15 +191,15 @@
 
 PutChunkInputRequestTypeDef = TypedDict(
     "PutChunkInputRequestTypeDef",
     {
         "BackupJobId": str,
         "UploadId": str,
         "ChunkIndex": int,
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Data": BlobTypeDef,
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 
 _RequiredPutObjectInputRequestTypeDef = TypedDict(
@@ -209,15 +209,15 @@
         "ObjectName": str,
     },
 )
 _OptionalPutObjectInputRequestTypeDef = TypedDict(
     "_OptionalPutObjectInputRequestTypeDef",
     {
         "MetadataString": str,
-        "InlineChunk": Union[str, bytes, IO[Any], StreamingBody],
+        "InlineChunk": BlobTypeDef,
         "InlineChunkLength": int,
         "InlineChunkChecksum": str,
         "InlineChunkChecksumAlgorithm": str,
         "ObjectChecksum": str,
         "ObjectChecksumAlgorithm": Literal["SUMMARY"],
         "ThrowOnDuplicate": bool,
     },
@@ -225,34 +225,14 @@
 )
 
 class PutObjectInputRequestTypeDef(
     _RequiredPutObjectInputRequestTypeDef, _OptionalPutObjectInputRequestTypeDef
 ):
     pass
 
-_RequiredStartObjectInputRequestTypeDef = TypedDict(
-    "_RequiredStartObjectInputRequestTypeDef",
-    {
-        "BackupJobId": str,
-        "ObjectName": str,
-    },
-)
-_OptionalStartObjectInputRequestTypeDef = TypedDict(
-    "_OptionalStartObjectInputRequestTypeDef",
-    {
-        "ThrowOnDuplicate": bool,
-    },
-    total=False,
-)
-
-class StartObjectInputRequestTypeDef(
-    _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
-):
-    pass
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -329,7 +309,31 @@
 StartObjectOutputTypeDef = TypedDict(
     "StartObjectOutputTypeDef",
     {
         "UploadId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredListObjectsInputRequestTypeDef = TypedDict(
+    "_RequiredListObjectsInputRequestTypeDef",
+    {
+        "StorageJobId": str,
+    },
+)
+_OptionalListObjectsInputRequestTypeDef = TypedDict(
+    "_OptionalListObjectsInputRequestTypeDef",
+    {
+        "StartingObjectName": str,
+        "StartingObjectPrefix": str,
+        "MaxResults": int,
+        "NextToken": str,
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectsInputRequestTypeDef(
+    _RequiredListObjectsInputRequestTypeDef, _OptionalListObjectsInputRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage.egg-info/PKG-INFO` & `mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backupstorage
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.BackupStorage 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.BackupStorage 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 backupstorage type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 backupstorage type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backupstorage)](https://pepy.tech/project/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
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
@@ -289,48 +289,50 @@
 )
 
 
 def check_value(value: DataChecksumAlgorithmType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_backupstorage.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_backupstorage.type_defs import (
     BackupObjectTypeDef,
+    BlobTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
     ResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
     GetObjectMetadataInputRequestTypeDef,
     ListChunksInputRequestTypeDef,
-    ListObjectsInputRequestTypeDef,
+    TimestampTypeDef,
+    StartObjectInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
     PutChunkInputRequestTypeDef,
     PutObjectInputRequestTypeDef,
-    StartObjectInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChunkOutputTypeDef,
     GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
     ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
     PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
     StartObjectOutputTypeDef,
+    ListObjectsInputRequestTypeDef,
 )
 
 
-def get_structure() -> BackupObjectTypeDef:
+def get_value() -> BackupObjectTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/mypy_boto3_backupstorage.egg-info/SOURCES.txt` & `mypy-boto3-backupstorage-1.28.16/mypy_boto3_backupstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.15.post1/setup.py` & `mypy-boto3-backupstorage-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backupstorage",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_backupstorage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BackupStorage 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.BackupStorage 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 backupstorage type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 backupstorage type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_backupstorage": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

