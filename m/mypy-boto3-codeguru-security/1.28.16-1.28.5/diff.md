# Comparing `tmp/mypy-boto3-codeguru-security-1.28.16.tar.gz` & `tmp/mypy-boto3-codeguru-security-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-security-1.28.16.tar", last modified: Tue Aug  1 11:36:28 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguru-security-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-codeguru-security-1.28.16.tar` & `mypy-boto3-codeguru-security-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.592924 mypy-boto3-codeguru-security-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-08-01 11:36:28.592924 mypy-boto3-codeguru-security-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13541 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.592924 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-08-01 11:13:19.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-08-01 11:13:19.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.592924 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:28.592924 mypy-boto3-codeguru-security-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-security-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.754719 mypy-boto3-codeguru-security-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-18 19:32:41.754719 mypy-boto3-codeguru-security-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.754719 mypy-boto3-codeguru-security-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/setup.py
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/LICENSE` & `mypy-boto3-codeguru-security-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.16/PKG-INFO` & `mypy-boto3-codeguru-security-1.28.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.28.16
-Summary: Type annotations for boto3.CodeGuruSecurity 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.5
+Summary: Type annotations for boto3.CodeGuruSecurity 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codeguru-security type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 codeguru-security type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -326,37 +326,40 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_codeguru_security.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
     ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
+    ResourceIdOutputTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
     PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
-    TimestampTypeDef,
+    GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
+    ListFindingsMetricsRequestRequestTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ScanNameWithFindingNumTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -366,34 +369,32 @@
     CreateUploadUrlResponseTypeDef,
     GetScanResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
+    UpdateAccountConfigurationRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
-    GetMetricsSummaryRequestRequestTypeDef,
     ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListFindingsMetricsRequestRequestTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
     BatchGetFindingsResponseTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_value() -> FindingMetricsValuePerSeverityTypeDef:
+def get_structure() -> FindingMetricsValuePerSeverityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/README.md` & `mypy-boto3-codeguru-security-1.28.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -294,37 +294,40 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_codeguru_security.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
     ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
+    ResourceIdOutputTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
     PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
-    TimestampTypeDef,
+    GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
+    ListFindingsMetricsRequestRequestTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ScanNameWithFindingNumTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -334,34 +337,32 @@
     CreateUploadUrlResponseTypeDef,
     GetScanResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
+    UpdateAccountConfigurationRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
-    GetMetricsSummaryRequestRequestTypeDef,
     ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListFindingsMetricsRequestRequestTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
     BatchGetFindingsResponseTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_value() -> FindingMetricsValuePerSeverityTypeDef:
