# Comparing `tmp/mypy-boto3-qldb-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-qldb-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qldb-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:55 2023, max compression
+gzip compressed data, was "mypy-boto3-qldb-1.28.16.tar", last modified: Tue Aug  1 11:37:35 2023, max compression
```

## Comparing `mypy-boto3-qldb-1.28.15.post1.tar` & `mypy-boto3-qldb-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.761347 mypy-boto3-qldb-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-07-29 10:03:55.753347 mypy-boto3-qldb-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.737347 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-29 09:53:41.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.753347 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:55.761347 mypy-boto3-qldb-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:35.728783 mypy-boto3-qldb-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-08-01 11:37:35.724783 mypy-boto3-qldb-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:35.712783 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-08-01 11:26:44.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-08-01 11:26:44.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:35.724783 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-08-01 11:37:35.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 11:37:35.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:35.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:35.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:35.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 11:37:35.000000 mypy-boto3-qldb-1.28.16/mypy_boto3_qldb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:35.728783 mypy-boto3-qldb-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-01 11:26:43.000000 mypy-boto3-qldb-1.28.16/setup.py
```

### Comparing `mypy-boto3-qldb-1.28.15.post1/LICENSE` & `mypy-boto3-qldb-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15.post1/PKG-INFO` & `mypy-boto3-qldb-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.QLDB 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 qldb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 qldb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb)](https://pepy.tech/project/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
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
@@ -294,31 +294,32 @@
 )
 
 
 def check_value(value: EncryptionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_qldb.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateLedgerRequestRequestTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
+    TimestampTypeDef,
     ValueHolderTypeDef,
     GetDigestRequestRequestTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
@@ -353,15 +354,15 @@
     JournalS3ExportDescriptionTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
+def get_value() -> CancelJournalKinesisStreamRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-qldb-1.28.15.post1/README.md` & `mypy-boto3-qldb-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb)](https://pepy.tech/project/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
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
@@ -262,31 +262,32 @@
 )
 
 
 def check_value(value: EncryptionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_qldb.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateLedgerRequestRequestTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
+    TimestampTypeDef,
     ValueHolderTypeDef,
     GetDigestRequestRequestTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
@@ -321,15 +322,15 @@
     JournalS3ExportDescriptionTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
+def get_value() -> CancelJournalKinesisStreamRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/__main__.py` & `mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QLDB 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.QLDB 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB\nOther"
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

### Comparing `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/client.py` & `mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_qldb.client import QLDBClient
 
     session = Session()
     client: QLDBClient = session.client("qldb")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OutputFormatType, PermissionsModeType
 from .type_defs import (
     CancelJournalKinesisStreamResponseTypeDef,
     CreateLedgerResponseTypeDef,
@@ -34,14 +33,15 @@
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
     ListLedgersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3ExportConfigurationTypeDef,
     StreamJournalToKinesisResponseTypeDef,
+    TimestampTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     ValueHolderTypeDef,
 )
 
 __all__ = ("QLDBClient",)
 
@@ -162,16 +162,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#describe_ledger)
         """
 
     def export_journal_to_s3(
         self,
         *,
         Name: str,
-        InclusiveStartTime: Union[datetime, str],
-        ExclusiveEndTime: Union[datetime, str],
+        InclusiveStartTime: TimestampTypeDef,
+        ExclusiveEndTime: TimestampTypeDef,
         S3ExportConfiguration: S3ExportConfigurationTypeDef,
         RoleArn: str,
         OutputFormat: OutputFormatType = ...
     ) -> ExportJournalToS3ResponseTypeDef:
         """
         Exports journal contents within a date and time range from a ledger into a
         specified Amazon Simple Storage Service (Amazon S3) bucket.
@@ -282,19 +282,19 @@
         """
 
     def stream_journal_to_kinesis(
         self,
         *,
         LedgerName: str,
         RoleArn: str,
-        InclusiveStartTime: Union[datetime, str],
+        InclusiveStartTime: TimestampTypeDef,
         KinesisConfiguration: KinesisConfigurationTypeDef,
         StreamName: str,
         Tags: Mapping[str, str] = ...,
-        ExclusiveEndTime: Union[datetime, str] = ...
+        ExclusiveEndTime: TimestampTypeDef = ...
     ) -> StreamJournalToKinesisResponseTypeDef:
         """
         Creates a journal stream for a given Amazon QLDB ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.stream_journal_to_kinesis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#stream_journal_to_kinesis)
         """
```

### Comparing `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/client.pyi` & `mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_qldb.client import QLDBClient
 
     session = Session()
     client: QLDBClient = session.client("qldb")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OutputFormatType, PermissionsModeType
 from .type_defs import (
     CancelJournalKinesisStreamResponseTypeDef,
     CreateLedgerResponseTypeDef,
@@ -34,14 +33,15 @@
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
     ListLedgersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3ExportConfigurationTypeDef,
     StreamJournalToKinesisResponseTypeDef,
+    TimestampTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     ValueHolderTypeDef,
 )
 
 __all__ = ("QLDBClient",)
 
@@ -150,16 +150,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.describe_ledger)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#describe_ledger)
         """
     def export_journal_to_s3(
         self,
         *,
         Name: str,
-        InclusiveStartTime: Union[datetime, str],
-        ExclusiveEndTime: Union[datetime, str],
+        InclusiveStartTime: TimestampTypeDef,
+        ExclusiveEndTime: TimestampTypeDef,
         S3ExportConfiguration: S3ExportConfigurationTypeDef,
         RoleArn: str,
         OutputFormat: OutputFormatType = ...
     ) -> ExportJournalToS3ResponseTypeDef:
         """
         Exports journal contents within a date and time range from a ledger into a
         specified Amazon Simple Storage Service (Amazon S3) bucket.
@@ -260,19 +260,19 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#list_tags_for_resource)
         """
     def stream_journal_to_kinesis(
         self,
         *,
         LedgerName: str,
         RoleArn: str,
-        InclusiveStartTime: Union[datetime, str],
+        InclusiveStartTime: TimestampTypeDef,
         KinesisConfiguration: KinesisConfigurationTypeDef,
         StreamName: str,
         Tags: Mapping[str, str] = ...,
-        ExclusiveEndTime: Union[datetime, str] = ...
+        ExclusiveEndTime: TimestampTypeDef = ...
     ) -> StreamJournalToKinesisResponseTypeDef:
         """
         Creates a journal stream for a given Amazon QLDB ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.stream_journal_to_kinesis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#stream_journal_to_kinesis)
         """
```

### Comparing `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/literals.py` & `mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/literals.pyi` & `mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/type_defs.py` & `mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_qldb.type_defs import CancelJournalKinesisStreamRequestRequestTypeDef
 
-    data: CancelJournalKinesisStreamRequestRequestTypeDef = {...}
+    data: CancelJournalKinesisStreamRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -37,14 +37,15 @@
     "ResponseMetadataTypeDef",
     "CreateLedgerRequestRequestTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
+    "TimestampTypeDef",
     "ValueHolderTypeDef",
     "GetDigestRequestRequestTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
@@ -173,14 +174,15 @@
 
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
 
+TimestampTypeDef = Union[datetime, str]
 ValueHolderTypeDef = TypedDict(
     "ValueHolderTypeDef",
     {
         "IonText": str,
     },
     total=False,
 )
@@ -554,24 +556,24 @@
 
 
 _RequiredStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_RequiredStreamJournalToKinesisRequestRequestTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
-        "InclusiveStartTime": Union[datetime, str],
+        "InclusiveStartTime": TimestampTypeDef,
         "KinesisConfiguration": KinesisConfigurationTypeDef,
         "StreamName": str,
     },
 )
 _OptionalStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_OptionalStreamJournalToKinesisRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "ExclusiveEndTime": TimestampTypeDef,
     },
     total=False,
 )
 
 
 class StreamJournalToKinesisRequestRequestTypeDef(
     _RequiredStreamJournalToKinesisRequestRequestTypeDef,
@@ -615,16 +617,16 @@
     },
 )
 
 _RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
         "Name": str,
