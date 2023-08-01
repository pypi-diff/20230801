# Comparing `tmp/mypy-boto3-mturk-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-mturk-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mturk-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:44 2023, max compression
+gzip compressed data, was "mypy-boto3-mturk-1.28.16.tar", last modified: Tue Aug  1 11:37:24 2023, max compression
```

## Comparing `mypy-boto3-mturk-1.28.15.post1.tar` & `mypy-boto3-mturk-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33641 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33586 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-29 09:51:52.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-07-29 09:51:55.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39254 2023-07-29 09:51:52.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:24.968810 mypy-boto3-mturk-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18422 2023-08-01 11:37:24.960810 mypy-boto3-mturk-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16946 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:24.960810 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33316 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33261 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-08-01 11:24:52.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39526 2023-08-01 11:24:53.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39467 2023-08-01 11:24:52.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:24.960810 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18422 2023-08-01 11:37:24.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 11:37:24.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:24.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:24.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:24.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:37:24.000000 mypy-boto3-mturk-1.28.16/mypy_boto3_mturk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:24.968810 mypy-boto3-mturk-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:24:51.000000 mypy-boto3-mturk-1.28.16/setup.py
```

### Comparing `mypy-boto3-mturk-1.28.15.post1/LICENSE` & `mypy-boto3-mturk-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15.post1/PKG-INFO` & `mypy-boto3-mturk-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MTurk 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mturk type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mturk type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mturk)](https://pepy.tech/project/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
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
@@ -362,20 +362,20 @@
 )
 
 
 def check_value(value: AssignmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mturk.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mturk.type_defs import (
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
@@ -415,15 +415,15 @@
     ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
-    UpdateExpirationForHITRequestRequestTypeDef,
+    TimestampTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
     CreateHITTypeResponseTypeDef,
     GetAccountBalanceResponseTypeDef,
     GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
@@ -448,34 +448,37 @@
     QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
     PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
+    UpdateExpirationForHITRequestRequestTypeDef,
     HITTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
+    QualificationRequirementUnionTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
     ListHITsResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     CreateHITRequestRequestTypeDef,
     CreateHITWithHITTypeRequestRequestTypeDef,
+    ReviewPolicyUnionTypeDef,
 )
 
 
-def get_structure() -> AcceptQualificationRequestRequestRequestTypeDef:
+def get_value() -> AcceptQualificationRequestRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mturk-1.28.15.post1/README.md` & `mypy-boto3-mturk-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mturk)](https://pepy.tech/project/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
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
@@ -330,20 +330,20 @@
 )
 
 
 def check_value(value: AssignmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mturk.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mturk.type_defs import (
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
@@ -383,15 +383,15 @@
     ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
-    UpdateExpirationForHITRequestRequestTypeDef,
+    TimestampTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
     CreateHITTypeResponseTypeDef,
     GetAccountBalanceResponseTypeDef,
     GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
@@ -416,34 +416,37 @@
     QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
     PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
+    UpdateExpirationForHITRequestRequestTypeDef,
     HITTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
+    QualificationRequirementUnionTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
     ListHITsResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     CreateHITRequestRequestTypeDef,
     CreateHITWithHITTypeRequestRequestTypeDef,
+    ReviewPolicyUnionTypeDef,
 )
 
 
-def get_structure() -> AcceptQualificationRequestRequestRequestTypeDef:
+def get_value() -> AcceptQualificationRequestRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__init__.py` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__init__.pyi` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/client.py` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_mturk.client import MTurkClient
 
     session = Session()
     client: MTurkClient = session.client("mturk")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssignmentStatusType,
     EventTypeType,
     QualificationStatusType,
@@ -58,18 +57,17 @@
     ListQualificationTypesResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersResponseTypeDef,
-    QualificationRequirementOutputTypeDef,
-    QualificationRequirementTypeDef,
-    ReviewPolicyOutputTypeDef,
-    ReviewPolicyTypeDef,
+    QualificationRequirementUnionTypeDef,
+    ReviewPolicyUnionTypeDef,
+    TimestampTypeDef,
     UpdateQualificationTypeResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -182,20 +180,18 @@
         Title: str,
         Description: str,
         MaxAssignments: int = ...,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
-        QualificationRequirements: Sequence[
-            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
-        ] = ...,
+        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
-        HITReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
+        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
@@ -207,17 +203,15 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[
-            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
-        ] = ...
+        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#create_hit_type)
         """
@@ -227,16 +221,16 @@
         *,
         HITTypeId: str,
         LifetimeInSeconds: int,
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
-        HITReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
+        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task (HIT)
         using an existing HITTypeID generated by the `CreateHITType` operation.
 
@@ -580,15 +574,15 @@
         notification specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.send_test_event_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#send_test_event_notification)
         """
 
     def update_expiration_for_hit(
-        self, *, HITId: str, ExpireAt: Union[datetime, str]
+        self, *, HITId: str, ExpireAt: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         The `UpdateExpirationForHIT` operation allows you update the expiration time of
         a HIT.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.update_expiration_for_hit)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#update_expiration_for_hit)
```

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/client.pyi` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_mturk.client import MTurkClient
 
     session = Session()
     client: MTurkClient = session.client("mturk")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssignmentStatusType,
     EventTypeType,
     QualificationStatusType,
@@ -58,18 +57,17 @@
     ListQualificationTypesResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersResponseTypeDef,
-    QualificationRequirementOutputTypeDef,
-    QualificationRequirementTypeDef,
-    ReviewPolicyOutputTypeDef,
-    ReviewPolicyTypeDef,
+    QualificationRequirementUnionTypeDef,
+    ReviewPolicyUnionTypeDef,
+    TimestampTypeDef,
     UpdateQualificationTypeResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -171,20 +169,18 @@
         Title: str,
         Description: str,
         MaxAssignments: int = ...,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
-        QualificationRequirements: Sequence[
-            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
-        ] = ...,
+        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
-        HITReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
+        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
@@ -195,17 +191,15 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[
-            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
-        ] = ...
+        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#create_hit_type)
         """
@@ -214,16 +208,16 @@
         *,
         HITTypeId: str,
         LifetimeInSeconds: int,
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
-        HITReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
+        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task (HIT)
         using an existing HITTypeID generated by the `CreateHITType` operation.
 
@@ -538,15 +532,15 @@
         a notification message as if a HIT event occurred, according to the provided
         notification specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.send_test_event_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#send_test_event_notification)
         """
     def update_expiration_for_hit(
-        self, *, HITId: str, ExpireAt: Union[datetime, str]
+        self, *, HITId: str, ExpireAt: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         The `UpdateExpirationForHIT` operation allows you update the expiration time of
         a HIT.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.update_expiration_for_hit)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#update_expiration_for_hit)
```

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/literals.py` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/literals.pyi` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/paginator.py` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/paginator.pyi` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/type_defs.py` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mturk.type_defs import AcceptQualificationRequestRequestRequestTypeDef
 
-    data: AcceptQualificationRequestRequestRequestTypeDef = {...}
+    data: AcceptQualificationRequestRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -78,15 +78,15 @@
     "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
-    "UpdateExpirationForHITRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UpdateHITReviewStatusRequestRequestTypeDef",
     "UpdateHITTypeOfHITRequestRequestTypeDef",
     "UpdateQualificationTypeRequestRequestTypeDef",
     "CreateHITTypeResponseTypeDef",
     "GetAccountBalanceResponseTypeDef",
     "GetFileUploadURLResponseTypeDef",
     "ListAssignmentsForHITResponseTypeDef",
@@ -111,30 +111,33 @@
     "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
     "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
+    "UpdateExpirationForHITRequestRequestTypeDef",
     "HITTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
+    "QualificationRequirementUnionTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
     "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
     "ListHITsResponseTypeDef",
     "ListReviewableHITsResponseTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
     "ListReviewPolicyResultsForHITResponseTypeDef",
     "CreateHITRequestRequestTypeDef",
     "CreateHITWithHITTypeRequestRequestTypeDef",
+    "ReviewPolicyUnionTypeDef",
 )
 
 _RequiredAcceptQualificationRequestRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptQualificationRequestRequestRequestTypeDef",
     {
         "QualificationRequestId": str,
     },
@@ -775,22 +778,15 @@
 
 class SendBonusRequestRequestTypeDef(
     _RequiredSendBonusRequestRequestTypeDef, _OptionalSendBonusRequestRequestTypeDef
 ):
     pass
 
 
-UpdateExpirationForHITRequestRequestTypeDef = TypedDict(
-    "UpdateExpirationForHITRequestRequestTypeDef",
-    {
-        "HITId": str,
-        "ExpireAt": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredUpdateHITReviewStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHITReviewStatusRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalUpdateHITReviewStatusRequestRequestTypeDef = TypedDict(
@@ -1209,14 +1205,22 @@
     {
         "ReviewResults": List[ReviewResultDetailTypeDef],
         "ReviewActions": List[ReviewActionDetailTypeDef],
     },
     total=False,
 )
 
+UpdateExpirationForHITRequestRequestTypeDef = TypedDict(
+    "UpdateExpirationForHITRequestRequestTypeDef",
+    {
+        "HITId": str,
+        "ExpireAt": TimestampTypeDef,
+    },
+)
+
 HITTypeDef = TypedDict(
     "HITTypeDef",
     {
         "HITId": str,
         "HITTypeId": str,
         "HITGroupId": str,
         "HITLayoutId": str,
@@ -1237,42 +1241,17 @@
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
 
-_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHITTypeRequestRequestTypeDef",
-    {
-        "AssignmentDurationInSeconds": int,
-        "Reward": str,
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHITTypeRequestRequestTypeDef",
-    {
-        "AutoApprovalDelayInSeconds": int,
-        "Keywords": str,
-        "QualificationRequirements": Sequence[
-            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class CreateHITTypeRequestRequestTypeDef(
-    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
-):
-    pass
-
-
+QualificationRequirementUnionTypeDef = Union[
+    QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef
+]
 GetQualificationScoreResponseTypeDef = TypedDict(
     "GetQualificationScoreResponseTypeDef",
     {
         "Qualification": QualificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1386,14 +1365,40 @@
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHITTypeRequestRequestTypeDef",
+    {
+        "AssignmentDurationInSeconds": int,
+        "Reward": str,
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHITTypeRequestRequestTypeDef",
+    {
+        "AutoApprovalDelayInSeconds": int,
+        "Keywords": str,
+        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateHITTypeRequestRequestTypeDef(
+    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
+):
+    pass
+
+
 ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
     "ListReviewPolicyResultsForHITResponseTypeDef",
     {
         "HITId": str,
         "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
         "HITReviewPolicy": ReviewPolicyOutputTypeDef,
         "AssignmentReviewReport": ReviewReportTypeDef,
@@ -1417,17 +1422,15 @@
     "_OptionalCreateHITRequestRequestTypeDef",
     {
         "MaxAssignments": int,
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
         "Question": str,
         "RequesterAnnotation": str,
-        "QualificationRequirements": Sequence[
-            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
-        ],
+        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
         "UniqueRequestToken": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "HITLayoutId": str,
         "HITLayoutParameters": Sequence[HITLayoutParameterTypeDef],
     },
     total=False,
@@ -1464,7 +1467,10 @@
 
 
 class CreateHITWithHITTypeRequestRequestTypeDef(
     _RequiredCreateHITWithHITTypeRequestRequestTypeDef,
     _OptionalCreateHITWithHITTypeRequestRequestTypeDef,
 ):
     pass
+
+
+ReviewPolicyUnionTypeDef = Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef]
```

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/type_defs.pyi` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mturk.type_defs import AcceptQualificationRequestRequestRequestTypeDef
 
-    data: AcceptQualificationRequestRequestRequestTypeDef = {...}
+    data: AcceptQualificationRequestRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -77,15 +77,15 @@
     "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
-    "UpdateExpirationForHITRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UpdateHITReviewStatusRequestRequestTypeDef",
     "UpdateHITTypeOfHITRequestRequestTypeDef",
     "UpdateQualificationTypeRequestRequestTypeDef",
     "CreateHITTypeResponseTypeDef",
     "GetAccountBalanceResponseTypeDef",
     "GetFileUploadURLResponseTypeDef",
     "ListAssignmentsForHITResponseTypeDef",
@@ -110,30 +110,33 @@
     "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
     "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
+    "UpdateExpirationForHITRequestRequestTypeDef",
     "HITTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
+    "QualificationRequirementUnionTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
     "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
     "ListHITsResponseTypeDef",
     "ListReviewableHITsResponseTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
     "ListReviewPolicyResultsForHITResponseTypeDef",
     "CreateHITRequestRequestTypeDef",
     "CreateHITWithHITTypeRequestRequestTypeDef",
+    "ReviewPolicyUnionTypeDef",
 )
 
 _RequiredAcceptQualificationRequestRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptQualificationRequestRequestRequestTypeDef",
     {
         "QualificationRequestId": str,
     },
@@ -744,22 +747,15 @@
 )
 
 class SendBonusRequestRequestTypeDef(
     _RequiredSendBonusRequestRequestTypeDef, _OptionalSendBonusRequestRequestTypeDef
 ):
     pass
 
-UpdateExpirationForHITRequestRequestTypeDef = TypedDict(
-    "UpdateExpirationForHITRequestRequestTypeDef",
-    {
-        "HITId": str,
-        "ExpireAt": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredUpdateHITReviewStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHITReviewStatusRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalUpdateHITReviewStatusRequestRequestTypeDef = TypedDict(
@@ -1160,14 +1156,22 @@
     {
         "ReviewResults": List[ReviewResultDetailTypeDef],
         "ReviewActions": List[ReviewActionDetailTypeDef],
     },
     total=False,
 )
 
+UpdateExpirationForHITRequestRequestTypeDef = TypedDict(
+    "UpdateExpirationForHITRequestRequestTypeDef",
+    {
+        "HITId": str,
+        "ExpireAt": TimestampTypeDef,
+    },
+)
+
 HITTypeDef = TypedDict(
     "HITTypeDef",
     {
         "HITId": str,
         "HITTypeId": str,
         "HITGroupId": str,
         "HITLayoutId": str,
@@ -1188,40 +1192,17 @@
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
 
-_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHITTypeRequestRequestTypeDef",
-    {
-        "AssignmentDurationInSeconds": int,
-        "Reward": str,
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHITTypeRequestRequestTypeDef",
-    {
-        "AutoApprovalDelayInSeconds": int,
-        "Keywords": str,
-        "QualificationRequirements": Sequence[
-            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class CreateHITTypeRequestRequestTypeDef(
-    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
-):
-    pass
-
+QualificationRequirementUnionTypeDef = Union[
+    QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef
+]
 GetQualificationScoreResponseTypeDef = TypedDict(
     "GetQualificationScoreResponseTypeDef",
     {
         "Qualification": QualificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1331,14 +1312,38 @@
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHITTypeRequestRequestTypeDef",
+    {
+        "AssignmentDurationInSeconds": int,
+        "Reward": str,
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHITTypeRequestRequestTypeDef",
+    {
+        "AutoApprovalDelayInSeconds": int,
+        "Keywords": str,
+        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
+    },
+    total=False,
+)
+
+class CreateHITTypeRequestRequestTypeDef(
+    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
+):
+    pass
+
 ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
     "ListReviewPolicyResultsForHITResponseTypeDef",
     {
         "HITId": str,
         "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
         "HITReviewPolicy": ReviewPolicyOutputTypeDef,
         "AssignmentReviewReport": ReviewReportTypeDef,
@@ -1362,17 +1367,15 @@
     "_OptionalCreateHITRequestRequestTypeDef",
     {
         "MaxAssignments": int,
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
         "Question": str,
         "RequesterAnnotation": str,
-        "QualificationRequirements": Sequence[
-            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
-        ],
+        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
         "UniqueRequestToken": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "HITLayoutId": str,
         "HITLayoutParameters": Sequence[HITLayoutParameterTypeDef],
     },
     total=False,
@@ -1406,7 +1409,9 @@
 )
 
 class CreateHITWithHITTypeRequestRequestTypeDef(
     _RequiredCreateHITWithHITTypeRequestRequestTypeDef,
     _OptionalCreateHITWithHITTypeRequestRequestTypeDef,
 ):
     pass
+
+ReviewPolicyUnionTypeDef = Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef]
```

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/PKG-INFO` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MTurk 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mturk type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mturk type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mturk)](https://pepy.tech/project/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
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
@@ -362,20 +362,20 @@
 )
 
 
 def check_value(value: AssignmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mturk.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mturk.type_defs import (
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
@@ -415,15 +415,15 @@
     ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
-    UpdateExpirationForHITRequestRequestTypeDef,
+    TimestampTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
     CreateHITTypeResponseTypeDef,
     GetAccountBalanceResponseTypeDef,
     GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
@@ -448,34 +448,37 @@
     QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
     PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
+    UpdateExpirationForHITRequestRequestTypeDef,
     HITTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
+    QualificationRequirementUnionTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
     ListHITsResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     CreateHITRequestRequestTypeDef,
     CreateHITWithHITTypeRequestRequestTypeDef,
+    ReviewPolicyUnionTypeDef,
 )
 
 
-def get_structure() -> AcceptQualificationRequestRequestRequestTypeDef:
+def get_value() -> AcceptQualificationRequestRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/SOURCES.txt` & `mypy-boto3-mturk-1.28.16/mypy_boto3_mturk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15.post1/setup.py` & `mypy-boto3-mturk-1.28.16/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mturk",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_mturk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MTurk 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 mturk type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 mturk type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mturk": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

