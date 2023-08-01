# Comparing `tmp/mypy-boto3-guardduty-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-guardduty-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-guardduty-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:14 2023, max compression
+gzip compressed data, was "mypy-boto3-guardduty-1.28.16.tar", last modified: Tue Aug  1 11:36:54 2023, max compression
```

## Comparing `mypy-boto3-guardduty-1.28.15.post1.tar` & `mypy-boto3-guardduty-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25973 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50024 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49939 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    94150 2023-07-29 09:46:49.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94063 2023-07-29 09:46:47.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25973 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:54.252877 mypy-boto3-guardduty-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:23.000000 mypy-boto3-guardduty-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-08-01 11:36:54.248877 mypy-boto3-guardduty-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24542 2023-08-01 11:19:23.000000 mypy-boto3-guardduty-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:54.236877 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-08-01 11:19:23.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-01 11:19:23.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:19:23.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49767 2023-08-01 11:19:24.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49682 2023-08-01 11:19:23.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-08-01 11:19:24.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-08-01 11:19:24.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-08-01 11:19:24.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-08-01 11:19:24.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:23.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94431 2023-08-01 11:19:29.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94344 2023-08-01 11:19:25.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:23.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:54.248877 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-08-01 11:36:54.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:36:54.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:54.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:54.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:54.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:36:54.000000 mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:54.252877 mypy-boto3-guardduty-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:19:23.000000 mypy-boto3-guardduty-1.28.16/setup.py
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/LICENSE` & `mypy-boto3-guardduty-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15.post1/PKG-INFO` & `mypy-boto3-guardduty-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GuardDuty 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 guardduty type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 guardduty type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
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
@@ -381,20 +381,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_guardduty.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_guardduty.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccessKeyDetailsTypeDef,
@@ -615,14 +615,15 @@
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
     CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
     GetFilterResponseTypeDef,
     CreateFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
@@ -661,14 +662,15 @@
     CreateDetectorRequestRequestTypeDef,
     UpdateDetectorRequestRequestTypeDef,
     UpdateMemberDetectorsRequestRequestTypeDef,
     OrganizationDataSourceConfigurationsResultTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     PortProbeActionTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     UpdateMalwareScanSettingsRequestRequestTypeDef,
     ScanDetectionsTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListCoverageResponseTypeDef,
     S3BucketDetailTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetDetectorResponseTypeDef,
@@ -682,15 +684,15 @@
     GetMemberDetectorsResponseTypeDef,
     ServiceTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/README.md` & `mypy-boto3-guardduty-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
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
@@ -349,20 +349,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_guardduty.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_guardduty.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccessKeyDetailsTypeDef,
@@ -583,14 +583,15 @@
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
     CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
     GetFilterResponseTypeDef,
     CreateFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
@@ -629,14 +630,15 @@
     CreateDetectorRequestRequestTypeDef,
     UpdateDetectorRequestRequestTypeDef,
     UpdateMemberDetectorsRequestRequestTypeDef,
     OrganizationDataSourceConfigurationsResultTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     PortProbeActionTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     UpdateMalwareScanSettingsRequestRequestTypeDef,
     ScanDetectionsTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListCoverageResponseTypeDef,
     S3BucketDetailTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetDetectorResponseTypeDef,
@@ -650,15 +652,15 @@
     GetMemberDetectorsResponseTypeDef,
     ServiceTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__init__.py` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__init__.pyi` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__main__.py` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GuardDuty 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.GuardDuty 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\nOther"
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

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/client.py` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_guardduty.client import GuardDutyClient
 
     session = Session()
     client: GuardDutyClient = session.client("guardduty")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableMembersType,
     CoverageStatisticsTypeType,
     EbsSnapshotPreservationType,
@@ -58,16 +58,15 @@
     DescribeMalwareScansResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaOutputTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
@@ -90,16 +89,15 @@
     ListOrganizationAdminAccountsResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
-    ScanResourceCriteriaOutputTypeDef,
-    ScanResourceCriteriaTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     SortCriteriaTypeDef,
     StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     UsageCriteriaTypeDef,
@@ -210,15 +208,15 @@
         """
 
     def create_filter(
         self,
         *,
         DetectorId: str,
         Name: str,
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef],
+        FindingCriteria: FindingCriteriaUnionTypeDef,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
@@ -525,15 +523,15 @@
         """
 
     def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_findings_statistics)
         """
@@ -686,15 +684,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_filters)
         """
 
     def list_findings(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
@@ -850,15 +848,15 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_filter)
         """
@@ -894,17 +892,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_ip_set)
         """
 
     def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
