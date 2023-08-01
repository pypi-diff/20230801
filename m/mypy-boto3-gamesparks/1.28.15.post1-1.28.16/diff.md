# Comparing `tmp/mypy-boto3-gamesparks-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-gamesparks-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-gamesparks-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:11 2023, max compression
+gzip compressed data, was "mypy-boto3-gamesparks-1.28.16.tar", last modified: Tue Aug  1 11:36:52 2023, max compression
```

## Comparing `mypy-boto3-gamesparks-1.28.15.post1.tar` & `mypy-boto3-gamesparks-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:11.485162 mypy-boto3-gamesparks-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-29 10:03:11.485162 mypy-boto3-gamesparks-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:11.473162 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29790 2023-07-29 09:46:01.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-07-29 09:46:01.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:00.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:11.485162 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-29 10:03:11.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:11.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:11.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:11.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:11.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:11.000000 mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:11.485162 mypy-boto3-gamesparks-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:45:59.000000 mypy-boto3-gamesparks-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.024882 mypy-boto3-gamesparks-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-08-01 11:36:52.016882 mypy-boto3-gamesparks-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.008882 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-08-01 11:18:38.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29778 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:18:37.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.016882 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-08-01 11:36:51.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:36:51.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:51.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:51.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:51.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:51.000000 mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:52.024882 mypy-boto3-gamesparks-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:18:36.000000 mypy-boto3-gamesparks-1.28.16/setup.py
```

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/LICENSE` & `mypy-boto3-gamesparks-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/PKG-INFO` & `mypy-boto3-gamesparks-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamesparks
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GameSparks 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GameSparks 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 gamesparks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 gamesparks type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamesparks)](https://pepy.tech/project/mypy-boto3-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameSparks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[boto3.GameSparks 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [mypy-boto3-gamesparks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/).
 
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
@@ -342,23 +342,24 @@
 )
 
 
 def check_value(value: DeploymentActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_gamesparks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_gamesparks.type_defs import (
+    BlobTypeDef,
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
     ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
@@ -378,15 +379,14 @@
     GetGameConfigurationRequestRequestTypeDef,
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    ImportGameConfigurationSourceTypeDef,
     PaginatorConfigTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListGamesRequestRequestTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
@@ -397,14 +397,15 @@
     SectionModificationTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
+    ImportGameConfigurationSourceTypeDef,
     CreateGameResultTypeDef,
     DisconnectPlayerResultTypeDef,
     ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
     GetPlayerConnectionStatusResultTypeDef,
     ListTagsForResourceResultTypeDef,
     StartGeneratedCodeJobResultTypeDef,
@@ -420,38 +421,38 @@
     ListExtensionVersionsResultTypeDef,
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
-    ImportGameConfigurationRequestRequestTypeDef,
     ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
     ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListGamesRequestListGamesPaginateTypeDef,
     ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
+    ImportGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
     ImportGameConfigurationResultTypeDef,
     UpdateGameConfigurationResultTypeDef,
     CreateSnapshotResultTypeDef,
     GetSnapshotResultTypeDef,
     UpdateSnapshotResultTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/README.md` & `mypy-boto3-gamesparks-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamesparks)](https://pepy.tech/project/mypy-boto3-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameSparks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[boto3.GameSparks 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [mypy-boto3-gamesparks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/).
 
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
@@ -310,23 +310,24 @@
 )
 
 
 def check_value(value: DeploymentActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_gamesparks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_gamesparks.type_defs import (
+    BlobTypeDef,
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
     ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
@@ -346,15 +347,14 @@
     GetGameConfigurationRequestRequestTypeDef,
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    ImportGameConfigurationSourceTypeDef,
     PaginatorConfigTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListGamesRequestRequestTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
@@ -365,14 +365,15 @@
     SectionModificationTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
+    ImportGameConfigurationSourceTypeDef,
     CreateGameResultTypeDef,
     DisconnectPlayerResultTypeDef,
     ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
     GetPlayerConnectionStatusResultTypeDef,
     ListTagsForResourceResultTypeDef,
     StartGeneratedCodeJobResultTypeDef,
@@ -388,38 +389,38 @@
     ListExtensionVersionsResultTypeDef,
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
-    ImportGameConfigurationRequestRequestTypeDef,
     ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
     ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListGamesRequestListGamesPaginateTypeDef,
     ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
+    ImportGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
     ImportGameConfigurationResultTypeDef,
     UpdateGameConfigurationResultTypeDef,
     CreateSnapshotResultTypeDef,
     GetSnapshotResultTypeDef,
     UpdateSnapshotResultTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/__init__.py` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/__init__.pyi` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/__main__.py` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GameSparks 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.GameSparks 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks\nOther"
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

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/client.py` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/client.pyi` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/literals.py` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/literals.pyi` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/paginator.py` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/paginator.pyi` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/type_defs.py` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for gamesparks service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_gamesparks.type_defs import ConnectionTypeDef
+    from mypy_boto3_gamesparks.type_defs import BlobTypeDef
 
-    data: ConnectionTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -30,14 +30,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "ConnectionTypeDef",
     "CreateGameRequestRequestTypeDef",
     "GameDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateStageRequestRequestTypeDef",
     "StageDetailsTypeDef",
@@ -57,15 +58,14 @@
     "GetGameConfigurationRequestRequestTypeDef",
     "GetGameRequestRequestTypeDef",
     "GetGeneratedCodeJobRequestRequestTypeDef",
     "GetPlayerConnectionStatusRequestRequestTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetStageDeploymentRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "ImportGameConfigurationSourceTypeDef",
     "PaginatorConfigTypeDef",
     "ListExtensionVersionsRequestRequestTypeDef",
     "ListExtensionsRequestRequestTypeDef",
     "ListGamesRequestRequestTypeDef",
     "ListGeneratedCodeJobsRequestRequestTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "SnapshotSummaryTypeDef",
@@ -76,14 +76,15 @@
     "SectionModificationTypeDef",
     "StartStageDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGameRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
+    "ImportGameConfigurationSourceTypeDef",
     "CreateGameResultTypeDef",
     "DisconnectPlayerResultTypeDef",
     "ExportSnapshotResultTypeDef",
     "GetGameResultTypeDef",
     "GetPlayerConnectionStatusResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StartGeneratedCodeJobResultTypeDef",
@@ -99,36 +100,37 @@
     "ListExtensionVersionsResultTypeDef",
     "GameConfigurationDetailsTypeDef",
     "SnapshotDetailsTypeDef",
     "ListGamesResultTypeDef",
     "GetGeneratedCodeJobResultTypeDef",
     "ListGeneratedCodeJobsResultTypeDef",
     "StartGeneratedCodeJobRequestRequestTypeDef",
-    "ImportGameConfigurationRequestRequestTypeDef",
     "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
     "ListExtensionsRequestListExtensionsPaginateTypeDef",
     "ListGamesRequestListGamesPaginateTypeDef",
     "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
     "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
     "ListStagesRequestListStagesPaginateTypeDef",
     "ListSnapshotsResultTypeDef",
     "ListStagesResultTypeDef",
     "UpdateGameConfigurationRequestRequestTypeDef",
+    "ImportGameConfigurationRequestRequestTypeDef",
     "GetStageDeploymentResultTypeDef",
     "StartStageDeploymentResultTypeDef",
     "ListStageDeploymentsResultTypeDef",
     "GetGameConfigurationResultTypeDef",
     "ImportGameConfigurationResultTypeDef",
     "UpdateGameConfigurationResultTypeDef",
     "CreateSnapshotResultTypeDef",
     "GetSnapshotResultTypeDef",
     "UpdateSnapshotResultTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Created": datetime,
         "Id": str,
     },
     total=False,
@@ -464,21 +466,14 @@
     "GetStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
 
-ImportGameConfigurationSourceTypeDef = TypedDict(
-    "ImportGameConfigurationSourceTypeDef",
-    {
-        "File": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -774,14 +769,21 @@
 
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
 
+ImportGameConfigurationSourceTypeDef = TypedDict(
+    "ImportGameConfigurationSourceTypeDef",
+    {
+        "File": BlobTypeDef,
+    },
+)
+
 CreateGameResultTypeDef = TypedDict(
     "CreateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -981,22 +983,14 @@
     {
         "GameName": str,
         "Generator": GeneratorTypeDef,
         "SnapshotId": str,
     },
 )
 
-ImportGameConfigurationRequestRequestTypeDef = TypedDict(
-    "ImportGameConfigurationRequestRequestTypeDef",
-    {
-        "GameName": str,
-        "ImportSource": ImportGameConfigurationSourceTypeDef,
-    },
-)
-
 _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
     "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
     {
         "Name": str,
         "Namespace": str,
     },
 )
@@ -1144,14 +1138,22 @@
     "UpdateGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
         "Modifications": Sequence[SectionModificationTypeDef],
     },
 )
 
+ImportGameConfigurationRequestRequestTypeDef = TypedDict(
+    "ImportGameConfigurationRequestRequestTypeDef",
+    {
+        "GameName": str,
+        "ImportSource": ImportGameConfigurationSourceTypeDef,
+    },
+)
+
 GetStageDeploymentResultTypeDef = TypedDict(
     "GetStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks/type_defs.pyi` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for gamesparks service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_gamesparks.type_defs import ConnectionTypeDef
