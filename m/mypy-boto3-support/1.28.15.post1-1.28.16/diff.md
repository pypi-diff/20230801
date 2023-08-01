# Comparing `tmp/mypy-boto3-support-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-support-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-support-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:19 2023, max compression
+gzip compressed data, was "mypy-boto3-support-1.28.16.tar", last modified: Tue Aug  1 11:37:58 2023, max compression
```

## Comparing `mypy-boto3-support-1.28.15.post1.tar` & `mypy-boto3-support-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.565433 mypy-boto3-support-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-07-29 10:04:19.561433 mypy-boto3-support-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.557433 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-29 10:00:36.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-07-29 10:00:36.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-29 10:00:36.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.561433 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:19.565433 mypy-boto3-support-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:58.744711 mypy-boto3-support-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-08-01 11:37:58.740712 mypy-boto3-support-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:58.728711 mypy-boto3-support-1.28.16/mypy_boto3_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-08-01 11:34:12.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-08-01 11:34:12.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-08-01 11:34:12.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-08-01 11:34:12.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/mypy_boto3_support/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:58.740712 mypy-boto3-support-1.28.16/mypy_boto3_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-08-01 11:37:58.000000 mypy-boto3-support-1.28.16/mypy_boto3_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:37:58.000000 mypy-boto3-support-1.28.16/mypy_boto3_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:58.000000 mypy-boto3-support-1.28.16/mypy_boto3_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:58.000000 mypy-boto3-support-1.28.16/mypy_boto3_support.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:58.000000 mypy-boto3-support-1.28.16/mypy_boto3_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:37:58.000000 mypy-boto3-support-1.28.16/mypy_boto3_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:58.744711 mypy-boto3-support-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:34:11.000000 mypy-boto3-support-1.28.16/setup.py
```

### Comparing `mypy-boto3-support-1.28.15.post1/LICENSE` & `mypy-boto3-support-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15.post1/PKG-INFO` & `mypy-boto3-support-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Support 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Support 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 support type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 support type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-support)](https://pepy.tech/project/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
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
@@ -312,28 +312,28 @@
 )
 
 
 def check_value(value: DescribeCasesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
-    AttachmentOutputTypeDef,
-    AttachmentTypeDef,
     ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
     AttachmentDetailsTypeDef,
+    AttachmentOutputTypeDef,
+    BlobTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
@@ -351,45 +351,47 @@
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
-    AddAttachmentsToSetRequestRequestTypeDef,
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
     CreateCaseResponseTypeDef,
-    DescribeAttachmentResponseTypeDef,
     ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
+    DescribeAttachmentResponseTypeDef,
+    AttachmentTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
     DescribeCasesRequestDescribeCasesPaginateTypeDef,
     DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
     RecentCaseCommunicationsTypeDef,
+    AttachmentUnionTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     TrustedAdvisorCheckResultTypeDef,
     TrustedAdvisorCheckSummaryTypeDef,
     CaseDetailsTypeDef,
+    AddAttachmentsToSetRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentOutputTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-support-1.28.15.post1/README.md` & `mypy-boto3-support-1.28.16/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-support)](https://pepy.tech/project/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
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
@@ -280,28 +280,28 @@
 )
 
 
 def check_value(value: DescribeCasesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
-    AttachmentOutputTypeDef,
-    AttachmentTypeDef,
     ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
     AttachmentDetailsTypeDef,
+    AttachmentOutputTypeDef,
+    BlobTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
@@ -319,45 +319,47 @@
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
-    AddAttachmentsToSetRequestRequestTypeDef,
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
     CreateCaseResponseTypeDef,
-    DescribeAttachmentResponseTypeDef,
     ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
+    DescribeAttachmentResponseTypeDef,
+    AttachmentTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
     DescribeCasesRequestDescribeCasesPaginateTypeDef,
     DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
     RecentCaseCommunicationsTypeDef,
+    AttachmentUnionTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     TrustedAdvisorCheckResultTypeDef,
     TrustedAdvisorCheckSummaryTypeDef,
     CaseDetailsTypeDef,
+    AddAttachmentsToSetRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentOutputTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__init__.py` & `mypy-boto3-support-1.28.16/mypy_boto3_support/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__init__.pyi` & `mypy-boto3-support-1.28.16/mypy_boto3_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__main__.py` & `mypy-boto3-support-1.28.16/mypy_boto3_support/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Support 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Support 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
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

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/client.py` & `mypy-boto3-support-1.28.16/mypy_boto3_support/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,23 @@
     from mypy_boto3_support.client import SupportClient
 
     session = Session()
     client: SupportClient = session.client("support")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
-    AttachmentOutputTypeDef,
-    AttachmentTypeDef,
+    AttachmentUnionTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
@@ -85,18 +84,15 @@
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#exceptions)
         """
 
     def add_attachments_to_set(
-        self,
-        *,
-        attachments: Sequence[Union[AttachmentTypeDef, AttachmentOutputTypeDef]],
-        attachmentSetId: str = ...
+        self, *, attachments: Sequence[AttachmentUnionTypeDef], attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#add_attachments_to_set)
         """
```

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/client.pyi` & `mypy-boto3-support-1.28.16/mypy_boto3_support/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,23 @@
     from mypy_boto3_support.client import SupportClient
 
     session = Session()
     client: SupportClient = session.client("support")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
-    AttachmentOutputTypeDef,
-    AttachmentTypeDef,
+    AttachmentUnionTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
@@ -80,18 +79,15 @@
         """
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#exceptions)
         """
     def add_attachments_to_set(
-        self,
-        *,
-        attachments: Sequence[Union[AttachmentTypeDef, AttachmentOutputTypeDef]],
-        attachmentSetId: str = ...
+        self, *, attachments: Sequence[AttachmentUnionTypeDef], attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#add_attachments_to_set)
         """
```

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/literals.py` & `mypy-boto3-support-1.28.16/mypy_boto3_support/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/literals.pyi` & `mypy-boto3-support-1.28.16/mypy_boto3_support/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/paginator.py` & `mypy-boto3-support-1.28.16/mypy_boto3_support/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/paginator.pyi` & `mypy-boto3-support-1.28.16/mypy_boto3_support/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/type_defs.py` & `mypy-boto3-support-1.28.16/mypy_boto3_support/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 Type annotations for support service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_support.type_defs import AttachmentOutputTypeDef
+    from mypy_boto3_support.type_defs import ResponseMetadataTypeDef
 
-    data: AttachmentOutputTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AttachmentOutputTypeDef",
-    "AttachmentTypeDef",
     "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
     "AttachmentDetailsTypeDef",
+    "AttachmentOutputTypeDef",
+    "BlobTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeCasesRequestRequestTypeDef",
@@ -49,61 +49,45 @@
     "DescribeTrustedAdvisorChecksRequestRequestTypeDef",
     "TrustedAdvisorCheckDescriptionTypeDef",
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     "ResolveCaseRequestRequestTypeDef",
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
-    "AddAttachmentsToSetRequestRequestTypeDef",
     "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseResponseTypeDef",
     "CreateCaseResponseTypeDef",
-    "DescribeAttachmentResponseTypeDef",
     "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
+    "DescribeAttachmentResponseTypeDef",
+    "AttachmentTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
     "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
+    "AttachmentUnionTypeDef",
     "DescribeServicesResponseTypeDef",
     "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
+    "AddAttachmentsToSetRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
 
-AttachmentOutputTypeDef = TypedDict(
-    "AttachmentOutputTypeDef",
-    {
-        "fileName": str,
-        "data": bytes,
-    },
-    total=False,
-)
-
-AttachmentTypeDef = TypedDict(
-    "AttachmentTypeDef",
-    {
-        "fileName": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -140,14 +124,24 @@
     {
         "attachmentId": str,
         "fileName": str,
     },
     total=False,
 )
 
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
+    {
+        "fileName": str,
+        "data": bytes,
+    },
+    total=False,
+)
+
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": str,
         "name": str,
     },
     total=False,