+def get_structure() -> FindingMetricsValuePerSeverityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/__init__.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/__init__.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/__main__.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruSecurity 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.CodeGuruSecurity 1.28.5\nVersion:         1.28.5\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/client.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_codeguru_security.client import CodeGuruSecurityClient
 
     session = Session()
     client: CodeGuruSecurityClient = session.client("codeguru-security")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AnalysisTypeType, ScanTypeType, StatusType
 from .paginator import GetFindingsPaginator, ListFindingsMetricsPaginator, ListScansPaginator
 from .type_defs import (
     BatchGetFindingsResponseTypeDef,
@@ -30,15 +31,14 @@
     GetFindingsResponseTypeDef,
     GetMetricsSummaryResponseTypeDef,
     GetScanResponseTypeDef,
     ListFindingsMetricsResponseTypeDef,
     ListScansResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ResourceIdTypeDef,
-    TimestampTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -166,15 +166,17 @@
         """
         Returns a list of all findings generated by a particular scan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_findings)
         """
 
-    def get_metrics_summary(self, *, date: TimestampTypeDef) -> GetMetricsSummaryResponseTypeDef:
+    def get_metrics_summary(
+        self, *, date: Union[datetime, str]
+    ) -> GetMetricsSummaryResponseTypeDef:
         """
         Returns top level metrics about an account from a specified date, including
         number of open findings, the categories with most findings, the scans with most
         open findings, and scans with most open critical findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_metrics_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_metrics_summary)
@@ -187,16 +189,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_scan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_scan)
         """
 
     def list_findings_metrics(
         self,
         *,
-        endDate: TimestampTypeDef,
-        startDate: TimestampTypeDef,
+        endDate: Union[datetime, str],
+        startDate: Union[datetime, str],
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFindingsMetricsResponseTypeDef:
         """
         Returns metrics about all findings in an account within a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_findings_metrics)
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/client.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_codeguru_security.client import CodeGuruSecurityClient
 
     session = Session()
     client: CodeGuruSecurityClient = session.client("codeguru-security")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AnalysisTypeType, ScanTypeType, StatusType
 from .paginator import GetFindingsPaginator, ListFindingsMetricsPaginator, ListScansPaginator
 from .type_defs import (
     BatchGetFindingsResponseTypeDef,
@@ -30,15 +31,14 @@
     GetFindingsResponseTypeDef,
     GetMetricsSummaryResponseTypeDef,
     GetScanResponseTypeDef,
     ListFindingsMetricsResponseTypeDef,
     ListScansResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ResourceIdTypeDef,
-    TimestampTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -153,15 +153,17 @@
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of all findings generated by a particular scan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_findings)
         """
-    def get_metrics_summary(self, *, date: TimestampTypeDef) -> GetMetricsSummaryResponseTypeDef:
+    def get_metrics_summary(
+        self, *, date: Union[datetime, str]
+    ) -> GetMetricsSummaryResponseTypeDef:
         """
         Returns top level metrics about an account from a specified date, including
         number of open findings, the categories with most findings, the scans with most
         open findings, and scans with most open critical findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_metrics_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_metrics_summary)
@@ -172,16 +174,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_scan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_scan)
         """
     def list_findings_metrics(
         self,
         *,
-        endDate: TimestampTypeDef,
-        startDate: TimestampTypeDef,
+        endDate: Union[datetime, str],
+        startDate: Union[datetime, str],
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFindingsMetricsResponseTypeDef:
         """
         Returns metrics about all findings in an account within a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_findings_metrics)
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/literals.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -31,15 +30,14 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
@@ -167,15 +165,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -254,28 +251,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/literals.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -30,14 +31,15 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
@@ -165,15 +167,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -252,28 +253,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/paginator.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,25 +19,25 @@
     client: CodeGuruSecurityClient = session.client("codeguru-security")
 
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     list_findings_metrics_paginator: ListFindingsMetricsPaginator = client.get_paginator("list_findings_metrics")
     list_scans_paginator: ListScansPaginator = client.get_paginator("list_scans")
     ```
 """
-from typing import Generic, Iterator, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import StatusType
 from .type_defs import (
     GetFindingsResponseTypeDef,
     ListFindingsMetricsResponseTypeDef,
     ListScansResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = ("GetFindingsPaginator", "ListFindingsMetricsPaginator", "ListScansPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -73,16 +73,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
     """
 
     def paginate(
         self,
         *,
-        endDate: TimestampTypeDef,
-        startDate: TimestampTypeDef,
+        endDate: Union[datetime, str],
+        startDate: Union[datetime, str],
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/paginator.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -19,25 +19,25 @@
     client: CodeGuruSecurityClient = session.client("codeguru-security")
 
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     list_findings_metrics_paginator: ListFindingsMetricsPaginator = client.get_paginator("list_findings_metrics")
     list_scans_paginator: ListScansPaginator = client.get_paginator("list_scans")
     ```
 """
-from typing import Generic, Iterator, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import StatusType
 from .type_defs import (
     GetFindingsResponseTypeDef,
     ListFindingsMetricsResponseTypeDef,
     ListScansResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = ("GetFindingsPaginator", "ListFindingsMetricsPaginator", "ListScansPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -69,16 +69,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
     """
 
     def paginate(
         self,
         *,
-        endDate: TimestampTypeDef,
-        startDate: TimestampTypeDef,
+        endDate: Union[datetime, str],
+        startDate: Union[datetime, str],
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/type_defs.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codeguru_security.type_defs import FindingMetricsValuePerSeverityTypeDef
 
-    data: FindingMetricsValuePerSeverityTypeDef = ...
+    data: FindingMetricsValuePerSeverityTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -34,21 +34,24 @@
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
+    "ResourceIdOutputTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
     "PaginatorConfigTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "TimestampTypeDef",
+    "GetMetricsSummaryRequestRequestTypeDef",
     "GetScanRequestRequestTypeDef",
+    "ListFindingsMetricsRequestRequestTypeDef",
     "ListScansRequestRequestTypeDef",
     "ScanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ScanNameWithFindingNumTypeDef",
     "RecommendationTypeDef",
     "SuggestedFixTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -58,21 +61,19 @@
     "CreateUploadUrlResponseTypeDef",
     "GetScanResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
-    "UpdateAccountConfigurationRequestRequestTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
-    "ListScansRequestListScansPaginateTypeDef",
-    "GetMetricsSummaryRequestRequestTypeDef",
     "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    "ListFindingsMetricsRequestRequestTypeDef",
+    "ListScansRequestListScansPaginateTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
     "VulnerabilityTypeDef",
     "GetMetricsSummaryResponseTypeDef",
     "FindingTypeDef",
@@ -85,15 +86,14 @@
     {
         "critical": float,
         "high": float,
         "info": float,
         "low": float,
         "medium": float,
     },
-    total=False,
 )
 
 BatchGetFindingsErrorTypeDef = TypedDict(
     "BatchGetFindingsErrorTypeDef",
     {
         "errorCode": ErrorCodeType,
         "findingId": str,
@@ -123,56 +123,67 @@
 
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
-    total=False,
 )
 
 CodeLineTypeDef = TypedDict(
     "CodeLineTypeDef",
     {
         "content": str,
         "number": int,
     },
-    total=False,
 )
 
 ResourceIdTypeDef = TypedDict(
     "ResourceIdTypeDef",
     {
         "codeArtifactId": str,
     },
     total=False,
 )
 
+ResourceIdOutputTypeDef = TypedDict(
+    "ResourceIdOutputTypeDef",
+    {
+        "codeArtifactId": str,
+    },
+)
+
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "kmsKeyArn": str,
+    },
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "id": str,
         "subResourceId": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -200,15 +211,21 @@
 
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
 
-TimestampTypeDef = Union[datetime, str]
+GetMetricsSummaryRequestRequestTypeDef = TypedDict(
+    "GetMetricsSummaryRequestRequestTypeDef",
+    {
+        "date": Union[datetime, str],
+    },
+)
+
 _RequiredGetScanRequestRequestTypeDef = TypedDict(
     "_RequiredGetScanRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetScanRequestRequestTypeDef = TypedDict(
@@ -222,78 +239,88 @@
 
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestRequestTypeDef",
+    {
+        "endDate": Union[datetime, str],
+        "startDate": Union[datetime, str],
+    },
+)
+_OptionalListFindingsMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListFindingsMetricsRequestRequestTypeDef(
+    _RequiredListFindingsMetricsRequestRequestTypeDef,
+    _OptionalListFindingsMetricsRequestRequestTypeDef,
+):
+    pass
+
+
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredScanSummaryTypeDef = TypedDict(
-    "_RequiredScanSummaryTypeDef",
+ScanSummaryTypeDef = TypedDict(
+    "ScanSummaryTypeDef",
     {
         "createdAt": datetime,
         "runId": str,
         "scanName": str,
-        "scanState": ScanStateType,
-    },
-)
-_OptionalScanSummaryTypeDef = TypedDict(
-    "_OptionalScanSummaryTypeDef",
-    {
         "scanNameArn": str,
+        "scanState": ScanStateType,
         "updatedAt": datetime,
     },
-    total=False,
 )
 
-
-class ScanSummaryTypeDef(_RequiredScanSummaryTypeDef, _OptionalScanSummaryTypeDef):
-    pass
-
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
     },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
-    total=False,
 )
 
 SuggestedFixTypeDef = TypedDict(
     "SuggestedFixTypeDef",
     {
         "code": str,
         "description": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -313,15 +340,14 @@
     {
         "closedFindings": FindingMetricsValuePerSeverityTypeDef,
         "date": datetime,
         "meanTimeToClose": FindingMetricsValuePerSeverityTypeDef,
         "newFindings": FindingMetricsValuePerSeverityTypeDef,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
@@ -365,15 +391,14 @@
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
         "startLine": int,
     },
-    total=False,
 )
 
 _RequiredCreateScanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScanRequestRequestTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "scanName": str,
@@ -396,43 +421,43 @@
 ):
     pass
 
 
 CreateScanResponseTypeDef = TypedDict(
     "CreateScanResponseTypeDef",
     {
-        "resourceId": ResourceIdTypeDef,
+        "resourceId": ResourceIdOutputTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateAccountConfigurationRequestRequestTypeDef",
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
     {
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountConfigurationResponseTypeDef = TypedDict(
-    "UpdateAccountConfigurationResponseTypeDef",
+UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
     "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
     {
         "scanName": str,
@@ -451,34 +476,19 @@
 class GetFindingsRequestGetFindingsPaginateTypeDef(
     _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
     _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
 ):
     pass
 
 
-ListScansRequestListScansPaginateTypeDef = TypedDict(
-    "ListScansRequestListScansPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetMetricsSummaryRequestRequestTypeDef = TypedDict(
-    "GetMetricsSummaryRequestRequestTypeDef",
-    {
-        "date": TimestampTypeDef,
-    },
-)
-
 _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     {
-        "endDate": TimestampTypeDef,
-        "startDate": TimestampTypeDef,
+        "endDate": Union[datetime, str],
+        "startDate": Union[datetime, str],
     },
 )
 _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -489,38 +499,22 @@
 class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
     _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestRequestTypeDef",
-    {
-        "endDate": TimestampTypeDef,
-        "startDate": TimestampTypeDef,
-    },
-)
-_OptionalListFindingsMetricsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestRequestTypeDef",
+ListScansRequestListScansPaginateTypeDef = TypedDict(
+    "ListScansRequestListScansPaginateTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class ListFindingsMetricsRequestRequestTypeDef(
-    _RequiredListFindingsMetricsRequestRequestTypeDef,
-    _OptionalListFindingsMetricsRequestRequestTypeDef,
-):
-    pass
-
-
 ListScansResponseTypeDef = TypedDict(
     "ListScansResponseTypeDef",
     {
         "nextToken": str,
         "summaries": List[ScanSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -531,24 +525,22 @@
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
         "date": datetime,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
         "scansWithMostOpenCriticalFindings": List[ScanNameWithFindingNumTypeDef],
         "scansWithMostOpenFindings": List[ScanNameWithFindingNumTypeDef],
     },
-    total=False,
 )
 
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
         "suggestedFixes": List[SuggestedFixTypeDef],
     },
-    total=False,
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
@@ -561,15 +553,14 @@
     {
         "filePath": FilePathTypeDef,
         "id": str,
         "itemCount": int,
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
     },
-    total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -592,15 +583,14 @@
         "severity": SeverityType,
         "status": StatusType,
         "title": str,
         "type": str,
         "updatedAt": datetime,
         "vulnerability": VulnerabilityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security/type_defs.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codeguru_security.type_defs import FindingMetricsValuePerSeverityTypeDef
 
-    data: FindingMetricsValuePerSeverityTypeDef = ...
+    data: FindingMetricsValuePerSeverityTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -33,21 +33,24 @@
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
+    "ResourceIdOutputTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
     "PaginatorConfigTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "TimestampTypeDef",
+    "GetMetricsSummaryRequestRequestTypeDef",
     "GetScanRequestRequestTypeDef",
+    "ListFindingsMetricsRequestRequestTypeDef",
     "ListScansRequestRequestTypeDef",
     "ScanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ScanNameWithFindingNumTypeDef",
     "RecommendationTypeDef",
     "SuggestedFixTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -57,21 +60,19 @@
     "CreateUploadUrlResponseTypeDef",
     "GetScanResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
-    "UpdateAccountConfigurationRequestRequestTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
-    "ListScansRequestListScansPaginateTypeDef",
-    "GetMetricsSummaryRequestRequestTypeDef",
     "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    "ListFindingsMetricsRequestRequestTypeDef",
+    "ListScansRequestListScansPaginateTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
     "VulnerabilityTypeDef",
     "GetMetricsSummaryResponseTypeDef",
     "FindingTypeDef",
@@ -84,15 +85,14 @@
     {
         "critical": float,
         "high": float,
         "info": float,
         "low": float,
         "medium": float,
     },
-    total=False,
 )
 
 BatchGetFindingsErrorTypeDef = TypedDict(
     "BatchGetFindingsErrorTypeDef",
     {
         "errorCode": ErrorCodeType,
         "findingId": str,
@@ -122,56 +122,67 @@
 
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
-    total=False,
 )
 
 CodeLineTypeDef = TypedDict(
     "CodeLineTypeDef",
     {
         "content": str,
         "number": int,
     },
-    total=False,
 )
 
 ResourceIdTypeDef = TypedDict(
     "ResourceIdTypeDef",
     {
         "codeArtifactId": str,
     },
     total=False,
 )
 
+ResourceIdOutputTypeDef = TypedDict(
+    "ResourceIdOutputTypeDef",
+    {
+        "codeArtifactId": str,
+    },
+)
+
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "kmsKeyArn": str,
+    },
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "id": str,
         "subResourceId": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -197,15 +208,21 @@
 )
 
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
-TimestampTypeDef = Union[datetime, str]
+GetMetricsSummaryRequestRequestTypeDef = TypedDict(
+    "GetMetricsSummaryRequestRequestTypeDef",
+    {
+        "date": Union[datetime, str],
+    },
+)
+
 _RequiredGetScanRequestRequestTypeDef = TypedDict(
     "_RequiredGetScanRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetScanRequestRequestTypeDef = TypedDict(
@@ -217,76 +234,86 @@
 )
 
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
+_RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestRequestTypeDef",
+    {
+        "endDate": Union[datetime, str],
+        "startDate": Union[datetime, str],
+    },
+)
+_OptionalListFindingsMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListFindingsMetricsRequestRequestTypeDef(
+    _RequiredListFindingsMetricsRequestRequestTypeDef,
+    _OptionalListFindingsMetricsRequestRequestTypeDef,
+):
+    pass
+
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredScanSummaryTypeDef = TypedDict(
-    "_RequiredScanSummaryTypeDef",
+ScanSummaryTypeDef = TypedDict(
+    "ScanSummaryTypeDef",
     {
         "createdAt": datetime,
         "runId": str,
         "scanName": str,
-        "scanState": ScanStateType,
-    },
-)
-_OptionalScanSummaryTypeDef = TypedDict(
-    "_OptionalScanSummaryTypeDef",
-    {
         "scanNameArn": str,
+        "scanState": ScanStateType,
         "updatedAt": datetime,
     },
-    total=False,
 )
 
-class ScanSummaryTypeDef(_RequiredScanSummaryTypeDef, _OptionalScanSummaryTypeDef):
-    pass
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
     },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
-    total=False,
 )
 
 SuggestedFixTypeDef = TypedDict(
     "SuggestedFixTypeDef",
     {
         "code": str,
         "description": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -306,15 +333,14 @@
     {
         "closedFindings": FindingMetricsValuePerSeverityTypeDef,
         "date": datetime,
         "meanTimeToClose": FindingMetricsValuePerSeverityTypeDef,
         "newFindings": FindingMetricsValuePerSeverityTypeDef,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
@@ -358,15 +384,14 @@
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
         "startLine": int,
     },
-    total=False,
 )
 
 _RequiredCreateScanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScanRequestRequestTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "scanName": str,
@@ -387,43 +412,43 @@
     _RequiredCreateScanRequestRequestTypeDef, _OptionalCreateScanRequestRequestTypeDef
 ):
     pass
 
 CreateScanResponseTypeDef = TypedDict(
     "CreateScanResponseTypeDef",
     {
-        "resourceId": ResourceIdTypeDef,
+        "resourceId": ResourceIdOutputTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateAccountConfigurationRequestRequestTypeDef",
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
     {
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountConfigurationResponseTypeDef = TypedDict(
-    "UpdateAccountConfigurationResponseTypeDef",
+UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
     "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
     {
         "scanName": str,
@@ -440,34 +465,19 @@
 
 class GetFindingsRequestGetFindingsPaginateTypeDef(
     _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
     _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
 ):
     pass
 
-ListScansRequestListScansPaginateTypeDef = TypedDict(
-    "ListScansRequestListScansPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetMetricsSummaryRequestRequestTypeDef = TypedDict(
-    "GetMetricsSummaryRequestRequestTypeDef",
-    {
-        "date": TimestampTypeDef,
-    },
-)
-
 _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     {
-        "endDate": TimestampTypeDef,
-        "startDate": TimestampTypeDef,
+        "endDate": Union[datetime, str],
+        "startDate": Union[datetime, str],
     },
 )
 _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -476,36 +486,22 @@
 
 class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
     _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
 ):
     pass
 
-_RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestRequestTypeDef",
-    {
-        "endDate": TimestampTypeDef,
-        "startDate": TimestampTypeDef,
-    },
-)
-_OptionalListFindingsMetricsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestRequestTypeDef",
+ListScansRequestListScansPaginateTypeDef = TypedDict(
+    "ListScansRequestListScansPaginateTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListFindingsMetricsRequestRequestTypeDef(
-    _RequiredListFindingsMetricsRequestRequestTypeDef,
-    _OptionalListFindingsMetricsRequestRequestTypeDef,
-):
-    pass
-
 ListScansResponseTypeDef = TypedDict(
     "ListScansResponseTypeDef",
     {
         "nextToken": str,
         "summaries": List[ScanSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -516,24 +512,22 @@
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
         "date": datetime,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
         "scansWithMostOpenCriticalFindings": List[ScanNameWithFindingNumTypeDef],
         "scansWithMostOpenFindings": List[ScanNameWithFindingNumTypeDef],
     },
-    total=False,
 )
 
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
         "suggestedFixes": List[SuggestedFixTypeDef],
     },
-    total=False,
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
@@ -546,15 +540,14 @@
     {
         "filePath": FilePathTypeDef,
         "id": str,
         "itemCount": int,
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
     },
-    total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -577,15 +570,14 @@
         "severity": SeverityType,
         "status": StatusType,
         "title": str,
         "type": str,
         "updatedAt": datetime,
         "vulnerability": VulnerabilityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security.egg-info/PKG-INFO` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.28.16
-Summary: Type annotations for boto3.CodeGuruSecurity 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.5
+Summary: Type annotations for boto3.CodeGuruSecurity 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codeguru-security type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 codeguru-security type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -326,37 +326,40 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_codeguru_security.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
     ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
+    ResourceIdOutputTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
     PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
-    TimestampTypeDef,
+    GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
+    ListFindingsMetricsRequestRequestTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ScanNameWithFindingNumTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -366,34 +369,32 @@
     CreateUploadUrlResponseTypeDef,
     GetScanResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
+    UpdateAccountConfigurationRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
-    GetMetricsSummaryRequestRequestTypeDef,
     ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListFindingsMetricsRequestRequestTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
     BatchGetFindingsResponseTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_value() -> FindingMetricsValuePerSeverityTypeDef:
+def get_structure() -> FindingMetricsValuePerSeverityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeguru-security-1.28.16/mypy_boto3_codeguru_security.egg-info/SOURCES.txt` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.16/setup.py` & `mypy-boto3-codeguru-security-1.28.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-security",
-    version="1.28.16",
+    version="1.28.5",
     packages=["mypy_boto3_codeguru_security"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruSecurity 1.28.16 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.CodeGuruSecurity 1.28.5 service generated with"
+        " mypy-boto3-builder 7.15.1"
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
-    keywords="boto3 codeguru-security type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 codeguru-security type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codeguru_security": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

