# Comparing `tmp/mypy-boto3-qldb-session-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-qldb-session-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qldb-session-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:56 2023, max compression
+gzip compressed data, was "mypy-boto3-qldb-session-1.28.16.tar", last modified: Tue Aug  1 11:37:36 2023, max compression
```

## Comparing `mypy-boto3-qldb-session-1.28.15.post1.tar` & `mypy-boto3-qldb-session-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:56.317349 mypy-boto3-qldb-session-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-29 10:03:56.317349 mypy-boto3-qldb-session-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:56.305349 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:56.317349 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-29 10:03:56.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:03:56.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:56.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:56.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:56.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:56.000000 mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:56.317349 mypy-boto3-qldb-session-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-29 09:53:41.000000 mypy-boto3-qldb-session-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:36.820780 mypy-boto3-qldb-session-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-08-01 11:37:36.820780 mypy-boto3-qldb-session-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:36.820780 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-08-01 11:26:45.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:36.820780 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-08-01 11:37:36.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 11:37:36.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:36.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:36.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:36.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:37:36.000000 mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:36.820780 mypy-boto3-qldb-session-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:26:44.000000 mypy-boto3-qldb-session-1.28.16/setup.py
```

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/LICENSE` & `mypy-boto3-qldb-session-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/PKG-INFO` & `mypy-boto3-qldb-session-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb-session
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.QLDBSession 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.QLDBSession 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 qldb-session type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 qldb-session type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb-session)](https://pepy.tech/project/mypy-boto3-qldb-session)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDBSession 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
+[boto3.QLDBSession 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
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
 [mypy-boto3-qldb-session docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/).
 
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
@@ -287,46 +287,47 @@
 )
 
 
 def check_value(value: QLDBSessionServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_qldb_session.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_qldb_session.type_defs import (
     TimingInformationTypeDef,
-    CommitTransactionRequestTypeDef,
+    BlobTypeDef,
     IOUsageTypeDef,
-    ValueHolderTypeDef,
     FetchPageRequestTypeDef,
     ValueHolderOutputTypeDef,
     ResponseMetadataTypeDef,
     StartSessionRequestTypeDef,
     AbortTransactionResultTypeDef,
     EndSessionResultTypeDef,
     StartSessionResultTypeDef,
     StartTransactionResultTypeDef,
+    CommitTransactionRequestTypeDef,
+    ValueHolderTypeDef,
     CommitTransactionResultTypeDef,
-    ExecuteStatementRequestTypeDef,
     PageTypeDef,
-    SendCommandRequestRequestTypeDef,
+    ExecuteStatementRequestTypeDef,
     ExecuteStatementResultTypeDef,
     FetchPageResultTypeDef,
+    SendCommandRequestRequestTypeDef,
     SendCommandResultTypeDef,
 )
 
 
-def get_structure() -> TimingInformationTypeDef:
+def get_value() -> TimingInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/README.md` & `mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-qldb-session
+Version: 1.28.16
+Summary: Type annotations for boto3.QLDBSession 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 qldb-session type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-qldb-session"></a>
 
 # mypy-boto3-qldb-session
 
 [![PyPI - mypy-boto3-qldb-session](https://img.shields.io/pypi/v/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb-session)](https://pepy.tech/project/mypy-boto3-qldb-session)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDBSession 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
+[boto3.QLDBSession 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
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
 [mypy-boto3-qldb-session docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
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
@@ -255,46 +287,47 @@
 )
 
 
 def check_value(value: QLDBSessionServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_qldb_session.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_qldb_session.type_defs import (
     TimingInformationTypeDef,
-    CommitTransactionRequestTypeDef,
+    BlobTypeDef,
     IOUsageTypeDef,
-    ValueHolderTypeDef,
     FetchPageRequestTypeDef,
     ValueHolderOutputTypeDef,
     ResponseMetadataTypeDef,
     StartSessionRequestTypeDef,
     AbortTransactionResultTypeDef,
     EndSessionResultTypeDef,
     StartSessionResultTypeDef,
     StartTransactionResultTypeDef,
+    CommitTransactionRequestTypeDef,
+    ValueHolderTypeDef,
     CommitTransactionResultTypeDef,
-    ExecuteStatementRequestTypeDef,
     PageTypeDef,
-    SendCommandRequestRequestTypeDef,
+    ExecuteStatementRequestTypeDef,
     ExecuteStatementResultTypeDef,
     FetchPageResultTypeDef,
+    SendCommandRequestRequestTypeDef,
     SendCommandResultTypeDef,
 )
 
 
-def get_structure() -> TimingInformationTypeDef:
+def get_value() -> TimingInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/__main__.py` & `mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QLDBSession 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.QLDBSession 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession\nOther"
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

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/client.py` & `mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/client.pyi` & `mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/literals.py` & `mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/literals.pyi` & `mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/type_defs.py` & `mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_qldb_session.type_defs import TimingInformationTypeDef
 
-    data: TimingInformationTypeDef = {...}
+    data: TimingInformationTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -20,68 +20,53 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TimingInformationTypeDef",
-    "CommitTransactionRequestTypeDef",
+    "BlobTypeDef",
     "IOUsageTypeDef",
-    "ValueHolderTypeDef",
     "FetchPageRequestTypeDef",
     "ValueHolderOutputTypeDef",
     "ResponseMetadataTypeDef",
     "StartSessionRequestTypeDef",
     "AbortTransactionResultTypeDef",
     "EndSessionResultTypeDef",
     "StartSessionResultTypeDef",
     "StartTransactionResultTypeDef",
+    "CommitTransactionRequestTypeDef",
+    "ValueHolderTypeDef",
     "CommitTransactionResultTypeDef",
-    "ExecuteStatementRequestTypeDef",
     "PageTypeDef",
-    "SendCommandRequestRequestTypeDef",
+    "ExecuteStatementRequestTypeDef",
     "ExecuteStatementResultTypeDef",
     "FetchPageResultTypeDef",
+    "SendCommandRequestRequestTypeDef",
     "SendCommandResultTypeDef",
 )
 
 TimingInformationTypeDef = TypedDict(
     "TimingInformationTypeDef",
     {
         "ProcessingTimeMilliseconds": int,
     },
     total=False,
 )
 
-CommitTransactionRequestTypeDef = TypedDict(
-    "CommitTransactionRequestTypeDef",
-    {
-        "TransactionId": str,
-        "CommitDigest": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 IOUsageTypeDef = TypedDict(
     "IOUsageTypeDef",
     {
         "ReadIOs": int,
         "WriteIOs": int,
     },
     total=False,
 )
 
-ValueHolderTypeDef = TypedDict(
-    "ValueHolderTypeDef",
-    {
-        "IonBinary": Union[str, bytes, IO[Any], StreamingBody],
-        "IonText": str,
-    },
-    total=False,
-)
-
 FetchPageRequestTypeDef = TypedDict(
     "FetchPageRequestTypeDef",
     {
         "TransactionId": str,
         "NextPageToken": str,
     },
 )
@@ -143,25 +128,51 @@
     {
         "TransactionId": str,
         "TimingInformation": TimingInformationTypeDef,
     },
     total=False,
 )
 
+CommitTransactionRequestTypeDef = TypedDict(
+    "CommitTransactionRequestTypeDef",
+    {
+        "TransactionId": str,
+        "CommitDigest": BlobTypeDef,
+    },
+)
+
+ValueHolderTypeDef = TypedDict(
+    "ValueHolderTypeDef",
+    {
+        "IonBinary": BlobTypeDef,
+        "IonText": str,
+    },
+    total=False,
+)
+
 CommitTransactionResultTypeDef = TypedDict(
     "CommitTransactionResultTypeDef",
     {
         "TransactionId": str,
         "CommitDigest": bytes,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
     },
     total=False,
 )
 
+PageTypeDef = TypedDict(
+    "PageTypeDef",
+    {
+        "Values": List[ValueHolderOutputTypeDef],
+        "NextPageToken": str,
+    },
+    total=False,
+)
+
 _RequiredExecuteStatementRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementRequestTypeDef",
     {
         "TransactionId": str,
         "Statement": str,
     },
 )
@@ -176,38 +187,14 @@
 
 class ExecuteStatementRequestTypeDef(
     _RequiredExecuteStatementRequestTypeDef, _OptionalExecuteStatementRequestTypeDef
 ):
     pass
 
 
-PageTypeDef = TypedDict(
-    "PageTypeDef",
-    {
-        "Values": List[ValueHolderOutputTypeDef],
-        "NextPageToken": str,
-    },
-    total=False,
-)
-
-SendCommandRequestRequestTypeDef = TypedDict(
-    "SendCommandRequestRequestTypeDef",
-    {
-        "SessionToken": str,
-        "StartSession": StartSessionRequestTypeDef,
-        "StartTransaction": Mapping[str, Any],
-        "EndSession": Mapping[str, Any],
-        "CommitTransaction": CommitTransactionRequestTypeDef,
-        "AbortTransaction": Mapping[str, Any],
-        "ExecuteStatement": ExecuteStatementRequestTypeDef,
-        "FetchPage": FetchPageRequestTypeDef,
-    },
-    total=False,
-)
-
 ExecuteStatementResultTypeDef = TypedDict(
     "ExecuteStatementResultTypeDef",
     {
         "FirstPage": PageTypeDef,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
     },
@@ -220,14 +207,29 @@
         "Page": PageTypeDef,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
     },
     total=False,
 )
 
+SendCommandRequestRequestTypeDef = TypedDict(
+    "SendCommandRequestRequestTypeDef",
+    {
+        "SessionToken": str,
+        "StartSession": StartSessionRequestTypeDef,
+        "StartTransaction": Mapping[str, Any],
+        "EndSession": Mapping[str, Any],
+        "CommitTransaction": CommitTransactionRequestTypeDef,
+        "AbortTransaction": Mapping[str, Any],
+        "ExecuteStatement": ExecuteStatementRequestTypeDef,
+        "FetchPage": FetchPageRequestTypeDef,
+    },
+    total=False,
+)
+
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "StartSession": StartSessionResultTypeDef,
         "StartTransaction": StartTransactionResultTypeDef,
         "EndSession": EndSessionResultTypeDef,
         "CommitTransaction": CommitTransactionResultTypeDef,
```

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session/type_defs.pyi` & `mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,83 +4,68 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_qldb_session.type_defs import TimingInformationTypeDef
 
