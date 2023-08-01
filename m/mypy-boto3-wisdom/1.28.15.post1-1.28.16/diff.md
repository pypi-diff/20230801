# Comparing `tmp/mypy-boto3-wisdom-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-wisdom-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wisdom-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:26 2023, max compression
+gzip compressed data, was "mypy-boto3-wisdom-1.28.16.tar", last modified: Tue Aug  1 11:38:05 2023, max compression
```

## Comparing `mypy-boto3-wisdom-1.28.15.post1.tar` & `mypy-boto3-wisdom-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.117458 mypy-boto3-wisdom-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-07-29 10:04:26.117458 mypy-boto3-wisdom-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.109458 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25143 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25098 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-29 10:01:39.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-29 10:01:39.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-07-29 10:01:40.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-07-29 10:01:39.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.117458 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:26.117458 mypy-boto3-wisdom-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.112660 mypy-boto3-wisdom-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-08-01 11:38:05.112660 mypy-boto3-wisdom-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.112660 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25000 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37165 2023-08-01 11:35:20.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-08-01 11:35:20.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:35:19.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.112660 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-08-01 11:38:04.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 11:38:04.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:04.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:04.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:04.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:38:04.000000 mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:05.112660 mypy-boto3-wisdom-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:35:18.000000 mypy-boto3-wisdom-1.28.16/setup.py
```

### Comparing `mypy-boto3-wisdom-1.28.15.post1/LICENSE` & `mypy-boto3-wisdom-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15.post1/PKG-INFO` & `mypy-boto3-wisdom-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 wisdom type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 wisdom type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wisdom)](https://pepy.tech/project/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
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
@@ -345,20 +345,20 @@
 )
 
 
 def check_value(value: AssistantStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_wisdom.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_wisdom.type_defs import (
     AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
@@ -427,14 +427,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
     SessionDataTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
     CreateKnowledgeBaseRequestRequestTypeDef,
+    SourceConfigurationUnionTypeDef,
     AssistantAssociationDataTypeDef,
     AssistantAssociationSummaryTypeDef,
     CreateAssistantResponseTypeDef,
     GetAssistantResponseTypeDef,
     ListAssistantsResponseTypeDef,
     DocumentTypeDef,
     SearchContentRequestRequestTypeDef,
@@ -454,15 +455,15 @@
     RecommendationDataTypeDef,
     ResultDataTypeDef,
     GetRecommendationsResponseTypeDef,
     QueryAssistantResponseTypeDef,
 )
 
 
-def get_structure() -> AppIntegrationsConfigurationOutputTypeDef:
+def get_value() -> AppIntegrationsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wisdom-1.28.15.post1/README.md` & `mypy-boto3-wisdom-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wisdom)](https://pepy.tech/project/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
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
@@ -313,20 +313,20 @@
 )
 
 
 def check_value(value: AssistantStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_wisdom.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_wisdom.type_defs import (
     AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
@@ -395,14 +395,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
     SessionDataTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
     CreateKnowledgeBaseRequestRequestTypeDef,
+    SourceConfigurationUnionTypeDef,
     AssistantAssociationDataTypeDef,
     AssistantAssociationSummaryTypeDef,
     CreateAssistantResponseTypeDef,
     GetAssistantResponseTypeDef,
     ListAssistantsResponseTypeDef,
     DocumentTypeDef,
     SearchContentRequestRequestTypeDef,
@@ -422,15 +423,15 @@
     RecommendationDataTypeDef,
     ResultDataTypeDef,
     GetRecommendationsResponseTypeDef,
     QueryAssistantResponseTypeDef,
 )
 
 
-def get_structure() -> AppIntegrationsConfigurationOutputTypeDef:
+def get_value() -> AppIntegrationsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__init__.py` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__init__.pyi` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__main__.py` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectWisdomService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ConnectWisdomService 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
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

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/client.py` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_wisdom.client import ConnectWisdomServiceClient
 
     session = Session()
     client: ConnectWisdomServiceClient = session.client("wisdom")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import KnowledgeBaseTypeType
 from .paginator import (
     ListAssistantAssociationsPaginator,
     ListAssistantsPaginator,
@@ -50,16 +50,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     QueryAssistantResponseTypeDef,
     RenderingConfigurationTypeDef,
     SearchContentResponseTypeDef,
     SearchExpressionTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SourceConfigurationOutputTypeDef,
-    SourceConfigurationTypeDef,
+    SourceConfigurationUnionTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -180,17 +179,15 @@
         *,
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        sourceConfiguration: Union[
-            SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
-        ] = ...,
+        sourceConfiguration: SourceConfigurationUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/client/#create_knowledge_base)
```

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/client.pyi` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_wisdom.client import ConnectWisdomServiceClient
 
     session = Session()
     client: ConnectWisdomServiceClient = session.client("wisdom")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import KnowledgeBaseTypeType
 from .paginator import (
     ListAssistantAssociationsPaginator,
     ListAssistantsPaginator,
@@ -50,16 +50,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     QueryAssistantResponseTypeDef,
     RenderingConfigurationTypeDef,
     SearchContentResponseTypeDef,
     SearchExpressionTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SourceConfigurationOutputTypeDef,
-    SourceConfigurationTypeDef,
+    SourceConfigurationUnionTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -170,17 +169,15 @@
         *,
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        sourceConfiguration: Union[
-            SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
-        ] = ...,
+        sourceConfiguration: SourceConfigurationUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/client/#create_knowledge_base)
```

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/literals.py` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/literals.pyi` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/paginator.py` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/paginator.pyi` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/type_defs.py` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_wisdom.type_defs import AppIntegrationsConfigurationOutputTypeDef
 
-    data: AppIntegrationsConfigurationOutputTypeDef = {...}
+    data: AppIntegrationsConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AssistantStatusType,
     ContentStatusType,
     KnowledgeBaseStatusType,
     KnowledgeBaseTypeType,
     RecommendationSourceTypeType,
@@ -104,14 +104,15 @@
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
     "SessionDataTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
     "CreateKnowledgeBaseRequestRequestTypeDef",
+    "SourceConfigurationUnionTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
     "GetAssistantResponseTypeDef",
     "ListAssistantsResponseTypeDef",
     "DocumentTypeDef",
     "SearchContentRequestRequestTypeDef",
@@ -1107,14 +1108,17 @@
 class CreateKnowledgeBaseRequestRequestTypeDef(
     _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
     _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
 ):
     pass
 
 
+SourceConfigurationUnionTypeDef = Union[
+    SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+]
 _RequiredAssistantAssociationDataTypeDef = TypedDict(
     "_RequiredAssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
```

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/type_defs.pyi` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_wisdom.type_defs import AppIntegrationsConfigurationOutputTypeDef
 
-    data: AppIntegrationsConfigurationOutputTypeDef = {...}
+    data: AppIntegrationsConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AssistantStatusType,
     ContentStatusType,
     KnowledgeBaseStatusType,
     KnowledgeBaseTypeType,
     RecommendationSourceTypeType,
@@ -103,14 +103,15 @@
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
     "SessionDataTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
     "CreateKnowledgeBaseRequestRequestTypeDef",
+    "SourceConfigurationUnionTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
     "GetAssistantResponseTypeDef",
     "ListAssistantsResponseTypeDef",
     "DocumentTypeDef",
     "SearchContentRequestRequestTypeDef",
@@ -1062,14 +1063,17 @@
 
 class CreateKnowledgeBaseRequestRequestTypeDef(
     _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
     _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
 ):
     pass
 
+SourceConfigurationUnionTypeDef = Union[
+    SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+]
 _RequiredAssistantAssociationDataTypeDef = TypedDict(
     "_RequiredAssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
```

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/PKG-INFO` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 wisdom type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 wisdom type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wisdom)](https://pepy.tech/project/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
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
@@ -345,20 +345,20 @@
 )
 
 
 def check_value(value: AssistantStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_wisdom.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_wisdom.type_defs import (
     AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
@@ -427,14 +427,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
     SessionDataTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
     CreateKnowledgeBaseRequestRequestTypeDef,
+    SourceConfigurationUnionTypeDef,
     AssistantAssociationDataTypeDef,
     AssistantAssociationSummaryTypeDef,
     CreateAssistantResponseTypeDef,
     GetAssistantResponseTypeDef,
     ListAssistantsResponseTypeDef,
     DocumentTypeDef,
     SearchContentRequestRequestTypeDef,
@@ -454,15 +455,15 @@
     RecommendationDataTypeDef,
     ResultDataTypeDef,
     GetRecommendationsResponseTypeDef,
     QueryAssistantResponseTypeDef,
 )
 
 
-def get_structure() -> AppIntegrationsConfigurationOutputTypeDef:
+def get_value() -> AppIntegrationsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/SOURCES.txt` & `mypy-boto3-wisdom-1.28.16/mypy_boto3_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15.post1/setup.py` & `mypy-boto3-wisdom-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wisdom",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ConnectWisdomService 1.28.16 service generated with"
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
-    keywords="boto3 wisdom type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 wisdom type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_wisdom": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

