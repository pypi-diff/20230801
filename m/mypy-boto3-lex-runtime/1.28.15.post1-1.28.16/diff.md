# Comparing `tmp/mypy-boto3-lex-runtime-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-lex-runtime-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lex-runtime-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:30 2023, max compression
+gzip compressed data, was "mypy-boto3-lex-runtime-1.28.16.tar", last modified: Tue Aug  1 11:37:10 2023, max compression
```

## Comparing `mypy-boto3-lex-runtime-1.28.15.post1.tar` & `mypy-boto3-lex-runtime-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.665233 mypy-boto3-lex-runtime-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:18.000000 mypy-boto3-lex-runtime-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-07-29 10:03:30.653232 mypy-boto3-lex-runtime-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-07-29 09:49:18.000000 mypy-boto3-lex-runtime-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.649232 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-29 09:49:18.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-29 09:49:18.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:49:18.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-29 09:49:19.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-29 09:49:18.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-07-29 09:49:19.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-29 09:49:19.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:18.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-29 09:49:19.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-29 09:49:19.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:18.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.653232 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-07-29 10:03:30.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-29 10:03:30.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:30.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:03:30.000000 mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:30.665233 mypy-boto3-lex-runtime-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-29 09:49:18.000000 mypy-boto3-lex-runtime-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.484844 mypy-boto3-lex-runtime-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-08-01 11:37:10.480844 mypy-boto3-lex-runtime-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.472844 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-08-01 11:22:10.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.480844 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-08-01 11:37:10.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-01 11:37:10.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:10.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:10.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:10.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:37:10.000000 mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:10.484844 mypy-boto3-lex-runtime-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:22:09.000000 mypy-boto3-lex-runtime-1.28.16/setup.py
```

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/LICENSE` & `mypy-boto3-lex-runtime-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/PKG-INFO` & `mypy-boto3-lex-runtime-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-runtime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LexRuntimeService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LexRuntimeService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lex-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lex-runtime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-runtime)](https://pepy.tech/project/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
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
@@ -293,51 +293,55 @@
 )
 
 
 def check_value(value: ConfirmationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lex_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
     IntentSummaryTypeDef,
-    PostContentRequestRequestTypeDef,
     SentimentResponseTypeDef,
     ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    PostContentRequestRequestTypeDef,
     GenericAttachmentTypeDef,
     DeleteSessionResponseTypeDef,
     PostContentResponseTypeDef,
     PutSessionResponseTypeDef,
+    DialogActionUnionTypeDef,
     PredictedIntentTypeDef,
+    IntentSummaryUnionTypeDef,
     GetSessionResponseTypeDef,
+    ActiveContextUnionTypeDef,
+    ResponseCardTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
-    ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/README.md` & `mypy-boto3-lex-runtime-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-runtime)](https://pepy.tech/project/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
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
@@ -261,51 +261,55 @@
 )
 
 
 def check_value(value: ConfirmationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lex_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
     IntentSummaryTypeDef,
-    PostContentRequestRequestTypeDef,
     SentimentResponseTypeDef,
     ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    PostContentRequestRequestTypeDef,
     GenericAttachmentTypeDef,
     DeleteSessionResponseTypeDef,
     PostContentResponseTypeDef,
     PutSessionResponseTypeDef,
+    DialogActionUnionTypeDef,
     PredictedIntentTypeDef,
+    IntentSummaryUnionTypeDef,
     GetSessionResponseTypeDef,
+    ActiveContextUnionTypeDef,
+    ResponseCardTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
-    ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/__main__.py` & `mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexRuntimeService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LexRuntimeService 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService\nOther"
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

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/client.py` & `mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,25 @@
     from boto3.session import Session
     from mypy_boto3_lex_runtime.client import LexRuntimeServiceClient
 
     session = Session()
     client: LexRuntimeServiceClient = session.client("lex-runtime")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .type_defs import (
-    ActiveContextOutputTypeDef,
-    ActiveContextTypeDef,
+    ActiveContextUnionTypeDef,
+    BlobTypeDef,
     DeleteSessionResponseTypeDef,
-    DialogActionOutputTypeDef,
-    DialogActionTypeDef,
+    DialogActionUnionTypeDef,
     GetSessionResponseTypeDef,
-    IntentSummaryOutputTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryUnionTypeDef,
     PostContentResponseTypeDef,
     PostTextResponseTypeDef,
     PutSessionResponseTypeDef,
 )
 
 __all__ = ("LexRuntimeServiceClient",)
 
@@ -128,15 +125,15 @@
     def post_content(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         contentType: str,
-        inputStream: Union[str, bytes, IO[Any], StreamingBody],
+        inputStream: BlobTypeDef,
         sessionAttributes: str = ...,
         requestAttributes: str = ...,
         accept: str = ...,
         activeContexts: str = ...
     ) -> PostContentResponseTypeDef:
         """
         Sends user input (text or speech) to Amazon Lex.
@@ -150,15 +147,15 @@
         *,
         botName: str,
         botAlias: str,
         userId: str,
         inputText: str,
         sessionAttributes: Mapping[str, str] = ...,
         requestAttributes: Mapping[str, str] = ...,
-        activeContexts: Sequence[Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]] = ...
+        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
     ) -> PostTextResponseTypeDef:
         """
         Sends user input to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/client/#post_text)
         """
@@ -166,20 +163,18 @@
     def put_session(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         sessionAttributes: Mapping[str, str] = ...,
-        dialogAction: Union[DialogActionTypeDef, DialogActionOutputTypeDef] = ...,
-        recentIntentSummaryView: Sequence[
-            Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
-        ] = ...,
+        dialogAction: DialogActionUnionTypeDef = ...,
+        recentIntentSummaryView: Sequence[IntentSummaryUnionTypeDef] = ...,
         accept: str = ...,
-        activeContexts: Sequence[Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]] = ...
+        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.put_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/client/#put_session)
         """
```

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/client.pyi` & `mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,25 @@
     from boto3.session import Session
     from mypy_boto3_lex_runtime.client import LexRuntimeServiceClient
 
     session = Session()
     client: LexRuntimeServiceClient = session.client("lex-runtime")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .type_defs import (
-    ActiveContextOutputTypeDef,
-    ActiveContextTypeDef,
+    ActiveContextUnionTypeDef,
+    BlobTypeDef,
     DeleteSessionResponseTypeDef,
-    DialogActionOutputTypeDef,
-    DialogActionTypeDef,
+    DialogActionUnionTypeDef,
     GetSessionResponseTypeDef,
-    IntentSummaryOutputTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryUnionTypeDef,
     PostContentResponseTypeDef,
     PostTextResponseTypeDef,
     PutSessionResponseTypeDef,
 )
 
 __all__ = ("LexRuntimeServiceClient",)
 
