# Comparing `tmp/mypy-boto3-accessanalyzer-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-accessanalyzer-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-accessanalyzer-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:24 2023, max compression
+gzip compressed data, was "mypy-boto3-accessanalyzer-1.28.16.tar", last modified: Tue Aug  1 11:36:04 2023, max compression
```

## Comparing `mypy-boto3-accessanalyzer-1.28.15.post1.tar` & `mypy-boto3-accessanalyzer-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.036978 mypy-boto3-accessanalyzer-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19378 2023-07-29 10:02:24.024978 mypy-boto3-accessanalyzer-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.012978 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24974 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47463 2023-07-29 09:37:27.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47382 2023-07-29 09:37:26.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.024978 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19378 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:24.036978 mypy-boto3-accessanalyzer-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.780961 mypy-boto3-accessanalyzer-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-08-01 11:36:04.768961 mypy-boto3-accessanalyzer-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17936 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.768961 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24783 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24740 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47548 2023-08-01 11:09:57.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47468 2023-08-01 11:09:55.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:09:54.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.768961 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-08-01 11:36:04.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:36:04.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:04.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:36:04.000000 mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:04.780961 mypy-boto3-accessanalyzer-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:09:53.000000 mypy-boto3-accessanalyzer-1.28.16/setup.py
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/LICENSE` & `mypy-boto3-accessanalyzer-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/PKG-INFO` & `mypy-boto3-accessanalyzer-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AccessAnalyzer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 accessanalyzer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 accessanalyzer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-accessanalyzer)](https://pepy.tech/project/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
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
@@ -361,31 +361,32 @@
 )
 
 
 def check_value(value: AccessPreviewStatusReasonCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_accessanalyzer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_accessanalyzer.type_defs import (
     AccessPreviewStatusReasonTypeDef,
     AclGranteeTypeDef,
     AnalyzedResourceSummaryTypeDef,
     AnalyzedResourceTypeDef,
     StatusReasonTypeDef,
     ApplyArchiveRuleRequestRequestTypeDef,
     CriterionOutputTypeDef,
     CancelPolicyGenerationRequestRequestTypeDef,
+    TimestampTypeDef,
     TrailTypeDef,
     TrailPropertiesTypeDef,
     EbsSnapshotConfigurationOutputTypeDef,
     EcrRepositoryConfigurationTypeDef,
     EfsFileSystemConfigurationTypeDef,
     IamRoleConfigurationTypeDef,
     SecretsManagerSecretConfigurationTypeDef,
@@ -439,31 +440,26 @@
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPolicyGenerationResponseTypeDef,
-    CreateArchiveRuleRequestRequestTypeDef,
+    CriterionUnionTypeDef,
     InlineArchiveRuleTypeDef,
-    ListAccessPreviewFindingsRequestRequestTypeDef,
-    UpdateArchiveRuleRequestRequestTypeDef,
     FindingSourceTypeDef,
     JobDetailsTypeDef,
     KmsGrantConfigurationOutputTypeDef,
     KmsGrantConfigurationTypeDef,
-    ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
     ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef,
     ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef,
     ListAnalyzersRequestListAnalyzersPaginateTypeDef,
     ListArchiveRulesRequestListArchiveRulesPaginateTypeDef,
     ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef,
     ValidatePolicyRequestValidatePolicyPaginateTypeDef,
-    ListFindingsRequestListFindingsPaginateTypeDef,
-    ListFindingsRequestRequestTypeDef,
     ListPolicyGenerationsResponseTypeDef,
     NetworkOriginConfigurationOutputTypeDef,
     NetworkOriginConfigurationTypeDef,
     PathElementTypeDef,
     SpanTypeDef,
     RdsDbClusterSnapshotConfigurationOutputTypeDef,
     RdsDbClusterSnapshotConfigurationTypeDef,
@@ -472,14 +468,20 @@
     ListAccessPreviewsResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
     StartPolicyGenerationRequestRequestTypeDef,
     GeneratedPolicyPropertiesTypeDef,
+    CreateArchiveRuleRequestRequestTypeDef,
+    ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
+    ListAccessPreviewFindingsRequestRequestTypeDef,
+    ListFindingsRequestListFindingsPaginateTypeDef,
+    ListFindingsRequestRequestTypeDef,
+    UpdateArchiveRuleRequestRequestTypeDef,
     CreateAnalyzerRequestRequestTypeDef,
     AccessPreviewFindingTypeDef,
     FindingSummaryTypeDef,
     FindingTypeDef,
     KmsKeyConfigurationOutputTypeDef,
     KmsKeyConfigurationTypeDef,
     S3AccessPointConfigurationOutputTypeDef,
@@ -493,20 +495,21 @@
     S3BucketConfigurationTypeDef,
     ValidatePolicyFindingTypeDef,
     GetGeneratedPolicyResponseTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ValidatePolicyResponseTypeDef,
     AccessPreviewTypeDef,
-    CreateAccessPreviewRequestRequestTypeDef,
+    ConfigurationUnionTypeDef,
     GetAccessPreviewResponseTypeDef,
+    CreateAccessPreviewRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessPreviewStatusReasonTypeDef:
+def get_value() -> AccessPreviewStatusReasonTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/README.md` & `mypy-boto3-accessanalyzer-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-accessanalyzer)](https://pepy.tech/project/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
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
@@ -329,31 +329,32 @@
 )
 
 
 def check_value(value: AccessPreviewStatusReasonCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_accessanalyzer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_accessanalyzer.type_defs import (
     AccessPreviewStatusReasonTypeDef,
     AclGranteeTypeDef,
     AnalyzedResourceSummaryTypeDef,
     AnalyzedResourceTypeDef,
     StatusReasonTypeDef,
     ApplyArchiveRuleRequestRequestTypeDef,
     CriterionOutputTypeDef,
     CancelPolicyGenerationRequestRequestTypeDef,
+    TimestampTypeDef,
     TrailTypeDef,
     TrailPropertiesTypeDef,
     EbsSnapshotConfigurationOutputTypeDef,
     EcrRepositoryConfigurationTypeDef,
     EfsFileSystemConfigurationTypeDef,
     IamRoleConfigurationTypeDef,
     SecretsManagerSecretConfigurationTypeDef,
@@ -407,31 +408,26 @@
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPolicyGenerationResponseTypeDef,
-    CreateArchiveRuleRequestRequestTypeDef,
+    CriterionUnionTypeDef,
     InlineArchiveRuleTypeDef,
-    ListAccessPreviewFindingsRequestRequestTypeDef,
-    UpdateArchiveRuleRequestRequestTypeDef,
     FindingSourceTypeDef,
     JobDetailsTypeDef,
     KmsGrantConfigurationOutputTypeDef,
     KmsGrantConfigurationTypeDef,
-    ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
     ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef,
     ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef,
     ListAnalyzersRequestListAnalyzersPaginateTypeDef,
     ListArchiveRulesRequestListArchiveRulesPaginateTypeDef,
     ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef,
     ValidatePolicyRequestValidatePolicyPaginateTypeDef,
-    ListFindingsRequestListFindingsPaginateTypeDef,
-    ListFindingsRequestRequestTypeDef,
     ListPolicyGenerationsResponseTypeDef,
     NetworkOriginConfigurationOutputTypeDef,
     NetworkOriginConfigurationTypeDef,
     PathElementTypeDef,
     SpanTypeDef,
     RdsDbClusterSnapshotConfigurationOutputTypeDef,
     RdsDbClusterSnapshotConfigurationTypeDef,
@@ -440,14 +436,20 @@
     ListAccessPreviewsResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
     StartPolicyGenerationRequestRequestTypeDef,
     GeneratedPolicyPropertiesTypeDef,
+    CreateArchiveRuleRequestRequestTypeDef,
+    ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
+    ListAccessPreviewFindingsRequestRequestTypeDef,
+    ListFindingsRequestListFindingsPaginateTypeDef,
+    ListFindingsRequestRequestTypeDef,
+    UpdateArchiveRuleRequestRequestTypeDef,
     CreateAnalyzerRequestRequestTypeDef,
     AccessPreviewFindingTypeDef,
     FindingSummaryTypeDef,
     FindingTypeDef,
     KmsKeyConfigurationOutputTypeDef,
     KmsKeyConfigurationTypeDef,
     S3AccessPointConfigurationOutputTypeDef,
@@ -461,20 +463,21 @@
     S3BucketConfigurationTypeDef,
     ValidatePolicyFindingTypeDef,
     GetGeneratedPolicyResponseTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ValidatePolicyResponseTypeDef,
     AccessPreviewTypeDef,
-    CreateAccessPreviewRequestRequestTypeDef,
+    ConfigurationUnionTypeDef,
     GetAccessPreviewResponseTypeDef,
+    CreateAccessPreviewRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessPreviewStatusReasonTypeDef:
+def get_value() -> AccessPreviewStatusReasonTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__init__.py` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__init__.pyi` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__main__.py` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AccessAnalyzer 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AccessAnalyzer 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer\nOther"
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

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/client.py` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_accessanalyzer.client import AccessAnalyzerClient
 
     session = Session()
     client: AccessAnalyzerClient = session.client("accessanalyzer")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     FindingStatusUpdateType,
     LocaleType,
     PolicyTypeType,
@@ -34,20 +34,18 @@
     ListArchiveRulesPaginator,
     ListFindingsPaginator,
     ListPolicyGenerationsPaginator,
     ValidatePolicyPaginator,
 )
 from .type_defs import (
     CloudTrailDetailsTypeDef,
-    ConfigurationOutputTypeDef,
-    ConfigurationTypeDef,
+    ConfigurationUnionTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
-    CriterionOutputTypeDef,
-    CriterionTypeDef,
+    CriterionUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccessPreviewResponseTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     GetFindingResponseTypeDef,
     GetGeneratedPolicyResponseTypeDef,
@@ -146,15 +144,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#close)
         """
 
     def create_access_preview(
         self,
         *,
         analyzerArn: str,
-        configurations: Mapping[str, Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]],
+        configurations: Mapping[str, ConfigurationUnionTypeDef],
         clientToken: str = ...
     ) -> CreateAccessPreviewResponseTypeDef:
         """
         Creates an access preview that allows you to preview IAM Access Analyzer
         findings for your resource before deploying resource permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_access_preview)
@@ -178,15 +176,15 @@
         """
 
     def create_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
+        filter: Mapping[str, CriterionUnionTypeDef],
         clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates an archive rule for the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_archive_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#create_archive_rule)
@@ -287,15 +285,15 @@
         """
 
     def list_access_preview_findings(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
+        filter: Mapping[str, CriterionUnionTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListAccessPreviewFindingsResponseTypeDef:
         """
         Retrieves a list of access preview findings generated by the specified access
         preview.
 
@@ -349,15 +347,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#list_archive_rules)
         """
 
     def list_findings(
         self,
         *,
         analyzerArn: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
+        filter: Mapping[str, CriterionUnionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a list of findings generated by the specified analyzer.
 
@@ -424,15 +422,15 @@
         """
 
     def update_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
+        filter: Mapping[str, CriterionUnionTypeDef],
         clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the criteria and values for the specified archive rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.update_archive_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#update_archive_rule)
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/client.pyi` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_accessanalyzer.client import AccessAnalyzerClient
 
     session = Session()
     client: AccessAnalyzerClient = session.client("accessanalyzer")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     FindingStatusUpdateType,
     LocaleType,
     PolicyTypeType,
@@ -34,20 +34,18 @@
     ListArchiveRulesPaginator,
     ListFindingsPaginator,
     ListPolicyGenerationsPaginator,
     ValidatePolicyPaginator,
 )
 from .type_defs import (
     CloudTrailDetailsTypeDef,
-    ConfigurationOutputTypeDef,
-    ConfigurationTypeDef,
+    ConfigurationUnionTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
-    CriterionOutputTypeDef,
-    CriterionTypeDef,
+    CriterionUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccessPreviewResponseTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     GetFindingResponseTypeDef,
     GetGeneratedPolicyResponseTypeDef,
@@ -137,15 +135,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#close)
         """
     def create_access_preview(
         self,
         *,
         analyzerArn: str,
-        configurations: Mapping[str, Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]],
+        configurations: Mapping[str, ConfigurationUnionTypeDef],
         clientToken: str = ...
     ) -> CreateAccessPreviewResponseTypeDef:
         """
         Creates an access preview that allows you to preview IAM Access Analyzer
         findings for your resource before deploying resource permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_access_preview)
@@ -167,15 +165,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#create_analyzer)
         """
     def create_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
+        filter: Mapping[str, CriterionUnionTypeDef],
         clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates an archive rule for the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_archive_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#create_archive_rule)
@@ -266,15 +264,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#get_generated_policy)
         """
     def list_access_preview_findings(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
+        filter: Mapping[str, CriterionUnionTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListAccessPreviewFindingsResponseTypeDef:
         """
         Retrieves a list of access preview findings generated by the specified access
         preview.
 
@@ -323,15 +321,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_archive_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#list_archive_rules)
         """
     def list_findings(
         self,
         *,
         analyzerArn: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
+        filter: Mapping[str, CriterionUnionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a list of findings generated by the specified analyzer.
 
@@ -391,15 +389,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#untag_resource)
         """
     def update_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
+        filter: Mapping[str, CriterionUnionTypeDef],
         clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the criteria and values for the specified archive rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.update_archive_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#update_archive_rule)
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/literals.py` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/literals.pyi` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/paginator.py` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,28 +29,27 @@
     list_analyzers_paginator: ListAnalyzersPaginator = client.get_paginator("list_analyzers")
     list_archive_rules_paginator: ListArchiveRulesPaginator = client.get_paginator("list_archive_rules")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_policy_generations_paginator: ListPolicyGenerationsPaginator = client.get_paginator("list_policy_generations")
     validate_policy_paginator: ValidatePolicyPaginator = client.get_paginator("validate_policy")
     ```
 """
-from typing import Generic, Iterator, Mapping, TypeVar, Union
+from typing import Generic, Iterator, Mapping, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     LocaleType,
     PolicyTypeType,
     ResourceTypeType,
     TypeType,
     ValidatePolicyResourceTypeType,
 )
 from .type_defs import (
-    CriterionOutputTypeDef,
-    CriterionTypeDef,
+    CriterionUnionTypeDef,
     ListAccessPreviewFindingsResponseTypeDef,
     ListAccessPreviewsResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListPolicyGenerationsResponseTypeDef,
@@ -66,60 +65,55 @@
     "ListAnalyzersPaginator",
     "ListArchiveRulesPaginator",
     "ListFindingsPaginator",
     "ListPolicyGenerationsPaginator",
     "ValidatePolicyPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAccessPreviewFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
+        filter: Mapping[str, CriterionUnionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPreviewFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewfindingspaginator)
         """
 
-
 class ListAccessPreviewsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviews)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewspaginator)
     """
 
     def paginate(
         self, *, analyzerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPreviewsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviews.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewspaginator)
         """
 
-
 class ListAnalyzedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listanalyzedresourcespaginator)
     """
 
     def paginate(
@@ -130,80 +124,75 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnalyzedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listanalyzedresourcespaginator)
         """
 
-
 class ListAnalyzersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listanalyzerspaginator)
     """
 
     def paginate(
         self, *, type: TypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnalyzersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listanalyzerspaginator)
         """
 
