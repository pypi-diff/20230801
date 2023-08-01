# Comparing `tmp/mypy-boto3-mwaa-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-mwaa-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mwaa-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:45 2023, max compression
+gzip compressed data, was "mypy-boto3-mwaa-1.28.16.tar", last modified: Tue Aug  1 11:37:25 2023, max compression
```

## Comparing `mypy-boto3-mwaa-1.28.15.post1.tar` & `mypy-boto3-mwaa-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:45.185304 mypy-boto3-mwaa-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-07-29 10:03:45.177304 mypy-boto3-mwaa-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:45.173304 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:45.177304 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:45.185304 mypy-boto3-mwaa-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-29 09:51:55.000000 mypy-boto3-mwaa-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:25.644808 mypy-boto3-mwaa-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-08-01 11:37:25.644808 mypy-boto3-mwaa-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:25.640808 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-08-01 11:24:54.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-08-01 11:24:54.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:25.644808 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-08-01 11:37:25.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-01 11:37:25.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:25.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:25.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:25.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 11:37:25.000000 mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:25.644808 mypy-boto3-mwaa-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-01 11:24:53.000000 mypy-boto3-mwaa-1.28.16/setup.py
```

### Comparing `mypy-boto3-mwaa-1.28.15.post1/LICENSE` & `mypy-boto3-mwaa-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15.post1/PKG-INFO` & `mypy-boto3-mwaa-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MWAA 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mwaa type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mwaa type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mwaa)](https://pepy.tech/project/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: EnvironmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mwaa.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     NetworkConfigurationTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
@@ -338,37 +338,39 @@
     UpdateErrorTypeDef,
     PaginatorConfigTypeDef,
     ListEnvironmentsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
+    TimestampTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
     CreateCliTokenResponseTypeDef,
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     LastUpdateTypeDef,
     ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
     GetEnvironmentOutputTypeDef,
 )
 
 
-def get_structure() -> CreateCliTokenRequestRequestTypeDef:
+def get_value() -> CreateCliTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mwaa-1.28.15.post1/README.md` & `mypy-boto3-mwaa-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mwaa)](https://pepy.tech/project/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
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
@@ -282,20 +282,20 @@
 )
 
 
 def check_value(value: EnvironmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mwaa.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     NetworkConfigurationTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
@@ -306,37 +306,39 @@
     UpdateErrorTypeDef,
     PaginatorConfigTypeDef,
     ListEnvironmentsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
+    TimestampTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
     CreateCliTokenResponseTypeDef,
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     LastUpdateTypeDef,
     ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
     GetEnvironmentOutputTypeDef,
 )
 
 
