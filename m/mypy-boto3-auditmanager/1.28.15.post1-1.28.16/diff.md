# Comparing `tmp/mypy-boto3-auditmanager-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-auditmanager-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-auditmanager-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
+gzip compressed data, was "mypy-boto3-auditmanager-1.28.16.tar", last modified: Tue Aug  1 11:36:15 2023, max compression
```

## Comparing `mypy-boto3-auditmanager-1.28.15.post1.tar` & `mypy-boto3-auditmanager-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.469021 mypy-boto3-auditmanager-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-07-29 10:02:34.469021 mypy-boto3-auditmanager-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.465021 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43379 2023-07-29 09:38:43.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43311 2023-07-29 09:38:43.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-29 09:38:43.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-29 09:38:43.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57940 2023-07-29 09:38:46.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57895 2023-07-29 09:38:45.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.469021 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.469021 mypy-boto3-auditmanager-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.268945 mypy-boto3-auditmanager-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:14.000000 mypy-boto3-auditmanager-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-08-01 11:36:15.268945 mypy-boto3-auditmanager-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-08-01 11:11:14.000000 mypy-boto3-auditmanager-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.260945 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 11:11:14.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 11:11:14.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:11:14.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43309 2023-08-01 11:11:15.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43241 2023-08-01 11:11:15.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-08-01 11:11:16.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-08-01 11:11:15.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:14.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58030 2023-08-01 11:11:17.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57985 2023-08-01 11:11:16.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:14.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.268945 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-08-01 11:36:15.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 11:36:15.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:15.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:15.000000 mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:15.268945 mypy-boto3-auditmanager-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:11:14.000000 mypy-boto3-auditmanager-1.28.16/setup.py
```

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/LICENSE` & `mypy-boto3-auditmanager-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/PKG-INFO` & `mypy-boto3-auditmanager-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AuditManager 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 auditmanager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 auditmanager type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-auditmanager)](https://pepy.tech/project/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
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
@@ -312,20 +312,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_auditmanager.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_auditmanager.type_defs import (
     AWSAccountTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
     RoleTypeDef,
@@ -450,14 +450,15 @@
     GetAssessmentReportUrlResponseTypeDef,
     GetInsightsByAssessmentResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetServicesInScopeResponseTypeDef,
     ListNotificationsResponseTypeDef,
     AssessmentMetadataTypeDef,
     CreateAssessmentRequestRequestTypeDef,
+    ScopeUnionTypeDef,
     UpdateAssessmentRequestRequestTypeDef,
     ListAssessmentsResponseTypeDef,
     AssessmentControlSetTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     BatchCreateDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlResponseTypeDef,
     ListControlDomainInsightsByAssessmentResponseTypeDef,
@@ -487,15 +488,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountTypeDef:
+def get_value() -> AWSAccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/README.md` & `mypy-boto3-auditmanager-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-auditmanager)](https://pepy.tech/project/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
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
@@ -280,20 +280,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_auditmanager.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_auditmanager.type_defs import (
     AWSAccountTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
     RoleTypeDef,
@@ -418,14 +418,15 @@
     GetAssessmentReportUrlResponseTypeDef,
     GetInsightsByAssessmentResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetServicesInScopeResponseTypeDef,
     ListNotificationsResponseTypeDef,
     AssessmentMetadataTypeDef,
     CreateAssessmentRequestRequestTypeDef,
+    ScopeUnionTypeDef,
     UpdateAssessmentRequestRequestTypeDef,
     ListAssessmentsResponseTypeDef,
     AssessmentControlSetTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     BatchCreateDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlResponseTypeDef,
     ListControlDomainInsightsByAssessmentResponseTypeDef,
@@ -455,15 +456,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountTypeDef:
+def get_value() -> AWSAccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/__main__.py` & `mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AuditManager 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AuditManager 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
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

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/client.py` & `mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_auditmanager.client import AuditManagerClient
 
     session = Session()
     client: AuditManagerClient = session.client("auditmanager")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssessmentStatusType,
     ControlSetStatusType,
     ControlStatusType,
@@ -76,16 +76,15 @@
     ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManualEvidenceTypeDef,
     RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountResponseTypeDef,
     RoleTypeDef,
-    ScopeOutputTypeDef,
-    ScopeTypeDef,
+    ScopeUnionTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     UpdateAssessmentControlSetStatusResponseTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentResponseTypeDef,
@@ -220,15 +219,15 @@
         """
 
     def create_assessment(
         self,
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
-        scope: Union[ScopeTypeDef, ScopeOutputTypeDef],
+        scope: ScopeUnionTypeDef,
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
@@ -736,15 +735,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#untag_resource)
         """
 
     def update_assessment(
         self,
         *,
         assessmentId: str,
-        scope: Union[ScopeTypeDef, ScopeOutputTypeDef],
+        scope: ScopeUnionTypeDef,
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         roles: Sequence[RoleTypeDef] = ...
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
```

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/client.pyi` & `mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_auditmanager.client import AuditManagerClient
 
     session = Session()
     client: AuditManagerClient = session.client("auditmanager")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssessmentStatusType,
     ControlSetStatusType,
     ControlStatusType,