-
 class ListArchiveRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListArchiveRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listarchiverulespaginator)
     """
 
     def paginate(
         self, *, analyzerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListArchiveRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListArchiveRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listarchiverulespaginator)
         """
 
-
 class ListFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         analyzerArn: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
+        filter: Mapping[str, CriterionUnionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listfindingspaginator)
         """
 
-
 class ListPolicyGenerationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListPolicyGenerations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listpolicygenerationspaginator)
     """
 
     def paginate(
         self, *, principalArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyGenerationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListPolicyGenerations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listpolicygenerationspaginator)
         """
 
-
 class ValidatePolicyPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ValidatePolicy)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#validatepolicypaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/paginator.pyi` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,27 @@
     list_analyzers_paginator: ListAnalyzersPaginator = client.get_paginator("list_analyzers")
     list_archive_rules_paginator: ListArchiveRulesPaginator = client.get_paginator("list_archive_rules")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_policy_generations_paginator: ListPolicyGenerationsPaginator = client.get_paginator("list_policy_generations")
     validate_policy_paginator: ValidatePolicyPaginator = client.get_paginator("validate_policy")
     ```
 """
-from typing import Generic, Iterator, Mapping, TypeVar, Union
+from typing import Generic, Iterator, Mapping, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     LocaleType,
     PolicyTypeType,
     ResourceTypeType,
     TypeType,
     ValidatePolicyResourceTypeType,
 )
 from .type_defs import (
-    CriterionOutputTypeDef,
-    CriterionTypeDef,
+    CriterionUnionTypeDef,
     ListAccessPreviewFindingsResponseTypeDef,
     ListAccessPreviewsResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListPolicyGenerationsResponseTypeDef,
@@ -66,55 +65,60 @@
     "ListAnalyzersPaginator",
     "ListArchiveRulesPaginator",
     "ListFindingsPaginator",
     "ListPolicyGenerationsPaginator",
     "ValidatePolicyPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAccessPreviewFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
+        filter: Mapping[str, CriterionUnionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPreviewFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewfindingspaginator)
         """
 
+
 class ListAccessPreviewsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviews)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewspaginator)
     """
 
     def paginate(
         self, *, analyzerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPreviewsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviews.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewspaginator)
         """
 
+
 class ListAnalyzedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listanalyzedresourcespaginator)
     """
 
     def paginate(
@@ -125,75 +129,80 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnalyzedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listanalyzedresourcespaginator)
         """
 
+
 class ListAnalyzersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listanalyzerspaginator)
     """
 
     def paginate(
         self, *, type: TypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnalyzersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listanalyzerspaginator)
         """
 
+
 class ListArchiveRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListArchiveRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listarchiverulespaginator)
     """
 
     def paginate(
         self, *, analyzerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListArchiveRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListArchiveRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listarchiverulespaginator)
         """
 
+
 class ListFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         analyzerArn: str,
-        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
+        filter: Mapping[str, CriterionUnionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listfindingspaginator)
         """
 
+
 class ListPolicyGenerationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListPolicyGenerations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listpolicygenerationspaginator)
     """
 
     def paginate(
         self, *, principalArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyGenerationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListPolicyGenerations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listpolicygenerationspaginator)
         """
 
