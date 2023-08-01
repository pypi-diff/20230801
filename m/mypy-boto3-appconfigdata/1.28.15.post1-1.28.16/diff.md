# Comparing `tmp/mypy-boto3-appconfigdata-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-appconfigdata-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appconfigdata-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:27 2023, max compression
+gzip compressed data, was "mypy-boto3-appconfigdata-1.28.16.tar", last modified: Tue Aug  1 11:36:08 2023, max compression
```

## Comparing `mypy-boto3-appconfigdata-1.28.15.post1.tar` & `mypy-boto3-appconfigdata-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.712993 mypy-boto3-appconfigdata-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-07-29 10:02:27.712993 mypy-boto3-appconfigdata-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.708993 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-29 09:38:05.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-29 09:38:05.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-29 09:38:05.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.712993 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-07-29 10:02:27.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-29 10:02:27.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:27.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:02:27.000000 mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:27.712993 mypy-boto3-appconfigdata-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-29 09:38:04.000000 mypy-boto3-appconfigdata-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.500956 mypy-boto3-appconfigdata-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-08-01 11:36:08.496955 mypy-boto3-appconfigdata-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.496955 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.496955 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-08-01 11:36:08.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 11:36:08.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:08.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:36:08.000000 mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:08.500956 mypy-boto3-appconfigdata-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 11:10:35.000000 mypy-boto3-appconfigdata-1.28.16/setup.py
```

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/LICENSE` & `mypy-boto3-appconfigdata-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/PKG-INFO` & `mypy-boto3-appconfigdata-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfigdata
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppConfigData 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppConfigData 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appconfigdata type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appconfigdata type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfigdata.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfigdata)](https://pepy.tech/project/mypy-boto3-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfigData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[boto3.AppConfigData 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
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
 [mypy-boto3-appconfigdata docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/).
 
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
@@ -287,32 +287,32 @@
 )
 
 
 def check_value(value: AppConfigDataServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appconfigdata.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appconfigdata.type_defs import (
     GetLatestConfigurationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StartConfigurationSessionRequestRequestTypeDef,
     GetLatestConfigurationResponseTypeDef,
     StartConfigurationSessionResponseTypeDef,
 )
 
 
-def get_structure() -> GetLatestConfigurationRequestRequestTypeDef:
+def get_value() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/README.md` & `mypy-boto3-appconfigdata-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfigdata.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfigdata)](https://pepy.tech/project/mypy-boto3-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfigData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[boto3.AppConfigData 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
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
 [mypy-boto3-appconfigdata docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/).
 
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
@@ -255,32 +255,32 @@
 )
 
 
 def check_value(value: AppConfigDataServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appconfigdata.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appconfigdata.type_defs import (
     GetLatestConfigurationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StartConfigurationSessionRequestRequestTypeDef,
     GetLatestConfigurationResponseTypeDef,
     StartConfigurationSessionResponseTypeDef,
 )
 
 
-def get_structure() -> GetLatestConfigurationRequestRequestTypeDef:
+def get_value() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/__main__.py` & `mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppConfigData 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AppConfigData 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData\nOther"
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

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/client.py` & `mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/client.pyi` & `mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/literals.py` & `mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/literals.pyi` & `mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/type_defs.py` & `mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appconfigdata.type_defs import GetLatestConfigurationRequestRequestTypeDef
 
-    data: GetLatestConfigurationRequestRequestTypeDef = {...}
+    data: GetLatestConfigurationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "GetLatestConfigurationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StartConfigurationSessionRequestRequestTypeDef",
     "GetLatestConfigurationResponseTypeDef",
     "StartConfigurationSessionResponseTypeDef",
 )
@@ -60,22 +59,20 @@
     "_OptionalStartConfigurationSessionRequestRequestTypeDef",
     {
         "RequiredMinimumPollIntervalInSeconds": int,
     },
     total=False,
 )
 
-
 class StartConfigurationSessionRequestRequestTypeDef(
     _RequiredStartConfigurationSessionRequestRequestTypeDef,
     _OptionalStartConfigurationSessionRequestRequestTypeDef,
 ):
     pass
 
-
 GetLatestConfigurationResponseTypeDef = TypedDict(
     "GetLatestConfigurationResponseTypeDef",
     {
         "NextPollConfigurationToken": str,
         "NextPollIntervalInSeconds": int,
         "ContentType": str,
         "Configuration": StreamingBody,
```

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata/type_defs.pyi` & `mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appconfigdata.type_defs import GetLatestConfigurationRequestRequestTypeDef
 
-    data: GetLatestConfigurationRequestRequestTypeDef = {...}
+    data: GetLatestConfigurationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "GetLatestConfigurationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StartConfigurationSessionRequestRequestTypeDef",
     "GetLatestConfigurationResponseTypeDef",
     "StartConfigurationSessionResponseTypeDef",
 )
@@ -59,20 +60,22 @@
     "_OptionalStartConfigurationSessionRequestRequestTypeDef",
     {
         "RequiredMinimumPollIntervalInSeconds": int,
     },
     total=False,
 )
 
+
 class StartConfigurationSessionRequestRequestTypeDef(
     _RequiredStartConfigurationSessionRequestRequestTypeDef,
     _OptionalStartConfigurationSessionRequestRequestTypeDef,
 ):
     pass
 
+
 GetLatestConfigurationResponseTypeDef = TypedDict(
     "GetLatestConfigurationResponseTypeDef",
     {
         "NextPollConfigurationToken": str,
         "NextPollIntervalInSeconds": int,
         "ContentType": str,
         "Configuration": StreamingBody,
```

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata.egg-info/PKG-INFO` & `mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfigdata
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppConfigData 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppConfigData 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appconfigdata type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appconfigdata type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfigdata.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfigdata)](https://pepy.tech/project/mypy-boto3-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfigData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[boto3.AppConfigData 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
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
 [mypy-boto3-appconfigdata docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/).
 
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
@@ -287,32 +287,32 @@
 )
 
 
 def check_value(value: AppConfigDataServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appconfigdata.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appconfigdata.type_defs import (
     GetLatestConfigurationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StartConfigurationSessionRequestRequestTypeDef,
     GetLatestConfigurationResponseTypeDef,
     StartConfigurationSessionResponseTypeDef,
 )
 
 
-def get_structure() -> GetLatestConfigurationRequestRequestTypeDef:
+def get_value() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/mypy_boto3_appconfigdata.egg-info/SOURCES.txt` & `mypy-boto3-appconfigdata-1.28.16/mypy_boto3_appconfigdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.15.post1/setup.py` & `mypy-boto3-appconfigdata-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appconfigdata",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_appconfigdata"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppConfigData 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.AppConfigData 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 appconfigdata type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 appconfigdata type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_appconfigdata": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