-def get_structure() -> CreateCliTokenRequestRequestTypeDef:
+def get_value() -> CreateCliTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__init__.py` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__init__.pyi` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/client.py` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,31 +10,30 @@
     from mypy_boto3_mwaa.client import MWAAClient
 
     session = Session()
     client: MWAAClient = session.client("mwaa")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import WebserverAccessModeType
 from .paginator import ListEnvironmentsPaginator
 from .type_defs import (
     CreateCliTokenResponseTypeDef,
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     GetEnvironmentOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationInputTypeDef,
     MetricDatumTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -103,15 +102,15 @@
 
     def create_environment(
         self,
         *,
         DagS3Path: str,
         ExecutionRoleArn: str,
         Name: str,
-        NetworkConfiguration: Union[NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef],
+        NetworkConfiguration: NetworkConfigurationUnionTypeDef,
         SourceBucketArn: str,
         AirflowConfigurationOptions: Mapping[str, str] = ...,
         AirflowVersion: str = ...,
         EnvironmentClass: str = ...,
         KmsKey: str = ...,
         LoggingConfiguration: LoggingConfigurationInputTypeDef = ...,
         MaxWorkers: int = ...,
```

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/client.pyi` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,31 +10,30 @@
     from mypy_boto3_mwaa.client import MWAAClient
 
     session = Session()
     client: MWAAClient = session.client("mwaa")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import WebserverAccessModeType
 from .paginator import ListEnvironmentsPaginator
 from .type_defs import (
     CreateCliTokenResponseTypeDef,
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     GetEnvironmentOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationInputTypeDef,
     MetricDatumTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -95,15 +94,15 @@
         """
     def create_environment(
         self,
         *,
         DagS3Path: str,
         ExecutionRoleArn: str,
         Name: str,
-        NetworkConfiguration: Union[NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef],
+        NetworkConfiguration: NetworkConfigurationUnionTypeDef,
         SourceBucketArn: str,
         AirflowConfigurationOptions: Mapping[str, str] = ...,
         AirflowVersion: str = ...,
         EnvironmentClass: str = ...,
         KmsKey: str = ...,
         LoggingConfiguration: LoggingConfigurationInputTypeDef = ...,
         MaxWorkers: int = ...,
```

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/literals.py` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/literals.pyi` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/paginator.py` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/paginator.pyi` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/type_defs.py` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mwaa.type_defs import CreateCliTokenRequestRequestTypeDef
 
-    data: CreateCliTokenRequestRequestTypeDef = {...}
+    data: CreateCliTokenRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -41,23 +41,25 @@
     "UpdateErrorTypeDef",
     "PaginatorConfigTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
     "StatisticSetTypeDef",
+    "TimestampTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateNetworkConfigurationInputTypeDef",
     "CreateCliTokenResponseTypeDef",
     "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenResponseTypeDef",
     "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "LastUpdateTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
@@ -191,14 +193,15 @@
         "Minimum": float,
         "SampleCount": int,
         "Sum": float,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -265,14 +268,17 @@
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
@@ -312,15 +318,15 @@
     total=False,
 )
 
 _RequiredMetricDatumTypeDef = TypedDict(
     "_RequiredMetricDatumTypeDef",
     {
         "MetricName": str,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
     "_OptionalMetricDatumTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
         "StatisticValues": StatisticSetTypeDef,
```

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/type_defs.pyi` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mwaa.type_defs import CreateCliTokenRequestRequestTypeDef
 
-    data: CreateCliTokenRequestRequestTypeDef = {...}
+    data: CreateCliTokenRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -40,23 +40,25 @@
     "UpdateErrorTypeDef",
     "PaginatorConfigTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
     "StatisticSetTypeDef",
+    "TimestampTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateNetworkConfigurationInputTypeDef",
     "CreateCliTokenResponseTypeDef",
     "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenResponseTypeDef",
     "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "LastUpdateTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
@@ -190,14 +192,15 @@
         "Minimum": float,
         "SampleCount": int,
         "Sum": float,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -264,14 +267,17 @@
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
@@ -311,15 +317,15 @@
     total=False,
 )
 
 _RequiredMetricDatumTypeDef = TypedDict(
     "_RequiredMetricDatumTypeDef",
     {
         "MetricName": str,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
     "_OptionalMetricDatumTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
         "StatisticValues": StatisticSetTypeDef,
```

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/PKG-INFO` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MWAA 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mwaa type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mwaa type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mwaa)](https://pepy.tech/project/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: EnvironmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mwaa.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     NetworkConfigurationTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
@@ -338,37 +338,39 @@
     UpdateErrorTypeDef,
     PaginatorConfigTypeDef,
     ListEnvironmentsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
+    TimestampTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
     CreateCliTokenResponseTypeDef,
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     LastUpdateTypeDef,
     ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
     GetEnvironmentOutputTypeDef,
 )
 
 
-def get_structure() -> CreateCliTokenRequestRequestTypeDef:
+def get_value() -> CreateCliTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/SOURCES.txt` & `mypy-boto3-mwaa-1.28.16/mypy_boto3_mwaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15.post1/setup.py` & `mypy-boto3-mwaa-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mwaa",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_mwaa"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MWAA 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 mwaa type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 mwaa type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mwaa": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