+
 class ValidatePolicyPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ValidatePolicy)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#validatepolicypaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/type_defs.py` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_accessanalyzer.type_defs import AccessPreviewStatusReasonTypeDef
 
-    data: AccessPreviewStatusReasonTypeDef = {...}
+    data: AccessPreviewStatusReasonTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -48,14 +48,15 @@
     "AclGranteeTypeDef",
     "AnalyzedResourceSummaryTypeDef",
     "AnalyzedResourceTypeDef",
     "StatusReasonTypeDef",
     "ApplyArchiveRuleRequestRequestTypeDef",
     "CriterionOutputTypeDef",
     "CancelPolicyGenerationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "TrailTypeDef",
     "TrailPropertiesTypeDef",
     "EbsSnapshotConfigurationOutputTypeDef",
     "EcrRepositoryConfigurationTypeDef",
     "EfsFileSystemConfigurationTypeDef",
     "IamRoleConfigurationTypeDef",
     "SecretsManagerSecretConfigurationTypeDef",
@@ -109,31 +110,26 @@
     "CreateAccessPreviewResponseTypeDef",
     "CreateAnalyzerResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAnalyzedResourceResponseTypeDef",
     "ListAnalyzedResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartPolicyGenerationResponseTypeDef",
-    "CreateArchiveRuleRequestRequestTypeDef",
+    "CriterionUnionTypeDef",
     "InlineArchiveRuleTypeDef",
