# Comparing `tmp/mypy-boto3-lexv2-runtime-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-lexv2-runtime-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lexv2-runtime-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:31 2023, max compression
+gzip compressed data, was "mypy-boto3-lexv2-runtime-1.28.16.tar", last modified: Tue Aug  1 11:37:11 2023, max compression
```

## Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1.tar` & `mypy-boto3-lexv2-runtime-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:31.233236 mypy-boto3-lexv2-runtime-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-29 10:03:31.233236 mypy-boto3-lexv2-runtime-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:31.233236 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:31.233236 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-29 10:03:30.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-29 10:03:31.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:30.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:30.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:31.233236 mypy-boto3-lexv2-runtime-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-29 09:49:41.000000 mypy-boto3-lexv2-runtime-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:11.564841 mypy-boto3-lexv2-runtime-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-08-01 11:37:11.556841 mypy-boto3-lexv2-runtime-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:11.544841 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-08-01 11:22:33.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:11.556841 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-08-01 11:37:11.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 11:37:11.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:11.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:11.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:11.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:37:11.000000 mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:11.564841 mypy-boto3-lexv2-runtime-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 11:22:32.000000 mypy-boto3-lexv2-runtime-1.28.16/setup.py
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/LICENSE` & `mypy-boto3-lexv2-runtime-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/PKG-INFO` & `mypy-boto3-lexv2-runtime-1.28.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-runtime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LexRuntimeV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LexRuntimeV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lexv2-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lexv2-runtime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lexv2-runtime)](https://pepy.tech/project/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
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
@@ -294,43 +294,44 @@
 )
 
 
 def check_value(value: ConfirmationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lexv2_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DialogActionTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentOutputTypeDef,
     IntentTypeDef,
     RecognizedBotMemberTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
     RuntimeHintValueTypeDef,
     RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
     SentimentScoreTypeDef,
     ValueOutputTypeDef,
     ValueTypeDef,
     ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    RecognizeUtteranceRequestRequestTypeDef,
     ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
     DeleteSessionResponseTypeDef,
     PutSessionResponseTypeDef,
     RecognizeUtteranceResponseTypeDef,
     RuntimeHintDetailsOutputTypeDef,
     RuntimeHintDetailsTypeDef,
@@ -339,21 +340,23 @@
     SlotTypeDef,
     SessionStateOutputTypeDef,
     SessionStateTypeDef,
     MessageOutputTypeDef,
     MessageTypeDef,
     InterpretationTypeDef,
     RecognizeTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
+    SessionStateUnionTypeDef,
+    MessageUnionTypeDef,
     GetSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
+    PutSessionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/README.md` & `mypy-boto3-lexv2-runtime-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lexv2-runtime)](https://pepy.tech/project/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
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
@@ -262,43 +262,44 @@
 )
 
 
 def check_value(value: ConfirmationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lexv2_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DialogActionTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentOutputTypeDef,
     IntentTypeDef,
     RecognizedBotMemberTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
     RuntimeHintValueTypeDef,
     RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
     SentimentScoreTypeDef,
     ValueOutputTypeDef,
     ValueTypeDef,
     ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    RecognizeUtteranceRequestRequestTypeDef,
     ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
     DeleteSessionResponseTypeDef,
     PutSessionResponseTypeDef,
     RecognizeUtteranceResponseTypeDef,
     RuntimeHintDetailsOutputTypeDef,
     RuntimeHintDetailsTypeDef,
@@ -307,21 +308,23 @@
     SlotTypeDef,
     SessionStateOutputTypeDef,
     SessionStateTypeDef,
     MessageOutputTypeDef,
     MessageTypeDef,
     InterpretationTypeDef,
     RecognizeTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
+    SessionStateUnionTypeDef,
+    MessageUnionTypeDef,
     GetSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
+    PutSessionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/__main__.py` & `mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexRuntimeV2 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LexRuntimeV2 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2\nOther"
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

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/client.py` & `mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,54 +9,49 @@
     from boto3.session import Session
     from mypy_boto3_lexv2_runtime.client import LexRuntimeV2Client
 
     session = Session()
     client: LexRuntimeV2Client = session.client("lexv2-runtime")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .type_defs import (
+    BlobTypeDef,
     DeleteSessionResponseTypeDef,
     GetSessionResponseTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
+    MessageUnionTypeDef,
     PutSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
     RecognizeUtteranceResponseTypeDef,
-    SessionStateOutputTypeDef,
-    SessionStateTypeDef,
+    SessionStateUnionTypeDef,
 )
 
 __all__ = ("LexRuntimeV2Client",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadGatewayException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     DependencyFailedException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class LexRuntimeV2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/)
     """
 
     meta: ClientMeta
@@ -65,114 +60,106 @@
     def exceptions(self) -> Exceptions:
         """
         LexRuntimeV2Client exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#close)
         """
-
     def delete_session(
         self, *, botId: str, botAliasId: str, localeId: str, sessionId: str
     ) -> DeleteSessionResponseTypeDef:
         """
         Removes session information for a specified bot, alias, and user ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.delete_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#delete_session)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#generate_presigned_url)
         """
-
     def get_session(
         self, *, botId: str, botAliasId: str, localeId: str, sessionId: str
     ) -> GetSessionResponseTypeDef:
         """
         Returns session information for a specified bot, alias, and user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.get_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#get_session)
         """
-
     def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: Union[SessionStateTypeDef, SessionStateOutputTypeDef],
-        messages: Sequence[Union[MessageTypeDef, MessageOutputTypeDef]] = ...,
+        sessionState: SessionStateUnionTypeDef,
+        messages: Sequence[MessageUnionTypeDef] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#put_session)
         """
-
     def recognize_text(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: Union[SessionStateTypeDef, SessionStateOutputTypeDef] = ...,
+        sessionState: SessionStateUnionTypeDef = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#recognize_text)
         """
-
     def recognize_utterance(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         requestContentType: str,
         sessionState: str = ...,
         requestAttributes: str = ...,
         responseContentType: str = ...,
-        inputStream: Union[str, bytes, IO[Any], StreamingBody] = ...
+        inputStream: BlobTypeDef = ...
     ) -> RecognizeUtteranceResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_utterance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#recognize_utterance)
         """
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/client.pyi` & `mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,51 +9,52 @@
     from boto3.session import Session
     from mypy_boto3_lexv2_runtime.client import LexRuntimeV2Client
 
     session = Session()
     client: LexRuntimeV2Client = session.client("lexv2-runtime")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .type_defs import (
+    BlobTypeDef,
     DeleteSessionResponseTypeDef,
     GetSessionResponseTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
+    MessageUnionTypeDef,
     PutSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
     RecognizeUtteranceResponseTypeDef,
-    SessionStateOutputTypeDef,
-    SessionStateTypeDef,
+    SessionStateUnionTypeDef,
 )
 
 __all__ = ("LexRuntimeV2Client",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadGatewayException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     DependencyFailedException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class LexRuntimeV2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/)
     """
 
     meta: ClientMeta
@@ -62,106 +63,114 @@
     def exceptions(self) -> Exceptions:
         """
         LexRuntimeV2Client exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#close)
         """
+
     def delete_session(
         self, *, botId: str, botAliasId: str, localeId: str, sessionId: str
     ) -> DeleteSessionResponseTypeDef:
         """
         Removes session information for a specified bot, alias, and user ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.delete_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#delete_session)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#generate_presigned_url)
         """
+
     def get_session(
         self, *, botId: str, botAliasId: str, localeId: str, sessionId: str
     ) -> GetSessionResponseTypeDef:
         """
         Returns session information for a specified bot, alias, and user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.get_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#get_session)
         """
+
     def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: Union[SessionStateTypeDef, SessionStateOutputTypeDef],
-        messages: Sequence[Union[MessageTypeDef, MessageOutputTypeDef]] = ...,
+        sessionState: SessionStateUnionTypeDef,
+        messages: Sequence[MessageUnionTypeDef] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#put_session)
         """
+
     def recognize_text(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: Union[SessionStateTypeDef, SessionStateOutputTypeDef] = ...,
+        sessionState: SessionStateUnionTypeDef = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#recognize_text)
         """
+
     def recognize_utterance(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         requestContentType: str,
         sessionState: str = ...,
         requestAttributes: str = ...,
         responseContentType: str = ...,
-        inputStream: Union[str, bytes, IO[Any], StreamingBody] = ...
+        inputStream: BlobTypeDef = ...
     ) -> RecognizeUtteranceResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_utterance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#recognize_utterance)
         """
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/literals.py` & `mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/literals.pyi` & `mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/type_defs.py` & `mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lexv2_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -30,33 +30,34 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
+    "BlobTypeDef",
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DialogActionTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentOutputTypeDef",
     "IntentTypeDef",
     "RecognizedBotMemberTypeDef",
-    "RecognizeUtteranceRequestRequestTypeDef",
     "RuntimeHintValueTypeDef",
     "RuntimeHintsOutputTypeDef",
     "RuntimeHintsTypeDef",
     "SentimentScoreTypeDef",
     "ValueOutputTypeDef",
     "ValueTypeDef",
     "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
+    "RecognizeUtteranceRequestRequestTypeDef",
     "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
     "DeleteSessionResponseTypeDef",
     "PutSessionResponseTypeDef",
     "RecognizeUtteranceResponseTypeDef",
     "RuntimeHintDetailsOutputTypeDef",
     "RuntimeHintDetailsTypeDef",
@@ -65,27 +66,30 @@
     "SlotTypeDef",
     "SessionStateOutputTypeDef",
     "SessionStateTypeDef",
     "MessageOutputTypeDef",
     "MessageTypeDef",
     "InterpretationTypeDef",
     "RecognizeTextRequestRequestTypeDef",
-    "PutSessionRequestRequestTypeDef",
+    "SessionStateUnionTypeDef",
+    "MessageUnionTypeDef",
     "GetSessionResponseTypeDef",
     "RecognizeTextResponseTypeDef",
+    "PutSessionRequestRequestTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -228,43 +232,14 @@
 
 class RecognizedBotMemberTypeDef(
     _RequiredRecognizedBotMemberTypeDef, _OptionalRecognizedBotMemberTypeDef
 ):
     pass
 
 
-_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "requestContentType": str,
-    },
-)
-_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
-    {
-        "sessionState": str,
-        "requestAttributes": str,
-        "responseContentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class RecognizeUtteranceRequestRequestTypeDef(
-    _RequiredRecognizeUtteranceRequestRequestTypeDef,
-    _OptionalRecognizeUtteranceRequestRequestTypeDef,
-):
-    pass
-
-
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
@@ -349,14 +324,43 @@
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
         "contextAttributes": Mapping[str, str],
     },
 )
 
+_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "requestContentType": str,
+    },
+)
+_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
+    {
+        "sessionState": str,
+        "requestAttributes": str,
+        "responseContentType": str,
+        "inputStream": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class RecognizeUtteranceRequestRequestTypeDef(
+    _RequiredRecognizeUtteranceRequestRequestTypeDef,
+    _OptionalRecognizeUtteranceRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredImageResponseCardOutputTypeDef = TypedDict(
     "_RequiredImageResponseCardOutputTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardOutputTypeDef = TypedDict(
@@ -587,57 +591,58 @@
 
 class RecognizeTextRequestRequestTypeDef(
     _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
 ):
     pass
 
 
+SessionStateUnionTypeDef = Union[SessionStateTypeDef, SessionStateOutputTypeDef]
+MessageUnionTypeDef = Union[MessageTypeDef, MessageOutputTypeDef]
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "sessionId": str,
+        "messages": List[MessageOutputTypeDef],
+        "interpretations": List[InterpretationTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecognizeTextResponseTypeDef = TypedDict(
+    "RecognizeTextResponseTypeDef",
+    {
+        "messages": List[MessageOutputTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "interpretations": List[InterpretationTypeDef],
+        "requestAttributes": Dict[str, str],
+        "sessionId": str,
+        "recognizedBotMember": RecognizedBotMemberTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
         "sessionState": SessionStateTypeDef,
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
-        "messages": Sequence[Union[MessageTypeDef, MessageOutputTypeDef]],
+        "messages": Sequence[MessageUnionTypeDef],
         "requestAttributes": Mapping[str, str],
         "responseContentType": str,
     },
     total=False,
 )
 
 
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
-
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "sessionId": str,
-        "messages": List[MessageOutputTypeDef],
-        "interpretations": List[InterpretationTypeDef],
-        "sessionState": SessionStateOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RecognizeTextResponseTypeDef = TypedDict(
-    "RecognizeTextResponseTypeDef",
-    {
-        "messages": List[MessageOutputTypeDef],
-        "sessionState": SessionStateOutputTypeDef,
-        "interpretations": List[InterpretationTypeDef],
-        "requestAttributes": Dict[str, str],
-        "sessionId": str,
-        "recognizedBotMember": RecognizedBotMemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime/type_defs.pyi` & `mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lexv2_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -29,33 +29,34 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
+    "BlobTypeDef",
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DialogActionTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentOutputTypeDef",
     "IntentTypeDef",
     "RecognizedBotMemberTypeDef",
-    "RecognizeUtteranceRequestRequestTypeDef",
     "RuntimeHintValueTypeDef",
     "RuntimeHintsOutputTypeDef",
     "RuntimeHintsTypeDef",
     "SentimentScoreTypeDef",
     "ValueOutputTypeDef",
     "ValueTypeDef",
     "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
+    "RecognizeUtteranceRequestRequestTypeDef",
     "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
     "DeleteSessionResponseTypeDef",
     "PutSessionResponseTypeDef",
     "RecognizeUtteranceResponseTypeDef",
     "RuntimeHintDetailsOutputTypeDef",
     "RuntimeHintDetailsTypeDef",
@@ -64,27 +65,30 @@
     "SlotTypeDef",
     "SessionStateOutputTypeDef",
     "SessionStateTypeDef",
     "MessageOutputTypeDef",
     "MessageTypeDef",
     "InterpretationTypeDef",
     "RecognizeTextRequestRequestTypeDef",
-    "PutSessionRequestRequestTypeDef",
+    "SessionStateUnionTypeDef",
+    "MessageUnionTypeDef",
     "GetSessionResponseTypeDef",
     "RecognizeTextResponseTypeDef",
+    "PutSessionRequestRequestTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -217,41 +221,14 @@
 )
 
 class RecognizedBotMemberTypeDef(
     _RequiredRecognizedBotMemberTypeDef, _OptionalRecognizedBotMemberTypeDef
 ):
     pass
 
-_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "requestContentType": str,
-    },
-)
-_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
-    {
-        "sessionState": str,
-        "requestAttributes": str,
-        "responseContentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class RecognizeUtteranceRequestRequestTypeDef(
-    _RequiredRecognizeUtteranceRequestRequestTypeDef,
-    _OptionalRecognizeUtteranceRequestRequestTypeDef,
-):
-    pass
-
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
@@ -332,14 +309,41 @@
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
         "contextAttributes": Mapping[str, str],
     },
 )
 
+_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "requestContentType": str,
+    },
+)
+_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
+    {
+        "sessionState": str,
+        "requestAttributes": str,
+        "responseContentType": str,
+        "inputStream": BlobTypeDef,
+    },
+    total=False,
+)
+
+class RecognizeUtteranceRequestRequestTypeDef(
+    _RequiredRecognizeUtteranceRequestRequestTypeDef,
+    _OptionalRecognizeUtteranceRequestRequestTypeDef,
+):
+    pass
+
 _RequiredImageResponseCardOutputTypeDef = TypedDict(
     "_RequiredImageResponseCardOutputTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardOutputTypeDef = TypedDict(
@@ -560,39 +564,16 @@
 )
 
 class RecognizeTextRequestRequestTypeDef(
     _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
 ):
     pass
 
-_RequiredPutSessionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSessionRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "sessionState": SessionStateTypeDef,
-    },
-)
-_OptionalPutSessionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSessionRequestRequestTypeDef",
-    {
-        "messages": Sequence[Union[MessageTypeDef, MessageOutputTypeDef]],
-        "requestAttributes": Mapping[str, str],
-        "responseContentType": str,
-    },
-    total=False,
-)
-
-class PutSessionRequestRequestTypeDef(
-    _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
-):
-    pass
-
+SessionStateUnionTypeDef = Union[SessionStateTypeDef, SessionStateOutputTypeDef]
+MessageUnionTypeDef = Union[MessageTypeDef, MessageOutputTypeDef]
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "sessionId": str,
         "messages": List[MessageOutputTypeDef],
         "interpretations": List[InterpretationTypeDef],
         "sessionState": SessionStateOutputTypeDef,
@@ -608,7 +589,32 @@
         "interpretations": List[InterpretationTypeDef],
         "requestAttributes": Dict[str, str],
         "sessionId": str,
         "recognizedBotMember": RecognizedBotMemberTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredPutSessionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSessionRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "sessionState": SessionStateTypeDef,
+    },
+)
+_OptionalPutSessionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSessionRequestRequestTypeDef",
+    {
+        "messages": Sequence[MessageUnionTypeDef],
+        "requestAttributes": Mapping[str, str],
+        "responseContentType": str,
+    },
+    total=False,
+)
+
+class PutSessionRequestRequestTypeDef(
+    _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO` & `mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-runtime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LexRuntimeV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LexRuntimeV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lexv2-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lexv2-runtime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lexv2-runtime)](https://pepy.tech/project/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
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
@@ -294,43 +294,44 @@
 )
 
 
 def check_value(value: ConfirmationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lexv2_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DialogActionTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentOutputTypeDef,
     IntentTypeDef,
     RecognizedBotMemberTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
     RuntimeHintValueTypeDef,
     RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
     SentimentScoreTypeDef,
     ValueOutputTypeDef,
     ValueTypeDef,
     ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    RecognizeUtteranceRequestRequestTypeDef,
     ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
     DeleteSessionResponseTypeDef,
     PutSessionResponseTypeDef,
     RecognizeUtteranceResponseTypeDef,
     RuntimeHintDetailsOutputTypeDef,
     RuntimeHintDetailsTypeDef,
@@ -339,21 +340,23 @@
     SlotTypeDef,
     SessionStateOutputTypeDef,
     SessionStateTypeDef,
     MessageOutputTypeDef,
     MessageTypeDef,
     InterpretationTypeDef,
     RecognizeTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
+    SessionStateUnionTypeDef,
+    MessageUnionTypeDef,
     GetSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
+    PutSessionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt` & `mypy-boto3-lexv2-runtime-1.28.16/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.15.post1/setup.py` & `mypy-boto3-lexv2-runtime-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lexv2-runtime",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_lexv2_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexRuntimeV2 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.LexRuntimeV2 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 lexv2-runtime type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 lexv2-runtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_lexv2_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