@@ -428,36 +422,14 @@
         "resourcesProcessed": int,
         "resourcesFlagged": int,
         "resourcesIgnored": int,
         "resourcesSuppressed": int,
     },
 )
 
-_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachments": Sequence[Union[AttachmentTypeDef, AttachmentOutputTypeDef]],
-    },
-)
-_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachmentSetId": str,
-    },
-    total=False,
-)
-
-
-class AddAttachmentsToSetRequestRequestTypeDef(
-    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
-    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
-):
-    pass
-
-
 AddAttachmentsToSetResponseTypeDef = TypedDict(
     "AddAttachmentsToSetResponseTypeDef",
     {
         "attachmentSetId": str,
         "expiryTime": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -475,22 +447,14 @@
     "CreateCaseResponseTypeDef",
     {
         "caseId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
-    {
-        "attachment": AttachmentOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResolveCaseResponseTypeDef = TypedDict(
     "ResolveCaseResponseTypeDef",
     {
         "initialCaseStatus": str,
         "finalCaseStatus": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -504,14 +468,31 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachmentTypeDef = TypedDict(
+    "AttachmentTypeDef",
+    {
+        "fileName": str,
+        "data": BlobTypeDef,
+    },
+    total=False,
+)
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
@@ -629,14 +610,15 @@
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
+AttachmentUnionTypeDef = Union[AttachmentTypeDef, AttachmentOutputTypeDef]
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -702,14 +684,36 @@
         "recentCommunications": RecentCaseCommunicationsTypeDef,
         "ccEmailAddresses": List[str],
         "language": str,
     },
     total=False,
 )
 
+_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachments": Sequence[AttachmentUnionTypeDef],
+    },
+)
+_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachmentSetId": str,
+    },
+    total=False,
+)
+
+
+class AddAttachmentsToSetRequestRequestTypeDef(
+    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
+    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/type_defs.pyi` & `mypy-boto3-support-1.28.16/mypy_boto3_support/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 Type annotations for support service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_support.type_defs import AttachmentOutputTypeDef
+    from mypy_boto3_support.type_defs import ResponseMetadataTypeDef
 
-    data: AttachmentOutputTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AttachmentOutputTypeDef",
-    "AttachmentTypeDef",
     "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
     "AttachmentDetailsTypeDef",
+    "AttachmentOutputTypeDef",
+    "BlobTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeCasesRequestRequestTypeDef",
@@ -48,61 +48,45 @@
     "DescribeTrustedAdvisorChecksRequestRequestTypeDef",
     "TrustedAdvisorCheckDescriptionTypeDef",
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     "ResolveCaseRequestRequestTypeDef",
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
-    "AddAttachmentsToSetRequestRequestTypeDef",
     "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseResponseTypeDef",
     "CreateCaseResponseTypeDef",
-    "DescribeAttachmentResponseTypeDef",
     "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
+    "DescribeAttachmentResponseTypeDef",
+    "AttachmentTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
     "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
+    "AttachmentUnionTypeDef",
     "DescribeServicesResponseTypeDef",
     "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
+    "AddAttachmentsToSetRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
 
-AttachmentOutputTypeDef = TypedDict(
-    "AttachmentOutputTypeDef",
-    {
-        "fileName": str,
-        "data": bytes,
-    },
-    total=False,
-)
-
-AttachmentTypeDef = TypedDict(
-    "AttachmentTypeDef",
-    {
-        "fileName": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -137,14 +121,24 @@
     {
         "attachmentId": str,
         "fileName": str,
     },
     total=False,
 )
 
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
+    {
+        "fileName": str,
+        "data": bytes,
+    },
+    total=False,
+)
+
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": str,
         "name": str,
     },
     total=False,