-    "ListAccessPreviewFindingsRequestRequestTypeDef",
-    "UpdateArchiveRuleRequestRequestTypeDef",
     "FindingSourceTypeDef",
     "JobDetailsTypeDef",
     "KmsGrantConfigurationOutputTypeDef",
     "KmsGrantConfigurationTypeDef",
-    "ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
     "ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef",
     "ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef",
     "ListAnalyzersRequestListAnalyzersPaginateTypeDef",
     "ListArchiveRulesRequestListArchiveRulesPaginateTypeDef",
     "ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef",
     "ValidatePolicyRequestValidatePolicyPaginateTypeDef",
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    "ListFindingsRequestRequestTypeDef",
     "ListPolicyGenerationsResponseTypeDef",
     "NetworkOriginConfigurationOutputTypeDef",
     "NetworkOriginConfigurationTypeDef",
     "PathElementTypeDef",
     "SpanTypeDef",
     "RdsDbClusterSnapshotConfigurationOutputTypeDef",
     "RdsDbClusterSnapshotConfigurationTypeDef",
@@ -142,14 +138,20 @@
     "ListAccessPreviewsResponseTypeDef",
     "GetAnalyzerResponseTypeDef",
     "ListAnalyzersResponseTypeDef",
     "GetArchiveRuleResponseTypeDef",
     "ListArchiveRulesResponseTypeDef",
     "StartPolicyGenerationRequestRequestTypeDef",
     "GeneratedPolicyPropertiesTypeDef",
+    "CreateArchiveRuleRequestRequestTypeDef",
+    "ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
+    "ListAccessPreviewFindingsRequestRequestTypeDef",
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    "ListFindingsRequestRequestTypeDef",
+    "UpdateArchiveRuleRequestRequestTypeDef",
     "CreateAnalyzerRequestRequestTypeDef",
     "AccessPreviewFindingTypeDef",
     "FindingSummaryTypeDef",
     "FindingTypeDef",
     "KmsKeyConfigurationOutputTypeDef",
     "KmsKeyConfigurationTypeDef",
     "S3AccessPointConfigurationOutputTypeDef",
@@ -163,16 +165,17 @@
     "S3BucketConfigurationTypeDef",
     "ValidatePolicyFindingTypeDef",
     "GetGeneratedPolicyResponseTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ValidatePolicyResponseTypeDef",
     "AccessPreviewTypeDef",
-    "CreateAccessPreviewRequestRequestTypeDef",
+    "ConfigurationUnionTypeDef",
     "GetAccessPreviewResponseTypeDef",