-    data: TimingInformationTypeDef = {...}
+    data: TimingInformationTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TimingInformationTypeDef",
-    "CommitTransactionRequestTypeDef",
+    "BlobTypeDef",
     "IOUsageTypeDef",
-    "ValueHolderTypeDef",
     "FetchPageRequestTypeDef",
     "ValueHolderOutputTypeDef",
     "ResponseMetadataTypeDef",
     "StartSessionRequestTypeDef",
     "AbortTransactionResultTypeDef",
     "EndSessionResultTypeDef",
     "StartSessionResultTypeDef",
     "StartTransactionResultTypeDef",
+    "CommitTransactionRequestTypeDef",
+    "ValueHolderTypeDef",
     "CommitTransactionResultTypeDef",
-    "ExecuteStatementRequestTypeDef",
     "PageTypeDef",
-    "SendCommandRequestRequestTypeDef",
+    "ExecuteStatementRequestTypeDef",
     "ExecuteStatementResultTypeDef",
     "FetchPageResultTypeDef",
+    "SendCommandRequestRequestTypeDef",
     "SendCommandResultTypeDef",
 )
 
 TimingInformationTypeDef = TypedDict(
     "TimingInformationTypeDef",
     {
         "ProcessingTimeMilliseconds": int,
     },
     total=False,
 )
 
