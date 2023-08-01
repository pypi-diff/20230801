# Comparing `tmp/mypy-boto3-amplify-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-amplify-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplify-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:23 2023, max compression
+gzip compressed data, was "mypy-boto3-amplify-1.28.16.tar", last modified: Tue Aug  1 11:36:04 2023, max compression
```

## Comparing `mypy-boto3-amplify-1.28.15.post1.tar` & `mypy-boto3-amplify-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.892978 mypy-boto3-amplify-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-29 10:02:23.892978 mypy-boto3-amplify-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.868978 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28127 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35813 2023-07-29 09:37:41.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35754 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.892978 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:23.892978 mypy-boto3-amplify-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.776961 mypy-boto3-amplify-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-08-01 11:36:04.776961 mypy-boto3-amplify-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.764961 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27936 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27888 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-08-01 11:10:10.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-08-01 11:10:10.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36030 2023-08-01 11:10:11.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35971 2023-08-01 11:10:10.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.776961 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-08-01 11:36:04.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:36:04.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:04.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:36:04.000000 mypy-boto3-amplify-1.28.16/mypy_boto3_amplify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:04.776961 mypy-boto3-amplify-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:10:09.000000 mypy-boto3-amplify-1.28.16/setup.py
```

### Comparing `mypy-boto3-amplify-1.28.15.post1/LICENSE` & `mypy-boto3-amplify-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15.post1/PKG-INFO` & `mypy-boto3-amplify-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Amplify 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amplify type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 amplify type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
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
@@ -328,20 +328,20 @@
 )
 
 
 def check_value(value: DomainStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amplify.type_defs import (
     AutoBranchCreationConfigOutputTypeDef,
     CustomRuleTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
@@ -358,15 +358,15 @@
     DeleteAppRequestRequestTypeDef,
     DeleteBackendEnvironmentRequestRequestTypeDef,
     DeleteBranchRequestRequestTypeDef,
     DeleteDomainAssociationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     JobSummaryTypeDef,
     DeleteWebhookRequestRequestTypeDef,
-    GenerateAccessLogsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetAppRequestRequestTypeDef,
     GetArtifactUrlRequestRequestTypeDef,
     GetBackendEnvironmentRequestRequestTypeDef,
     GetBranchRequestRequestTypeDef,
     GetDomainAssociationRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetWebhookRequestRequestTypeDef,
@@ -377,21 +377,21 @@
     ListBackendEnvironmentsRequestRequestTypeDef,
     ListBranchesRequestRequestTypeDef,
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
     AppTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     DeleteBackendEnvironmentResultTypeDef,
     DeleteBranchResultTypeDef,
@@ -413,14 +413,16 @@
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
     ListJobsResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
+    GenerateAccessLogsRequestRequestTypeDef,
+    StartJobRequestRequestTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
@@ -433,15 +435,15 @@
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
 
 
-def get_structure() -> AutoBranchCreationConfigOutputTypeDef:
+def get_value() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplify-1.28.15.post1/README.md` & `mypy-boto3-amplify-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
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
@@ -296,20 +296,20 @@
 )
 
 
 def check_value(value: DomainStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amplify.type_defs import (
     AutoBranchCreationConfigOutputTypeDef,
     CustomRuleTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
@@ -326,15 +326,15 @@
     DeleteAppRequestRequestTypeDef,
     DeleteBackendEnvironmentRequestRequestTypeDef,
     DeleteBranchRequestRequestTypeDef,
     DeleteDomainAssociationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     JobSummaryTypeDef,
     DeleteWebhookRequestRequestTypeDef,
-    GenerateAccessLogsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetAppRequestRequestTypeDef,
     GetArtifactUrlRequestRequestTypeDef,
     GetBackendEnvironmentRequestRequestTypeDef,
     GetBranchRequestRequestTypeDef,
     GetDomainAssociationRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetWebhookRequestRequestTypeDef,
@@ -345,21 +345,21 @@
     ListBackendEnvironmentsRequestRequestTypeDef,
     ListBranchesRequestRequestTypeDef,
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
     AppTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     DeleteBackendEnvironmentResultTypeDef,
     DeleteBranchResultTypeDef,
@@ -381,14 +381,16 @@
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
     ListJobsResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
+    GenerateAccessLogsRequestRequestTypeDef,
+    StartJobRequestRequestTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
@@ -401,15 +403,15 @@
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
 
 
-def get_structure() -> AutoBranchCreationConfigOutputTypeDef:
+def get_value() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__init__.py` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__init__.pyi` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__main__.py` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Amplify 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Amplify 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify\nOther"
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

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/client.py` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,27 @@
     from mypy_boto3_amplify.client import AmplifyClient
 
     session = Session()
     client: AmplifyClient = session.client("amplify")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import JobTypeType, PlatformType, StageType
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
-    AutoBranchCreationConfigOutputTypeDef,
-    AutoBranchCreationConfigTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     CreateWebhookResultTypeDef,
     CustomRuleTypeDef,
@@ -58,14 +56,15 @@
     ListJobsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebhooksResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     SubDomainSettingTypeDef,
+    TimestampTypeDef,
     UpdateAppResultTypeDef,
     UpdateBranchResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
     UpdateWebhookResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -146,17 +145,15 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: Union[
-            AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
-        ] = ...
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#create_app)
         """
@@ -295,16 +292,16 @@
         """
 
     def generate_access_logs(
         self,
         *,
         domainName: str,
         appId: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...
     ) -> GenerateAccessLogsResultTypeDef:
         """
         Returns the website access logs for a specific time range using a presigned URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.generate_access_logs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#generate_access_logs)
         """
@@ -481,15 +478,15 @@
         appId: str,
         branchName: str,
         jobType: JobTypeType,
         jobId: str = ...,
         jobReason: str = ...,
         commitId: str = ...,
         commitMessage: str = ...,
-        commitTime: Union[datetime, str] = ...
+        commitTime: TimestampTypeDef = ...
     ) -> StartJobResultTypeDef:
         """
         Starts a new job for a branch of an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.start_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#start_job)
         """
@@ -532,17 +529,15 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: Union[
-            AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
-        ] = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/client.pyi` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,27 @@
     from mypy_boto3_amplify.client import AmplifyClient
 
     session = Session()
     client: AmplifyClient = session.client("amplify")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import JobTypeType, PlatformType, StageType
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
-    AutoBranchCreationConfigOutputTypeDef,
-    AutoBranchCreationConfigTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     CreateWebhookResultTypeDef,
     CustomRuleTypeDef,
@@ -58,14 +56,15 @@
     ListJobsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebhooksResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     SubDomainSettingTypeDef,
+    TimestampTypeDef,
     UpdateAppResultTypeDef,
     UpdateBranchResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
     UpdateWebhookResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -139,17 +138,15 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: Union[
-            AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
-        ] = ...
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#create_app)
         """
@@ -276,16 +273,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#delete_webhook)
         """
     def generate_access_logs(
         self,
         *,
         domainName: str,
         appId: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...
     ) -> GenerateAccessLogsResultTypeDef:
         """
         Returns the website access logs for a specific time range using a presigned URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.generate_access_logs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#generate_access_logs)
         """
@@ -444,15 +441,15 @@
         appId: str,
         branchName: str,
         jobType: JobTypeType,
         jobId: str = ...,
         jobReason: str = ...,
         commitId: str = ...,
         commitMessage: str = ...,
-        commitTime: Union[datetime, str] = ...
+        commitTime: TimestampTypeDef = ...
     ) -> StartJobResultTypeDef:
         """
         Starts a new job for a branch of an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.start_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#start_job)
         """
@@ -491,17 +488,15 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: Union[
-            AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
-        ] = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/literals.py` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/literals.pyi` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/paginator.py` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/paginator.pyi` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/type_defs.py` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
-    data: AutoBranchCreationConfigOutputTypeDef = {...}
+    data: AutoBranchCreationConfigOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -48,15 +48,15 @@
     "DeleteAppRequestRequestTypeDef",
     "DeleteBackendEnvironmentRequestRequestTypeDef",
     "DeleteBranchRequestRequestTypeDef",
     "DeleteDomainAssociationRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "JobSummaryTypeDef",
     "DeleteWebhookRequestRequestTypeDef",
-    "GenerateAccessLogsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetArtifactUrlRequestRequestTypeDef",
     "GetBackendEnvironmentRequestRequestTypeDef",
     "GetBranchRequestRequestTypeDef",
     "GetDomainAssociationRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetWebhookRequestRequestTypeDef",
@@ -67,21 +67,21 @@
     "ListBackendEnvironmentsRequestRequestTypeDef",
     "ListBranchesRequestRequestTypeDef",
     "ListDomainAssociationsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
-    "StartJobRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
     "AppTypeDef",
+    "AutoBranchCreationConfigUnionTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateBranchResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "DeleteBackendEnvironmentResultTypeDef",
     "DeleteBranchResultTypeDef",
@@ -103,14 +103,16 @@
     "ListWebhooksResultTypeDef",
     "UpdateWebhookResultTypeDef",
     "DeleteJobResultTypeDef",
     "ListJobsResultTypeDef",
     "StartDeploymentResultTypeDef",
     "StartJobResultTypeDef",
     "StopJobResultTypeDef",
+    "GenerateAccessLogsRequestRequestTypeDef",
+    "StartJobRequestRequestTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
@@ -475,38 +477,15 @@
 DeleteWebhookRequestRequestTypeDef = TypedDict(
     "DeleteWebhookRequestRequestTypeDef",
     {
         "webhookId": str,
     },
 )
 
-_RequiredGenerateAccessLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateAccessLogsRequestRequestTypeDef",
-    {
-        "domainName": str,
-        "appId": str,
-    },
-)
-_OptionalGenerateAccessLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateAccessLogsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GenerateAccessLogsRequestRequestTypeDef(
-    _RequiredGenerateAccessLogsRequestRequestTypeDef,
-    _OptionalGenerateAccessLogsRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 GetAppRequestRequestTypeDef = TypedDict(
     "GetAppRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
@@ -768,41 +747,14 @@
 
 class StartDeploymentRequestRequestTypeDef(
     _RequiredStartDeploymentRequestRequestTypeDef, _OptionalStartDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredStartJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartJobRequestRequestTypeDef",
-    {
-        "appId": str,
-        "branchName": str,
-        "jobType": JobTypeType,
-    },
-)
-_OptionalStartJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartJobRequestRequestTypeDef",
-    {
-        "jobId": str,
-        "jobReason": str,
-        "commitId": str,
-        "commitMessage": str,
-        "commitTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class StartJobRequestRequestTypeDef(
-    _RequiredStartJobRequestRequestTypeDef, _OptionalStartJobRequestRequestTypeDef
-):
-    pass
-
-
 StopJobRequestRequestTypeDef = TypedDict(
     "StopJobRequestRequestTypeDef",
     {
         "appId": str,
         "branchName": str,
         "jobId": str,
     },
@@ -919,14 +871,17 @@
 )
 
 
 class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
     pass
 
 
+AutoBranchCreationConfigUnionTypeDef = Union[
+    AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
+]
 _RequiredCreateAppRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAppRequestRequestTypeDef = TypedDict(
@@ -1256,14 +1211,65 @@
     "StopJobResultTypeDef",
     {
         "jobSummary": JobSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGenerateAccessLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateAccessLogsRequestRequestTypeDef",
+    {
+        "domainName": str,
+        "appId": str,
+    },
+)
+_OptionalGenerateAccessLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateAccessLogsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GenerateAccessLogsRequestRequestTypeDef(
+    _RequiredGenerateAccessLogsRequestRequestTypeDef,
+    _OptionalGenerateAccessLogsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "branchName": str,
+        "jobType": JobTypeType,
+    },
+)
+_OptionalStartJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartJobRequestRequestTypeDef",
+    {
+        "jobId": str,
+        "jobReason": str,
+        "commitId": str,
+        "commitMessage": str,
+        "commitTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class StartJobRequestRequestTypeDef(
+    _RequiredStartJobRequestRequestTypeDef, _OptionalStartJobRequestRequestTypeDef
+):
+    pass
+
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "summary": JobSummaryTypeDef,
         "steps": List[StepTypeDef],
     },
 )
```

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/type_defs.pyi` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
-    data: AutoBranchCreationConfigOutputTypeDef = {...}
+    data: AutoBranchCreationConfigOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -47,15 +47,15 @@
     "DeleteAppRequestRequestTypeDef",
     "DeleteBackendEnvironmentRequestRequestTypeDef",
     "DeleteBranchRequestRequestTypeDef",
     "DeleteDomainAssociationRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "JobSummaryTypeDef",
     "DeleteWebhookRequestRequestTypeDef",
-    "GenerateAccessLogsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetArtifactUrlRequestRequestTypeDef",
     "GetBackendEnvironmentRequestRequestTypeDef",
     "GetBranchRequestRequestTypeDef",
     "GetDomainAssociationRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetWebhookRequestRequestTypeDef",
@@ -66,21 +66,21 @@
     "ListBackendEnvironmentsRequestRequestTypeDef",
     "ListBranchesRequestRequestTypeDef",
     "ListDomainAssociationsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
-    "StartJobRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
     "AppTypeDef",
+    "AutoBranchCreationConfigUnionTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateBranchResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "DeleteBackendEnvironmentResultTypeDef",
     "DeleteBranchResultTypeDef",
@@ -102,14 +102,16 @@
     "ListWebhooksResultTypeDef",
     "UpdateWebhookResultTypeDef",
     "DeleteJobResultTypeDef",
     "ListJobsResultTypeDef",
     "StartDeploymentResultTypeDef",
     "StartJobResultTypeDef",
     "StopJobResultTypeDef",
+    "GenerateAccessLogsRequestRequestTypeDef",
+    "StartJobRequestRequestTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
@@ -458,36 +460,15 @@
 DeleteWebhookRequestRequestTypeDef = TypedDict(
     "DeleteWebhookRequestRequestTypeDef",
     {
         "webhookId": str,
     },
 )
 
-_RequiredGenerateAccessLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateAccessLogsRequestRequestTypeDef",
-    {
-        "domainName": str,
-        "appId": str,
-    },
-)
-_OptionalGenerateAccessLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateAccessLogsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GenerateAccessLogsRequestRequestTypeDef(
-    _RequiredGenerateAccessLogsRequestRequestTypeDef,
-    _OptionalGenerateAccessLogsRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 GetAppRequestRequestTypeDef = TypedDict(
     "GetAppRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
@@ -733,39 +714,14 @@
 )
 
 class StartDeploymentRequestRequestTypeDef(
     _RequiredStartDeploymentRequestRequestTypeDef, _OptionalStartDeploymentRequestRequestTypeDef
 ):
     pass
 
-_RequiredStartJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartJobRequestRequestTypeDef",
-    {
-        "appId": str,
-        "branchName": str,
-        "jobType": JobTypeType,
-    },
-)
-_OptionalStartJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartJobRequestRequestTypeDef",
-    {
-        "jobId": str,
-        "jobReason": str,
-        "commitId": str,
-        "commitMessage": str,
-        "commitTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class StartJobRequestRequestTypeDef(
-    _RequiredStartJobRequestRequestTypeDef, _OptionalStartJobRequestRequestTypeDef
-):
-    pass
-
 StopJobRequestRequestTypeDef = TypedDict(
     "StopJobRequestRequestTypeDef",
     {
         "appId": str,
         "branchName": str,
         "jobId": str,
     },
@@ -876,14 +832,17 @@
     },
     total=False,
 )
 
 class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
     pass
 