@@ -119,15 +116,15 @@
     def post_content(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         contentType: str,
-        inputStream: Union[str, bytes, IO[Any], StreamingBody],
+        inputStream: BlobTypeDef,
         sessionAttributes: str = ...,
         requestAttributes: str = ...,
         accept: str = ...,
         activeContexts: str = ...
     ) -> PostContentResponseTypeDef:
         """
         Sends user input (text or speech) to Amazon Lex.
@@ -140,35 +137,33 @@
         *,
         botName: str,
         botAlias: str,
         userId: str,
         inputText: str,
         sessionAttributes: Mapping[str, str] = ...,
         requestAttributes: Mapping[str, str] = ...,
-        activeContexts: Sequence[Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]] = ...
+        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
     ) -> PostTextResponseTypeDef:
         """
         Sends user input to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/client/#post_text)
         """
     def put_session(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         sessionAttributes: Mapping[str, str] = ...,
-        dialogAction: Union[DialogActionTypeDef, DialogActionOutputTypeDef] = ...,
-        recentIntentSummaryView: Sequence[
-            Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
-        ] = ...,
+        dialogAction: DialogActionUnionTypeDef = ...,
+        recentIntentSummaryView: Sequence[IntentSummaryUnionTypeDef] = ...,
         accept: str = ...,
-        activeContexts: Sequence[Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]] = ...
+        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.put_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/client/#put_session)
         """
