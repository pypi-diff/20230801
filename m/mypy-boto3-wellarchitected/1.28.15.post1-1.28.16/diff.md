# Comparing `tmp/mypy-boto3-wellarchitected-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-wellarchitected-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wellarchitected-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:25 2023, max compression
+gzip compressed data, was "mypy-boto3-wellarchitected-1.28.16.tar", last modified: Tue Aug  1 11:38:05 2023, max compression
```

## Comparing `mypy-boto3-wellarchitected-1.28.15.post1.tar` & `mypy-boto3-wellarchitected-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.901457 mypy-boto3-wellarchitected-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:35.000000 mypy-boto3-wellarchitected-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-29 10:04:25.897457 mypy-boto3-wellarchitected-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16585 2023-07-29 10:01:35.000000 mypy-boto3-wellarchitected-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.897457 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-29 10:01:35.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-29 10:01:35.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 10:01:35.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-29 10:01:36.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-29 10:01:36.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-07-29 10:01:36.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-29 10:01:36.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:35.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53350 2023-07-29 10:01:38.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53293 2023-07-29 10:01:37.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:35.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.897457 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-29 10:04:25.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-29 10:04:25.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:25.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:04:25.000000 mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:25.901457 mypy-boto3-wellarchitected-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-29 10:01:35.000000 mypy-boto3-wellarchitected-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.136660 mypy-boto3-wellarchitected-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-08-01 11:38:05.136660 mypy-boto3-wellarchitected-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.136660 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38042 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37980 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53518 2023-08-01 11:35:18.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53461 2023-08-01 11:35:17.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:35:16.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.136660 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-08-01 11:38:04.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-01 11:38:04.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:04.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:04.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:04.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:38:04.000000 mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:05.136660 mypy-boto3-wellarchitected-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-01 11:35:15.000000 mypy-boto3-wellarchitected-1.28.16/setup.py
```

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/LICENSE` & `mypy-boto3-wellarchitected-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/PKG-INFO` & `mypy-boto3-wellarchitected-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WellArchitected 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WellArchitected 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 wellarchitected type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 wellarchitected type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wellarchitected)](https://pepy.tech/project/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
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
@@ -318,20 +318,20 @@
 )
 
 
 def check_value(value: AdditionalResourceTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_wellarchitected.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
@@ -445,14 +445,15 @@
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     PillarDifferenceTypeDef,
     ProfileQuestionTypeDef,
     ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
     WorkloadTypeDef,
     ChoiceTypeDef,
     PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
@@ -478,15 +479,15 @@
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
     ConsolidatedReportMetricTypeDef,
     GetConsolidatedReportOutputTypeDef,
 )
 
 
-def get_structure() -> ChoiceContentTypeDef:
+def get_value() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/README.md` & `mypy-boto3-wellarchitected-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wellarchitected)](https://pepy.tech/project/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
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
@@ -286,20 +286,20 @@
 )
 
 
 def check_value(value: AdditionalResourceTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_wellarchitected.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
@@ -413,14 +413,15 @@
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     PillarDifferenceTypeDef,
     ProfileQuestionTypeDef,
     ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
     WorkloadTypeDef,
     ChoiceTypeDef,
     PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
@@ -446,15 +447,15 @@
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
     ConsolidatedReportMetricTypeDef,
     GetConsolidatedReportOutputTypeDef,
 )
 
 
-def get_structure() -> ChoiceContentTypeDef:
+def get_value() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/__main__.py` & `mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WellArchitected 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.WellArchitected 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected\nOther"
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

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/client.py` & `mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_wellarchitected.client import WellArchitectedClient
 
     session = Session()
     client: WellArchitectedClient = session.client("wellarchitected")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
     DiscoveryIntegrationStatusType,
     LensStatusTypeType,
@@ -74,16 +74,15 @@
     ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
-    WorkloadDiscoveryConfigOutputTypeDef,
-    WorkloadDiscoveryConfigTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -232,17 +231,15 @@
         PillarPriorities: Sequence[str] = ...,
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
-        DiscoveryConfig: Union[
-            WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
-        ] = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
@@ -810,17 +807,15 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
-        DiscoveryConfig: Union[
-            WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
-        ] = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
         Applications: Sequence[str] = ...
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload)
```

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/client.pyi` & `mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_wellarchitected.client import WellArchitectedClient
 
     session = Session()
     client: WellArchitectedClient = session.client("wellarchitected")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
     DiscoveryIntegrationStatusType,
     LensStatusTypeType,
@@ -74,16 +74,15 @@
     ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
-    WorkloadDiscoveryConfigOutputTypeDef,
-    WorkloadDiscoveryConfigTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -219,17 +218,15 @@
         PillarPriorities: Sequence[str] = ...,
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
-        DiscoveryConfig: Union[
-            WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
-        ] = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
@@ -751,17 +748,15 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
-        DiscoveryConfig: Union[
-            WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
-        ] = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
         Applications: Sequence[str] = ...
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload)
```

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/literals.py` & `mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/literals.pyi` & `mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/type_defs.py` & `mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_wellarchitected.type_defs import ChoiceContentTypeDef
 
-    data: ChoiceContentTypeDef = {...}
+    data: ChoiceContentTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
@@ -171,14 +171,15 @@
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
+    "WorkloadDiscoveryConfigUnionTypeDef",
     "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
@@ -1814,14 +1815,17 @@
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+WorkloadDiscoveryConfigUnionTypeDef = Union[
+    WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
+]
 WorkloadTypeDef = TypedDict(
     "WorkloadTypeDef",
     {
         "WorkloadId": str,
         "WorkloadArn": str,
         "WorkloadName": str,
         "Description": str,
```

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected/type_defs.pyi` & `mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_wellarchitected.type_defs import ChoiceContentTypeDef
 
-    data: ChoiceContentTypeDef = {...}
+    data: ChoiceContentTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
@@ -170,14 +170,15 @@
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
+    "WorkloadDiscoveryConfigUnionTypeDef",
     "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
@@ -1757,14 +1758,17 @@
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+WorkloadDiscoveryConfigUnionTypeDef = Union[
+    WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
+]
 WorkloadTypeDef = TypedDict(
     "WorkloadTypeDef",
     {
         "WorkloadId": str,
         "WorkloadArn": str,
         "WorkloadName": str,
         "Description": str,
```

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected.egg-info/PKG-INFO` & `mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WellArchitected 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WellArchitected 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 wellarchitected type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 wellarchitected type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wellarchitected)](https://pepy.tech/project/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
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
@@ -318,20 +318,20 @@
 )
 
 
 def check_value(value: AdditionalResourceTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_wellarchitected.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
@@ -445,14 +445,15 @@
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     PillarDifferenceTypeDef,
     ProfileQuestionTypeDef,
     ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
     WorkloadTypeDef,
     ChoiceTypeDef,
     PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
@@ -478,15 +479,15 @@
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
     ConsolidatedReportMetricTypeDef,
     GetConsolidatedReportOutputTypeDef,
 )
 
 
-def get_structure() -> ChoiceContentTypeDef:
+def get_value() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/mypy_boto3_wellarchitected.egg-info/SOURCES.txt` & `mypy-boto3-wellarchitected-1.28.16/mypy_boto3_wellarchitected.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.28.15.post1/setup.py` & `mypy-boto3-wellarchitected-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wellarchitected",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_wellarchitected"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WellArchitected 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.WellArchitected 1.28.16 service generated with"
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
-    keywords="boto3 wellarchitected type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 wellarchitected type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_wellarchitected": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