-        ScanResourceCriteria: Union[
-            ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
-        ] = ...,
+        ScanResourceCriteria: ScanResourceCriteriaUnionTypeDef = ...,
         EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_malware_scan_settings)
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/client.pyi` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_guardduty.client import GuardDutyClient
 
     session = Session()
     client: GuardDutyClient = session.client("guardduty")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableMembersType,
     CoverageStatisticsTypeType,
     EbsSnapshotPreservationType,
@@ -58,16 +58,15 @@
     DescribeMalwareScansResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaOutputTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
@@ -90,16 +89,15 @@
     ListOrganizationAdminAccountsResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
-    ScanResourceCriteriaOutputTypeDef,
-    ScanResourceCriteriaTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     SortCriteriaTypeDef,
     StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     UsageCriteriaTypeDef,
@@ -199,15 +197,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#create_detector)
         """
     def create_filter(
         self,
         *,
         DetectorId: str,
         Name: str,
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef],
+        FindingCriteria: FindingCriteriaUnionTypeDef,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
@@ -486,15 +484,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_findings)
         """
     def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_findings_statistics)
         """
@@ -633,15 +631,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_filters)
         """
     def list_findings(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
@@ -782,15 +780,15 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_filter)
         """
@@ -823,17 +821,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_ip_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_ip_set)
         """
     def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
-        ScanResourceCriteria: Union[
-            ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
-        ] = ...,
+        ScanResourceCriteria: ScanResourceCriteriaUnionTypeDef = ...,
         EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_malware_scan_settings)
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/literals.py` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/literals.pyi` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/paginator.py` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,24 @@
     list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_threat_intel_sets_paginator: ListThreatIntelSetsPaginator = client.get_paginator("list_threat_intel_sets")
     ```
 """
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     CoverageFilterCriteriaTypeDef,
     CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaOutputTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
@@ -161,15 +160,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/paginator.pyi` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,24 @@
     list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_threat_intel_sets_paginator: ListThreatIntelSetsPaginator = client.get_paginator("list_threat_intel_sets")
     ```
 """
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     CoverageFilterCriteriaTypeDef,
     CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaOutputTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
@@ -154,15 +153,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/type_defs.py` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_guardduty.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
-    data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
+    data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
     AutoEnableMembersType,
     CoverageFilterCriterionKeyType,
     CoverageSortKeyType,
     CoverageStatisticsTypeType,
@@ -281,14 +281,15 @@
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
     "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
     "GetFilterResponseTypeDef",
     "CreateFilterRequestRequestTypeDef",
+    "FindingCriteriaUnionTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
@@ -327,14 +328,15 @@
     "CreateDetectorRequestRequestTypeDef",
     "UpdateDetectorRequestRequestTypeDef",
     "UpdateMemberDetectorsRequestRequestTypeDef",
     "OrganizationDataSourceConfigurationsResultTypeDef",
     "OrganizationDataSourceConfigurationsTypeDef",
     "PortProbeActionTypeDef",
     "GetMalwareScanSettingsResponseTypeDef",
+    "ScanResourceCriteriaUnionTypeDef",
     "UpdateMalwareScanSettingsRequestRequestTypeDef",
     "ScanDetectionsTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "ListCoverageResponseTypeDef",
     "S3BucketDetailTypeDef",
     "GetRemainingFreeTrialDaysResponseTypeDef",
     "GetDetectorResponseTypeDef",
@@ -2743,14 +2745,15 @@
 
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
 
+FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingStatisticTypes": Sequence[Literal["COUNT_BY_SEVERITY"]],
     },
 )
@@ -3453,14 +3456,17 @@
     {
         "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ScanResourceCriteriaUnionTypeDef = Union[
+    ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
+]
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/type_defs.pyi` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_guardduty.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
-    data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
+    data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
     AutoEnableMembersType,
     CoverageFilterCriterionKeyType,
     CoverageSortKeyType,
     CoverageStatisticsTypeType,
@@ -280,14 +280,15 @@
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
     "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
     "GetFilterResponseTypeDef",
     "CreateFilterRequestRequestTypeDef",
+    "FindingCriteriaUnionTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
@@ -326,14 +327,15 @@
     "CreateDetectorRequestRequestTypeDef",
     "UpdateDetectorRequestRequestTypeDef",
     "UpdateMemberDetectorsRequestRequestTypeDef",
     "OrganizationDataSourceConfigurationsResultTypeDef",
     "OrganizationDataSourceConfigurationsTypeDef",
     "PortProbeActionTypeDef",
     "GetMalwareScanSettingsResponseTypeDef",
+    "ScanResourceCriteriaUnionTypeDef",
     "UpdateMalwareScanSettingsRequestRequestTypeDef",
     "ScanDetectionsTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "ListCoverageResponseTypeDef",
     "S3BucketDetailTypeDef",
     "GetRemainingFreeTrialDaysResponseTypeDef",
     "GetDetectorResponseTypeDef",
@@ -2692,14 +2694,15 @@
 )
 
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
+FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingStatisticTypes": Sequence[Literal["COUNT_BY_SEVERITY"]],
     },
 )
@@ -3374,14 +3377,17 @@
     {
         "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ScanResourceCriteriaUnionTypeDef = Union[
+    ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
+]
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/PKG-INFO` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GuardDuty 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 guardduty type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 guardduty type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
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
@@ -381,20 +381,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_guardduty.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_guardduty.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccessKeyDetailsTypeDef,
@@ -615,14 +615,15 @@
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
     CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
     GetFilterResponseTypeDef,
     CreateFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
@@ -661,14 +662,15 @@
     CreateDetectorRequestRequestTypeDef,
     UpdateDetectorRequestRequestTypeDef,
     UpdateMemberDetectorsRequestRequestTypeDef,
     OrganizationDataSourceConfigurationsResultTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     PortProbeActionTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     UpdateMalwareScanSettingsRequestRequestTypeDef,
     ScanDetectionsTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListCoverageResponseTypeDef,
     S3BucketDetailTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetDetectorResponseTypeDef,
@@ -682,15 +684,15 @@
     GetMemberDetectorsResponseTypeDef,
     ServiceTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/SOURCES.txt` & `mypy-boto3-guardduty-1.28.16/mypy_boto3_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15.post1/setup.py` & `mypy-boto3-guardduty-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-guardduty",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.GuardDuty 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 guardduty type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 guardduty type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_guardduty": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