```

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/literals.py` & `mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/literals.pyi` & `mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/type_defs.py` & `mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -29,51 +29,55 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
+    "BlobTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentSummaryOutputTypeDef",
     "IntentConfidenceTypeDef",
     "IntentSummaryTypeDef",
-    "PostContentRequestRequestTypeDef",
     "SentimentResponseTypeDef",
     "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
+    "PostContentRequestRequestTypeDef",
     "GenericAttachmentTypeDef",
     "DeleteSessionResponseTypeDef",
     "PostContentResponseTypeDef",
     "PutSessionResponseTypeDef",
+    "DialogActionUnionTypeDef",
     "PredictedIntentTypeDef",
+    "IntentSummaryUnionTypeDef",
     "GetSessionResponseTypeDef",
+    "ActiveContextUnionTypeDef",
+    "ResponseCardTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
-    "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -113,21 +117,19 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
-
 class DialogActionOutputTypeDef(
     _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
 ):
     pass
 
-
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
@@ -139,19 +141,17 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
-
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
-
 _RequiredGetSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -160,21 +160,19 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "checkpointLabelFilter": str,
     },
     total=False,
 )
 
-
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredIntentSummaryOutputTypeDef = TypedDict(
     "_RequiredIntentSummaryOutputTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
 _OptionalIntentSummaryOutputTypeDef = TypedDict(
@@ -186,21 +184,19 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
-
 class IntentSummaryOutputTypeDef(
     _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
 ):
     pass
 
-
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
@@ -220,47 +216,17 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
-
 class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
-
-_RequiredPostContentRequestRequestTypeDef = TypedDict(
-    "_RequiredPostContentRequestRequestTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-        "userId": str,
-        "contentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalPostContentRequestRequestTypeDef = TypedDict(
-    "_OptionalPostContentRequestRequestTypeDef",
-    {
-        "sessionAttributes": str,
-        "requestAttributes": str,
-        "accept": str,
-        "activeContexts": str,
-    },
-    total=False,
-)
-
-
-class PostContentRequestRequestTypeDef(
-    _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
-):
-    pass
-
-
 SentimentResponseTypeDef = TypedDict(
     "SentimentResponseTypeDef",
     {
         "sentimentLabel": str,
         "sentimentScore": str,
     },
     total=False,
@@ -280,14 +246,40 @@
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
         "parameters": Mapping[str, str],
     },
 )
 
+_RequiredPostContentRequestRequestTypeDef = TypedDict(
+    "_RequiredPostContentRequestRequestTypeDef",
+    {
+        "botName": str,
+        "botAlias": str,
+        "userId": str,
+        "contentType": str,
+        "inputStream": BlobTypeDef,
+    },
+)
+_OptionalPostContentRequestRequestTypeDef = TypedDict(
+    "_OptionalPostContentRequestRequestTypeDef",
+    {
+        "sessionAttributes": str,
+        "requestAttributes": str,
+        "accept": str,
+        "activeContexts": str,
+    },
+    total=False,
+)
+
+class PostContentRequestRequestTypeDef(
+    _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
+):
+    pass
+
 GenericAttachmentTypeDef = TypedDict(
     "GenericAttachmentTypeDef",
     {
         "title": str,
         "subTitle": str,
         "attachmentLinkUrl": str,
         "imageUrl": str,
@@ -347,101 +339,98 @@
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DialogActionUnionTypeDef = Union[DialogActionTypeDef, DialogActionOutputTypeDef]
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "slots": Dict[str, str],
     },
     total=False,
 )
 
+IntentSummaryUnionTypeDef = Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
         "dialogAction": DialogActionOutputTypeDef,
         "activeContexts": List[ActiveContextOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActiveContextUnionTypeDef = Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]
+ResponseCardTypeDef = TypedDict(
+    "ResponseCardTypeDef",
+    {
+        "version": str,
+        "contentType": Literal["application/vnd.amazonaws.card.generic"],
+        "genericAttachments": List[GenericAttachmentTypeDef],
+    },
+    total=False,
+)
+
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "inputText": str,
     },
 )
 _OptionalPostTextRequestRequestTypeDef = TypedDict(
     "_OptionalPostTextRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
-        "activeContexts": Sequence[Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]],
+        "activeContexts": Sequence[ActiveContextUnionTypeDef],
     },
     total=False,
 )
 
-
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "dialogAction": DialogActionTypeDef,
-        "recentIntentSummaryView": Sequence[
-            Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
-        ],
+        "recentIntentSummaryView": Sequence[IntentSummaryUnionTypeDef],
         "accept": str,
-        "activeContexts": Sequence[Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]],
+        "activeContexts": Sequence[ActiveContextUnionTypeDef],
     },
     total=False,
 )
 
-
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
-
-ResponseCardTypeDef = TypedDict(
-    "ResponseCardTypeDef",
-    {
-        "version": str,
-        "contentType": Literal["application/vnd.amazonaws.card.generic"],
-        "genericAttachments": List[GenericAttachmentTypeDef],
-    },
-    total=False,
-)
-
 PostTextResponseTypeDef = TypedDict(
     "PostTextResponseTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "alternativeIntents": List[PredictedIntentTypeDef],
         "slots": Dict[str, str],
```

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime/type_defs.pyi` & `mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -29,50 +29,56 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
+    "BlobTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentSummaryOutputTypeDef",
     "IntentConfidenceTypeDef",
     "IntentSummaryTypeDef",
