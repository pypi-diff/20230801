# Comparing `tmp/mypy-boto3-macie2-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-macie2-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-macie2-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:35 2023, max compression
+gzip compressed data, was "mypy-boto3-macie2-1.28.16.tar", last modified: Tue Aug  1 11:37:16 2023, max compression
```

## Comparing `mypy-boto3-macie2-1.28.15.post1.tar` & `mypy-boto3-macie2-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:35.633262 mypy-boto3-macie2-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:24.000000 mypy-boto3-macie2-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29259 2023-07-29 10:03:35.633262 mypy-boto3-macie2-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27770 2023-07-29 09:50:24.000000 mypy-boto3-macie2-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:35.629262 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-29 09:50:24.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-29 09:50:24.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:50:24.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60494 2023-07-29 09:50:25.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    60391 2023-07-29 09:50:24.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-07-29 09:50:25.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-07-29 09:50:25.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19591 2023-07-29 09:50:25.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-07-29 09:50:25.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:24.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93322 2023-07-29 09:50:28.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93267 2023-07-29 09:50:27.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:24.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-29 09:50:25.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-29 09:50:25.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:35.633262 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29259 2023-07-29 10:03:35.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:35.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:35.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:35.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:35.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:35.000000 mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:35.633262 mypy-boto3-macie2-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:50:24.000000 mypy-boto3-macie2-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:16.332831 mypy-boto3-macie2-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:16.000000 mypy-boto3-macie2-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29463 2023-08-01 11:37:16.332831 mypy-boto3-macie2-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-08-01 11:23:16.000000 mypy-boto3-macie2-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:16.324831 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-01 11:23:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-01 11:23:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:23:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59896 2023-08-01 11:23:17.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59793 2023-08-01 11:23:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-08-01 11:23:17.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-08-01 11:23:17.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-08-01 11:23:17.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-08-01 11:23:17.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94166 2023-08-01 11:23:22.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94111 2023-08-01 11:23:21.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-01 11:23:17.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-01 11:23:17.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:16.332831 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29463 2023-08-01 11:37:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:37:16.000000 mypy-boto3-macie2-1.28.16/mypy_boto3_macie2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:16.332831 mypy-boto3-macie2-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:23:16.000000 mypy-boto3-macie2-1.28.16/setup.py
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/LICENSE` & `mypy-boto3-macie2-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.15.post1/PKG-INFO` & `mypy-boto3-macie2-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Macie2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Macie2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 macie2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 macie2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie2)](https://pepy.tech/project/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -453,20 +453,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_macie2.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
@@ -684,14 +684,16 @@
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
     UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
     TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
     TagScopeTermOutputTypeDef,
@@ -703,18 +705,20 @@
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     PutClassificationExportConfigurationRequestRequestTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
     GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
     ListClassificationJobsRequestRequestTypeDef,
     OccurrencesTypeDef,
     GetClassificationScopeResponseTypeDef,
     UpdateClassificationScopeRequestRequestTypeDef,
     SearchResourcesCriteriaTypeDef,
     UsageRecordTypeDef,
@@ -754,20 +758,21 @@
     JobSummaryTypeDef,
     S3JobDefinitionOutputTypeDef,
     S3JobDefinitionTypeDef,
     ClassificationDetailsTypeDef,
     ListClassificationJobsResponseTypeDef,
     DescribeClassificationJobResponseTypeDef,
     CreateClassificationJobRequestRequestTypeDef,
+    S3JobDefinitionUnionTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptInvitationRequestRequestTypeDef:
+def get_value() -> AcceptInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/README.md` & `mypy-boto3-macie2-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie2)](https://pepy.tech/project/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -421,20 +421,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_macie2.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
@@ -652,14 +652,16 @@
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
     UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
     TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
     TagScopeTermOutputTypeDef,
@@ -671,18 +673,20 @@
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     PutClassificationExportConfigurationRequestRequestTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
     GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
     ListClassificationJobsRequestRequestTypeDef,
     OccurrencesTypeDef,
     GetClassificationScopeResponseTypeDef,
     UpdateClassificationScopeRequestRequestTypeDef,
     SearchResourcesCriteriaTypeDef,
     UsageRecordTypeDef,
@@ -722,20 +726,21 @@
     JobSummaryTypeDef,
     S3JobDefinitionOutputTypeDef,
     S3JobDefinitionTypeDef,
     ClassificationDetailsTypeDef,
     ListClassificationJobsResponseTypeDef,
     DescribeClassificationJobResponseTypeDef,
     CreateClassificationJobRequestRequestTypeDef,
+    S3JobDefinitionUnionTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptInvitationRequestRequestTypeDef:
+def get_value() -> AcceptInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/__init__.py` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/__init__.pyi` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/__main__.py` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Macie2 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Macie2 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2\nOther"
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

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/client.py` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_macie2.client import Macie2Client
 
     session = Session()
     client: Macie2Client = session.client("macie2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutomatedDiscoveryStatusType,
     FindingPublishingFrequencyType,
     FindingsFilterActionType,
@@ -62,16 +62,15 @@
     CreateInvitationsResponseTypeDef,
     CreateMemberResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DescribeBucketsResponseTypeDef,
     DescribeClassificationJobResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    FindingCriteriaOutputTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetAllowListResponseTypeDef,
     GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     GetClassificationScopeResponseTypeDef,
@@ -87,16 +86,15 @@
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
     GetUsageStatisticsResponseTypeDef,
     GetUsageTotalsResponseTypeDef,
-    JobScheduleFrequencyOutputTypeDef,
-    JobScheduleFrequencyTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
@@ -108,24 +106,21 @@
     ListResourceProfileArtifactsResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
     RevealConfigurationTypeDef,
     S3ClassificationScopeUpdateTypeDef,
-    S3JobDefinitionOutputTypeDef,
-    S3JobDefinitionTypeDef,
+    S3JobDefinitionUnionTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     SearchResourcesResponseTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SecurityHubConfigurationTypeDef,
-    SensitivityInspectionTemplateExcludesOutputTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesOutputTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
     SeverityLevelTypeDef,
     SortCriteriaTypeDef,
     SuppressDataIdentifierTypeDef,
     TestCustomDataIdentifierResponseTypeDef,
     UpdateAllowListResponseTypeDef,
     UpdateFindingsFilterResponseTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
@@ -235,25 +230,23 @@
 
     def create_classification_job(
         self,
         *,
         clientToken: str,
         jobType: JobTypeType,
         name: str,
-        s3JobDefinition: Union[S3JobDefinitionTypeDef, S3JobDefinitionOutputTypeDef],
+        s3JobDefinition: S3JobDefinitionUnionTypeDef,
         allowListIds: Sequence[str] = ...,
         customDataIdentifierIds: Sequence[str] = ...,
         description: str = ...,
         initialRun: bool = ...,
         managedDataIdentifierIds: Sequence[str] = ...,
         managedDataIdentifierSelector: ManagedDataIdentifierSelectorType = ...,
         samplingPercentage: int = ...,
-        scheduleFrequency: Union[
-            JobScheduleFrequencyTypeDef, JobScheduleFrequencyOutputTypeDef
-        ] = ...,
+        scheduleFrequency: JobScheduleFrequencyUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateClassificationJobResponseTypeDef:
         """
         Creates and defines the settings for a classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_classification_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#create_classification_job)
@@ -280,15 +273,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#create_custom_data_identifier)
         """
 
     def create_findings_filter(
         self,
         *,
         action: FindingsFilterActionType,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef],
+        findingCriteria: FindingCriteriaUnionTypeDef,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         position: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFindingsFilterResponseTypeDef:
         """
@@ -564,15 +557,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#get_custom_data_identifier)
         """
 
     def get_finding_statistics(
         self,
         *,
         groupBy: GroupByType,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         size: int = ...,
         sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...
     ) -> GetFindingStatisticsResponseTypeDef:
         """
         Retrieves (queries) aggregated statistical data about findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_finding_statistics)
@@ -759,15 +752,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_custom_data_identifiers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#list_custom_data_identifiers)
         """
 
     def list_findings(
         self,
         *,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a subset of information about one or more findings.
 
@@ -985,15 +978,15 @@
     def update_findings_filter(
         self,
         *,
         id: str,
         action: FindingsFilterActionType = ...,
         clientToken: str = ...,
         description: str = ...,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         name: str = ...,
         position: int = ...
     ) -> UpdateFindingsFilterResponseTypeDef:
         """
         Updates the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_findings_filter)
@@ -1067,22 +1060,16 @@
         """
 
     def update_sensitivity_inspection_template(
         self,
         *,
         id: str,
         description: str = ...,
-        excludes: Union[
-            SensitivityInspectionTemplateExcludesTypeDef,
-            SensitivityInspectionTemplateExcludesOutputTypeDef,
-        ] = ...,
-        includes: Union[
-            SensitivityInspectionTemplateIncludesTypeDef,
-            SensitivityInspectionTemplateIncludesOutputTypeDef,
-        ] = ...
+        excludes: SensitivityInspectionTemplateExcludesUnionTypeDef = ...,
+        includes: SensitivityInspectionTemplateIncludesUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the settings for the sensitivity inspection template for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_sensitivity_inspection_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#update_sensitivity_inspection_template)
         """
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/client.pyi` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_macie2.client import Macie2Client
 
     session = Session()
     client: Macie2Client = session.client("macie2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutomatedDiscoveryStatusType,
     FindingPublishingFrequencyType,
     FindingsFilterActionType,
@@ -62,16 +62,15 @@
     CreateInvitationsResponseTypeDef,
     CreateMemberResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DescribeBucketsResponseTypeDef,
     DescribeClassificationJobResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    FindingCriteriaOutputTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetAllowListResponseTypeDef,
     GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     GetClassificationScopeResponseTypeDef,
@@ -87,16 +86,15 @@
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
     GetUsageStatisticsResponseTypeDef,
     GetUsageTotalsResponseTypeDef,
-    JobScheduleFrequencyOutputTypeDef,
-    JobScheduleFrequencyTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
@@ -108,24 +106,21 @@
     ListResourceProfileArtifactsResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
     RevealConfigurationTypeDef,
     S3ClassificationScopeUpdateTypeDef,
-    S3JobDefinitionOutputTypeDef,
-    S3JobDefinitionTypeDef,
+    S3JobDefinitionUnionTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     SearchResourcesResponseTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SecurityHubConfigurationTypeDef,
-    SensitivityInspectionTemplateExcludesOutputTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesOutputTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
     SeverityLevelTypeDef,
     SortCriteriaTypeDef,
     SuppressDataIdentifierTypeDef,
     TestCustomDataIdentifierResponseTypeDef,
     UpdateAllowListResponseTypeDef,
     UpdateFindingsFilterResponseTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
@@ -225,25 +220,23 @@
         """
     def create_classification_job(
         self,
         *,
         clientToken: str,
         jobType: JobTypeType,
         name: str,
-        s3JobDefinition: Union[S3JobDefinitionTypeDef, S3JobDefinitionOutputTypeDef],
+        s3JobDefinition: S3JobDefinitionUnionTypeDef,
         allowListIds: Sequence[str] = ...,
         customDataIdentifierIds: Sequence[str] = ...,
         description: str = ...,
         initialRun: bool = ...,
         managedDataIdentifierIds: Sequence[str] = ...,
         managedDataIdentifierSelector: ManagedDataIdentifierSelectorType = ...,
         samplingPercentage: int = ...,
-        scheduleFrequency: Union[
-            JobScheduleFrequencyTypeDef, JobScheduleFrequencyOutputTypeDef
-        ] = ...,
+        scheduleFrequency: JobScheduleFrequencyUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateClassificationJobResponseTypeDef:
         """
         Creates and defines the settings for a classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_classification_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#create_classification_job)
@@ -268,15 +261,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_custom_data_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#create_custom_data_identifier)
         """
     def create_findings_filter(
         self,
         *,
         action: FindingsFilterActionType,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef],
+        findingCriteria: FindingCriteriaUnionTypeDef,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         position: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFindingsFilterResponseTypeDef:
         """
@@ -524,15 +517,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_custom_data_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#get_custom_data_identifier)
         """
     def get_finding_statistics(
         self,
         *,
         groupBy: GroupByType,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         size: int = ...,
         sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...
     ) -> GetFindingStatisticsResponseTypeDef:
         """
         Retrieves (queries) aggregated statistical data about findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_finding_statistics)
@@ -700,15 +693,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_custom_data_identifiers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#list_custom_data_identifiers)
         """
     def list_findings(
         self,
         *,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a subset of information about one or more findings.
 
@@ -906,15 +899,15 @@
     def update_findings_filter(
         self,
         *,
         id: str,
         action: FindingsFilterActionType = ...,
         clientToken: str = ...,
         description: str = ...,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         name: str = ...,
         position: int = ...
     ) -> UpdateFindingsFilterResponseTypeDef:
         """
         Updates the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_findings_filter)
@@ -981,22 +974,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#update_reveal_configuration)
         """
     def update_sensitivity_inspection_template(
         self,
         *,
         id: str,
         description: str = ...,
-        excludes: Union[
-            SensitivityInspectionTemplateExcludesTypeDef,
-            SensitivityInspectionTemplateExcludesOutputTypeDef,
-        ] = ...,
-        includes: Union[
-            SensitivityInspectionTemplateIncludesTypeDef,
-            SensitivityInspectionTemplateIncludesOutputTypeDef,
-        ] = ...
+        excludes: SensitivityInspectionTemplateExcludesUnionTypeDef = ...,
+        includes: SensitivityInspectionTemplateIncludesUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the settings for the sensitivity inspection template for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_sensitivity_inspection_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/client/#update_sensitivity_inspection_template)
         """
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/literals.py` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/literals.pyi` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/paginator.py` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,25 +45,24 @@
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_resource_profile_artifacts_paginator: ListResourceProfileArtifactsPaginator = client.get_paginator("list_resource_profile_artifacts")
     list_resource_profile_detections_paginator: ListResourceProfileDetectionsPaginator = client.get_paginator("list_resource_profile_detections")
     list_sensitivity_inspection_templates_paginator: ListSensitivityInspectionTemplatesPaginator = client.get_paginator("list_sensitivity_inspection_templates")
     search_resources_paginator: SearchResourcesPaginator = client.get_paginator("search_resources")
     ```
 """
-from typing import Generic, Iterator, Mapping, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Mapping, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import TimeRangeType
 from .type_defs import (
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketSortCriteriaTypeDef,
     DescribeBucketsResponseTypeDef,
-    FindingCriteriaOutputTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -223,15 +222,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/paginator.pyi` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -45,25 +45,24 @@
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_resource_profile_artifacts_paginator: ListResourceProfileArtifactsPaginator = client.get_paginator("list_resource_profile_artifacts")
     list_resource_profile_detections_paginator: ListResourceProfileDetectionsPaginator = client.get_paginator("list_resource_profile_detections")
     list_sensitivity_inspection_templates_paginator: ListSensitivityInspectionTemplatesPaginator = client.get_paginator("list_sensitivity_inspection_templates")
     search_resources_paginator: SearchResourcesPaginator = client.get_paginator("search_resources")
     ```
 """
-from typing import Generic, Iterator, Mapping, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Mapping, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import TimeRangeType
 from .type_defs import (
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketSortCriteriaTypeDef,
     DescribeBucketsResponseTypeDef,
-    FindingCriteriaOutputTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -214,15 +213,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        findingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/type_defs.py` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_macie2.type_defs import AcceptInvitationRequestRequestTypeDef
 
-    data: AcceptInvitationRequestRequestTypeDef = {...}
+    data: AcceptInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
     AllowListStatusCodeType,
     AllowsUnencryptedObjectUploadsType,
     AutomatedDiscoveryStatusType,
     AvailabilityCodeType,
@@ -297,14 +297,16 @@
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
+    "SensitivityInspectionTemplateExcludesUnionTypeDef",
+    "SensitivityInspectionTemplateIncludesUnionTypeDef",
     "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
     "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
     "TagScopeTermOutputTypeDef",
@@ -316,18 +318,20 @@
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     "PutClassificationExportConfigurationResponseTypeDef",
     "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
+    "FindingCriteriaUnionTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
+    "JobScheduleFrequencyUnionTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     "ListClassificationJobsRequestRequestTypeDef",
     "OccurrencesTypeDef",
     "GetClassificationScopeResponseTypeDef",
     "UpdateClassificationScopeRequestRequestTypeDef",
     "SearchResourcesCriteriaTypeDef",
     "UsageRecordTypeDef",
@@ -367,14 +371,15 @@
     "JobSummaryTypeDef",
     "S3JobDefinitionOutputTypeDef",
     "S3JobDefinitionTypeDef",
     "ClassificationDetailsTypeDef",
     "ListClassificationJobsResponseTypeDef",
     "DescribeClassificationJobResponseTypeDef",
     "CreateClassificationJobRequestRequestTypeDef",
+    "S3JobDefinitionUnionTypeDef",
     "FindingTypeDef",
     "GetFindingsResponseTypeDef",
 )
 
 _RequiredAcceptInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptInvitationRequestRequestTypeDef",
     {
@@ -2678,14 +2683,20 @@
     {
         "comparator": SearchResourcesComparatorType,
         "tagValues": Sequence[SearchResourcesTagCriterionPairTypeDef],
     },
     total=False,
 )
 
+SensitivityInspectionTemplateExcludesUnionTypeDef = Union[
+    SensitivityInspectionTemplateExcludesTypeDef, SensitivityInspectionTemplateExcludesOutputTypeDef
+]
+SensitivityInspectionTemplateIncludesUnionTypeDef = Union[
+    SensitivityInspectionTemplateIncludesTypeDef, SensitivityInspectionTemplateIncludesOutputTypeDef
+]
 _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
@@ -2952,14 +2963,15 @@
 class CreateFindingsFilterRequestRequestTypeDef(
     _RequiredCreateFindingsFilterRequestRequestTypeDef,
     _OptionalCreateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
 
+FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingStatisticsRequestRequestTypeDef",
     {
         "groupBy": GroupByType,
     },
 )
 _OptionalGetFindingStatisticsRequestRequestTypeDef = TypedDict(
@@ -3024,14 +3036,17 @@
 class UpdateFindingsFilterRequestRequestTypeDef(
     _RequiredUpdateFindingsFilterRequestRequestTypeDef,
     _OptionalUpdateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
 
+JobScheduleFrequencyUnionTypeDef = Union[
+    JobScheduleFrequencyTypeDef, JobScheduleFrequencyOutputTypeDef
+]
 ListClassificationJobsRequestListClassificationJobsPaginateTypeDef = TypedDict(
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     {
         "filterCriteria": ListJobsFilterCriteriaTypeDef,
         "sortCriteria": ListJobsSortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3573,14 +3588,15 @@
 class CreateClassificationJobRequestRequestTypeDef(
     _RequiredCreateClassificationJobRequestRequestTypeDef,
     _OptionalCreateClassificationJobRequestRequestTypeDef,
 ):
     pass
 
 
+S3JobDefinitionUnionTypeDef = Union[S3JobDefinitionTypeDef, S3JobDefinitionOutputTypeDef]
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "accountId": str,
         "archived": bool,
         "category": FindingCategoryType,
         "classificationDetails": ClassificationDetailsTypeDef,
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/type_defs.pyi` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_macie2.type_defs import AcceptInvitationRequestRequestTypeDef
 
-    data: AcceptInvitationRequestRequestTypeDef = {...}
+    data: AcceptInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
     AllowListStatusCodeType,
     AllowsUnencryptedObjectUploadsType,
     AutomatedDiscoveryStatusType,
     AvailabilityCodeType,
@@ -296,14 +296,16 @@
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
+    "SensitivityInspectionTemplateExcludesUnionTypeDef",
+    "SensitivityInspectionTemplateIncludesUnionTypeDef",
     "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
     "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
     "TagScopeTermOutputTypeDef",
@@ -315,18 +317,20 @@
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     "PutClassificationExportConfigurationResponseTypeDef",
     "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
+    "FindingCriteriaUnionTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
+    "JobScheduleFrequencyUnionTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     "ListClassificationJobsRequestRequestTypeDef",
     "OccurrencesTypeDef",
     "GetClassificationScopeResponseTypeDef",
     "UpdateClassificationScopeRequestRequestTypeDef",
     "SearchResourcesCriteriaTypeDef",
     "UsageRecordTypeDef",
@@ -366,14 +370,15 @@
     "JobSummaryTypeDef",
     "S3JobDefinitionOutputTypeDef",
     "S3JobDefinitionTypeDef",
     "ClassificationDetailsTypeDef",
     "ListClassificationJobsResponseTypeDef",
     "DescribeClassificationJobResponseTypeDef",
     "CreateClassificationJobRequestRequestTypeDef",
+    "S3JobDefinitionUnionTypeDef",
     "FindingTypeDef",
     "GetFindingsResponseTypeDef",
 )
 
 _RequiredAcceptInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptInvitationRequestRequestTypeDef",
     {
@@ -2641,14 +2646,20 @@
     {
         "comparator": SearchResourcesComparatorType,
         "tagValues": Sequence[SearchResourcesTagCriterionPairTypeDef],
     },
     total=False,
 )
 
+SensitivityInspectionTemplateExcludesUnionTypeDef = Union[
+    SensitivityInspectionTemplateExcludesTypeDef, SensitivityInspectionTemplateExcludesOutputTypeDef
+]
+SensitivityInspectionTemplateIncludesUnionTypeDef = Union[
+    SensitivityInspectionTemplateIncludesTypeDef, SensitivityInspectionTemplateIncludesOutputTypeDef
+]
 _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
@@ -2905,14 +2916,15 @@
 
 class CreateFindingsFilterRequestRequestTypeDef(
     _RequiredCreateFindingsFilterRequestRequestTypeDef,
     _OptionalCreateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
+FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingStatisticsRequestRequestTypeDef",
     {
         "groupBy": GroupByType,
     },
 )
 _OptionalGetFindingStatisticsRequestRequestTypeDef = TypedDict(
@@ -2973,14 +2985,17 @@
 
 class UpdateFindingsFilterRequestRequestTypeDef(
     _RequiredUpdateFindingsFilterRequestRequestTypeDef,
     _OptionalUpdateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
+JobScheduleFrequencyUnionTypeDef = Union[
+    JobScheduleFrequencyTypeDef, JobScheduleFrequencyOutputTypeDef
+]
 ListClassificationJobsRequestListClassificationJobsPaginateTypeDef = TypedDict(
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     {
         "filterCriteria": ListJobsFilterCriteriaTypeDef,
         "sortCriteria": ListJobsSortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3518,14 +3533,15 @@
 
 class CreateClassificationJobRequestRequestTypeDef(
     _RequiredCreateClassificationJobRequestRequestTypeDef,
     _OptionalCreateClassificationJobRequestRequestTypeDef,
 ):
     pass
 
+S3JobDefinitionUnionTypeDef = Union[S3JobDefinitionTypeDef, S3JobDefinitionOutputTypeDef]
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "accountId": str,
         "archived": bool,
         "category": FindingCategoryType,
         "classificationDetails": ClassificationDetailsTypeDef,
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/waiter.py` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2/waiter.pyi` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2.egg-info/PKG-INFO` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Macie2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Macie2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 macie2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 macie2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie2)](https://pepy.tech/project/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -453,20 +453,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_macie2.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
@@ -684,14 +684,16 @@
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
     UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
     TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
     TagScopeTermOutputTypeDef,
@@ -703,18 +705,20 @@
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     PutClassificationExportConfigurationRequestRequestTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
     GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
     ListClassificationJobsRequestRequestTypeDef,
     OccurrencesTypeDef,
     GetClassificationScopeResponseTypeDef,
     UpdateClassificationScopeRequestRequestTypeDef,
     SearchResourcesCriteriaTypeDef,
     UsageRecordTypeDef,
@@ -754,20 +758,21 @@
     JobSummaryTypeDef,
     S3JobDefinitionOutputTypeDef,
     S3JobDefinitionTypeDef,
     ClassificationDetailsTypeDef,
     ListClassificationJobsResponseTypeDef,
     DescribeClassificationJobResponseTypeDef,
     CreateClassificationJobRequestRequestTypeDef,
+    S3JobDefinitionUnionTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptInvitationRequestRequestTypeDef:
+def get_value() -> AcceptInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-macie2-1.28.15.post1/mypy_boto3_macie2.egg-info/SOURCES.txt` & `mypy-boto3-macie2-1.28.16/mypy_boto3_macie2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.15.post1/setup.py` & `mypy-boto3-macie2-1.28.16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-macie2",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_macie2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Macie2 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Macie2 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 macie2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 macie2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_macie2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