-CommitTransactionRequestTypeDef = TypedDict(
-    "CommitTransactionRequestTypeDef",
-    {
-        "TransactionId": str,
-        "CommitDigest": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 IOUsageTypeDef = TypedDict(
     "IOUsageTypeDef",
     {
         "ReadIOs": int,
         "WriteIOs": int,
     },
     total=False,
 )
 
-ValueHolderTypeDef = TypedDict(
-    "ValueHolderTypeDef",
-    {
-        "IonBinary": Union[str, bytes, IO[Any], StreamingBody],
-        "IonText": str,
-    },
-    total=False,
-)
-
 FetchPageRequestTypeDef = TypedDict(
     "FetchPageRequestTypeDef",
     {
         "TransactionId": str,
         "NextPageToken": str,
     },
 )
@@ -142,25 +127,51 @@
     {
         "TransactionId": str,
         "TimingInformation": TimingInformationTypeDef,
     },
     total=False,
 )
 
+CommitTransactionRequestTypeDef = TypedDict(
+    "CommitTransactionRequestTypeDef",
+    {
+        "TransactionId": str,
+        "CommitDigest": BlobTypeDef,
+    },
+)
+
+ValueHolderTypeDef = TypedDict(
+    "ValueHolderTypeDef",
+    {
+        "IonBinary": BlobTypeDef,
+        "IonText": str,
+    },
+    total=False,
+)
+
 CommitTransactionResultTypeDef = TypedDict(
     "CommitTransactionResultTypeDef",
     {
         "TransactionId": str,
         "CommitDigest": bytes,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
     },
     total=False,
 )
 
+PageTypeDef = TypedDict(
+    "PageTypeDef",
+    {
+        "Values": List[ValueHolderOutputTypeDef],
+        "NextPageToken": str,
+    },
+    total=False,
+)
+
 _RequiredExecuteStatementRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementRequestTypeDef",
     {
         "TransactionId": str,
         "Statement": str,
     },
 )