+    from mypy_boto3_gamesparks.type_defs import BlobTypeDef
 
-    data: ConnectionTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -29,14 +29,15 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "ConnectionTypeDef",
     "CreateGameRequestRequestTypeDef",
     "GameDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateStageRequestRequestTypeDef",
     "StageDetailsTypeDef",
@@ -56,15 +57,14 @@
     "GetGameConfigurationRequestRequestTypeDef",
     "GetGameRequestRequestTypeDef",
     "GetGeneratedCodeJobRequestRequestTypeDef",
     "GetPlayerConnectionStatusRequestRequestTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetStageDeploymentRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "ImportGameConfigurationSourceTypeDef",
     "PaginatorConfigTypeDef",
     "ListExtensionVersionsRequestRequestTypeDef",
     "ListExtensionsRequestRequestTypeDef",
     "ListGamesRequestRequestTypeDef",
     "ListGeneratedCodeJobsRequestRequestTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "SnapshotSummaryTypeDef",
@@ -75,14 +75,15 @@
     "SectionModificationTypeDef",
     "StartStageDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGameRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
+    "ImportGameConfigurationSourceTypeDef",
     "CreateGameResultTypeDef",
     "DisconnectPlayerResultTypeDef",
     "ExportSnapshotResultTypeDef",
     "GetGameResultTypeDef",
     "GetPlayerConnectionStatusResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StartGeneratedCodeJobResultTypeDef",