@@ -76,16 +76,15 @@
     ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManualEvidenceTypeDef,
     RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountResponseTypeDef,
     RoleTypeDef,
-    ScopeOutputTypeDef,
-    ScopeTypeDef,
+    ScopeUnionTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     UpdateAssessmentControlSetStatusResponseTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentResponseTypeDef,
@@ -208,15 +207,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#close)
         """
     def create_assessment(
         self,
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
-        scope: Union[ScopeTypeDef, ScopeOutputTypeDef],
+        scope: ScopeUnionTypeDef,
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
@@ -676,15 +675,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#untag_resource)
         """
     def update_assessment(
         self,
         *,
         assessmentId: str,
-        scope: Union[ScopeTypeDef, ScopeOutputTypeDef],
+        scope: ScopeUnionTypeDef,
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         roles: Sequence[RoleTypeDef] = ...
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
```

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/literals.py` & `mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/literals.pyi` & `mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/type_defs.py` & `mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_auditmanager.type_defs import AWSAccountTypeDef
 
-    data: AWSAccountTypeDef = {...}
+    data: AWSAccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountStatusType,
     ActionEnumType,
     AssessmentReportStatusType,
     AssessmentStatusType,
     ControlResponseType,
@@ -177,14 +177,15 @@
     "GetAssessmentReportUrlResponseTypeDef",
     "GetInsightsByAssessmentResponseTypeDef",
     "GetInsightsResponseTypeDef",
     "GetServicesInScopeResponseTypeDef",
     "ListNotificationsResponseTypeDef",
     "AssessmentMetadataTypeDef",
     "CreateAssessmentRequestRequestTypeDef",
+    "ScopeUnionTypeDef",
     "UpdateAssessmentRequestRequestTypeDef",
     "ListAssessmentsResponseTypeDef",
     "AssessmentControlSetTypeDef",
     "UpdateAssessmentControlResponseTypeDef",
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
@@ -1749,14 +1750,15 @@
 
 class CreateAssessmentRequestRequestTypeDef(
     _RequiredCreateAssessmentRequestRequestTypeDef, _OptionalCreateAssessmentRequestRequestTypeDef
 ):
     pass
 
 
+ScopeUnionTypeDef = Union[ScopeTypeDef, ScopeOutputTypeDef]
 _RequiredUpdateAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
         "scope": ScopeTypeDef,
     },
 )
```

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/type_defs.pyi` & `mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_auditmanager.type_defs import AWSAccountTypeDef
 
-    data: AWSAccountTypeDef = {...}
+    data: AWSAccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountStatusType,
     ActionEnumType,
     AssessmentReportStatusType,
     AssessmentStatusType,
     ControlResponseType,
@@ -176,14 +176,15 @@
     "GetAssessmentReportUrlResponseTypeDef",
     "GetInsightsByAssessmentResponseTypeDef",
     "GetInsightsResponseTypeDef",
     "GetServicesInScopeResponseTypeDef",
     "ListNotificationsResponseTypeDef",
     "AssessmentMetadataTypeDef",
     "CreateAssessmentRequestRequestTypeDef",
+    "ScopeUnionTypeDef",
     "UpdateAssessmentRequestRequestTypeDef",
     "ListAssessmentsResponseTypeDef",
     "AssessmentControlSetTypeDef",
     "UpdateAssessmentControlResponseTypeDef",
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
@@ -1714,14 +1715,15 @@
 )
 
 class CreateAssessmentRequestRequestTypeDef(
     _RequiredCreateAssessmentRequestRequestTypeDef, _OptionalCreateAssessmentRequestRequestTypeDef
 ):
     pass
 
+ScopeUnionTypeDef = Union[ScopeTypeDef, ScopeOutputTypeDef]
 _RequiredUpdateAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
         "scope": ScopeTypeDef,
     },
 )
```

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/PKG-INFO` & `mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AuditManager 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 auditmanager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 auditmanager type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-auditmanager)](https://pepy.tech/project/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
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
@@ -312,20 +312,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_auditmanager.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_auditmanager.type_defs import (
     AWSAccountTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
     RoleTypeDef,
@@ -450,14 +450,15 @@
     GetAssessmentReportUrlResponseTypeDef,
     GetInsightsByAssessmentResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetServicesInScopeResponseTypeDef,
     ListNotificationsResponseTypeDef,
     AssessmentMetadataTypeDef,
     CreateAssessmentRequestRequestTypeDef,
+    ScopeUnionTypeDef,
     UpdateAssessmentRequestRequestTypeDef,
     ListAssessmentsResponseTypeDef,
     AssessmentControlSetTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     BatchCreateDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlResponseTypeDef,
     ListControlDomainInsightsByAssessmentResponseTypeDef,
@@ -487,15 +488,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountTypeDef:
+def get_value() -> AWSAccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/SOURCES.txt` & `mypy-boto3-auditmanager-1.28.16/mypy_boto3_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15.post1/setup.py` & `mypy-boto3-auditmanager-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-auditmanager",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.AuditManager 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 auditmanager type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 auditmanager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_auditmanager": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

