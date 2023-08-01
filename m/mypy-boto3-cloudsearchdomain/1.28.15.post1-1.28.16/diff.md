# Comparing `tmp/mypy-boto3-cloudsearchdomain-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-cloudsearchdomain-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudsearchdomain-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:44 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudsearchdomain-1.28.16.tar", last modified: Tue Aug  1 11:36:25 2023, max compression
```

## Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1.tar` & `mypy-boto3-cloudsearchdomain-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:44.165060 mypy-boto3-cloudsearchdomain-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-07-29 10:02:44.157060 mypy-boto3-cloudsearchdomain-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:44.153060 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:44.157060 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:44.165060 mypy-boto3-cloudsearchdomain-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearchdomain-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.356929 mypy-boto3-cloudsearchdomain-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:12:45.000000 mypy-boto3-cloudsearchdomain-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-08-01 11:36:25.348929 mypy-boto3-cloudsearchdomain-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-01 11:12:45.000000 mypy-boto3-cloudsearchdomain-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.348929 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-01 11:12:45.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-01 11:12:45.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 11:12:45.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-08-01 11:12:46.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-01 11:12:45.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-08-01 11:12:46.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-08-01 11:12:46.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:12:45.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-01 11:12:46.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-08-01 11:12:46.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:12:45.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.348929 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-08-01 11:36:25.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-01 11:36:25.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:25.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:36:25.000000 mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:25.356929 mypy-boto3-cloudsearchdomain-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-01 11:12:45.000000 mypy-boto3-cloudsearchdomain-1.28.16/setup.py
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/LICENSE` & `mypy-boto3-cloudsearchdomain-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/PKG-INFO` & `mypy-boto3-cloudsearchdomain-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearchdomain
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudSearchDomain 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudSearchDomain 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudsearchdomain type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cloudsearchdomain type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearchdomain)](https://pepy.tech/project/mypy-boto3-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearchDomain 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[boto3.CloudSearchDomain 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [mypy-boto3-cloudsearchdomain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/).
 
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
@@ -289,23 +289,24 @@
 )
 
 
 def check_value(value: ContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudsearchdomain.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearchdomain.type_defs import (
+    BlobTypeDef,
     BucketTypeDef,
     DocumentServiceWarningTypeDef,
     FieldStatsTypeDef,
     HitTypeDef,
     ResponseMetadataTypeDef,
     SearchRequestRequestTypeDef,
     SearchStatusTypeDef,
@@ -318,15 +319,15 @@
     UploadDocumentsResponseTypeDef,
     SuggestModelTypeDef,
     SearchResponseTypeDef,
     SuggestResponseTypeDef,
 )
 
 
-def get_structure() -> BucketTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/README.md` & `mypy-boto3-cloudsearchdomain-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearchdomain)](https://pepy.tech/project/mypy-boto3-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearchDomain 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[boto3.CloudSearchDomain 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [mypy-boto3-cloudsearchdomain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/).
 
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
@@ -257,23 +257,24 @@
 )
 
 
 def check_value(value: ContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudsearchdomain.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearchdomain.type_defs import (
+    BlobTypeDef,
     BucketTypeDef,
     DocumentServiceWarningTypeDef,
     FieldStatsTypeDef,
     HitTypeDef,
     ResponseMetadataTypeDef,
     SearchRequestRequestTypeDef,
     SearchStatusTypeDef,
@@ -286,15 +287,15 @@
     UploadDocumentsResponseTypeDef,
     SuggestModelTypeDef,
     SearchResponseTypeDef,
     SuggestResponseTypeDef,
 )
 
 
-def get_structure() -> BucketTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/__main__.py` & `mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudSearchDomain 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CloudSearchDomain 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain\nOther"
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

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/client.py` & `mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,21 +9,25 @@
     from boto3.session import Session
     from mypy_boto3_cloudsearchdomain.client import CloudSearchDomainClient
 
     session = Session()
     client: CloudSearchDomainClient = session.client("cloudsearchdomain")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import ContentTypeType, QueryParserType
-from .type_defs import SearchResponseTypeDef, SuggestResponseTypeDef, UploadDocumentsResponseTypeDef
+from .type_defs import (
+    BlobTypeDef,
+    SearchResponseTypeDef,
+    SuggestResponseTypeDef,
+    UploadDocumentsResponseTypeDef,
+)
 
 __all__ = ("CloudSearchDomainClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -115,15 +119,15 @@
         Retrieves autocomplete suggestions for a partial query string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.suggest)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/client/#suggest)
         """
 
     def upload_documents(
-        self, *, documents: Union[str, bytes, IO[Any], StreamingBody], contentType: ContentTypeType
+        self, *, documents: BlobTypeDef, contentType: ContentTypeType
     ) -> UploadDocumentsResponseTypeDef:
         """
         Posts a batch of documents to a search domain for indexing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.upload_documents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/client/#upload_documents)
         """
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/client.pyi` & `mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,25 @@
     from boto3.session import Session
     from mypy_boto3_cloudsearchdomain.client import CloudSearchDomainClient
 
     session = Session()
     client: CloudSearchDomainClient = session.client("cloudsearchdomain")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import ContentTypeType, QueryParserType
-from .type_defs import SearchResponseTypeDef, SuggestResponseTypeDef, UploadDocumentsResponseTypeDef
+from .type_defs import (
+    BlobTypeDef,
+    SearchResponseTypeDef,
+    SuggestResponseTypeDef,
+    UploadDocumentsResponseTypeDef,
+)
 
 __all__ = ("CloudSearchDomainClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -106,15 +110,15 @@
         """
         Retrieves autocomplete suggestions for a partial query string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.suggest)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/client/#suggest)
         """
     def upload_documents(
-        self, *, documents: Union[str, bytes, IO[Any], StreamingBody], contentType: ContentTypeType
+        self, *, documents: BlobTypeDef, contentType: ContentTypeType
     ) -> UploadDocumentsResponseTypeDef:
         """
         Posts a batch of documents to a search domain for indexing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.upload_documents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/client/#upload_documents)
         """
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/literals.py` & `mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/literals.pyi` & `mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/type_defs.py` & `mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cloudsearchdomain service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cloudsearchdomain.type_defs import BucketTypeDef
+    from mypy_boto3_cloudsearchdomain.type_defs import BlobTypeDef
 
-    data: BucketTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
 
@@ -21,14 +21,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "BucketTypeDef",
     "DocumentServiceWarningTypeDef",
     "FieldStatsTypeDef",
     "HitTypeDef",
     "ResponseMetadataTypeDef",
     "SearchRequestRequestTypeDef",
     "SearchStatusTypeDef",
@@ -40,14 +41,15 @@
     "HitsTypeDef",
     "UploadDocumentsResponseTypeDef",
     "SuggestModelTypeDef",
     "SearchResponseTypeDef",
     "SuggestResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "value": str,
         "count": int,
     },
     total=False,
@@ -180,15 +182,15 @@
     },
     total=False,
 )
 
 UploadDocumentsRequestRequestTypeDef = TypedDict(
     "UploadDocumentsRequestRequestTypeDef",
     {
-        "documents": Union[str, bytes, IO[Any], StreamingBody],
+        "documents": BlobTypeDef,
         "contentType": ContentTypeType,
     },
 )
 
 BucketInfoTypeDef = TypedDict(
     "BucketInfoTypeDef",
     {
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain/type_defs.pyi` & `mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cloudsearchdomain service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cloudsearchdomain.type_defs import BucketTypeDef
+    from mypy_boto3_cloudsearchdomain.type_defs import BlobTypeDef
 
-    data: BucketTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
 
@@ -20,14 +20,15 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "BucketTypeDef",
     "DocumentServiceWarningTypeDef",
     "FieldStatsTypeDef",
     "HitTypeDef",
     "ResponseMetadataTypeDef",
     "SearchRequestRequestTypeDef",
     "SearchStatusTypeDef",
@@ -39,14 +40,15 @@
     "HitsTypeDef",
     "UploadDocumentsResponseTypeDef",
     "SuggestModelTypeDef",
     "SearchResponseTypeDef",
     "SuggestResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "value": str,
         "count": int,
     },
     total=False,
@@ -175,15 +177,15 @@
     },
     total=False,
 )
 
 UploadDocumentsRequestRequestTypeDef = TypedDict(
     "UploadDocumentsRequestRequestTypeDef",
     {
-        "documents": Union[str, bytes, IO[Any], StreamingBody],
+        "documents": BlobTypeDef,
         "contentType": ContentTypeType,
     },
 )
 
 BucketInfoTypeDef = TypedDict(
     "BucketInfoTypeDef",
     {
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO` & `mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearchdomain
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudSearchDomain 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudSearchDomain 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudsearchdomain type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cloudsearchdomain type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearchdomain)](https://pepy.tech/project/mypy-boto3-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearchDomain 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[boto3.CloudSearchDomain 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [mypy-boto3-cloudsearchdomain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/).
 
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
@@ -289,23 +289,24 @@
 )
 
 
 def check_value(value: ContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudsearchdomain.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearchdomain.type_defs import (
+    BlobTypeDef,
     BucketTypeDef,
     DocumentServiceWarningTypeDef,
     FieldStatsTypeDef,
     HitTypeDef,
     ResponseMetadataTypeDef,
     SearchRequestRequestTypeDef,
     SearchStatusTypeDef,
@@ -318,15 +319,15 @@
     UploadDocumentsResponseTypeDef,
     SuggestModelTypeDef,
     SearchResponseTypeDef,
     SuggestResponseTypeDef,
 )
 
 
-def get_structure() -> BucketTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt` & `mypy-boto3-cloudsearchdomain-1.28.16/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.15.post1/setup.py` & `mypy-boto3-cloudsearchdomain-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudsearchdomain",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_cloudsearchdomain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudSearchDomain 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CloudSearchDomain 1.28.16 service generated with"
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
-    keywords="boto3 cloudsearchdomain type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 cloudsearchdomain type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_cloudsearchdomain": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

