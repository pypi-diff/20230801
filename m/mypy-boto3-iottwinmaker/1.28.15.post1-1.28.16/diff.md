# Comparing `tmp/mypy-boto3-iottwinmaker-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iottwinmaker-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iottwinmaker-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:23 2023, max compression
+gzip compressed data, was "mypy-boto3-iottwinmaker-1.28.16.tar", last modified: Tue Aug  1 11:37:03 2023, max compression
```

## Comparing `mypy-boto3-iottwinmaker-1.28.15.post1.tar` & `mypy-boto3-iottwinmaker-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.413197 mypy-boto3-iottwinmaker-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-07-29 10:03:23.413197 mypy-boto3-iottwinmaker-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.409197 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24868 2023-07-29 09:48:16.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24828 2023-07-29 09:48:16.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-29 09:48:16.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-07-29 09:48:16.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46211 2023-07-29 09:48:17.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46130 2023-07-29 09:48:17.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.413197 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:23.413197 mypy-boto3-iottwinmaker-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.452858 mypy-boto3-iottwinmaker-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-08-01 11:37:03.440858 mypy-boto3-iottwinmaker-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.436858 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24754 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24714 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46363 2023-08-01 11:21:02.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46282 2023-08-01 11:21:01.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:00.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.440858 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-08-01 11:37:03.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 11:37:03.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:03.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:03.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:03.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:37:03.000000 mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:03.452858 mypy-boto3-iottwinmaker-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:20:59.000000 mypy-boto3-iottwinmaker-1.28.16/setup.py
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/LICENSE` & `mypy-boto3-iottwinmaker-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/PKG-INFO` & `mypy-boto3-iottwinmaker-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTTwinMaker 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iottwinmaker type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iottwinmaker type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iottwinmaker)](https://pepy.tech/project/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
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
@@ -307,20 +307,20 @@
 )
 
 
 def check_value(value: ColumnTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iottwinmaker.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iottwinmaker.type_defs import (
     ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
@@ -345,14 +345,15 @@
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
+    TimestampTypeDef,
     GetSceneRequestRequestTypeDef,
     SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
@@ -361,15 +362,14 @@
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyValueOutputTypeDef,
-    PropertyValueTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
     CreateComponentTypeResponseTypeDef,
     CreateEntityResponseTypeDef,
@@ -395,57 +395,59 @@
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
     GetPropertyValueHistoryRequestRequestTypeDef,
+    PropertyValueTypeDef,
     GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
     PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
-    PropertyValueEntryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
     FunctionRequestTypeDef,
     FunctionResponseTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
+    PropertyValueEntryTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
-    BatchPutPropertyValuesRequestRequestTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
     GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
+    PropertyValueEntryUnionTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
+    BatchPutPropertyValuesRequestRequestTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/README.md` & `mypy-boto3-iottwinmaker-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iottwinmaker)](https://pepy.tech/project/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
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
@@ -275,20 +275,20 @@
 )
 
 
 def check_value(value: ColumnTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iottwinmaker.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iottwinmaker.type_defs import (
     ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
@@ -313,14 +313,15 @@
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
+    TimestampTypeDef,
     GetSceneRequestRequestTypeDef,
     SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
@@ -329,15 +330,14 @@
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyValueOutputTypeDef,
-    PropertyValueTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
     CreateComponentTypeResponseTypeDef,
     CreateEntityResponseTypeDef,
@@ -363,57 +363,59 @@
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
     GetPropertyValueHistoryRequestRequestTypeDef,
+    PropertyValueTypeDef,
     GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
     PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
-    PropertyValueEntryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
     FunctionRequestTypeDef,
     FunctionResponseTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
+    PropertyValueEntryTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
-    BatchPutPropertyValuesRequestRequestTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
     GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
+    PropertyValueEntryUnionTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
+    BatchPutPropertyValuesRequestRequestTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/__main__.py` & `mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTTwinMaker 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTTwinMaker 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker\nOther"
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

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/client.py` & `mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_iottwinmaker.client import IoTTwinMakerClient
 
     session = Session()
     client: IoTTwinMakerClient = session.client("iottwinmaker")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OrderByTimeType, PricingModeType
 from .type_defs import (
     BatchPutPropertyValuesResponseTypeDef,
     ComponentRequestTypeDef,
@@ -51,18 +50,18 @@
     ListSyncResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyFilterTypeDef,
     PropertyGroupRequestTypeDef,
-    PropertyValueEntryOutputTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryUnionTypeDef,
     SyncResourceFilterTypeDef,
     TabularConditionsTypeDef,
+    TimestampTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
 )
 
@@ -106,18 +105,15 @@
         IoTTwinMakerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#exceptions)
         """
 
     def batch_put_property_values(
-        self,
-        *,
-        workspaceId: str,
-        entries: Sequence[Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]]
+        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryUnionTypeDef]
     ) -> BatchPutPropertyValuesResponseTypeDef:
         """
         Sets values for multiple time series properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.batch_put_property_values)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#batch_put_property_values)
         """
@@ -341,16 +337,16 @@
         *,
         workspaceId: str,
         selectedProperties: Sequence[str],
         entityId: str = ...,
         componentName: str = ...,
         componentTypeId: str = ...,
         propertyFilters: Sequence[PropertyFilterTypeDef] = ...,
-        startDateTime: Union[datetime, str] = ...,
-        endDateTime: Union[datetime, str] = ...,
+        startDateTime: TimestampTypeDef = ...,
+        endDateTime: TimestampTypeDef = ...,
         interpolation: InterpolationParametersTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         orderByTime: OrderByTimeType = ...,
         startTime: str = ...,
         endTime: str = ...
     ) -> GetPropertyValueHistoryResponseTypeDef:
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/client.pyi` & `mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_iottwinmaker.client import IoTTwinMakerClient
 
     session = Session()
     client: IoTTwinMakerClient = session.client("iottwinmaker")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OrderByTimeType, PricingModeType
 from .type_defs import (
     BatchPutPropertyValuesResponseTypeDef,
     ComponentRequestTypeDef,
@@ -51,18 +50,18 @@
     ListSyncResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyFilterTypeDef,
     PropertyGroupRequestTypeDef,
-    PropertyValueEntryOutputTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryUnionTypeDef,
     SyncResourceFilterTypeDef,
     TabularConditionsTypeDef,
+    TimestampTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
 )
 
@@ -102,18 +101,15 @@
         """
         IoTTwinMakerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#exceptions)
         """
     def batch_put_property_values(
-        self,
-        *,
-        workspaceId: str,
-        entries: Sequence[Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]]
+        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryUnionTypeDef]
     ) -> BatchPutPropertyValuesResponseTypeDef:
         """
         Sets values for multiple time series properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.batch_put_property_values)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#batch_put_property_values)
         """
@@ -318,16 +314,16 @@
         *,
         workspaceId: str,
         selectedProperties: Sequence[str],
         entityId: str = ...,
         componentName: str = ...,
         componentTypeId: str = ...,
         propertyFilters: Sequence[PropertyFilterTypeDef] = ...,
-        startDateTime: Union[datetime, str] = ...,
-        endDateTime: Union[datetime, str] = ...,
+        startDateTime: TimestampTypeDef = ...,
+        endDateTime: TimestampTypeDef = ...,
         interpolation: InterpolationParametersTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         orderByTime: OrderByTimeType = ...,
         startTime: str = ...,
         endTime: str = ...
     ) -> GetPropertyValueHistoryResponseTypeDef:
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/literals.py` & `mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/literals.pyi` & `mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/type_defs.py` & `mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iottwinmaker.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -71,14 +71,15 @@
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
     "GetEntityRequestRequestTypeDef",
     "InterpolationParametersTypeDef",
     "PropertyFilterTypeDef",
+    "TimestampTypeDef",
     "GetSceneRequestRequestTypeDef",
     "SceneErrorTypeDef",
     "GetSyncJobRequestRequestTypeDef",
     "GetWorkspaceRequestRequestTypeDef",
     "ListComponentTypesFilterTypeDef",
     "ListEntitiesFilterTypeDef",
     "ListScenesRequestRequestTypeDef",
@@ -87,15 +88,14 @@
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
     "PropertyValueOutputTypeDef",
-    "PropertyValueTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "CreateComponentTypeResponseTypeDef",
     "CreateEntityResponseTypeDef",
@@ -121,52 +121,54 @@
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
     "GetPropertyValueHistoryRequestRequestTypeDef",
+    "PropertyValueTypeDef",
     "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
     "PropertyValueEntryOutputTypeDef",
     "PropertyValueHistoryTypeDef",
-    "PropertyValueEntryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
     "FunctionRequestTypeDef",
     "FunctionResponseTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
+    "PropertyValueEntryTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
     "BatchPutPropertyErrorTypeDef",
     "GetPropertyValueHistoryResponseTypeDef",
-    "BatchPutPropertyValuesRequestRequestTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
     "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
+    "PropertyValueEntryUnionTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
+    "BatchPutPropertyValuesRequestRequestTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -557,14 +559,15 @@
         "propertyName": str,
         "operator": str,
         "value": "DataValueTypeDef",
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 GetSceneRequestRequestTypeDef = TypedDict(
     "GetSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -816,34 +819,14 @@
 
 class PropertyValueOutputTypeDef(
     _RequiredPropertyValueOutputTypeDef, _OptionalPropertyValueOutputTypeDef
 ):
     pass
 
 
-_RequiredPropertyValueTypeDef = TypedDict(
-    "_RequiredPropertyValueTypeDef",
-    {
-        "value": "DataValueTypeDef",
-    },
-)
-_OptionalPropertyValueTypeDef = TypedDict(
-    "_OptionalPropertyValueTypeDef",
-    {
-        "timestamp": Union[datetime, str],
-        "time": str,
-    },
-    total=False,
-)
-
-
-class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
-    pass
-
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1251,16 +1234,16 @@
 _OptionalGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_OptionalGetPropertyValueHistoryRequestRequestTypeDef",
     {
         "entityId": str,
         "componentName": str,
         "componentTypeId": str,
         "propertyFilters": Sequence[PropertyFilterTypeDef],
-        "startDateTime": Union[datetime, str],
-        "endDateTime": Union[datetime, str],
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
         "interpolation": InterpolationParametersTypeDef,
         "nextToken": str,
         "maxResults": int,
         "orderByTime": OrderByTimeType,
         "startTime": str,
         "endTime": str,
     },
@@ -1271,14 +1254,34 @@
 class GetPropertyValueHistoryRequestRequestTypeDef(
     _RequiredGetPropertyValueHistoryRequestRequestTypeDef,
     _OptionalGetPropertyValueHistoryRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredPropertyValueTypeDef = TypedDict(
+    "_RequiredPropertyValueTypeDef",
+    {
+        "value": "DataValueTypeDef",
+    },
+)
+_OptionalPropertyValueTypeDef = TypedDict(
+    "_OptionalPropertyValueTypeDef",
+    {
+        "timestamp": TimestampTypeDef,
+        "time": str,
+    },
+    total=False,
+)
+
+
+class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
+    pass
+
+
 GetSceneResponseTypeDef = TypedDict(
     "GetSceneResponseTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
         "arn": str,
@@ -1429,35 +1432,14 @@
 
 class PropertyValueHistoryTypeDef(
     _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
 ):
     pass
 
 
-_RequiredPropertyValueEntryTypeDef = TypedDict(
-    "_RequiredPropertyValueEntryTypeDef",
-    {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
-    },
-)
-_OptionalPropertyValueEntryTypeDef = TypedDict(
-    "_OptionalPropertyValueEntryTypeDef",
-    {
-        "propertyValues": Sequence[PropertyValueTypeDef],
-    },
-    total=False,
-)
-
-
-class PropertyValueEntryTypeDef(
-    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
-):
-    pass
-
-
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1628,14 +1610,35 @@
         "properties": Dict[str, PropertyResponseTypeDef],
         "propertyGroups": Dict[str, ComponentPropertyGroupResponseTypeDef],
         "syncSource": str,
     },
     total=False,
 )
 
+_RequiredPropertyValueEntryTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryTypeDef",
+    {
+        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+    },
+)
+_OptionalPropertyValueEntryTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryTypeDef",
+    {
+        "propertyValues": Sequence[PropertyValueTypeDef],
+    },
+    total=False,
+)
+
+
+class PropertyValueEntryTypeDef(
+    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+):
+    pass
+
+
 _RequiredGetPropertyValueRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueRequestRequestTypeDef",
     {
         "selectedProperties": Sequence[str],
         "workspaceId": str,
     },
 )
@@ -1674,22 +1677,14 @@
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
-    "BatchPutPropertyValuesRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "entries": Sequence[Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]],
-    },
-)
-
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityName": str,
     },
 )
@@ -1872,21 +1867,30 @@
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PropertyValueEntryUnionTypeDef = Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]
 BatchPutPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutPropertyErrorEntryTypeDef",
     {
         "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
+BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
+    "BatchPutPropertyValuesRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "entries": Sequence[PropertyValueEntryUnionTypeDef],
+    },
+)
+
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/type_defs.pyi` & `mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iottwinmaker.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -70,14 +70,15 @@
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
     "GetEntityRequestRequestTypeDef",
     "InterpolationParametersTypeDef",
     "PropertyFilterTypeDef",
+    "TimestampTypeDef",
     "GetSceneRequestRequestTypeDef",
     "SceneErrorTypeDef",
     "GetSyncJobRequestRequestTypeDef",
     "GetWorkspaceRequestRequestTypeDef",
     "ListComponentTypesFilterTypeDef",
     "ListEntitiesFilterTypeDef",
     "ListScenesRequestRequestTypeDef",
@@ -86,15 +87,14 @@
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
     "PropertyValueOutputTypeDef",
-    "PropertyValueTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "CreateComponentTypeResponseTypeDef",
     "CreateEntityResponseTypeDef",
@@ -120,52 +120,54 @@
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
     "GetPropertyValueHistoryRequestRequestTypeDef",
+    "PropertyValueTypeDef",
     "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
     "PropertyValueEntryOutputTypeDef",
     "PropertyValueHistoryTypeDef",
-    "PropertyValueEntryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
     "FunctionRequestTypeDef",
     "FunctionResponseTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
+    "PropertyValueEntryTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
     "BatchPutPropertyErrorTypeDef",
     "GetPropertyValueHistoryResponseTypeDef",
-    "BatchPutPropertyValuesRequestRequestTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
     "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
+    "PropertyValueEntryUnionTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
+    "BatchPutPropertyValuesRequestRequestTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -538,14 +540,15 @@
         "propertyName": str,
         "operator": str,
         "value": "DataValueTypeDef",
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 GetSceneRequestRequestTypeDef = TypedDict(
     "GetSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -779,32 +782,14 @@
 )
 
 class PropertyValueOutputTypeDef(
     _RequiredPropertyValueOutputTypeDef, _OptionalPropertyValueOutputTypeDef
 ):
     pass
 
-_RequiredPropertyValueTypeDef = TypedDict(
-    "_RequiredPropertyValueTypeDef",
-    {
-        "value": "DataValueTypeDef",
-    },
-)
-_OptionalPropertyValueTypeDef = TypedDict(
-    "_OptionalPropertyValueTypeDef",
-    {
-        "timestamp": Union[datetime, str],
-        "time": str,
-    },
-    total=False,
-)
-
-class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
-    pass
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1198,16 +1183,16 @@
 _OptionalGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_OptionalGetPropertyValueHistoryRequestRequestTypeDef",
     {
         "entityId": str,
         "componentName": str,
         "componentTypeId": str,
         "propertyFilters": Sequence[PropertyFilterTypeDef],
-        "startDateTime": Union[datetime, str],
-        "endDateTime": Union[datetime, str],
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
         "interpolation": InterpolationParametersTypeDef,
         "nextToken": str,
         "maxResults": int,
         "orderByTime": OrderByTimeType,
         "startTime": str,
         "endTime": str,
     },
@@ -1216,14 +1201,32 @@
 
 class GetPropertyValueHistoryRequestRequestTypeDef(
     _RequiredGetPropertyValueHistoryRequestRequestTypeDef,
     _OptionalGetPropertyValueHistoryRequestRequestTypeDef,
 ):
     pass
 
+_RequiredPropertyValueTypeDef = TypedDict(
+    "_RequiredPropertyValueTypeDef",
+    {
+        "value": "DataValueTypeDef",
+    },
+)
+_OptionalPropertyValueTypeDef = TypedDict(
+    "_OptionalPropertyValueTypeDef",
+    {
+        "timestamp": TimestampTypeDef,
+        "time": str,
+    },
+    total=False,
+)
+
+class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
+    pass
+
 GetSceneResponseTypeDef = TypedDict(
     "GetSceneResponseTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
         "arn": str,
@@ -1364,33 +1367,14 @@
 )
 
 class PropertyValueHistoryTypeDef(
     _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
 ):
     pass
 
-_RequiredPropertyValueEntryTypeDef = TypedDict(
-    "_RequiredPropertyValueEntryTypeDef",
-    {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
-    },
-)
-_OptionalPropertyValueEntryTypeDef = TypedDict(
-    "_OptionalPropertyValueEntryTypeDef",
-    {
-        "propertyValues": Sequence[PropertyValueTypeDef],
-    },
-    total=False,
-)
-
-class PropertyValueEntryTypeDef(
-    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
-):
-    pass
-
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1557,14 +1541,33 @@
         "properties": Dict[str, PropertyResponseTypeDef],
         "propertyGroups": Dict[str, ComponentPropertyGroupResponseTypeDef],
         "syncSource": str,
     },
     total=False,
 )
 
+_RequiredPropertyValueEntryTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryTypeDef",
+    {
+        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+    },
+)
+_OptionalPropertyValueEntryTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryTypeDef",
+    {
+        "propertyValues": Sequence[PropertyValueTypeDef],
+    },
+    total=False,
+)
+
+class PropertyValueEntryTypeDef(
+    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+):
+    pass
+
 _RequiredGetPropertyValueRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueRequestRequestTypeDef",
     {
         "selectedProperties": Sequence[str],
         "workspaceId": str,
     },
 )
@@ -1601,22 +1604,14 @@
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
-    "BatchPutPropertyValuesRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "entries": Sequence[Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]],
-    },
-)
-
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityName": str,
     },
 )
@@ -1791,21 +1786,30 @@
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PropertyValueEntryUnionTypeDef = Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]
 BatchPutPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutPropertyErrorEntryTypeDef",
     {
         "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
+BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
+    "BatchPutPropertyValuesRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "entries": Sequence[PropertyValueEntryUnionTypeDef],
+    },
+)
+
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/PKG-INFO` & `mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTTwinMaker 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iottwinmaker type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iottwinmaker type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iottwinmaker)](https://pepy.tech/project/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
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
@@ -307,20 +307,20 @@
 )
 
 
 def check_value(value: ColumnTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iottwinmaker.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iottwinmaker.type_defs import (
     ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
@@ -345,14 +345,15 @@
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
+    TimestampTypeDef,
     GetSceneRequestRequestTypeDef,
     SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
@@ -361,15 +362,14 @@
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyValueOutputTypeDef,
-    PropertyValueTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
     CreateComponentTypeResponseTypeDef,
     CreateEntityResponseTypeDef,
@@ -395,57 +395,59 @@
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
     GetPropertyValueHistoryRequestRequestTypeDef,
+    PropertyValueTypeDef,
     GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
     PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
-    PropertyValueEntryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
     FunctionRequestTypeDef,
     FunctionResponseTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
+    PropertyValueEntryTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
-    BatchPutPropertyValuesRequestRequestTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
     GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
+    PropertyValueEntryUnionTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
+    BatchPutPropertyValuesRequestRequestTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt` & `mypy-boto3-iottwinmaker-1.28.16/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.15.post1/setup.py` & `mypy-boto3-iottwinmaker-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iottwinmaker",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.IoTTwinMaker 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 iottwinmaker type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iottwinmaker type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iottwinmaker": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

