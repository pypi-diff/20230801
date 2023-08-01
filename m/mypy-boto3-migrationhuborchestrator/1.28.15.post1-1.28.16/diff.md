# Comparing `tmp/mypy-boto3-migrationhuborchestrator-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-migrationhuborchestrator-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:44 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.28.16.tar", last modified: Tue Aug  1 11:37:23 2023, max compression
```

## Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1.tar` & `mypy-boto3-migrationhuborchestrator-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.161300 mypy-boto3-migrationhuborchestrator-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-07-29 10:03:44.149299 mypy-boto3-migrationhuborchestrator-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.145300 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25333 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25291 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-07-29 09:51:45.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32504 2023-07-29 09:51:45.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.149299 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:44.161300 mypy-boto3-migrationhuborchestrator-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.980813 mypy-boto3-migrationhuborchestrator-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18166 2023-08-01 11:37:23.972813 mypy-boto3-migrationhuborchestrator-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.968813 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25180 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25138 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-08-01 11:24:42.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-08-01 11:24:42.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32630 2023-08-01 11:24:43.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32602 2023-08-01 11:24:42.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.972813 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18166 2023-08-01 11:37:23.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-01 11:37:23.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:23.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 11:37:23.000000 mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:23.980813 mypy-boto3-migrationhuborchestrator-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-01 11:24:41.000000 mypy-boto3-migrationhuborchestrator-1.28.16/setup.py
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/LICENSE` & `mypy-boto3-migrationhuborchestrator-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 migrationhuborchestrator type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 migrationhuborchestrator type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhuborchestrator)](https://pepy.tech/project/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
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
@@ -349,26 +349,25 @@
 )
 
 
 def check_value(value: DataTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
-    StepInputOutputTypeDef,
-    StepInputTypeDef,
     ResponseMetadataTypeDef,
+    StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
@@ -394,31 +393,30 @@
     WorkflowStepGroupSummaryTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
     PlatformCommandTypeDef,
     PlatformScriptKeyTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
+    StepInputTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
     WorkflowStepOutputUnionOutputTypeDef,
     WorkflowStepOutputUnionTypeDef,
-    CreateMigrationWorkflowRequestRequestTypeDef,
-    UpdateMigrationWorkflowRequestRequestTypeDef,
-    CreateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowResponseTypeDef,
-    UpdateMigrationWorkflowResponseTypeDef,
     UpdateWorkflowStepResponseTypeDef,
+    CreateMigrationWorkflowResponseTypeDef,
+    UpdateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
     ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
@@ -433,23 +431,27 @@
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     StepAutomationConfigurationTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
+    StepInputUnionTypeDef,
     WorkflowStepOutputTypeDef,
     GetTemplateStepResponseTypeDef,
-    CreateWorkflowStepRequestRequestTypeDef,
+    CreateMigrationWorkflowRequestRequestTypeDef,
+    UpdateMigrationWorkflowRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
+    WorkflowStepUnionTypeDef,
+    CreateWorkflowStepRequestRequestTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
 
 
-def get_structure() -> StepInputOutputTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/README.md` & `mypy-boto3-migrationhuborchestrator-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhuborchestrator)](https://pepy.tech/project/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
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
@@ -317,26 +317,25 @@
 )
 
 
 def check_value(value: DataTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
-    StepInputOutputTypeDef,
-    StepInputTypeDef,
     ResponseMetadataTypeDef,
+    StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
@@ -362,31 +361,30 @@
     WorkflowStepGroupSummaryTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
     PlatformCommandTypeDef,
     PlatformScriptKeyTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
+    StepInputTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
     WorkflowStepOutputUnionOutputTypeDef,
     WorkflowStepOutputUnionTypeDef,
-    CreateMigrationWorkflowRequestRequestTypeDef,
-    UpdateMigrationWorkflowRequestRequestTypeDef,
-    CreateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowResponseTypeDef,
-    UpdateMigrationWorkflowResponseTypeDef,
     UpdateWorkflowStepResponseTypeDef,
+    CreateMigrationWorkflowResponseTypeDef,
+    UpdateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
     ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
@@ -401,23 +399,27 @@
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     StepAutomationConfigurationTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
+    StepInputUnionTypeDef,
     WorkflowStepOutputTypeDef,
     GetTemplateStepResponseTypeDef,
-    CreateWorkflowStepRequestRequestTypeDef,
+    CreateMigrationWorkflowRequestRequestTypeDef,
+    UpdateMigrationWorkflowRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
+    WorkflowStepUnionTypeDef,
+    CreateWorkflowStepRequestRequestTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
 
 
-def get_structure() -> StepInputOutputTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__init__.py` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__init__.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__main__.py` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubOrchestrator 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MigrationHubOrchestrator 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator\nOther"
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/client.py` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migrationhuborchestrator.client import MigrationHubOrchestratorClient
 
     session = Session()
     client: MigrationHubOrchestratorClient = session.client("migrationhuborchestrator")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MigrationWorkflowStatusEnumType, StepActionTypeType, StepStatusType
 from .paginator import (
     ListPluginsPaginator,
     ListTemplatesPaginator,
@@ -45,22 +45,21 @@
     ListTagsForResourceResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
-    StepInputOutputTypeDef,
-    StepInputTypeDef,
+    StepInputUnionTypeDef,
     StopMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepResponseTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
-    WorkflowStepOutputTypeDef,
+    WorkflowStepUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -120,15 +119,15 @@
 
     def create_workflow(
         self,
         *,
         name: str,
         templateId: str,
         applicationConfigurationId: str,
-        inputParameters: Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
+        inputParameters: Mapping[str, StepInputUnionTypeDef],
         description: str = ...,
         stepTargets: Sequence[str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMigrationWorkflowResponseTypeDef:
         """
         Create a workflow to orchestrate your migrations.
 
@@ -142,15 +141,15 @@
         name: str,
         stepGroupId: str,
         workflowId: str,
         stepActionType: StepActionTypeType,
         description: str = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]] = ...,
+        outputs: Sequence[WorkflowStepUnionTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...
     ) -> CreateWorkflowStepResponseTypeDef:
         """
         Create a step in the migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step)
@@ -397,15 +396,15 @@
 
     def update_workflow(
         self,
         *,
         id: str,
         name: str = ...,
         description: str = ...,
-        inputParameters: Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]] = ...,
+        inputParameters: Mapping[str, StepInputUnionTypeDef] = ...,
         stepTargets: Sequence[str] = ...
     ) -> UpdateMigrationWorkflowResponseTypeDef:
         """
         Update a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/client/#update_workflow)
@@ -418,15 +417,15 @@
         stepGroupId: str,
         workflowId: str,
         name: str = ...,
         description: str = ...,
         stepActionType: StepActionTypeType = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]] = ...,
+        outputs: Sequence[WorkflowStepUnionTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...,
         status: StepStatusType = ...
     ) -> UpdateWorkflowStepResponseTypeDef:
         """
         Update a step in a migration workflow.
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/client.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migrationhuborchestrator.client import MigrationHubOrchestratorClient
 
     session = Session()
     client: MigrationHubOrchestratorClient = session.client("migrationhuborchestrator")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MigrationWorkflowStatusEnumType, StepActionTypeType, StepStatusType
 from .paginator import (
     ListPluginsPaginator,
     ListTemplatesPaginator,
@@ -45,22 +45,21 @@
     ListTagsForResourceResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
-    StepInputOutputTypeDef,
-    StepInputTypeDef,
+    StepInputUnionTypeDef,
     StopMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepResponseTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
-    WorkflowStepOutputTypeDef,
+    WorkflowStepUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -113,15 +112,15 @@
         """
     def create_workflow(
         self,
         *,
         name: str,
         templateId: str,
         applicationConfigurationId: str,
-        inputParameters: Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
+        inputParameters: Mapping[str, StepInputUnionTypeDef],
         description: str = ...,
         stepTargets: Sequence[str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMigrationWorkflowResponseTypeDef:
         """
         Create a workflow to orchestrate your migrations.
 
@@ -134,15 +133,15 @@
         name: str,
         stepGroupId: str,
         workflowId: str,
         stepActionType: StepActionTypeType,
         description: str = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]] = ...,