@@ -98,36 +99,37 @@
     "ListExtensionVersionsResultTypeDef",
     "GameConfigurationDetailsTypeDef",
     "SnapshotDetailsTypeDef",
     "ListGamesResultTypeDef",
     "GetGeneratedCodeJobResultTypeDef",
     "ListGeneratedCodeJobsResultTypeDef",
     "StartGeneratedCodeJobRequestRequestTypeDef",
-    "ImportGameConfigurationRequestRequestTypeDef",
     "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
     "ListExtensionsRequestListExtensionsPaginateTypeDef",
     "ListGamesRequestListGamesPaginateTypeDef",
     "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
     "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
     "ListStagesRequestListStagesPaginateTypeDef",
     "ListSnapshotsResultTypeDef",
     "ListStagesResultTypeDef",
     "UpdateGameConfigurationRequestRequestTypeDef",
+    "ImportGameConfigurationRequestRequestTypeDef",
     "GetStageDeploymentResultTypeDef",
     "StartStageDeploymentResultTypeDef",
     "ListStageDeploymentsResultTypeDef",
     "GetGameConfigurationResultTypeDef",
     "ImportGameConfigurationResultTypeDef",
     "UpdateGameConfigurationResultTypeDef",
     "CreateSnapshotResultTypeDef",
     "GetSnapshotResultTypeDef",
     "UpdateSnapshotResultTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Created": datetime,
         "Id": str,
     },
     total=False,