-        "InclusiveStartTime": Union[datetime, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "InclusiveStartTime": TimestampTypeDef,
+        "ExclusiveEndTime": TimestampTypeDef,
         "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
 _OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/type_defs.pyi` & `mypy-boto3-qldb-1.28.16/mypy_boto3_qldb/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_qldb.type_defs import CancelJournalKinesisStreamRequestRequestTypeDef
 
-    data: CancelJournalKinesisStreamRequestRequestTypeDef = {...}
+    data: CancelJournalKinesisStreamRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -36,14 +36,15 @@
     "ResponseMetadataTypeDef",
     "CreateLedgerRequestRequestTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
+    "TimestampTypeDef",
     "ValueHolderTypeDef",
     "GetDigestRequestRequestTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
@@ -168,14 +169,15 @@
 )
 
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
+TimestampTypeDef = Union[datetime, str]
 ValueHolderTypeDef = TypedDict(
     "ValueHolderTypeDef",
     {
         "IonText": str,
     },
     total=False,
 )
@@ -533,24 +535,24 @@
     pass
 
 _RequiredStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_RequiredStreamJournalToKinesisRequestRequestTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
-        "InclusiveStartTime": Union[datetime, str],
+        "InclusiveStartTime": TimestampTypeDef,
         "KinesisConfiguration": KinesisConfigurationTypeDef,
         "StreamName": str,
     },
 )
 _OptionalStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_OptionalStreamJournalToKinesisRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "ExclusiveEndTime": TimestampTypeDef,
     },
     total=False,
 )
 
 class StreamJournalToKinesisRequestRequestTypeDef(
     _RequiredStreamJournalToKinesisRequestRequestTypeDef,
     _OptionalStreamJournalToKinesisRequestRequestTypeDef,
@@ -592,16 +594,16 @@
     },
 )
 
 _RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
         "Name": str,
-        "InclusiveStartTime": Union[datetime, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "InclusiveStartTime": TimestampTypeDef,
+        "ExclusiveEndTime": TimestampTypeDef,
         "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
 _OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/PKG-INFO` & `mypy-boto3-qldb-1.28.16/mypy_boto3_qldb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.QLDB 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 qldb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 qldb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb)](https://pepy.tech/project/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
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
@@ -294,31 +294,32 @@
 )
 
 
 def check_value(value: EncryptionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_qldb.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateLedgerRequestRequestTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
+    TimestampTypeDef,
     ValueHolderTypeDef,
     GetDigestRequestRequestTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
@@ -353,15 +354,15 @@
     JournalS3ExportDescriptionTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
+def get_value() -> CancelJournalKinesisStreamRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/SOURCES.txt` & `mypy-boto3-qldb-1.28.16/mypy_boto3_qldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15.post1/setup.py` & `mypy-boto3-qldb-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qldb",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_qldb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.QLDB 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 qldb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 qldb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_qldb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