-    "PostContentRequestRequestTypeDef",
     "SentimentResponseTypeDef",
     "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
+    "PostContentRequestRequestTypeDef",
     "GenericAttachmentTypeDef",
     "DeleteSessionResponseTypeDef",
     "PostContentResponseTypeDef",
     "PutSessionResponseTypeDef",
+    "DialogActionUnionTypeDef",
     "PredictedIntentTypeDef",
+    "IntentSummaryUnionTypeDef",
     "GetSessionResponseTypeDef",
+    "ActiveContextUnionTypeDef",
+    "ResponseCardTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
-    "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -112,19 +118,21 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
+
 class DialogActionOutputTypeDef(
     _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
 ):
     pass
 
+
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
@@ -136,17 +144,19 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
+
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
+
 _RequiredGetSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -155,19 +165,21 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "checkpointLabelFilter": str,
     },
     total=False,
 )
 
+
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredIntentSummaryOutputTypeDef = TypedDict(
     "_RequiredIntentSummaryOutputTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
 _OptionalIntentSummaryOutputTypeDef = TypedDict(
@@ -179,19 +191,21 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
+
 class IntentSummaryOutputTypeDef(
     _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
 ):
     pass
 
+
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
@@ -211,42 +225,18 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
+
 class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
-_RequiredPostContentRequestRequestTypeDef = TypedDict(
-    "_RequiredPostContentRequestRequestTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-        "userId": str,
-        "contentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalPostContentRequestRequestTypeDef = TypedDict(
-    "_OptionalPostContentRequestRequestTypeDef",
-    {
-        "sessionAttributes": str,
-        "requestAttributes": str,
-        "accept": str,
-        "activeContexts": str,
-    },
-    total=False,
-)
-
-class PostContentRequestRequestTypeDef(
-    _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
-):
-    pass
 
 SentimentResponseTypeDef = TypedDict(
     "SentimentResponseTypeDef",
     {
         "sentimentLabel": str,
         "sentimentScore": str,
     },
@@ -267,14 +257,42 @@
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
         "parameters": Mapping[str, str],
     },
 )
 
+_RequiredPostContentRequestRequestTypeDef = TypedDict(
+    "_RequiredPostContentRequestRequestTypeDef",
+    {
+        "botName": str,
+        "botAlias": str,
+        "userId": str,
+        "contentType": str,
+        "inputStream": BlobTypeDef,
+    },
+)
+_OptionalPostContentRequestRequestTypeDef = TypedDict(
+    "_OptionalPostContentRequestRequestTypeDef",
+    {
+        "sessionAttributes": str,
+        "requestAttributes": str,
+        "accept": str,
+        "activeContexts": str,
+    },
+    total=False,
+)
+
+
+class PostContentRequestRequestTypeDef(
+    _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
+):
+    pass
+
+
 GenericAttachmentTypeDef = TypedDict(
     "GenericAttachmentTypeDef",
     {
         "title": str,
         "subTitle": str,
         "attachmentLinkUrl": str,
         "imageUrl": str,
@@ -334,96 +352,101 @@
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DialogActionUnionTypeDef = Union[DialogActionTypeDef, DialogActionOutputTypeDef]
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "slots": Dict[str, str],
     },
     total=False,
 )
 
+IntentSummaryUnionTypeDef = Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
         "dialogAction": DialogActionOutputTypeDef,
         "activeContexts": List[ActiveContextOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActiveContextUnionTypeDef = Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]
+ResponseCardTypeDef = TypedDict(
+    "ResponseCardTypeDef",
+    {
+        "version": str,
+        "contentType": Literal["application/vnd.amazonaws.card.generic"],
+        "genericAttachments": List[GenericAttachmentTypeDef],
+    },
+    total=False,
+)
+
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "inputText": str,
     },
 )
 _OptionalPostTextRequestRequestTypeDef = TypedDict(
     "_OptionalPostTextRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
-        "activeContexts": Sequence[Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]],
+        "activeContexts": Sequence[ActiveContextUnionTypeDef],
     },
     total=False,
 )
 