@@ -451,21 +453,14 @@
     "GetStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
 
-ImportGameConfigurationSourceTypeDef = TypedDict(
-    "ImportGameConfigurationSourceTypeDef",
-    {
-        "File": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -741,14 +736,21 @@
 )
 
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
+ImportGameConfigurationSourceTypeDef = TypedDict(
+    "ImportGameConfigurationSourceTypeDef",
+    {
+        "File": BlobTypeDef,
+    },
+)
+
 CreateGameResultTypeDef = TypedDict(
     "CreateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -948,22 +950,14 @@
     {
         "GameName": str,
         "Generator": GeneratorTypeDef,
         "SnapshotId": str,
     },
 )
 
-ImportGameConfigurationRequestRequestTypeDef = TypedDict(
-    "ImportGameConfigurationRequestRequestTypeDef",
-    {
-        "GameName": str,
-        "ImportSource": ImportGameConfigurationSourceTypeDef,
-    },
-)
-
 _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
     "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
     {
         "Name": str,
         "Namespace": str,
     },
 )
@@ -1101,14 +1095,22 @@
     "UpdateGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
         "Modifications": Sequence[SectionModificationTypeDef],
     },
 )
 
+ImportGameConfigurationRequestRequestTypeDef = TypedDict(
+    "ImportGameConfigurationRequestRequestTypeDef",
+    {
+        "GameName": str,
+        "ImportSource": ImportGameConfigurationSourceTypeDef,
+    },
+)
+
 GetStageDeploymentResultTypeDef = TypedDict(
     "GetStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks.egg-info/PKG-INFO` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamesparks
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GameSparks 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GameSparks 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 gamesparks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 gamesparks type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamesparks)](https://pepy.tech/project/mypy-boto3-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameSparks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[boto3.GameSparks 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [mypy-boto3-gamesparks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/).
 
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
@@ -342,23 +342,24 @@
 )
 
 
 def check_value(value: DeploymentActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_gamesparks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_gamesparks.type_defs import (
+    BlobTypeDef,
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
     ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
@@ -378,15 +379,14 @@
     GetGameConfigurationRequestRequestTypeDef,
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    ImportGameConfigurationSourceTypeDef,
     PaginatorConfigTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListGamesRequestRequestTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
@@ -397,14 +397,15 @@
     SectionModificationTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
+    ImportGameConfigurationSourceTypeDef,
     CreateGameResultTypeDef,
     DisconnectPlayerResultTypeDef,
     ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
     GetPlayerConnectionStatusResultTypeDef,
     ListTagsForResourceResultTypeDef,
     StartGeneratedCodeJobResultTypeDef,
@@ -420,38 +421,38 @@
     ListExtensionVersionsResultTypeDef,
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
-    ImportGameConfigurationRequestRequestTypeDef,
     ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
     ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListGamesRequestListGamesPaginateTypeDef,
     ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
+    ImportGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
     ImportGameConfigurationResultTypeDef,
     UpdateGameConfigurationResultTypeDef,
     CreateSnapshotResultTypeDef,
     GetSnapshotResultTypeDef,
     UpdateSnapshotResultTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/mypy_boto3_gamesparks.egg-info/SOURCES.txt` & `mypy-boto3-gamesparks-1.28.16/mypy_boto3_gamesparks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.15.post1/setup.py` & `mypy-boto3-gamesparks-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-gamesparks",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_gamesparks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GameSparks 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.GameSparks 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 gamesparks type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 gamesparks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_gamesparks": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

