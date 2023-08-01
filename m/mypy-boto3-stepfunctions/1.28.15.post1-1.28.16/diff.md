# Comparing `tmp/mypy-boto3-stepfunctions-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-stepfunctions-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-stepfunctions-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:18 2023, max compression
+gzip compressed data, was "mypy-boto3-stepfunctions-1.28.16.tar", last modified: Tue Aug  1 11:37:58 2023, max compression
```

## Comparing `mypy-boto3-stepfunctions-1.28.15.post1.tar` & `mypy-boto3-stepfunctions-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:18.989431 mypy-boto3-stepfunctions-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-07-29 10:04:18.981431 mypy-boto3-stepfunctions-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:18.977431 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28552 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28506 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44183 2023-07-29 10:00:30.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44118 2023-07-29 10:00:29.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:18.981431 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:18.989431 mypy-boto3-stepfunctions-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:58.320713 mypy-boto3-stepfunctions-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:03.000000 mypy-boto3-stepfunctions-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18207 2023-08-01 11:37:58.320713 mypy-boto3-stepfunctions-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-08-01 11:34:03.000000 mypy-boto3-stepfunctions-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:58.320713 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-01 11:34:04.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-01 11:34:03.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:34:04.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28393 2023-08-01 11:34:04.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28347 2023-08-01 11:34:04.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-08-01 11:34:04.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-08-01 11:34:04.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-08-01 11:34:04.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-08-01 11:34:04.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:04.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44339 2023-08-01 11:34:05.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44274 2023-08-01 11:34:05.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:03.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:58.320713 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18207 2023-08-01 11:37:58.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-01 11:37:58.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:58.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:58.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:58.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:37:58.000000 mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:58.320713 mypy-boto3-stepfunctions-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:33:59.000000 mypy-boto3-stepfunctions-1.28.16/setup.py
```

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/LICENSE` & `mypy-boto3-stepfunctions-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/PKG-INFO` & `mypy-boto3-stepfunctions-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SFN 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 stepfunctions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 stepfunctions type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -335,20 +335,20 @@
 )
 
 
 def check_value(value: ExecutionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_stepfunctions.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_stepfunctions.type_defs import (
     ActivityFailedEventDetailsTypeDef,
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
@@ -458,20 +458,21 @@
     ListStateMachinesOutputTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     CreateStateMachineInputRequestTypeDef,
+    LoggingConfigurationUnionTypeDef,
     UpdateStateMachineInputRequestTypeDef,
     GetExecutionHistoryOutputTypeDef,
 )
 
 
-def get_structure() -> ActivityFailedEventDetailsTypeDef:
+def get_value() -> ActivityFailedEventDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/README.md` & `mypy-boto3-stepfunctions-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -303,20 +303,20 @@
 )
 
 
 def check_value(value: ExecutionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_stepfunctions.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_stepfunctions.type_defs import (
     ActivityFailedEventDetailsTypeDef,
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
@@ -426,20 +426,21 @@
     ListStateMachinesOutputTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     CreateStateMachineInputRequestTypeDef,
+    LoggingConfigurationUnionTypeDef,
     UpdateStateMachineInputRequestTypeDef,
     GetExecutionHistoryOutputTypeDef,
 )
 
 
-def get_structure() -> ActivityFailedEventDetailsTypeDef:
+def get_value() -> ActivityFailedEventDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__init__.py` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__init__.pyi` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__main__.py` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SFN 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.SFN 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
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

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/client.py` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_stepfunctions.client import SFNClient
 
     session = Session()
     client: SFNClient = session.client("stepfunctions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ExecutionStatusType, StateMachineTypeType
 from .paginator import (
     GetExecutionHistoryPaginator,
     ListActivitiesPaginator,
@@ -41,16 +41,15 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
@@ -152,17 +151,15 @@
     def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: Union[
-            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-        ] = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
@@ -510,17 +507,15 @@
 
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: Union[
-            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-        ] = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
```

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/client.pyi` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_stepfunctions.client import SFNClient
 
     session = Session()
     client: SFNClient = session.client("stepfunctions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ExecutionStatusType, StateMachineTypeType
 from .paginator import (
     GetExecutionHistoryPaginator,
     ListActivitiesPaginator,
@@ -41,16 +41,15 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
@@ -144,17 +143,15 @@
     def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: Union[
-            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-        ] = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
@@ -470,17 +467,15 @@
         """
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: Union[
-            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-        ] = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
```

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/literals.py` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/literals.pyi` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/paginator.py` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/paginator.pyi` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/type_defs.py` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_stepfunctions.type_defs import ActivityFailedEventDetailsTypeDef
 
-    data: ActivityFailedEventDetailsTypeDef = {...}
+    data: ActivityFailedEventDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ExecutionStatusType,
     HistoryEventTypeType,
     LogLevelType,
     MapRunStatusType,
     StateMachineStatusType,
@@ -142,14 +142,15 @@
     "ListStateMachinesOutputTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
     "CreateStateMachineInputRequestTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -1684,14 +1685,17 @@
 
 class CreateStateMachineInputRequestTypeDef(
     _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
 ):
     pass
 
 
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/type_defs.pyi` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_stepfunctions.type_defs import ActivityFailedEventDetailsTypeDef
 
-    data: ActivityFailedEventDetailsTypeDef = {...}
+    data: ActivityFailedEventDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ExecutionStatusType,
     HistoryEventTypeType,
     LogLevelType,
     MapRunStatusType,
     StateMachineStatusType,
@@ -141,14 +141,15 @@
     "ListStateMachinesOutputTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
     "CreateStateMachineInputRequestTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -1621,14 +1622,17 @@
 )
 
 class CreateStateMachineInputRequestTypeDef(
     _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
 ):
     pass
 
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/PKG-INFO` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SFN 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 stepfunctions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 stepfunctions type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -335,20 +335,20 @@
 )
 
 
 def check_value(value: ExecutionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_stepfunctions.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_stepfunctions.type_defs import (
     ActivityFailedEventDetailsTypeDef,
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
@@ -458,20 +458,21 @@
     ListStateMachinesOutputTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     CreateStateMachineInputRequestTypeDef,
+    LoggingConfigurationUnionTypeDef,
     UpdateStateMachineInputRequestTypeDef,
     GetExecutionHistoryOutputTypeDef,
 )
 
 
-def get_structure() -> ActivityFailedEventDetailsTypeDef:
+def get_value() -> ActivityFailedEventDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/SOURCES.txt` & `mypy-boto3-stepfunctions-1.28.16/mypy_boto3_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15.post1/setup.py` & `mypy-boto3-stepfunctions-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-stepfunctions",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SFN 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 stepfunctions type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 stepfunctions type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_stepfunctions": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

