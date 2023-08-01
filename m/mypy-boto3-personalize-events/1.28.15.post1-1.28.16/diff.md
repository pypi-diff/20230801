# Comparing `tmp/mypy-boto3-personalize-events-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-personalize-events-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-events-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:51 2023, max compression
+gzip compressed data, was "mypy-boto3-personalize-events-1.28.16.tar", last modified: Tue Aug  1 11:37:31 2023, max compression
```

## Comparing `mypy-boto3-personalize-events-1.28.15.post1.tar` & `mypy-boto3-personalize-events-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:51.317330 mypy-boto3-personalize-events-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:00.000000 mypy-boto3-personalize-events-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-07-29 10:03:51.317330 mypy-boto3-personalize-events-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11049 2023-07-29 09:53:00.000000 mypy-boto3-personalize-events-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:51.309330 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-29 09:53:00.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-29 09:53:00.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-29 09:53:00.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-29 09:53:01.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-29 09:53:01.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-29 09:53:01.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-07-29 09:53:01.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:00.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-29 09:53:01.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-29 09:53:01.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:00.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:51.317330 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-07-29 10:03:51.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-29 10:03:51.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:51.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:51.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:51.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 10:03:51.000000 mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:51.317330 mypy-boto3-personalize-events-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 09:53:00.000000 mypy-boto3-personalize-events-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:31.168794 mypy-boto3-personalize-events-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-08-01 11:37:31.168794 mypy-boto3-personalize-events-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:31.156794 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-01 11:26:03.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:31.168794 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-08-01 11:37:30.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 11:37:30.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:30.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:30.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:30.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 11:37:30.000000 mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:31.168794 mypy-boto3-personalize-events-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-01 11:26:00.000000 mypy-boto3-personalize-events-1.28.16/setup.py
```

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/LICENSE` & `mypy-boto3-personalize-events-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/PKG-INFO` & `mypy-boto3-personalize-events-1.28.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-events
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PersonalizeEvents 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PersonalizeEvents 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 personalize-events type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 personalize-events type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-events)](https://pepy.tech/project/mypy-boto3-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeEvents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[boto3.PersonalizeEvents 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [mypy-boto3-personalize-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/).
 
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
@@ -287,36 +287,37 @@
 )
 
 
 def check_value(value: PersonalizeEventsServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_personalize_events.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_personalize_events.type_defs import (
     ResponseMetadataTypeDef,
     MetricAttributionTypeDef,
+    TimestampTypeDef,
     ItemTypeDef,
     UserTypeDef,
     EmptyResponseMetadataTypeDef,
     EventTypeDef,
     PutItemsRequestRequestTypeDef,
     PutUsersRequestRequestTypeDef,
     PutEventsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/README.md` & `mypy-boto3-personalize-events-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-events)](https://pepy.tech/project/mypy-boto3-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeEvents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[boto3.PersonalizeEvents 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [mypy-boto3-personalize-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/).
 
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
@@ -255,36 +255,37 @@
 )
 
 
 def check_value(value: PersonalizeEventsServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_personalize_events.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_personalize_events.type_defs import (
     ResponseMetadataTypeDef,
     MetricAttributionTypeDef,
+    TimestampTypeDef,
     ItemTypeDef,
     UserTypeDef,
     EmptyResponseMetadataTypeDef,
     EventTypeDef,
     PutItemsRequestRequestTypeDef,
     PutUsersRequestRequestTypeDef,
     PutEventsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/__main__.py` & `mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PersonalizeEvents 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.PersonalizeEvents 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents\nOther"
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

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/client.py` & `mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/client.pyi` & `mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/literals.py` & `mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/literals.pyi` & `mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/type_defs.py` & `mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_personalize_events.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Sequence, Union
 
 if sys.version_info >= (3, 9):
@@ -20,14 +20,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ResponseMetadataTypeDef",
     "MetricAttributionTypeDef",
+    "TimestampTypeDef",
     "ItemTypeDef",
     "UserTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "PutItemsRequestRequestTypeDef",
     "PutUsersRequestRequestTypeDef",
     "PutEventsRequestRequestTypeDef",
@@ -47,14 +48,15 @@
 MetricAttributionTypeDef = TypedDict(
     "MetricAttributionTypeDef",
     {
         "eventAttributionSource": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredItemTypeDef = TypedDict(
     "_RequiredItemTypeDef",
     {
         "itemId": str,
     },
 )
 _OptionalItemTypeDef = TypedDict(
@@ -96,15 +98,15 @@
     },
 )
 
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventType": str,
-        "sentAt": Union[datetime, str],
+        "sentAt": TimestampTypeDef,
     },
 )
 _OptionalEventTypeDef = TypedDict(
     "_OptionalEventTypeDef",
     {
         "eventId": str,
         "eventValue": float,
```

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events/type_defs.pyi` & `mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_personalize_events.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ResponseMetadataTypeDef",
     "MetricAttributionTypeDef",
+    "TimestampTypeDef",
     "ItemTypeDef",
     "UserTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "PutItemsRequestRequestTypeDef",
     "PutUsersRequestRequestTypeDef",
     "PutEventsRequestRequestTypeDef",
@@ -46,14 +47,15 @@
 MetricAttributionTypeDef = TypedDict(
     "MetricAttributionTypeDef",
     {
         "eventAttributionSource": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredItemTypeDef = TypedDict(
     "_RequiredItemTypeDef",
     {
         "itemId": str,
     },
 )
 _OptionalItemTypeDef = TypedDict(
@@ -91,15 +93,15 @@
     },
 )
 
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventType": str,
-        "sentAt": Union[datetime, str],
+        "sentAt": TimestampTypeDef,
     },
 )
 _OptionalEventTypeDef = TypedDict(
     "_OptionalEventTypeDef",
     {
         "eventId": str,
         "eventValue": float,
```

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events.egg-info/PKG-INFO` & `mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-events
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PersonalizeEvents 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PersonalizeEvents 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 personalize-events type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 personalize-events type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-events)](https://pepy.tech/project/mypy-boto3-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeEvents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[boto3.PersonalizeEvents 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [mypy-boto3-personalize-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/).
 
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
@@ -287,36 +287,37 @@
 )
 
 
 def check_value(value: PersonalizeEventsServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_personalize_events.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_personalize_events.type_defs import (
     ResponseMetadataTypeDef,
     MetricAttributionTypeDef,
+    TimestampTypeDef,
     ItemTypeDef,
     UserTypeDef,
     EmptyResponseMetadataTypeDef,
     EventTypeDef,
     PutItemsRequestRequestTypeDef,
     PutUsersRequestRequestTypeDef,
     PutEventsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/mypy_boto3_personalize_events.egg-info/SOURCES.txt` & `mypy-boto3-personalize-events-1.28.16/mypy_boto3_personalize_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.15.post1/setup.py` & `mypy-boto3-personalize-events-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize-events",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_personalize_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PersonalizeEvents 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.PersonalizeEvents 1.28.16 service generated with"
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
-    keywords="boto3 personalize-events type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 personalize-events type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_personalize_events": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/"
```