@@ -417,34 +411,14 @@
         "resourcesProcessed": int,
         "resourcesFlagged": int,
         "resourcesIgnored": int,
         "resourcesSuppressed": int,
     },
 )
 
-_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachments": Sequence[Union[AttachmentTypeDef, AttachmentOutputTypeDef]],
-    },
-)
-_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachmentSetId": str,
-    },
-    total=False,
-)
-
-class AddAttachmentsToSetRequestRequestTypeDef(
-    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
-    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
-):
-    pass
-
 AddAttachmentsToSetResponseTypeDef = TypedDict(
     "AddAttachmentsToSetResponseTypeDef",
     {
         "attachmentSetId": str,
         "expiryTime": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -462,22 +436,14 @@
     "CreateCaseResponseTypeDef",
     {
         "caseId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
-    {
-        "attachment": AttachmentOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResolveCaseResponseTypeDef = TypedDict(
     "ResolveCaseResponseTypeDef",
     {
         "initialCaseStatus": str,
         "finalCaseStatus": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -491,14 +457,31 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachmentTypeDef = TypedDict(
+    "AttachmentTypeDef",
+    {
+        "fileName": str,
+        "data": BlobTypeDef,
+    },
+    total=False,
+)
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
@@ -614,14 +597,15 @@
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
+AttachmentUnionTypeDef = Union[AttachmentTypeDef, AttachmentOutputTypeDef]
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -685,14 +669,34 @@
         "recentCommunications": RecentCaseCommunicationsTypeDef,
         "ccEmailAddresses": List[str],
         "language": str,
     },
     total=False,
 )
 
+_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachments": Sequence[AttachmentUnionTypeDef],
+    },
+)
+_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachmentSetId": str,
+    },
+    total=False,
+)
+
+class AddAttachmentsToSetRequestRequestTypeDef(
+    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
+    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
+):
+    pass
+
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/PKG-INFO` & `mypy-boto3-support-1.28.16/mypy_boto3_support.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Support 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Support 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 support type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 support type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-support)](https://pepy.tech/project/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
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
@@ -312,28 +312,28 @@
 )
 
 
 def check_value(value: DescribeCasesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
-    AttachmentOutputTypeDef,
-    AttachmentTypeDef,
     ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
     AttachmentDetailsTypeDef,
+    AttachmentOutputTypeDef,
+    BlobTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
@@ -351,45 +351,47 @@
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
-    AddAttachmentsToSetRequestRequestTypeDef,
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
     CreateCaseResponseTypeDef,
-    DescribeAttachmentResponseTypeDef,
     ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
+    DescribeAttachmentResponseTypeDef,
+    AttachmentTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
     DescribeCasesRequestDescribeCasesPaginateTypeDef,
     DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
     RecentCaseCommunicationsTypeDef,
+    AttachmentUnionTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     TrustedAdvisorCheckResultTypeDef,
     TrustedAdvisorCheckSummaryTypeDef,
     CaseDetailsTypeDef,
+    AddAttachmentsToSetRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentOutputTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/SOURCES.txt` & `mypy-boto3-support-1.28.16/mypy_boto3_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15.post1/setup.py` & `mypy-boto3-support-1.28.16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-support",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Support 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Support 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 support type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 support type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_support": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