@@ -173,38 +184,14 @@
 )
 
 class ExecuteStatementRequestTypeDef(
     _RequiredExecuteStatementRequestTypeDef, _OptionalExecuteStatementRequestTypeDef
 ):
     pass
 
-PageTypeDef = TypedDict(
-    "PageTypeDef",
-    {
-        "Values": List[ValueHolderOutputTypeDef],
-        "NextPageToken": str,
-    },
-    total=False,
-)
-
-SendCommandRequestRequestTypeDef = TypedDict(
-    "SendCommandRequestRequestTypeDef",
-    {
-        "SessionToken": str,
-        "StartSession": StartSessionRequestTypeDef,
-        "StartTransaction": Mapping[str, Any],
-        "EndSession": Mapping[str, Any],
-        "CommitTransaction": CommitTransactionRequestTypeDef,
-        "AbortTransaction": Mapping[str, Any],
-        "ExecuteStatement": ExecuteStatementRequestTypeDef,
-        "FetchPage": FetchPageRequestTypeDef,
-    },
-    total=False,
-)
-
 ExecuteStatementResultTypeDef = TypedDict(
     "ExecuteStatementResultTypeDef",
     {
         "FirstPage": PageTypeDef,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
     },
@@ -217,14 +204,29 @@
         "Page": PageTypeDef,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
     },
     total=False,
 )
 
+SendCommandRequestRequestTypeDef = TypedDict(
+    "SendCommandRequestRequestTypeDef",
+    {
+        "SessionToken": str,
+        "StartSession": StartSessionRequestTypeDef,
+        "StartTransaction": Mapping[str, Any],
+        "EndSession": Mapping[str, Any],
+        "CommitTransaction": CommitTransactionRequestTypeDef,
+        "AbortTransaction": Mapping[str, Any],
+        "ExecuteStatement": ExecuteStatementRequestTypeDef,
+        "FetchPage": FetchPageRequestTypeDef,
+    },
+    total=False,
+)
+
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "StartSession": StartSessionResultTypeDef,
         "StartTransaction": StartTransactionResultTypeDef,
         "EndSession": EndSessionResultTypeDef,
         "CommitTransaction": CommitTransactionResultTypeDef,
```

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session.egg-info/PKG-INFO` & `mypy-boto3-qldb-session-1.28.16/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-qldb-session
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.QLDBSession 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 qldb-session type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-qldb-session"></a>
 
 # mypy-boto3-qldb-session
 
 [![PyPI - mypy-boto3-qldb-session](https://img.shields.io/pypi/v/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb-session)](https://pepy.tech/project/mypy-boto3-qldb-session)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDBSession 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
+[boto3.QLDBSession 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
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
 [mypy-boto3-qldb-session docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +41,15 @@
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
@@ -287,46 +255,47 @@
 )
 
 
 def check_value(value: QLDBSessionServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_qldb_session.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_qldb_session.type_defs import (
     TimingInformationTypeDef,
-    CommitTransactionRequestTypeDef,
+    BlobTypeDef,
     IOUsageTypeDef,
-    ValueHolderTypeDef,
     FetchPageRequestTypeDef,
     ValueHolderOutputTypeDef,
     ResponseMetadataTypeDef,
     StartSessionRequestTypeDef,
     AbortTransactionResultTypeDef,
     EndSessionResultTypeDef,
     StartSessionResultTypeDef,
     StartTransactionResultTypeDef,
+    CommitTransactionRequestTypeDef,
+    ValueHolderTypeDef,
     CommitTransactionResultTypeDef,
-    ExecuteStatementRequestTypeDef,
     PageTypeDef,
-    SendCommandRequestRequestTypeDef,
+    ExecuteStatementRequestTypeDef,
     ExecuteStatementResultTypeDef,
     FetchPageResultTypeDef,
+    SendCommandRequestRequestTypeDef,
     SendCommandResultTypeDef,
 )
 
 
-def get_structure() -> TimingInformationTypeDef:
+def get_value() -> TimingInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/mypy_boto3_qldb_session.egg-info/SOURCES.txt` & `mypy-boto3-qldb-session-1.28.16/mypy_boto3_qldb_session.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.15.post1/setup.py` & `mypy-boto3-qldb-session-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qldb-session",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_qldb_session"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QLDBSession 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.QLDBSession 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 qldb-session type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 qldb-session type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_qldb_session": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

