# Comparing `tmp/mypy-boto3-codecatalyst-1.28.16.tar.gz` & `tmp/mypy-boto3-codecatalyst-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecatalyst-1.28.16.tar", last modified: Tue Aug  1 11:36:25 2023, max compression
+gzip compressed data, was "mypy-boto3-codecatalyst-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-codecatalyst-1.28.16.tar` & `mypy-boto3-codecatalyst-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.740928 mypy-boto3-codecatalyst-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-08-01 11:36:25.740928 mypy-boto3-codecatalyst-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.736928 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27830 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27782 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39241 2023-08-01 11:13:07.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39172 2023-08-01 11:13:05.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.740928 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-08-01 11:36:25.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:36:25.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:25.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:25.000000 mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:25.740928 mypy-boto3-codecatalyst-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:13:04.000000 mypy-boto3-codecatalyst-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.012775 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37203 2023-07-20 19:46:46.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37150 2023-07-20 19:46:46.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/setup.py
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/LICENSE` & `mypy-boto3-codecatalyst-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.16/PKG-INFO` & `mypy-boto3-codecatalyst-1.28.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.28.16
-Summary: Type annotations for boto3.CodeCatalyst 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.8
+Summary: Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codecatalyst type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 codecatalyst type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecatalyst)](https://pepy.tech/project/mypy-boto3-codecatalyst)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
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
@@ -347,25 +347,25 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
-    TimestampTypeDef,
+    CreateAccessTokenRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
     CreateProjectRequestRequestTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
     CreateSourceRepositoryRequestRequestTypeDef,
@@ -388,31 +388,31 @@
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
     GetSourceRepositoryRequestRequestTypeDef,
     GetSpaceRequestRequestTypeDef,
     GetSubscriptionRequestRequestTypeDef,
     GetUserDetailsRequestRequestTypeDef,
+    IdeConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
+    ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateSpaceRequestRequestTypeDef,
-    CreateAccessTokenRequestRequestTypeDef,
-    ListEventLogsRequestRequestTypeDef,
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
     CreateSourceRepositoryResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
     DeleteProjectResponseTypeDef,
@@ -428,24 +428,24 @@
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    UpdateDevEnvironmentResponseTypeDef,
     ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSpacesRequestListSpacesPaginateTypeDef,
@@ -457,15 +457,15 @@
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
 )
 
 
-def get_value() -> AccessTokenSummaryTypeDef:
+def get_structure() -> AccessTokenSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/README.md` & `mypy-boto3-codecatalyst-1.28.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecatalyst)](https://pepy.tech/project/mypy-boto3-codecatalyst)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
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
@@ -315,25 +315,25 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
-    TimestampTypeDef,
+    CreateAccessTokenRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
     CreateProjectRequestRequestTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
     CreateSourceRepositoryRequestRequestTypeDef,
@@ -356,31 +356,31 @@
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
     GetSourceRepositoryRequestRequestTypeDef,
     GetSpaceRequestRequestTypeDef,
     GetSubscriptionRequestRequestTypeDef,
     GetUserDetailsRequestRequestTypeDef,
+    IdeConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
+    ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateSpaceRequestRequestTypeDef,
-    CreateAccessTokenRequestRequestTypeDef,
-    ListEventLogsRequestRequestTypeDef,
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
     CreateSourceRepositoryResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
     DeleteProjectResponseTypeDef,
@@ -396,24 +396,24 @@
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    UpdateDevEnvironmentResponseTypeDef,
     ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSpacesRequestListSpacesPaginateTypeDef,
@@ -425,15 +425,15 @@
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
 )
 
 