+
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "dialogAction": DialogActionTypeDef,
-        "recentIntentSummaryView": Sequence[
-            Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
-        ],
+        "recentIntentSummaryView": Sequence[IntentSummaryUnionTypeDef],
         "accept": str,
-        "activeContexts": Sequence[Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]],
+        "activeContexts": Sequence[ActiveContextUnionTypeDef],
     },
     total=False,
 )
 
+
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
-ResponseCardTypeDef = TypedDict(
-    "ResponseCardTypeDef",
-    {
-        "version": str,
-        "contentType": Literal["application/vnd.amazonaws.card.generic"],
-        "genericAttachments": List[GenericAttachmentTypeDef],
-    },
-    total=False,
-)
 
 PostTextResponseTypeDef = TypedDict(
     "PostTextResponseTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "alternativeIntents": List[PredictedIntentTypeDef],
```

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime.egg-info/PKG-INFO` & `mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-runtime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LexRuntimeService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LexRuntimeService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lex-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lex-runtime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-runtime)](https://pepy.tech/project/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
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
@@ -293,51 +293,55 @@
 )
 
 
 def check_value(value: ConfirmationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lex_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
     IntentSummaryTypeDef,
-    PostContentRequestRequestTypeDef,
     SentimentResponseTypeDef,
     ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    PostContentRequestRequestTypeDef,
     GenericAttachmentTypeDef,
     DeleteSessionResponseTypeDef,
     PostContentResponseTypeDef,
     PutSessionResponseTypeDef,
+    DialogActionUnionTypeDef,
     PredictedIntentTypeDef,
+    IntentSummaryUnionTypeDef,
     GetSessionResponseTypeDef,
+    ActiveContextUnionTypeDef,
+    ResponseCardTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
-    ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/mypy_boto3_lex_runtime.egg-info/SOURCES.txt` & `mypy-boto3-lex-runtime-1.28.16/mypy_boto3_lex_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.15.post1/setup.py` & `mypy-boto3-lex-runtime-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lex-runtime",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_lex_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexRuntimeService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.LexRuntimeService 1.28.16 service generated with"
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
-    keywords="boto3 lex-runtime type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 lex-runtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_lex_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