+        outputs: Sequence[WorkflowStepUnionTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...
     ) -> CreateWorkflowStepResponseTypeDef:
         """
         Create a step in the migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step)
@@ -364,15 +363,15 @@
         """
     def update_workflow(
         self,
         *,
         id: str,
         name: str = ...,
         description: str = ...,
-        inputParameters: Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]] = ...,
+        inputParameters: Mapping[str, StepInputUnionTypeDef] = ...,
         stepTargets: Sequence[str] = ...
     ) -> UpdateMigrationWorkflowResponseTypeDef:
         """
         Update a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/client/#update_workflow)
@@ -384,15 +383,15 @@
         stepGroupId: str,
         workflowId: str,
         name: str = ...,
         description: str = ...,
         stepActionType: StepActionTypeType = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]] = ...,
+        outputs: Sequence[WorkflowStepUnionTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...,
         status: StepStatusType = ...
     ) -> UpdateWorkflowStepResponseTypeDef:
         """
         Update a step in a migration workflow.
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/literals.py` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/literals.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/paginator.py` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/paginator.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/type_defs.py` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for migrationhuborchestrator service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_migrationhuborchestrator.type_defs import StepInputOutputTypeDef
+    from mypy_boto3_migrationhuborchestrator.type_defs import ResponseMetadataTypeDef
 
-    data: StepInputOutputTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -34,17 +34,16 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "StepInputOutputTypeDef",
-    "StepInputTypeDef",
     "ResponseMetadataTypeDef",
+    "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
@@ -70,31 +69,30 @@
     "WorkflowStepGroupSummaryTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
     "PlatformCommandTypeDef",
     "PlatformScriptKeyTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
+    "StepInputTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
     "WorkflowStepOutputUnionOutputTypeDef",
     "WorkflowStepOutputUnionTypeDef",
-    "CreateMigrationWorkflowRequestRequestTypeDef",
-    "UpdateMigrationWorkflowRequestRequestTypeDef",
-    "CreateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowResponseTypeDef",
-    "UpdateMigrationWorkflowResponseTypeDef",
     "UpdateWorkflowStepResponseTypeDef",
+    "CreateMigrationWorkflowResponseTypeDef",
+    "UpdateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
     "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
@@ -109,54 +107,47 @@
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
     "StepAutomationConfigurationTypeDef",
     "WorkflowStepAutomationConfigurationTypeDef",
+    "StepInputUnionTypeDef",
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
-    "CreateWorkflowStepRequestRequestTypeDef",
+    "CreateMigrationWorkflowRequestRequestTypeDef",
+    "UpdateMigrationWorkflowRequestRequestTypeDef",
     "GetWorkflowStepResponseTypeDef",
+    "WorkflowStepUnionTypeDef",
+    "CreateWorkflowStepRequestRequestTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
 
-StepInputOutputTypeDef = TypedDict(
-    "StepInputOutputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": List[str],
-        "mapOfStringValue": Dict[str, str],
-    },
-    total=False,
-)
-
-StepInputTypeDef = TypedDict(
-    "StepInputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": Sequence[str],
-        "mapOfStringValue": Mapping[str, str],
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
         "RetryAttempts": int,
     },
 )
 
+StepInputOutputTypeDef = TypedDict(
+    "StepInputOutputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": List[str],
+        "mapOfStringValue": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -551,14 +542,25 @@
 StartMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StartMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+StepInputTypeDef = TypedDict(
+    "StepInputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": Sequence[str],
+        "mapOfStringValue": Mapping[str, str],
+    },
+    total=False,
+)
+
 StopMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StopMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -620,84 +622,14 @@
         "integerValue": int,
         "stringValue": str,
         "listOfStringValue": Sequence[str],
     },
     total=False,
 )
 
-_RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "name": str,
-        "templateId": str,
-        "applicationConfigurationId": str,
-        "inputParameters": Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
-    },
-)
-_OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "description": str,
-        "stepTargets": Sequence[str],
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "inputParameters": Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
-        "stepTargets": Sequence[str],
-    },
-    total=False,
-)
-
-
-class UpdateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
-):
-    pass
-
-
-CreateMigrationWorkflowResponseTypeDef = TypedDict(
-    "CreateMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "templateId": str,
-        "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
-        "stepTargets": List[str],
-        "status": MigrationWorkflowStatusEnumType,
-        "creationTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateWorkflowStepResponseTypeDef = TypedDict(
     "CreateWorkflowStepResponseTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
         "name": str,
@@ -754,40 +686,58 @@
         "status": MigrationWorkflowStatusEnumType,
         "statusMessage": str,
         "lastStopTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateMigrationWorkflowResponseTypeDef = TypedDict(
-    "UpdateMigrationWorkflowResponseTypeDef",
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMigrationWorkflowResponseTypeDef = TypedDict(
+    "CreateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
-        "lastModifiedTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
+UpdateMigrationWorkflowResponseTypeDef = TypedDict(
+    "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
+        "arn": str,
         "name": str,
+        "description": str,
+        "templateId": str,
+        "adsApplicationConfigurationId": str,
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "stepTargets": List[str],
+        "status": MigrationWorkflowStatusEnumType,
+        "creationTime": datetime,
+        "lastModifiedTime": datetime,
+        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
@@ -1097,14 +1047,15 @@
         "command": PlatformCommandTypeDef,
         "runEnvironment": RunEnvironmentType,
         "targetType": TargetTypeType,
     },
     total=False,
 )
 
+StepInputUnionTypeDef = Union[StepInputTypeDef, StepInputOutputTypeDef]
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "required": bool,
         "value": WorkflowStepOutputUnionOutputTypeDef,
@@ -1126,40 +1077,62 @@
         "next": List[str],
         "outputs": List[StepOutputTypeDef],
         "stepAutomationConfiguration": StepAutomationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkflowStepRequestRequestTypeDef",
+_RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
     {
         "name": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "stepActionType": StepActionTypeType,
+        "templateId": str,
+        "applicationConfigurationId": str,
+        "inputParameters": Mapping[str, StepInputUnionTypeDef],
     },
 )
-_OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkflowStepRequestRequestTypeDef",
+_OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
     {
         "description": str,
-        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
-        "stepTarget": Sequence[str],
-        "outputs": Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]],
-        "previous": Sequence[str],
-        "next": Sequence[str],
+        "stepTargets": Sequence[str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class CreateWorkflowStepRequestRequestTypeDef(
-    _RequiredCreateWorkflowStepRequestRequestTypeDef,
-    _OptionalCreateWorkflowStepRequestRequestTypeDef,
+class CreateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "inputParameters": Mapping[str, StepInputUnionTypeDef],
+        "stepTargets": Sequence[str],
+    },
+    total=False,
+)
+
+
+class UpdateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
 
 GetWorkflowStepResponseTypeDef = TypedDict(
     "GetWorkflowStepResponseTypeDef",
     {
@@ -1184,14 +1157,45 @@
         "noOfSrvCompleted": int,
         "noOfSrvFailed": int,
         "totalNoOfSrv": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+WorkflowStepUnionTypeDef = Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]
+_RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkflowStepRequestRequestTypeDef",
+    {
+        "name": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "stepActionType": StepActionTypeType,
+    },
+)
+_OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkflowStepRequestRequestTypeDef",
+    {
+        "description": str,
+        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
+        "stepTarget": Sequence[str],
+        "outputs": Sequence[WorkflowStepUnionTypeDef],
+        "previous": Sequence[str],
+        "next": Sequence[str],
+    },
+    total=False,
+)
+
+
+class CreateWorkflowStepRequestRequestTypeDef(
+    _RequiredCreateWorkflowStepRequestRequestTypeDef,
+    _OptionalCreateWorkflowStepRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowStepRequestRequestTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
     },
@@ -1200,15 +1204,15 @@
     "_OptionalUpdateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": Sequence[str],
-        "outputs": Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]],
+        "outputs": Sequence[WorkflowStepUnionTypeDef],
         "previous": Sequence[str],
         "next": Sequence[str],
         "status": StepStatusType,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/type_defs.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for migrationhuborchestrator service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_migrationhuborchestrator.type_defs import StepInputOutputTypeDef
+    from mypy_boto3_migrationhuborchestrator.type_defs import ResponseMetadataTypeDef
 
-    data: StepInputOutputTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -33,17 +33,16 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "StepInputOutputTypeDef",
-    "StepInputTypeDef",
     "ResponseMetadataTypeDef",
+    "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
@@ -69,31 +68,30 @@
     "WorkflowStepGroupSummaryTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
     "PlatformCommandTypeDef",
     "PlatformScriptKeyTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
+    "StepInputTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
     "WorkflowStepOutputUnionOutputTypeDef",
     "WorkflowStepOutputUnionTypeDef",
-    "CreateMigrationWorkflowRequestRequestTypeDef",
-    "UpdateMigrationWorkflowRequestRequestTypeDef",
-    "CreateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowResponseTypeDef",
-    "UpdateMigrationWorkflowResponseTypeDef",
     "UpdateWorkflowStepResponseTypeDef",
+    "CreateMigrationWorkflowResponseTypeDef",
+    "UpdateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
     "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
@@ -108,54 +106,47 @@
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
     "StepAutomationConfigurationTypeDef",
     "WorkflowStepAutomationConfigurationTypeDef",
+    "StepInputUnionTypeDef",
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
-    "CreateWorkflowStepRequestRequestTypeDef",
+    "CreateMigrationWorkflowRequestRequestTypeDef",
+    "UpdateMigrationWorkflowRequestRequestTypeDef",
     "GetWorkflowStepResponseTypeDef",
+    "WorkflowStepUnionTypeDef",
+    "CreateWorkflowStepRequestRequestTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
 
-StepInputOutputTypeDef = TypedDict(
-    "StepInputOutputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": List[str],
-        "mapOfStringValue": Dict[str, str],
-    },
-    total=False,
-)
-
-StepInputTypeDef = TypedDict(
-    "StepInputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": Sequence[str],
-        "mapOfStringValue": Mapping[str, str],
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
         "RetryAttempts": int,
     },
 )
 
+StepInputOutputTypeDef = TypedDict(
+    "StepInputOutputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": List[str],
+        "mapOfStringValue": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -540,14 +531,25 @@
 StartMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StartMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+StepInputTypeDef = TypedDict(
+    "StepInputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": Sequence[str],
+        "mapOfStringValue": Mapping[str, str],
+    },
+    total=False,
+)
+
 StopMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StopMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -607,80 +609,14 @@
         "integerValue": int,
         "stringValue": str,
         "listOfStringValue": Sequence[str],
     },
     total=False,
 )
 
-_RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "name": str,
-        "templateId": str,
-        "applicationConfigurationId": str,
-        "inputParameters": Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
-    },
-)
-_OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "description": str,
-        "stepTargets": Sequence[str],
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "inputParameters": Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
-        "stepTargets": Sequence[str],
-    },
-    total=False,
-)
-
-class UpdateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
-):
-    pass
-
-CreateMigrationWorkflowResponseTypeDef = TypedDict(
-    "CreateMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "templateId": str,
-        "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
-        "stepTargets": List[str],
-        "status": MigrationWorkflowStatusEnumType,
-        "creationTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateWorkflowStepResponseTypeDef = TypedDict(
     "CreateWorkflowStepResponseTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
         "name": str,
@@ -737,40 +673,58 @@
         "status": MigrationWorkflowStatusEnumType,
         "statusMessage": str,
         "lastStopTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateMigrationWorkflowResponseTypeDef = TypedDict(
-    "UpdateMigrationWorkflowResponseTypeDef",
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMigrationWorkflowResponseTypeDef = TypedDict(
+    "CreateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
-        "lastModifiedTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
+UpdateMigrationWorkflowResponseTypeDef = TypedDict(
+    "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
+        "arn": str,
         "name": str,
+        "description": str,
+        "templateId": str,
+        "adsApplicationConfigurationId": str,
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "stepTargets": List[str],
+        "status": MigrationWorkflowStatusEnumType,
+        "creationTime": datetime,
+        "lastModifiedTime": datetime,
+        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
@@ -1072,14 +1026,15 @@
         "command": PlatformCommandTypeDef,
         "runEnvironment": RunEnvironmentType,
         "targetType": TargetTypeType,
     },
     total=False,
 )
 
+StepInputUnionTypeDef = Union[StepInputTypeDef, StepInputOutputTypeDef]
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "required": bool,
         "value": WorkflowStepOutputUnionOutputTypeDef,
@@ -1101,39 +1056,59 @@
         "next": List[str],
         "outputs": List[StepOutputTypeDef],
         "stepAutomationConfiguration": StepAutomationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkflowStepRequestRequestTypeDef",
+_RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
     {
         "name": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "stepActionType": StepActionTypeType,
+        "templateId": str,
+        "applicationConfigurationId": str,
+        "inputParameters": Mapping[str, StepInputUnionTypeDef],
     },
 )
-_OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkflowStepRequestRequestTypeDef",
+_OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
     {
         "description": str,
-        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
-        "stepTarget": Sequence[str],
-        "outputs": Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]],
-        "previous": Sequence[str],
-        "next": Sequence[str],
+        "stepTargets": Sequence[str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateWorkflowStepRequestRequestTypeDef(
-    _RequiredCreateWorkflowStepRequestRequestTypeDef,
-    _OptionalCreateWorkflowStepRequestRequestTypeDef,
+class CreateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "inputParameters": Mapping[str, StepInputUnionTypeDef],
+        "stepTargets": Sequence[str],
+    },
+    total=False,
+)
+
+class UpdateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
 GetWorkflowStepResponseTypeDef = TypedDict(
     "GetWorkflowStepResponseTypeDef",
     {
         "name": str,
@@ -1157,14 +1132,43 @@
         "noOfSrvCompleted": int,
         "noOfSrvFailed": int,
         "totalNoOfSrv": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+WorkflowStepUnionTypeDef = Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]
+_RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkflowStepRequestRequestTypeDef",
+    {
+        "name": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "stepActionType": StepActionTypeType,
+    },
+)
+_OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkflowStepRequestRequestTypeDef",
+    {
+        "description": str,
+        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
+        "stepTarget": Sequence[str],
+        "outputs": Sequence[WorkflowStepUnionTypeDef],
+        "previous": Sequence[str],
+        "next": Sequence[str],
+    },
+    total=False,
+)
+
+class CreateWorkflowStepRequestRequestTypeDef(
+    _RequiredCreateWorkflowStepRequestRequestTypeDef,
+    _OptionalCreateWorkflowStepRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowStepRequestRequestTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
     },
@@ -1173,15 +1177,15 @@
     "_OptionalUpdateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": Sequence[str],
-        "outputs": Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]],
+        "outputs": Sequence[WorkflowStepUnionTypeDef],
         "previous": Sequence[str],
         "next": Sequence[str],
         "status": StepStatusType,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 migrationhuborchestrator type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 migrationhuborchestrator type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhuborchestrator)](https://pepy.tech/project/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
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
@@ -349,26 +349,25 @@
 )
 
 
 def check_value(value: DataTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
-    StepInputOutputTypeDef,
-    StepInputTypeDef,
     ResponseMetadataTypeDef,
+    StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
@@ -394,31 +393,30 @@
     WorkflowStepGroupSummaryTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
     PlatformCommandTypeDef,
     PlatformScriptKeyTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
+    StepInputTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
     WorkflowStepOutputUnionOutputTypeDef,
     WorkflowStepOutputUnionTypeDef,
-    CreateMigrationWorkflowRequestRequestTypeDef,
-    UpdateMigrationWorkflowRequestRequestTypeDef,
-    CreateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowResponseTypeDef,
-    UpdateMigrationWorkflowResponseTypeDef,
     UpdateWorkflowStepResponseTypeDef,
+    CreateMigrationWorkflowResponseTypeDef,
+    UpdateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
     ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
@@ -433,23 +431,27 @@
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     StepAutomationConfigurationTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
+    StepInputUnionTypeDef,
     WorkflowStepOutputTypeDef,
     GetTemplateStepResponseTypeDef,
-    CreateWorkflowStepRequestRequestTypeDef,
+    CreateMigrationWorkflowRequestRequestTypeDef,
+    UpdateMigrationWorkflowRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
+    WorkflowStepUnionTypeDef,
+    CreateWorkflowStepRequestRequestTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
 
 
-def get_structure() -> StepInputOutputTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt` & `mypy-boto3-migrationhuborchestrator-1.28.16/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.post1/setup.py` & `mypy-boto3-migrationhuborchestrator-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhuborchestrator",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_migrationhuborchestrator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MigrationHubOrchestrator 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,17 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords=(
-        "boto3 migrationhuborchestrator type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="boto3 migrationhuborchestrator type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_migrationhuborchestrator": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/"
```