-def get_value() -> AccessTokenSummaryTypeDef:
+def get_structure() -> AccessTokenSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/__init__.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/__init__.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/__main__.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCatalyst 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.CodeCatalyst 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/client.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_codecatalyst.client import CodeCatalystClient
 
     session = Session()
     client: CodeCatalystClient = session.client("codecatalyst")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import InstanceTypeType
 from .paginator import (
     ListAccessTokensPaginator,
     ListDevEnvironmentSessionsPaginator,
@@ -60,15 +61,14 @@
     PersistentStorageConfigurationTypeDef,
     ProjectListFilterTypeDef,
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
-    TimestampTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -128,15 +128,15 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#close)
         """
 
     def create_access_token(
-        self, *, name: str, expiresTime: TimestampTypeDef = ...
+        self, *, name: str, expiresTime: Union[datetime, str] = ...
     ) -> CreateAccessTokenResponseTypeDef:
         """
         Creates a personal access token (PAT) for the current user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_access_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#create_access_token)
         """
@@ -367,16 +367,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#list_dev_environments)
         """
 
     def list_event_logs(
         self,
         *,
         spaceName: str,
-        startTime: TimestampTypeDef,
-        endTime: TimestampTypeDef,
+        startTime: Union[datetime, str],
+        endTime: Union[datetime, str],
         eventName: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListEventLogsResponseTypeDef:
         """
         Retrieves a list of events that occurred during a specified time period in a
         space.
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/client.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_codecatalyst.client import CodeCatalystClient
 
     session = Session()
     client: CodeCatalystClient = session.client("codecatalyst")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import InstanceTypeType
 from .paginator import (
     ListAccessTokensPaginator,
     ListDevEnvironmentSessionsPaginator,
@@ -60,15 +61,14 @@
     PersistentStorageConfigurationTypeDef,
     ProjectListFilterTypeDef,
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
-    TimestampTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -121,15 +121,15 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#close)
         """
     def create_access_token(
-        self, *, name: str, expiresTime: TimestampTypeDef = ...
+        self, *, name: str, expiresTime: Union[datetime, str] = ...
     ) -> CreateAccessTokenResponseTypeDef:
         """
         Creates a personal access token (PAT) for the current user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_access_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#create_access_token)
         """
@@ -339,16 +339,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#list_dev_environments)
         """
     def list_event_logs(
         self,
         *,
         spaceName: str,
-        startTime: TimestampTypeDef,
-        endTime: TimestampTypeDef,
+        startTime: Union[datetime, str],
+        endTime: Union[datetime, str],
         eventName: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListEventLogsResponseTypeDef:
         """
         Retrieves a list of events that occurred during a specified time period in a
         space.
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/literals.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,14 @@
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
@@ -264,15 +263,14 @@
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
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/literals.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,14 @@
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
@@ -262,15 +261,14 @@
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
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/paginator.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator("list_source_repositories")
     list_source_repository_branches_paginator: ListSourceRepositoryBranchesPaginator = client.get_paginator("list_source_repository_branches")
     list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     FilterTypeDef,
     ListAccessTokensResponseTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
@@ -45,15 +46,14 @@
     ListEventLogsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     PaginatorConfigTypeDef,
     ProjectListFilterTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = (
     "ListAccessTokensPaginator",
     "ListDevEnvironmentSessionsPaginator",
     "ListDevEnvironmentsPaginator",
     "ListEventLogsPaginator",
@@ -135,16 +135,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
-        startTime: TimestampTypeDef,
-        endTime: TimestampTypeDef,
+        startTime: Union[datetime, str],
+        endTime: Union[datetime, str],
         eventName: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
         """
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/paginator.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator("list_source_repositories")
     list_source_repository_branches_paginator: ListSourceRepositoryBranchesPaginator = client.get_paginator("list_source_repository_branches")
     list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     FilterTypeDef,
     ListAccessTokensResponseTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
@@ -45,15 +46,14 @@
     ListEventLogsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     PaginatorConfigTypeDef,
     ProjectListFilterTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = (
     "ListAccessTokensPaginator",
     "ListDevEnvironmentSessionsPaginator",
     "ListDevEnvironmentsPaginator",
     "ListEventLogsPaginator",
@@ -129,16 +129,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
-        startTime: TimestampTypeDef,
-        endTime: TimestampTypeDef,
+        startTime: Union[datetime, str],
+        endTime: Union[datetime, str],
         eventName: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
         """
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/type_defs.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codecatalyst.type_defs import AccessTokenSummaryTypeDef
 
-    data: AccessTokenSummaryTypeDef = ...
+    data: AccessTokenSummaryTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -32,15 +32,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessTokenSummaryTypeDef",
-    "TimestampTypeDef",
+    "CreateAccessTokenRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
     "CreateSourceRepositoryRequestRequestTypeDef",
@@ -63,31 +63,31 @@
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     "GetSourceRepositoryRequestRequestTypeDef",
     "GetSpaceRequestRequestTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
+    "IdeConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
+    "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
-    "CreateAccessTokenRequestRequestTypeDef",
-    "ListEventLogsRequestRequestTypeDef",
     "CreateAccessTokenResponseTypeDef",
     "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchResponseTypeDef",
     "CreateSourceRepositoryResponseTypeDef",
     "DeleteDevEnvironmentResponseTypeDef",
     "DeleteProjectResponseTypeDef",
@@ -103,24 +103,24 @@
     "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
-    "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
+    "UpdateDevEnvironmentResponseTypeDef",
     "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSpacesRequestListSpacesPaginateTypeDef",
@@ -131,37 +131,44 @@
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     "ListDevEnvironmentsResponseTypeDef",
     "ListEventLogsResponseTypeDef",
 )
 
-_RequiredAccessTokenSummaryTypeDef = TypedDict(
-    "_RequiredAccessTokenSummaryTypeDef",
+AccessTokenSummaryTypeDef = TypedDict(
+    "AccessTokenSummaryTypeDef",
     {
         "id": str,
         "name": str,
+        "expiresTime": datetime,
     },
 )
-_OptionalAccessTokenSummaryTypeDef = TypedDict(
-    "_OptionalAccessTokenSummaryTypeDef",
+
+_RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
-        "expiresTime": datetime,
+        "name": str,
+    },
+)
+_OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessTokenRequestRequestTypeDef",
+    {
+        "expiresTime": Union[datetime, str],
     },
     total=False,
 )
 
 
-class AccessTokenSummaryTypeDef(
-    _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
+class CreateAccessTokenRequestRequestTypeDef(
+    _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
 ):
     pass
 
 
-TimestampTypeDef = Union[datetime, str]
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -319,35 +326,22 @@
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
 
-_RequiredDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentRepositorySummaryTypeDef",
+DevEnvironmentRepositorySummaryTypeDef = TypedDict(
+    "DevEnvironmentRepositorySummaryTypeDef",
     {
         "repositoryName": str,
-    },
-)
-_OptionalDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentRepositorySummaryTypeDef",
-    {
         "branchName": str,
     },
-    total=False,
 )
 
-
-class DevEnvironmentRepositorySummaryTypeDef(
-    _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
-):
-    pass
-
-
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
@@ -379,15 +373,14 @@
 
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
 PersistentStorageTypeDef = TypedDict(
     "PersistentStorageTypeDef",
     {
         "sizeInGiB": int,
     },
@@ -395,56 +388,42 @@
 
 EmailAddressTypeDef = TypedDict(
     "EmailAddressTypeDef",
     {
         "email": str,
         "verified": bool,
     },
-    total=False,
 )
 
 EventPayloadTypeDef = TypedDict(
     "EventPayloadTypeDef",
     {
         "contentType": str,
         "data": str,
     },
-    total=False,
 )
 
 ProjectInformationTypeDef = TypedDict(
     "ProjectInformationTypeDef",
     {
         "name": str,
         "projectId": str,
     },
-    total=False,
 )
 
-_RequiredUserIdentityTypeDef = TypedDict(
-    "_RequiredUserIdentityTypeDef",
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
     {
         "userType": UserTypeType,
         "principalId": str,
-    },
-)
-_OptionalUserIdentityTypeDef = TypedDict(
-    "_OptionalUserIdentityTypeDef",
-    {
         "userName": str,
         "awsAccountId": str,
     },
-    total=False,
 )
 
-
-class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
-    pass
-
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -515,14 +494,22 @@
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
+IdeConfigurationOutputTypeDef = TypedDict(
+    "IdeConfigurationOutputTypeDef",
+    {
+        "runtime": str,
+        "name": str,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -559,14 +546,39 @@
 class ListDevEnvironmentSessionsRequestRequestTypeDef(
     _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
     _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListEventLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListEventLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestRequestTypeDef",
+    {
+        "eventName": str,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListEventLogsRequestRequestTypeDef(
+    _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredProjectListFilterTypeDef = TypedDict(
     "_RequiredProjectListFilterTypeDef",
     {
         "key": Literal["hasAccessTo"],
         "values": Sequence[str],
     },
 )
@@ -581,57 +593,33 @@
 
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
-
-
-_RequiredListSourceRepositoriesItemTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesItemTypeDef",
+ListSourceRepositoriesItemTypeDef = TypedDict(
+    "ListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
+        "description": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
     },
 )
-_OptionalListSourceRepositoriesItemTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesItemTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoriesItemTypeDef(
-    _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
-):
-    pass
-
 
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
@@ -657,15 +645,14 @@
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
-    total=False,
 )
 
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
@@ -693,35 +680,24 @@
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredSpaceSummaryTypeDef = TypedDict(
-    "_RequiredSpaceSummaryTypeDef",
+SpaceSummaryTypeDef = TypedDict(
+    "SpaceSummaryTypeDef",
     {
         "name": str,
         "regionName": str,
-    },
-)
-_OptionalSpaceSummaryTypeDef = TypedDict(
-    "_OptionalSpaceSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-
-class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
-    pass
-
-
 StopDevEnvironmentRequestRequestTypeDef = TypedDict(
     "StopDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
@@ -776,60 +752,14 @@
 
 class UpdateSpaceRequestRequestTypeDef(
     _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessTokenRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessTokenRequestRequestTypeDef",
-    {
-        "expiresTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateAccessTokenRequestRequestTypeDef(
-    _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredListEventLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestRequestTypeDef",
-    {
-        "spaceName": str,
-        "startTime": TimestampTypeDef,
-        "endTime": TimestampTypeDef,
-    },
-)
-_OptionalListEventLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestRequestTypeDef",
-    {
-        "eventName": str,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListEventLogsRequestRequestTypeDef(
-    _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
-):
-    pass
-
-
 CreateAccessTokenResponseTypeDef = TypedDict(
     "CreateAccessTokenResponseTypeDef",
     {
         "secret": str,
         "name": str,
         "expiresTime": datetime,
         "accessTokenId": str,
@@ -1092,29 +1022,14 @@
 class UpdateDevEnvironmentRequestRequestTypeDef(
     _RequiredUpdateDevEnvironmentRequestRequestTypeDef,
     _OptionalUpdateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateDevEnvironmentResponseTypeDef = TypedDict(
-    "UpdateDevEnvironmentResponseTypeDef",
-    {
-        "id": str,
-        "spaceName": str,
-        "projectName": str,
-        "alias": str,
-        "ides": List[IdeConfigurationTypeDef],
-        "instanceType": InstanceTypeType,
-        "inactivityTimeoutMinutes": int,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "instanceType": InstanceTypeType,
         "persistentStorage": PersistentStorageConfigurationTypeDef,
@@ -1179,45 +1094,32 @@
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDevEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentSummaryTypeDef",
+DevEnvironmentSummaryTypeDef = TypedDict(
+    "DevEnvironmentSummaryTypeDef",
     {
+        "spaceName": str,
+        "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
         "status": DevEnvironmentStatusType,
+        "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
+        "alias": str,
+        "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
     },
 )
-_OptionalDevEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentSummaryTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "statusReason": str,
-        "alias": str,
-        "ides": List[IdeTypeDef],
-    },
-    total=False,
-)
-
-
-class DevEnvironmentSummaryTypeDef(
-    _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
-):
-    pass
-
 
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
@@ -1243,46 +1145,35 @@
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventLogEntryTypeDef = TypedDict(
-    "_RequiredEventLogEntryTypeDef",
+EventLogEntryTypeDef = TypedDict(
+    "EventLogEntryTypeDef",
     {
         "id": str,
         "eventName": str,
         "eventType": str,
         "eventCategory": str,
         "eventSource": str,
         "eventTime": datetime,
         "operationType": OperationTypeType,
         "userIdentity": UserIdentityTypeDef,
-    },
-)
-_OptionalEventLogEntryTypeDef = TypedDict(
-    "_OptionalEventLogEntryTypeDef",
-    {
         "projectInformation": ProjectInformationTypeDef,
         "requestId": str,
         "requestPayload": EventPayloadTypeDef,
         "responsePayload": EventPayloadTypeDef,
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
-    total=False,
 )
 
-
-class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
-    pass
-
-
 _RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
@@ -1300,14 +1191,29 @@
 class ListDevEnvironmentsRequestRequestTypeDef(
     _RequiredListDevEnvironmentsRequestRequestTypeDef,
     _OptionalListDevEnvironmentsRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateDevEnvironmentResponseTypeDef = TypedDict(
+    "UpdateDevEnvironmentResponseTypeDef",
+    {
+        "id": str,
+        "spaceName": str,
+        "projectName": str,
+        "alias": str,
+        "ides": List[IdeConfigurationOutputTypeDef],
+        "instanceType": InstanceTypeType,
+        "inactivityTimeoutMinutes": int,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
     "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1360,16 +1266,16 @@
     pass
 
 
 _RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
     "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
     {
         "spaceName": str,
-        "startTime": TimestampTypeDef,
-        "endTime": TimestampTypeDef,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
     },
 )
 _OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
     "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
     {
         "eventName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst/type_defs.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codecatalyst.type_defs import AccessTokenSummaryTypeDef
 
-    data: AccessTokenSummaryTypeDef = ...
+    data: AccessTokenSummaryTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -31,15 +31,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessTokenSummaryTypeDef",
-    "TimestampTypeDef",
+    "CreateAccessTokenRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
     "CreateSourceRepositoryRequestRequestTypeDef",
@@ -62,31 +62,31 @@
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     "GetSourceRepositoryRequestRequestTypeDef",
     "GetSpaceRequestRequestTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
+    "IdeConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
+    "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
-    "CreateAccessTokenRequestRequestTypeDef",
-    "ListEventLogsRequestRequestTypeDef",
     "CreateAccessTokenResponseTypeDef",
     "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchResponseTypeDef",
     "CreateSourceRepositoryResponseTypeDef",
     "DeleteDevEnvironmentResponseTypeDef",
     "DeleteProjectResponseTypeDef",
@@ -102,24 +102,24 @@
     "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
-    "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
+    "UpdateDevEnvironmentResponseTypeDef",
     "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSpacesRequestListSpacesPaginateTypeDef",
@@ -130,35 +130,42 @@
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     "ListDevEnvironmentsResponseTypeDef",
     "ListEventLogsResponseTypeDef",
 )
 
-_RequiredAccessTokenSummaryTypeDef = TypedDict(
-    "_RequiredAccessTokenSummaryTypeDef",
+AccessTokenSummaryTypeDef = TypedDict(
+    "AccessTokenSummaryTypeDef",
     {
         "id": str,
         "name": str,
+        "expiresTime": datetime,
     },
 )
-_OptionalAccessTokenSummaryTypeDef = TypedDict(
-    "_OptionalAccessTokenSummaryTypeDef",
+
+_RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
-        "expiresTime": datetime,
+        "name": str,
+    },
+)
+_OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessTokenRequestRequestTypeDef",
+    {
+        "expiresTime": Union[datetime, str],
     },
     total=False,
 )
 
-class AccessTokenSummaryTypeDef(
-    _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
+class CreateAccessTokenRequestRequestTypeDef(
+    _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
 ):
     pass
 
-TimestampTypeDef = Union[datetime, str]
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -308,33 +315,22 @@
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
 
-_RequiredDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentRepositorySummaryTypeDef",
+DevEnvironmentRepositorySummaryTypeDef = TypedDict(
+    "DevEnvironmentRepositorySummaryTypeDef",
     {
         "repositoryName": str,
-    },
-)
-_OptionalDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentRepositorySummaryTypeDef",
-    {
         "branchName": str,
     },
-    total=False,
 )
 
-class DevEnvironmentRepositorySummaryTypeDef(
-    _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
-):
-    pass
-
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
@@ -364,15 +360,14 @@
 
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
 PersistentStorageTypeDef = TypedDict(
     "PersistentStorageTypeDef",
     {
         "sizeInGiB": int,
     },
@@ -380,54 +375,42 @@
 
 EmailAddressTypeDef = TypedDict(
     "EmailAddressTypeDef",
     {
         "email": str,
         "verified": bool,
     },
-    total=False,
 )
 
 EventPayloadTypeDef = TypedDict(
     "EventPayloadTypeDef",
     {
         "contentType": str,
         "data": str,
     },
-    total=False,
 )
 
 ProjectInformationTypeDef = TypedDict(
     "ProjectInformationTypeDef",
     {
         "name": str,
         "projectId": str,
     },
-    total=False,
 )
 
-_RequiredUserIdentityTypeDef = TypedDict(
-    "_RequiredUserIdentityTypeDef",
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
     {
         "userType": UserTypeType,
         "principalId": str,
-    },
-)
-_OptionalUserIdentityTypeDef = TypedDict(
-    "_OptionalUserIdentityTypeDef",
-    {
         "userName": str,
         "awsAccountId": str,
     },
-    total=False,
 )
 
-class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
-    pass
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -496,14 +479,22 @@
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
+IdeConfigurationOutputTypeDef = TypedDict(
+    "IdeConfigurationOutputTypeDef",
+    {
+        "runtime": str,
+        "name": str,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -538,14 +529,37 @@
 
 class ListDevEnvironmentSessionsRequestRequestTypeDef(
     _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
     _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListEventLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListEventLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestRequestTypeDef",
+    {
+        "eventName": str,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListEventLogsRequestRequestTypeDef(
+    _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
+):
+    pass
+
 _RequiredProjectListFilterTypeDef = TypedDict(
     "_RequiredProjectListFilterTypeDef",
     {
         "key": Literal["hasAccessTo"],
         "values": Sequence[str],
     },
 )
@@ -558,53 +572,33 @@
 )
 
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
-
-_RequiredListSourceRepositoriesItemTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesItemTypeDef",
+ListSourceRepositoriesItemTypeDef = TypedDict(
+    "ListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
+        "description": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
     },
 )
-_OptionalListSourceRepositoriesItemTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesItemTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-class ListSourceRepositoriesItemTypeDef(
-    _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
-):
-    pass
 
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
@@ -628,15 +622,14 @@
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
-    total=False,
 )
 
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
@@ -662,33 +655,24 @@
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredSpaceSummaryTypeDef = TypedDict(
-    "_RequiredSpaceSummaryTypeDef",
+SpaceSummaryTypeDef = TypedDict(
+    "SpaceSummaryTypeDef",
     {
         "name": str,
         "regionName": str,
-    },
-)
-_OptionalSpaceSummaryTypeDef = TypedDict(
-    "_OptionalSpaceSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
-    pass
-
 StopDevEnvironmentRequestRequestTypeDef = TypedDict(
     "StopDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
@@ -739,56 +723,14 @@
 )
 
 class UpdateSpaceRequestRequestTypeDef(
     _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessTokenRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessTokenRequestRequestTypeDef",
-    {
-        "expiresTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-class CreateAccessTokenRequestRequestTypeDef(
-    _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
-):
-    pass
-
-_RequiredListEventLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestRequestTypeDef",
-    {
-        "spaceName": str,
-        "startTime": TimestampTypeDef,
-        "endTime": TimestampTypeDef,
-    },
-)
-_OptionalListEventLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestRequestTypeDef",
-    {
-        "eventName": str,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListEventLogsRequestRequestTypeDef(
-    _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
-):
-    pass
-
 CreateAccessTokenResponseTypeDef = TypedDict(
     "CreateAccessTokenResponseTypeDef",
     {
         "secret": str,
         "name": str,
         "expiresTime": datetime,
         "accessTokenId": str,
@@ -1047,29 +989,14 @@
 
 class UpdateDevEnvironmentRequestRequestTypeDef(
     _RequiredUpdateDevEnvironmentRequestRequestTypeDef,
     _OptionalUpdateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
-UpdateDevEnvironmentResponseTypeDef = TypedDict(
-    "UpdateDevEnvironmentResponseTypeDef",
-    {
-        "id": str,
-        "spaceName": str,
-        "projectName": str,
-        "alias": str,
-        "ides": List[IdeConfigurationTypeDef],
-        "instanceType": InstanceTypeType,
-        "inactivityTimeoutMinutes": int,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "instanceType": InstanceTypeType,
         "persistentStorage": PersistentStorageConfigurationTypeDef,
@@ -1130,43 +1057,32 @@
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDevEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentSummaryTypeDef",
+DevEnvironmentSummaryTypeDef = TypedDict(
+    "DevEnvironmentSummaryTypeDef",
     {
+        "spaceName": str,
+        "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
         "status": DevEnvironmentStatusType,
+        "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
+        "alias": str,
+        "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
     },
 )
-_OptionalDevEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentSummaryTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "statusReason": str,
-        "alias": str,
-        "ides": List[IdeTypeDef],
-    },
-    total=False,
-)
-
-class DevEnvironmentSummaryTypeDef(
-    _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
-):
-    pass
 
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
@@ -1192,44 +1108,35 @@
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventLogEntryTypeDef = TypedDict(
-    "_RequiredEventLogEntryTypeDef",
+EventLogEntryTypeDef = TypedDict(
+    "EventLogEntryTypeDef",
     {
         "id": str,
         "eventName": str,
         "eventType": str,
         "eventCategory": str,
         "eventSource": str,
         "eventTime": datetime,
         "operationType": OperationTypeType,
         "userIdentity": UserIdentityTypeDef,
-    },
-)
-_OptionalEventLogEntryTypeDef = TypedDict(
-    "_OptionalEventLogEntryTypeDef",
-    {
         "projectInformation": ProjectInformationTypeDef,
         "requestId": str,
         "requestPayload": EventPayloadTypeDef,
         "responsePayload": EventPayloadTypeDef,
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
-    total=False,
 )
 
-class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
-    pass
-
 _RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
@@ -1245,14 +1152,29 @@
 
 class ListDevEnvironmentsRequestRequestTypeDef(
     _RequiredListDevEnvironmentsRequestRequestTypeDef,
     _OptionalListDevEnvironmentsRequestRequestTypeDef,
 ):
     pass
 
+UpdateDevEnvironmentResponseTypeDef = TypedDict(
+    "UpdateDevEnvironmentResponseTypeDef",
+    {
+        "id": str,
+        "spaceName": str,
+        "projectName": str,
+        "alias": str,
+        "ides": List[IdeConfigurationOutputTypeDef],
+        "instanceType": InstanceTypeType,
+        "inactivityTimeoutMinutes": int,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
     "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1301,16 +1223,16 @@
 ):
     pass
 
 _RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
     "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
     {
         "spaceName": str,
-        "startTime": TimestampTypeDef,
-        "endTime": TimestampTypeDef,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
     },
 )
 _OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
     "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
     {
         "eventName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst.egg-info/PKG-INFO` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.28.16
-Summary: Type annotations for boto3.CodeCatalyst 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.8
+Summary: Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codecatalyst type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 codecatalyst type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecatalyst)](https://pepy.tech/project/mypy-boto3-codecatalyst)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
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
@@ -347,25 +347,25 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
-    TimestampTypeDef,
+    CreateAccessTokenRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
     CreateProjectRequestRequestTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
     CreateSourceRepositoryRequestRequestTypeDef,
@@ -388,31 +388,31 @@
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
     GetSourceRepositoryRequestRequestTypeDef,
     GetSpaceRequestRequestTypeDef,
     GetSubscriptionRequestRequestTypeDef,
     GetUserDetailsRequestRequestTypeDef,
+    IdeConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
+    ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateSpaceRequestRequestTypeDef,
-    CreateAccessTokenRequestRequestTypeDef,
-    ListEventLogsRequestRequestTypeDef,
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
     CreateSourceRepositoryResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
     DeleteProjectResponseTypeDef,
@@ -428,24 +428,24 @@
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    UpdateDevEnvironmentResponseTypeDef,
     ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSpacesRequestListSpacesPaginateTypeDef,
@@ -457,15 +457,15 @@
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
 )
 
 
-def get_value() -> AccessTokenSummaryTypeDef:
+def get_structure() -> AccessTokenSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codecatalyst-1.28.16/mypy_boto3_codecatalyst.egg-info/SOURCES.txt` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.16/setup.py` & `mypy-boto3-codecatalyst-1.28.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codecatalyst",
-    version="1.28.16",
+    version="1.28.8",
     packages=["mypy_boto3_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCatalyst 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
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
-    keywords="boto3 codecatalyst type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 codecatalyst type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codecatalyst": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

