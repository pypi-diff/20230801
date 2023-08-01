# Comparing `tmp/mypy-boto3-ebs-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ebs-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ebs-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:00 2023, max compression
+gzip compressed data, was "mypy-boto3-ebs-1.28.16.tar", last modified: Tue Aug  1 11:36:41 2023, max compression
```

## Comparing `mypy-boto3-ebs-1.28.15.post1.tar` & `mypy-boto3-ebs-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:00.953121 mypy-boto3-ebs-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-07-29 10:03:00.953121 mypy-boto3-ebs-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:00.953121 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:43:05.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:00.953121 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-07-29 10:03:00.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-29 10:03:00.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:00.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:00.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:00.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:00.000000 mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:00.953121 mypy-boto3-ebs-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:43:04.000000 mypy-boto3-ebs-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:41.848902 mypy-boto3-ebs-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-08-01 11:36:41.848902 mypy-boto3-ebs-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:41.848902 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-08-01 11:15:38.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:41.848902 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-08-01 11:36:41.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 11:36:41.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:41.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:41.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:41.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:41.000000 mypy-boto3-ebs-1.28.16/mypy_boto3_ebs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:41.848902 mypy-boto3-ebs-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:15:37.000000 mypy-boto3-ebs-1.28.16/setup.py
```

### Comparing `mypy-boto3-ebs-1.28.15.post1/LICENSE` & `mypy-boto3-ebs-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.15.post1/PKG-INFO` & `mypy-boto3-ebs-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ebs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EBS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EBS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ebs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ebs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ebs)](https://pepy.tech/project/mypy-boto3-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EBS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[boto3.EBS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [mypy-boto3-ebs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/).
 
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
@@ -290,43 +290,44 @@
 )
 
 
 def check_value(value: ChecksumAggregationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ebs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ebs.type_defs import (
+    BlobTypeDef,
     BlockTypeDef,
     ChangedBlockTypeDef,
     CompleteSnapshotRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetSnapshotBlockRequestRequestTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
-    PutSnapshotBlockRequestRequestTypeDef,
     TagTypeDef,
+    PutSnapshotBlockRequestRequestTypeDef,
     CompleteSnapshotResponseTypeDef,
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     PutSnapshotBlockResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
 
 
-def get_structure() -> BlockTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ebs-1.28.15.post1/README.md` & `mypy-boto3-ebs-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ebs)](https://pepy.tech/project/mypy-boto3-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EBS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[boto3.EBS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [mypy-boto3-ebs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/).
 
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
@@ -258,43 +258,44 @@
 )
 
 
 def check_value(value: ChecksumAggregationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ebs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ebs.type_defs import (
+    BlobTypeDef,
     BlockTypeDef,
     ChangedBlockTypeDef,
     CompleteSnapshotRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetSnapshotBlockRequestRequestTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
-    PutSnapshotBlockRequestRequestTypeDef,
     TagTypeDef,
+    PutSnapshotBlockRequestRequestTypeDef,
     CompleteSnapshotResponseTypeDef,
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     PutSnapshotBlockResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
 
 
-def get_structure() -> BlockTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/__main__.py` & `mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EBS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.EBS 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS\nOther"
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

### Comparing `mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/client.py` & `mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
     from mypy_boto3_ebs.client import EBSClient
 
     session = Session()
     client: EBSClient = session.client("ebs")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .type_defs import (
+    BlobTypeDef,
     CompleteSnapshotResponseTypeDef,
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     PutSnapshotBlockResponseTypeDef,
     StartSnapshotResponseTypeDef,
     TagTypeDef,
@@ -165,15 +165,15 @@
         """
 
     def put_snapshot_block(
         self,
         *,
         SnapshotId: str,
         BlockIndex: int,
-        BlockData: Union[str, bytes, IO[Any], StreamingBody],
+        BlockData: BlobTypeDef,
         DataLength: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"],
         Progress: int = ...
     ) -> PutSnapshotBlockResponseTypeDef:
         """
         Writes a block of data to a snapshot.
```

### Comparing `mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/client.pyi` & `mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
     from mypy_boto3_ebs.client import EBSClient
 
     session = Session()
     client: EBSClient = session.client("ebs")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .type_defs import (
+    BlobTypeDef,
     CompleteSnapshotResponseTypeDef,
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     PutSnapshotBlockResponseTypeDef,
     StartSnapshotResponseTypeDef,
     TagTypeDef,
@@ -153,15 +153,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/client/#list_snapshot_blocks)
         """
     def put_snapshot_block(
         self,
         *,
         SnapshotId: str,
         BlockIndex: int,
-        BlockData: Union[str, bytes, IO[Any], StreamingBody],
+        BlockData: BlobTypeDef,
         DataLength: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"],
         Progress: int = ...
     ) -> PutSnapshotBlockResponseTypeDef:
         """
         Writes a block of data to a snapshot.
```

### Comparing `mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/literals.py` & `mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/literals.pyi` & `mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/type_defs.py` & `mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ebs service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ebs.type_defs import BlockTypeDef
+    from mypy_boto3_ebs.type_defs import BlobTypeDef
 
-    data: BlockTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -26,32 +26,34 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "BlockTypeDef",
     "ChangedBlockTypeDef",
     "CompleteSnapshotRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetSnapshotBlockRequestRequestTypeDef",
     "ListChangedBlocksRequestRequestTypeDef",
     "ListSnapshotBlocksRequestRequestTypeDef",
-    "PutSnapshotBlockRequestRequestTypeDef",
     "TagTypeDef",
+    "PutSnapshotBlockRequestRequestTypeDef",
     "CompleteSnapshotResponseTypeDef",
     "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksResponseTypeDef",
     "ListSnapshotBlocksResponseTypeDef",
     "PutSnapshotBlockResponseTypeDef",
     "StartSnapshotRequestRequestTypeDef",
     "StartSnapshotResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "BlockIndex": int,
         "BlockToken": str,
     },
     total=False,
@@ -155,20 +157,29 @@
 class ListSnapshotBlocksRequestRequestTypeDef(
     _RequiredListSnapshotBlocksRequestRequestTypeDef,
     _OptionalListSnapshotBlocksRequestRequestTypeDef,
 ):
     pass
 
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 _RequiredPutSnapshotBlockRequestRequestTypeDef = TypedDict(
     "_RequiredPutSnapshotBlockRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "BlockIndex": int,
-        "BlockData": Union[str, bytes, IO[Any], StreamingBody],
+        "BlockData": BlobTypeDef,
         "DataLength": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 _OptionalPutSnapshotBlockRequestRequestTypeDef = TypedDict(
     "_OptionalPutSnapshotBlockRequestRequestTypeDef",
@@ -181,23 +192,14 @@
 
 class PutSnapshotBlockRequestRequestTypeDef(
     _RequiredPutSnapshotBlockRequestRequestTypeDef, _OptionalPutSnapshotBlockRequestRequestTypeDef
 ):
     pass
 
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 CompleteSnapshotResponseTypeDef = TypedDict(
     "CompleteSnapshotResponseTypeDef",
     {
         "Status": StatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs/type_defs.pyi` & `mypy-boto3-ebs-1.28.16/mypy_boto3_ebs/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ebs service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ebs.type_defs import BlockTypeDef
+    from mypy_boto3_ebs.type_defs import BlobTypeDef
 
-    data: BlockTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -25,32 +25,34 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "BlockTypeDef",
     "ChangedBlockTypeDef",
     "CompleteSnapshotRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetSnapshotBlockRequestRequestTypeDef",
     "ListChangedBlocksRequestRequestTypeDef",
     "ListSnapshotBlocksRequestRequestTypeDef",
-    "PutSnapshotBlockRequestRequestTypeDef",
     "TagTypeDef",
+    "PutSnapshotBlockRequestRequestTypeDef",
     "CompleteSnapshotResponseTypeDef",
     "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksResponseTypeDef",
     "ListSnapshotBlocksResponseTypeDef",
     "PutSnapshotBlockResponseTypeDef",
     "StartSnapshotRequestRequestTypeDef",
     "StartSnapshotResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "BlockIndex": int,
         "BlockToken": str,
     },
     total=False,
@@ -148,20 +150,29 @@
 
 class ListSnapshotBlocksRequestRequestTypeDef(
     _RequiredListSnapshotBlocksRequestRequestTypeDef,
     _OptionalListSnapshotBlocksRequestRequestTypeDef,
 ):
     pass
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 _RequiredPutSnapshotBlockRequestRequestTypeDef = TypedDict(
     "_RequiredPutSnapshotBlockRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "BlockIndex": int,
-        "BlockData": Union[str, bytes, IO[Any], StreamingBody],
+        "BlockData": BlobTypeDef,
         "DataLength": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 _OptionalPutSnapshotBlockRequestRequestTypeDef = TypedDict(
     "_OptionalPutSnapshotBlockRequestRequestTypeDef",
@@ -172,23 +183,14 @@
 )
 
 class PutSnapshotBlockRequestRequestTypeDef(
     _RequiredPutSnapshotBlockRequestRequestTypeDef, _OptionalPutSnapshotBlockRequestRequestTypeDef
 ):
     pass
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 CompleteSnapshotResponseTypeDef = TypedDict(
     "CompleteSnapshotResponseTypeDef",
     {
         "Status": StatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs.egg-info/PKG-INFO` & `mypy-boto3-ebs-1.28.16/mypy_boto3_ebs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ebs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EBS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EBS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ebs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ebs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ebs)](https://pepy.tech/project/mypy-boto3-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EBS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[boto3.EBS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [mypy-boto3-ebs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/).
 
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
@@ -290,43 +290,44 @@
 )
 
 
 def check_value(value: ChecksumAggregationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ebs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ebs.type_defs import (
+    BlobTypeDef,
     BlockTypeDef,
     ChangedBlockTypeDef,
     CompleteSnapshotRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetSnapshotBlockRequestRequestTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
-    PutSnapshotBlockRequestRequestTypeDef,
     TagTypeDef,
+    PutSnapshotBlockRequestRequestTypeDef,
     CompleteSnapshotResponseTypeDef,
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     PutSnapshotBlockResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
 
 
-def get_structure() -> BlockTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ebs-1.28.15.post1/mypy_boto3_ebs.egg-info/SOURCES.txt` & `mypy-boto3-ebs-1.28.16/mypy_boto3_ebs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.15.post1/setup.py` & `mypy-boto3-ebs-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ebs",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ebs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EBS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.EBS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -33,15 +33,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 ebs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ebs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ebs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