+    "CreateAccessPreviewRequestRequestTypeDef",
 )
 
 AccessPreviewStatusReasonTypeDef = TypedDict(
     "AccessPreviewStatusReasonTypeDef",
     {
         "code": AccessPreviewStatusReasonCodeType,
     },
@@ -267,14 +270,15 @@
 CancelPolicyGenerationRequestRequestTypeDef = TypedDict(
     "CancelPolicyGenerationRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredTrailTypeDef = TypedDict(
     "_RequiredTrailTypeDef",
     {
         "cloudTrailArn": str,
     },
 )
 _OptionalTrailTypeDef = TypedDict(
@@ -913,21 +917,21 @@
 )
 
 _RequiredCloudTrailDetailsTypeDef = TypedDict(
     "_RequiredCloudTrailDetailsTypeDef",
     {
         "trails": Sequence[TrailTypeDef],
         "accessRole": str,
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalCloudTrailDetailsTypeDef = TypedDict(
     "_OptionalCloudTrailDetailsTypeDef",
     {
-        "endTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
     },
     total=False,
 )
 
 
 class CloudTrailDetailsTypeDef(
     _RequiredCloudTrailDetailsTypeDef, _OptionalCloudTrailDetailsTypeDef
@@ -996,93 +1000,23 @@
     "StartPolicyGenerationResponseTypeDef",
     {
         "jobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateArchiveRuleRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "ruleName": str,
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-    },
-)
-_OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateArchiveRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateArchiveRuleRequestRequestTypeDef(
-    _RequiredCreateArchiveRuleRequestRequestTypeDef, _OptionalCreateArchiveRuleRequestRequestTypeDef
-):
-    pass
-
-
+CriterionUnionTypeDef = Union[CriterionTypeDef, CriterionOutputTypeDef]
 InlineArchiveRuleTypeDef = TypedDict(
     "InlineArchiveRuleTypeDef",
     {
         "ruleName": str,
         "filter": Mapping[str, CriterionTypeDef],
     },
 )
 
-_RequiredListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccessPreviewFindingsRequestRequestTypeDef",
-    {
-        "accessPreviewId": str,
-        "analyzerArn": str,
-    },
-)
-_OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
-    {
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListAccessPreviewFindingsRequestRequestTypeDef(
-    _RequiredListAccessPreviewFindingsRequestRequestTypeDef,
-    _OptionalListAccessPreviewFindingsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "ruleName": str,
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-    },
-)
-_OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class UpdateArchiveRuleRequestRequestTypeDef(
-    _RequiredUpdateArchiveRuleRequestRequestTypeDef, _OptionalUpdateArchiveRuleRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredFindingSourceTypeDef = TypedDict(
     "_RequiredFindingSourceTypeDef",
     {
         "type": FindingSourceTypeType,
     },
 )
 _OptionalFindingSourceTypeDef = TypedDict(
@@ -1164,38 +1098,14 @@
 
 class KmsGrantConfigurationTypeDef(
     _RequiredKmsGrantConfigurationTypeDef, _OptionalKmsGrantConfigurationTypeDef
 ):
     pass
 
 
-_RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
-    "_RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
-    {
-        "accessPreviewId": str,
-        "analyzerArn": str,
-    },
-)
-_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
-    "_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
-    {
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef(
-    _RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
-    _OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef = TypedDict(
     "_RequiredListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef",
     {
         "analyzerArn": str,
     },
 )
 _OptionalListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef = TypedDict(
@@ -1298,62 +1208,14 @@
 class ValidatePolicyRequestValidatePolicyPaginateTypeDef(
     _RequiredValidatePolicyRequestValidatePolicyPaginateTypeDef,
     _OptionalValidatePolicyRequestValidatePolicyPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "_RequiredListFindingsRequestListFindingsPaginateTypeDef",
-    {
-        "analyzerArn": str,
-    },
-)
-_OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
-    {
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-        "sort": SortCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFindingsRequestListFindingsPaginateTypeDef(
-    _RequiredListFindingsRequestListFindingsPaginateTypeDef,
-    _OptionalListFindingsRequestListFindingsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFindingsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsRequestRequestTypeDef",
-    {
-        "analyzerArn": str,
-    },
-)
-_OptionalListFindingsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsRequestRequestTypeDef",
-    {
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-        "sort": SortCriteriaTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListFindingsRequestRequestTypeDef(
-    _RequiredListFindingsRequestRequestTypeDef, _OptionalListFindingsRequestRequestTypeDef
-):
-    pass
-
-
 ListPolicyGenerationsResponseTypeDef = TypedDict(
     "ListPolicyGenerationsResponseTypeDef",
     {
         "policyGenerations": List[PolicyGenerationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1516,14 +1378,157 @@
 
 class GeneratedPolicyPropertiesTypeDef(
     _RequiredGeneratedPolicyPropertiesTypeDef, _OptionalGeneratedPolicyPropertiesTypeDef
 ):
     pass
 
 
+_RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateArchiveRuleRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "ruleName": str,
+        "filter": Mapping[str, CriterionUnionTypeDef],
+    },
+)
+_OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateArchiveRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateArchiveRuleRequestRequestTypeDef(
+    _RequiredCreateArchiveRuleRequestRequestTypeDef, _OptionalCreateArchiveRuleRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
+    "_RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
+    {
+        "accessPreviewId": str,
+        "analyzerArn": str,
+    },
+)
+_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
+    "_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
+    {
+        "filter": Mapping[str, CriterionUnionTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef(
+    _RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
+    _OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccessPreviewFindingsRequestRequestTypeDef",
+    {
+        "accessPreviewId": str,
+        "analyzerArn": str,
+    },
+)
+_OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
+    {
+        "filter": Mapping[str, CriterionUnionTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListAccessPreviewFindingsRequestRequestTypeDef(
+    _RequiredListAccessPreviewFindingsRequestRequestTypeDef,
+    _OptionalListAccessPreviewFindingsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "_RequiredListFindingsRequestListFindingsPaginateTypeDef",
+    {
+        "analyzerArn": str,
+    },
+)
+_OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
+    {
+        "filter": Mapping[str, CriterionUnionTypeDef],
+        "sort": SortCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFindingsRequestListFindingsPaginateTypeDef(
+    _RequiredListFindingsRequestListFindingsPaginateTypeDef,
+    _OptionalListFindingsRequestListFindingsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFindingsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsRequestRequestTypeDef",
+    {
+        "analyzerArn": str,
+    },
+)
+_OptionalListFindingsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsRequestRequestTypeDef",
+    {
+        "filter": Mapping[str, CriterionUnionTypeDef],
+        "sort": SortCriteriaTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListFindingsRequestRequestTypeDef(
+    _RequiredListFindingsRequestRequestTypeDef, _OptionalListFindingsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "ruleName": str,
+        "filter": Mapping[str, CriterionUnionTypeDef],
+    },
+)
+_OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateArchiveRuleRequestRequestTypeDef(
+    _RequiredUpdateArchiveRuleRequestRequestTypeDef, _OptionalUpdateArchiveRuleRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateAnalyzerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnalyzerRequestRequestTypeDef",
     {
         "analyzerName": str,
         "type": TypeType,
     },
 )
@@ -1839,19 +1844,28 @@
 )
 
 
 class AccessPreviewTypeDef(_RequiredAccessPreviewTypeDef, _OptionalAccessPreviewTypeDef):
     pass
 
 
+ConfigurationUnionTypeDef = Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]
+GetAccessPreviewResponseTypeDef = TypedDict(
+    "GetAccessPreviewResponseTypeDef",
+    {
+        "accessPreview": AccessPreviewTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateAccessPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPreviewRequestRequestTypeDef",
     {
         "analyzerArn": str,
-        "configurations": Mapping[str, Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]],
+        "configurations": Mapping[str, ConfigurationUnionTypeDef],
     },
 )
 _OptionalCreateAccessPreviewRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAccessPreviewRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -1860,16 +1874,7 @@
 
 
 class CreateAccessPreviewRequestRequestTypeDef(
     _RequiredCreateAccessPreviewRequestRequestTypeDef,
     _OptionalCreateAccessPreviewRequestRequestTypeDef,
 ):
     pass
-
-
-GetAccessPreviewResponseTypeDef = TypedDict(
-    "GetAccessPreviewResponseTypeDef",
-    {
-        "accessPreview": AccessPreviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/type_defs.pyi` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_accessanalyzer.type_defs import AccessPreviewStatusReasonTypeDef
 
-    data: AccessPreviewStatusReasonTypeDef = {...}
+    data: AccessPreviewStatusReasonTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -47,14 +47,15 @@
     "AclGranteeTypeDef",
     "AnalyzedResourceSummaryTypeDef",
     "AnalyzedResourceTypeDef",
     "StatusReasonTypeDef",
     "ApplyArchiveRuleRequestRequestTypeDef",
     "CriterionOutputTypeDef",
     "CancelPolicyGenerationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "TrailTypeDef",
     "TrailPropertiesTypeDef",
     "EbsSnapshotConfigurationOutputTypeDef",
     "EcrRepositoryConfigurationTypeDef",
     "EfsFileSystemConfigurationTypeDef",
     "IamRoleConfigurationTypeDef",
     "SecretsManagerSecretConfigurationTypeDef",
@@ -108,31 +109,26 @@
     "CreateAccessPreviewResponseTypeDef",
     "CreateAnalyzerResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAnalyzedResourceResponseTypeDef",
     "ListAnalyzedResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartPolicyGenerationResponseTypeDef",
-    "CreateArchiveRuleRequestRequestTypeDef",
+    "CriterionUnionTypeDef",
     "InlineArchiveRuleTypeDef",
-    "ListAccessPreviewFindingsRequestRequestTypeDef",
-    "UpdateArchiveRuleRequestRequestTypeDef",
     "FindingSourceTypeDef",
     "JobDetailsTypeDef",
     "KmsGrantConfigurationOutputTypeDef",
     "KmsGrantConfigurationTypeDef",
-    "ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
     "ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef",
     "ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef",
     "ListAnalyzersRequestListAnalyzersPaginateTypeDef",
     "ListArchiveRulesRequestListArchiveRulesPaginateTypeDef",
     "ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef",
     "ValidatePolicyRequestValidatePolicyPaginateTypeDef",
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    "ListFindingsRequestRequestTypeDef",
     "ListPolicyGenerationsResponseTypeDef",
     "NetworkOriginConfigurationOutputTypeDef",
     "NetworkOriginConfigurationTypeDef",
     "PathElementTypeDef",
     "SpanTypeDef",
     "RdsDbClusterSnapshotConfigurationOutputTypeDef",
     "RdsDbClusterSnapshotConfigurationTypeDef",
@@ -141,14 +137,20 @@
     "ListAccessPreviewsResponseTypeDef",
     "GetAnalyzerResponseTypeDef",
     "ListAnalyzersResponseTypeDef",
     "GetArchiveRuleResponseTypeDef",
     "ListArchiveRulesResponseTypeDef",
     "StartPolicyGenerationRequestRequestTypeDef",
     "GeneratedPolicyPropertiesTypeDef",
+    "CreateArchiveRuleRequestRequestTypeDef",
+    "ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
+    "ListAccessPreviewFindingsRequestRequestTypeDef",
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    "ListFindingsRequestRequestTypeDef",
+    "UpdateArchiveRuleRequestRequestTypeDef",
     "CreateAnalyzerRequestRequestTypeDef",
     "AccessPreviewFindingTypeDef",
     "FindingSummaryTypeDef",
     "FindingTypeDef",
     "KmsKeyConfigurationOutputTypeDef",
     "KmsKeyConfigurationTypeDef",
     "S3AccessPointConfigurationOutputTypeDef",
@@ -162,16 +164,17 @@
     "S3BucketConfigurationTypeDef",
     "ValidatePolicyFindingTypeDef",
     "GetGeneratedPolicyResponseTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ValidatePolicyResponseTypeDef",
     "AccessPreviewTypeDef",
-    "CreateAccessPreviewRequestRequestTypeDef",
+    "ConfigurationUnionTypeDef",
     "GetAccessPreviewResponseTypeDef",
+    "CreateAccessPreviewRequestRequestTypeDef",
 )
 
 AccessPreviewStatusReasonTypeDef = TypedDict(
     "AccessPreviewStatusReasonTypeDef",
     {
         "code": AccessPreviewStatusReasonCodeType,
     },
@@ -262,14 +265,15 @@
 CancelPolicyGenerationRequestRequestTypeDef = TypedDict(
     "CancelPolicyGenerationRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredTrailTypeDef = TypedDict(
     "_RequiredTrailTypeDef",
     {
         "cloudTrailArn": str,
     },
 )
 _OptionalTrailTypeDef = TypedDict(
@@ -880,21 +884,21 @@
 )
 
 _RequiredCloudTrailDetailsTypeDef = TypedDict(
     "_RequiredCloudTrailDetailsTypeDef",
     {
         "trails": Sequence[TrailTypeDef],
         "accessRole": str,
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalCloudTrailDetailsTypeDef = TypedDict(
     "_OptionalCloudTrailDetailsTypeDef",
     {
-        "endTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
     },
     total=False,
 )
 
 class CloudTrailDetailsTypeDef(
     _RequiredCloudTrailDetailsTypeDef, _OptionalCloudTrailDetailsTypeDef
 ):
@@ -961,87 +965,23 @@
     "StartPolicyGenerationResponseTypeDef",
     {
         "jobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateArchiveRuleRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "ruleName": str,
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-    },
-)
-_OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateArchiveRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreateArchiveRuleRequestRequestTypeDef(
-    _RequiredCreateArchiveRuleRequestRequestTypeDef, _OptionalCreateArchiveRuleRequestRequestTypeDef
-):
-    pass
-
+CriterionUnionTypeDef = Union[CriterionTypeDef, CriterionOutputTypeDef]
 InlineArchiveRuleTypeDef = TypedDict(
     "InlineArchiveRuleTypeDef",
     {
         "ruleName": str,
         "filter": Mapping[str, CriterionTypeDef],
     },
 )
 
-_RequiredListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccessPreviewFindingsRequestRequestTypeDef",
-    {
-        "accessPreviewId": str,
-        "analyzerArn": str,
-    },
-)
-_OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
-    {
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListAccessPreviewFindingsRequestRequestTypeDef(
-    _RequiredListAccessPreviewFindingsRequestRequestTypeDef,
-    _OptionalListAccessPreviewFindingsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "ruleName": str,
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-    },
-)
-_OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class UpdateArchiveRuleRequestRequestTypeDef(
-    _RequiredUpdateArchiveRuleRequestRequestTypeDef, _OptionalUpdateArchiveRuleRequestRequestTypeDef
-):
-    pass
-
 _RequiredFindingSourceTypeDef = TypedDict(
     "_RequiredFindingSourceTypeDef",
     {
         "type": FindingSourceTypeType,
     },
 )
 _OptionalFindingSourceTypeDef = TypedDict(
@@ -1115,36 +1055,14 @@
 )
 
 class KmsGrantConfigurationTypeDef(
     _RequiredKmsGrantConfigurationTypeDef, _OptionalKmsGrantConfigurationTypeDef
 ):
     pass
 
-_RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
-    "_RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
-    {
-        "accessPreviewId": str,
-        "analyzerArn": str,
-    },
-)
-_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
-    "_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
-    {
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef(
-    _RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
-    _OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef = TypedDict(
     "_RequiredListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef",
     {
         "analyzerArn": str,
     },
 )
 _OptionalListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef = TypedDict(
@@ -1239,58 +1157,14 @@
 
 class ValidatePolicyRequestValidatePolicyPaginateTypeDef(
     _RequiredValidatePolicyRequestValidatePolicyPaginateTypeDef,
     _OptionalValidatePolicyRequestValidatePolicyPaginateTypeDef,
 ):
     pass
 
-_RequiredListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "_RequiredListFindingsRequestListFindingsPaginateTypeDef",
-    {
-        "analyzerArn": str,
-    },
-)
-_OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
-    {
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-        "sort": SortCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFindingsRequestListFindingsPaginateTypeDef(
-    _RequiredListFindingsRequestListFindingsPaginateTypeDef,
-    _OptionalListFindingsRequestListFindingsPaginateTypeDef,
-):
-    pass
-
-_RequiredListFindingsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsRequestRequestTypeDef",
-    {
-        "analyzerArn": str,
-    },
-)
-_OptionalListFindingsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsRequestRequestTypeDef",
-    {
-        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
-        "sort": SortCriteriaTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListFindingsRequestRequestTypeDef(
-    _RequiredListFindingsRequestRequestTypeDef, _OptionalListFindingsRequestRequestTypeDef
-):
-    pass
-
 ListPolicyGenerationsResponseTypeDef = TypedDict(
     "ListPolicyGenerationsResponseTypeDef",
     {
         "policyGenerations": List[PolicyGenerationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1449,14 +1323,145 @@
 )
 
 class GeneratedPolicyPropertiesTypeDef(
     _RequiredGeneratedPolicyPropertiesTypeDef, _OptionalGeneratedPolicyPropertiesTypeDef
 ):
     pass
 
+_RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateArchiveRuleRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "ruleName": str,
+        "filter": Mapping[str, CriterionUnionTypeDef],
+    },
+)
+_OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateArchiveRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreateArchiveRuleRequestRequestTypeDef(
+    _RequiredCreateArchiveRuleRequestRequestTypeDef, _OptionalCreateArchiveRuleRequestRequestTypeDef
+):
+    pass
+
+_RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
+    "_RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
+    {
+        "accessPreviewId": str,
+        "analyzerArn": str,
+    },
+)
+_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
+    "_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
+    {
+        "filter": Mapping[str, CriterionUnionTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef(
+    _RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
+    _OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
+):
+    pass
+
+_RequiredListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccessPreviewFindingsRequestRequestTypeDef",
+    {
+        "accessPreviewId": str,
+        "analyzerArn": str,
+    },
+)
+_OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
+    {
+        "filter": Mapping[str, CriterionUnionTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListAccessPreviewFindingsRequestRequestTypeDef(
+    _RequiredListAccessPreviewFindingsRequestRequestTypeDef,
+    _OptionalListAccessPreviewFindingsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "_RequiredListFindingsRequestListFindingsPaginateTypeDef",
+    {
+        "analyzerArn": str,
+    },
+)
+_OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
+    {
+        "filter": Mapping[str, CriterionUnionTypeDef],
+        "sort": SortCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFindingsRequestListFindingsPaginateTypeDef(
+    _RequiredListFindingsRequestListFindingsPaginateTypeDef,
+    _OptionalListFindingsRequestListFindingsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFindingsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsRequestRequestTypeDef",
+    {
+        "analyzerArn": str,
+    },
+)
+_OptionalListFindingsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsRequestRequestTypeDef",
+    {
+        "filter": Mapping[str, CriterionUnionTypeDef],
+        "sort": SortCriteriaTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListFindingsRequestRequestTypeDef(
+    _RequiredListFindingsRequestRequestTypeDef, _OptionalListFindingsRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "ruleName": str,
+        "filter": Mapping[str, CriterionUnionTypeDef],
+    },
+)
+_OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class UpdateArchiveRuleRequestRequestTypeDef(
+    _RequiredUpdateArchiveRuleRequestRequestTypeDef, _OptionalUpdateArchiveRuleRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateAnalyzerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnalyzerRequestRequestTypeDef",
     {
         "analyzerName": str,
         "type": TypeType,
     },
 )
@@ -1760,19 +1765,28 @@
     },
     total=False,
 )
 
 class AccessPreviewTypeDef(_RequiredAccessPreviewTypeDef, _OptionalAccessPreviewTypeDef):
     pass
 
+ConfigurationUnionTypeDef = Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]
+GetAccessPreviewResponseTypeDef = TypedDict(
+    "GetAccessPreviewResponseTypeDef",
+    {
+        "accessPreview": AccessPreviewTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateAccessPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPreviewRequestRequestTypeDef",
     {
         "analyzerArn": str,
-        "configurations": Mapping[str, Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]],
+        "configurations": Mapping[str, ConfigurationUnionTypeDef],
     },
 )
 _OptionalCreateAccessPreviewRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAccessPreviewRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -1780,15 +1794,7 @@
 )
 
 class CreateAccessPreviewRequestRequestTypeDef(
     _RequiredCreateAccessPreviewRequestRequestTypeDef,
     _OptionalCreateAccessPreviewRequestRequestTypeDef,
 ):
     pass
-
-GetAccessPreviewResponseTypeDef = TypedDict(
-    "GetAccessPreviewResponseTypeDef",
-    {
-        "accessPreview": AccessPreviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/PKG-INFO` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AccessAnalyzer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 accessanalyzer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 accessanalyzer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-accessanalyzer)](https://pepy.tech/project/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
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
@@ -361,31 +361,32 @@
 )
 
 
 def check_value(value: AccessPreviewStatusReasonCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_accessanalyzer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_accessanalyzer.type_defs import (
     AccessPreviewStatusReasonTypeDef,
     AclGranteeTypeDef,
     AnalyzedResourceSummaryTypeDef,
     AnalyzedResourceTypeDef,
     StatusReasonTypeDef,
     ApplyArchiveRuleRequestRequestTypeDef,
     CriterionOutputTypeDef,
     CancelPolicyGenerationRequestRequestTypeDef,
+    TimestampTypeDef,
     TrailTypeDef,
     TrailPropertiesTypeDef,
     EbsSnapshotConfigurationOutputTypeDef,
     EcrRepositoryConfigurationTypeDef,
     EfsFileSystemConfigurationTypeDef,
     IamRoleConfigurationTypeDef,
     SecretsManagerSecretConfigurationTypeDef,
@@ -439,31 +440,26 @@
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPolicyGenerationResponseTypeDef,
-    CreateArchiveRuleRequestRequestTypeDef,
+    CriterionUnionTypeDef,
     InlineArchiveRuleTypeDef,
-    ListAccessPreviewFindingsRequestRequestTypeDef,
-    UpdateArchiveRuleRequestRequestTypeDef,
     FindingSourceTypeDef,
     JobDetailsTypeDef,
     KmsGrantConfigurationOutputTypeDef,
     KmsGrantConfigurationTypeDef,
-    ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
     ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef,
     ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef,
     ListAnalyzersRequestListAnalyzersPaginateTypeDef,
     ListArchiveRulesRequestListArchiveRulesPaginateTypeDef,
     ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef,
     ValidatePolicyRequestValidatePolicyPaginateTypeDef,
-    ListFindingsRequestListFindingsPaginateTypeDef,
-    ListFindingsRequestRequestTypeDef,
     ListPolicyGenerationsResponseTypeDef,
     NetworkOriginConfigurationOutputTypeDef,
     NetworkOriginConfigurationTypeDef,
     PathElementTypeDef,
     SpanTypeDef,
     RdsDbClusterSnapshotConfigurationOutputTypeDef,
     RdsDbClusterSnapshotConfigurationTypeDef,
@@ -472,14 +468,20 @@
     ListAccessPreviewsResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
     StartPolicyGenerationRequestRequestTypeDef,
     GeneratedPolicyPropertiesTypeDef,
+    CreateArchiveRuleRequestRequestTypeDef,
+    ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
+    ListAccessPreviewFindingsRequestRequestTypeDef,
+    ListFindingsRequestListFindingsPaginateTypeDef,
+    ListFindingsRequestRequestTypeDef,
+    UpdateArchiveRuleRequestRequestTypeDef,
     CreateAnalyzerRequestRequestTypeDef,
     AccessPreviewFindingTypeDef,
     FindingSummaryTypeDef,
     FindingTypeDef,
     KmsKeyConfigurationOutputTypeDef,
     KmsKeyConfigurationTypeDef,
     S3AccessPointConfigurationOutputTypeDef,
@@ -493,20 +495,21 @@
     S3BucketConfigurationTypeDef,
     ValidatePolicyFindingTypeDef,
     GetGeneratedPolicyResponseTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ValidatePolicyResponseTypeDef,
     AccessPreviewTypeDef,
-    CreateAccessPreviewRequestRequestTypeDef,
+    ConfigurationUnionTypeDef,
     GetAccessPreviewResponseTypeDef,
+    CreateAccessPreviewRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessPreviewStatusReasonTypeDef:
+def get_value() -> AccessPreviewStatusReasonTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt` & `mypy-boto3-accessanalyzer-1.28.16/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15.post1/setup.py` & `mypy-boto3-accessanalyzer-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-accessanalyzer",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_accessanalyzer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.AccessAnalyzer 1.28.16 service generated with"
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
-    keywords="boto3 accessanalyzer type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 accessanalyzer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_accessanalyzer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