+AutoBranchCreationConfigUnionTypeDef = Union[
+    AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
+]
 _RequiredCreateAppRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAppRequestRequestTypeDef = TypedDict(
@@ -1205,14 +1164,61 @@
     "StopJobResultTypeDef",
     {
         "jobSummary": JobSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGenerateAccessLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateAccessLogsRequestRequestTypeDef",
+    {
+        "domainName": str,
+        "appId": str,
+    },
+)
+_OptionalGenerateAccessLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateAccessLogsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class GenerateAccessLogsRequestRequestTypeDef(
+    _RequiredGenerateAccessLogsRequestRequestTypeDef,
+    _OptionalGenerateAccessLogsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "branchName": str,
+        "jobType": JobTypeType,
+    },
+)
+_OptionalStartJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartJobRequestRequestTypeDef",
+    {
+        "jobId": str,
+        "jobReason": str,
+        "commitId": str,
+        "commitMessage": str,
+        "commitTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class StartJobRequestRequestTypeDef(
+    _RequiredStartJobRequestRequestTypeDef, _OptionalStartJobRequestRequestTypeDef
+):
+    pass
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "summary": JobSummaryTypeDef,
         "steps": List[StepTypeDef],
     },
 )
```

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/PKG-INFO` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Amplify 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amplify type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 amplify type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
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
@@ -328,20 +328,20 @@
 )
 
 
 def check_value(value: DomainStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amplify.type_defs import (
     AutoBranchCreationConfigOutputTypeDef,
     CustomRuleTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
@@ -358,15 +358,15 @@
     DeleteAppRequestRequestTypeDef,
     DeleteBackendEnvironmentRequestRequestTypeDef,
     DeleteBranchRequestRequestTypeDef,
     DeleteDomainAssociationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     JobSummaryTypeDef,
     DeleteWebhookRequestRequestTypeDef,
-    GenerateAccessLogsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetAppRequestRequestTypeDef,
     GetArtifactUrlRequestRequestTypeDef,
     GetBackendEnvironmentRequestRequestTypeDef,
     GetBranchRequestRequestTypeDef,
     GetDomainAssociationRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetWebhookRequestRequestTypeDef,
@@ -377,21 +377,21 @@
     ListBackendEnvironmentsRequestRequestTypeDef,
     ListBranchesRequestRequestTypeDef,
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
     AppTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     DeleteBackendEnvironmentResultTypeDef,
     DeleteBranchResultTypeDef,
@@ -413,14 +413,16 @@
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
     ListJobsResultTypeDef,
     StartDeploymentResultTypeDef,
     StartJobResultTypeDef,
     StopJobResultTypeDef,
+    GenerateAccessLogsRequestRequestTypeDef,
+    StartJobRequestRequestTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
@@ -433,15 +435,15 @@
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
 
 
-def get_structure() -> AutoBranchCreationConfigOutputTypeDef:
+def get_value() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/SOURCES.txt` & `mypy-boto3-amplify-1.28.16/mypy_boto3_amplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15.post1/setup.py` & `mypy-boto3-amplify-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplify",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_amplify"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Amplify 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 amplify type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 amplify type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_amplify": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

