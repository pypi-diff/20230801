# Comparing `tmp/mypy-boto3-codepipeline-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-codepipeline-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codepipeline-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:48 2023, max compression
+gzip compressed data, was "mypy-boto3-codepipeline-1.28.16.tar", last modified: Tue Aug  1 11:36:28 2023, max compression
```

## Comparing `mypy-boto3-codepipeline-1.28.15.post1.tar` & `mypy-boto3-codepipeline-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.181075 mypy-boto3-codepipeline-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-29 10:02:48.169075 mypy-boto3-codepipeline-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.157075 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32709 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-07-29 09:40:52.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-07-29 09:40:51.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51067 2023-07-29 09:40:53.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50996 2023-07-29 09:40:52.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:50.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.169075 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-29 10:02:47.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:02:47.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:47.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:47.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:47.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:02:47.000000 mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:48.181075 mypy-boto3-codepipeline-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:40:49.000000 mypy-boto3-codepipeline-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.900923 mypy-boto3-codepipeline-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-08-01 11:36:28.900923 mypy-boto3-codepipeline-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18178 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.888923 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32352 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32300 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51677 2023-08-01 11:13:25.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51606 2023-08-01 11:13:24.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:23.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.900923 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-08-01 11:36:28.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:36:28.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:28.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:28.000000 mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:28.900923 mypy-boto3-codepipeline-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:13:22.000000 mypy-boto3-codepipeline-1.28.16/setup.py
```

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/LICENSE` & `mypy-boto3-codepipeline-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/PKG-INFO` & `mypy-boto3-codepipeline-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodePipeline 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodePipeline 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codepipeline type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codepipeline type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
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
@@ -351,20 +351,20 @@
 )
 
 
 def check_value(value: ActionCategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codepipeline.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
     ResponseMetadataTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
@@ -374,15 +374,15 @@
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
     ActionRevisionOutputTypeDef,
-    ActionRevisionTypeDef,
+    TimestampTypeDef,
     ActionTypeArtifactDetailsTypeDef,
     ActionTypeIdentifierTypeDef,
     ActionTypePermissionsOutputTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
     ActionTypePermissionsTypeDef,
     ActionTypeSettingsTypeDef,
@@ -390,15 +390,14 @@
     ApprovalResultTypeDef,
     S3LocationTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
     EncryptionKeyTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
-    CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
@@ -444,26 +443,25 @@
     StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
     ActionDeclarationOutputTypeDef,
     ActionDeclarationTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
-    PutActionRevisionInputRequestTypeDef,
+    ActionRevisionTypeDef,
+    CurrentRevisionTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
-    PutJobSuccessResultInputRequestTypeDef,
-    PutThirdPartyJobSuccessResultInputRequestTypeDef,
     ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
     ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionTypesInputListActionTypesPaginateTypeDef,
     ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
@@ -475,54 +473,61 @@
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
     StageDeclarationOutputTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
+    ActionRevisionUnionTypeDef,
+    PutActionRevisionInputRequestTypeDef,
+    PutJobSuccessResultInputRequestTypeDef,
+    PutThirdPartyJobSuccessResultInputRequestTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ActionExecutionInputTypeDef,
     ActionExecutionOutputTypeDef,
     ArtifactTypeDef,
     GetPipelineExecutionOutputTypeDef,
     ActionTypeExecutorOutputTypeDef,
     ActionTypeExecutorTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListWebhookItemTypeDef,
     PutWebhookInputRequestTypeDef,
+    WebhookDefinitionUnionTypeDef,
     PipelineDeclarationOutputTypeDef,
     PipelineDeclarationTypeDef,
     StageStateTypeDef,
     ActionExecutionDetailTypeDef,
     JobDataTypeDef,
     ThirdPartyJobDataTypeDef,
     ActionTypeDeclarationOutputTypeDef,
     ActionTypeDeclarationTypeDef,
     ListWebhooksOutputTypeDef,
     PutWebhookOutputTypeDef,
     CreatePipelineOutputTypeDef,
     GetPipelineOutputTypeDef,
     UpdatePipelineOutputTypeDef,
     CreatePipelineInputRequestTypeDef,
+    PipelineDeclarationUnionTypeDef,
     UpdatePipelineInputRequestTypeDef,
     GetPipelineStateOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     JobDetailsTypeDef,
     JobTypeDef,
     ThirdPartyJobDetailsTypeDef,
     GetActionTypeOutputTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     UpdateActionTypeInputRequestTypeDef,
     GetJobDetailsOutputTypeDef,
     PollForJobsOutputTypeDef,
     GetThirdPartyJobDetailsOutputTypeDef,
 )
 
 
-def get_structure() -> AWSSessionCredentialsTypeDef:
+def get_value() -> AWSSessionCredentialsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/README.md` & `mypy-boto3-codepipeline-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
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
@@ -319,20 +319,20 @@
 )
 
 
 def check_value(value: ActionCategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codepipeline.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
     ResponseMetadataTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
@@ -342,15 +342,15 @@
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
     ActionRevisionOutputTypeDef,
-    ActionRevisionTypeDef,
+    TimestampTypeDef,
     ActionTypeArtifactDetailsTypeDef,
     ActionTypeIdentifierTypeDef,
     ActionTypePermissionsOutputTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
     ActionTypePermissionsTypeDef,
     ActionTypeSettingsTypeDef,
@@ -358,15 +358,14 @@
     ApprovalResultTypeDef,
     S3LocationTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
     EncryptionKeyTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
-    CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
@@ -412,26 +411,25 @@
     StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
     ActionDeclarationOutputTypeDef,
     ActionDeclarationTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
-    PutActionRevisionInputRequestTypeDef,
+    ActionRevisionTypeDef,
+    CurrentRevisionTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
-    PutJobSuccessResultInputRequestTypeDef,
-    PutThirdPartyJobSuccessResultInputRequestTypeDef,
     ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
     ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionTypesInputListActionTypesPaginateTypeDef,
     ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
@@ -443,54 +441,61 @@
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
     StageDeclarationOutputTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
+    ActionRevisionUnionTypeDef,
+    PutActionRevisionInputRequestTypeDef,
+    PutJobSuccessResultInputRequestTypeDef,
+    PutThirdPartyJobSuccessResultInputRequestTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ActionExecutionInputTypeDef,
     ActionExecutionOutputTypeDef,
     ArtifactTypeDef,
     GetPipelineExecutionOutputTypeDef,
     ActionTypeExecutorOutputTypeDef,
     ActionTypeExecutorTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListWebhookItemTypeDef,
     PutWebhookInputRequestTypeDef,
+    WebhookDefinitionUnionTypeDef,
     PipelineDeclarationOutputTypeDef,
     PipelineDeclarationTypeDef,
     StageStateTypeDef,
     ActionExecutionDetailTypeDef,
     JobDataTypeDef,
     ThirdPartyJobDataTypeDef,
     ActionTypeDeclarationOutputTypeDef,
     ActionTypeDeclarationTypeDef,
     ListWebhooksOutputTypeDef,
     PutWebhookOutputTypeDef,
     CreatePipelineOutputTypeDef,
     GetPipelineOutputTypeDef,
     UpdatePipelineOutputTypeDef,
     CreatePipelineInputRequestTypeDef,
+    PipelineDeclarationUnionTypeDef,
     UpdatePipelineInputRequestTypeDef,
     GetPipelineStateOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     JobDetailsTypeDef,
     JobTypeDef,
     ThirdPartyJobDetailsTypeDef,
     GetActionTypeOutputTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     UpdateActionTypeInputRequestTypeDef,
     GetJobDetailsOutputTypeDef,
     PollForJobsOutputTypeDef,
     GetThirdPartyJobDetailsOutputTypeDef,
 )
 
 
-def get_structure() -> AWSSessionCredentialsTypeDef:
+def get_value() -> AWSSessionCredentialsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/__init__.py` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/__init__.pyi` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/__main__.py` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodePipeline 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CodePipeline 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline\nOther"
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

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/client.py` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_codepipeline.client import CodePipelineClient
 
     session = Session()
     client: CodePipelineClient = session.client("codepipeline")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ActionCategoryType, ActionOwnerType, StageTransitionTypeType
 from .paginator import (
     ListActionExecutionsPaginator,
     ListActionTypesPaginator,
@@ -28,18 +28,16 @@
     ListWebhooksPaginator,
 )
 from .type_defs import (
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionExecutionFilterTypeDef,
-    ActionRevisionOutputTypeDef,
-    ActionRevisionTypeDef,
-    ActionTypeDeclarationOutputTypeDef,
-    ActionTypeDeclarationTypeDef,
+    ActionRevisionUnionTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     ActionTypeIdTypeDef,
     ActionTypeSettingsTypeDef,
     ApprovalResultTypeDef,
     ArtifactDetailsTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     CreatePipelineOutputTypeDef,
     CurrentRevisionTypeDef,
@@ -54,28 +52,26 @@
     GetThirdPartyJobDetailsOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
-    PipelineDeclarationOutputTypeDef,
-    PipelineDeclarationTypeDef,
+    PipelineDeclarationUnionTypeDef,
     PollForJobsOutputTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     PutActionRevisionOutputTypeDef,
     PutApprovalResultOutputTypeDef,
     PutWebhookOutputTypeDef,
     RetryStageExecutionOutputTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionOutputTypeDef,
     TagTypeDef,
     UpdatePipelineOutputTypeDef,
-    WebhookDefinitionOutputTypeDef,
-    WebhookDefinitionTypeDef,
+    WebhookDefinitionUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -201,18 +197,15 @@
         the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_custom_action_type)
         """
 
     def create_pipeline(
-        self,
-        *,
-        pipeline: Union[PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef],
-        tags: Sequence[TagTypeDef] = ...
+        self, *, pipeline: PipelineDeclarationUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_pipeline)
         """
@@ -446,15 +439,15 @@
 
     def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
+        actionRevision: ActionRevisionUnionTypeDef
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_action_revision)
         """
@@ -526,18 +519,15 @@
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_third_party_job_success_result)
         """
 
     def put_webhook(
-        self,
-        *,
-        webhook: Union[WebhookDefinitionTypeDef, WebhookDefinitionOutputTypeDef],
-        tags: Sequence[TagTypeDef] = ...
+        self, *, webhook: WebhookDefinitionUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> PutWebhookOutputTypeDef:
         """
         Defines a webhook and returns a unique webhook URL generated by CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_webhook)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_webhook)
         """
@@ -599,26 +589,26 @@
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#untag_resource)
         """
 
     def update_action_type(
-        self, *, actionType: Union[ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef]
+        self, *, actionType: ActionTypeDeclarationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an action type that was created with any supported integration model,
         where the action type is to be used by customers of the action type provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#update_action_type)
         """
 
     def update_pipeline(
-        self, *, pipeline: Union[PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef]
+        self, *, pipeline: PipelineDeclarationUnionTypeDef
     ) -> UpdatePipelineOutputTypeDef:
         """
         Updates a specified pipeline with edits or changes to its structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#update_pipeline)
         """
```

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/client.pyi` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_codepipeline.client import CodePipelineClient
 
     session = Session()
     client: CodePipelineClient = session.client("codepipeline")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ActionCategoryType, ActionOwnerType, StageTransitionTypeType
 from .paginator import (
     ListActionExecutionsPaginator,
     ListActionTypesPaginator,
@@ -28,18 +28,16 @@
     ListWebhooksPaginator,
 )
 from .type_defs import (
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionExecutionFilterTypeDef,
-    ActionRevisionOutputTypeDef,
-    ActionRevisionTypeDef,
-    ActionTypeDeclarationOutputTypeDef,
-    ActionTypeDeclarationTypeDef,
+    ActionRevisionUnionTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     ActionTypeIdTypeDef,
     ActionTypeSettingsTypeDef,
     ApprovalResultTypeDef,
     ArtifactDetailsTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     CreatePipelineOutputTypeDef,
     CurrentRevisionTypeDef,
@@ -54,28 +52,26 @@
     GetThirdPartyJobDetailsOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
-    PipelineDeclarationOutputTypeDef,
-    PipelineDeclarationTypeDef,
+    PipelineDeclarationUnionTypeDef,
     PollForJobsOutputTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     PutActionRevisionOutputTypeDef,
     PutApprovalResultOutputTypeDef,
     PutWebhookOutputTypeDef,
     RetryStageExecutionOutputTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionOutputTypeDef,
     TagTypeDef,
     UpdatePipelineOutputTypeDef,
-    WebhookDefinitionOutputTypeDef,
-    WebhookDefinitionTypeDef,
+    WebhookDefinitionUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -191,18 +187,15 @@
         Creates a new custom action that can be used in all pipelines associated with
         the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_custom_action_type)
         """
     def create_pipeline(
-        self,
-        *,
-        pipeline: Union[PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef],
-        tags: Sequence[TagTypeDef] = ...
+        self, *, pipeline: PipelineDeclarationUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_pipeline)
         """
@@ -414,15 +407,15 @@
         """
     def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
+        actionRevision: ActionRevisionUnionTypeDef
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_action_revision)
         """
@@ -488,18 +481,15 @@
         Represents the success of a third party job as returned to the pipeline by a job
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_third_party_job_success_result)
         """
     def put_webhook(
-        self,
-        *,
-        webhook: Union[WebhookDefinitionTypeDef, WebhookDefinitionOutputTypeDef],
-        tags: Sequence[TagTypeDef] = ...
+        self, *, webhook: WebhookDefinitionUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> PutWebhookOutputTypeDef:
         """
         Defines a webhook and returns a unique webhook URL generated by CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_webhook)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_webhook)
         """
@@ -554,25 +544,25 @@
         """
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#untag_resource)
         """
     def update_action_type(
-        self, *, actionType: Union[ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef]
+        self, *, actionType: ActionTypeDeclarationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an action type that was created with any supported integration model,
         where the action type is to be used by customers of the action type provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#update_action_type)
         """
     def update_pipeline(
-        self, *, pipeline: Union[PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef]
+        self, *, pipeline: PipelineDeclarationUnionTypeDef
     ) -> UpdatePipelineOutputTypeDef:
         """
         Updates a specified pipeline with edits or changes to its structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#update_pipeline)
         """
```

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/literals.py` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/literals.pyi` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/paginator.py` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/paginator.pyi` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/type_defs.py` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codepipeline.type_defs import AWSSessionCredentialsTypeDef
 
-    data: AWSSessionCredentialsTypeDef = {...}
+    data: AWSSessionCredentialsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,15 +52,15 @@
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
     "ActionRevisionOutputTypeDef",
-    "ActionRevisionTypeDef",
+    "TimestampTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
     "ActionTypeIdentifierTypeDef",
     "ActionTypePermissionsOutputTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
     "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
@@ -68,15 +68,14 @@
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
     "EncryptionKeyTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
-    "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
@@ -122,26 +121,25 @@
     "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
     "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
-    "PutActionRevisionInputRequestTypeDef",
+    "ActionRevisionTypeDef",
+    "CurrentRevisionTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "PutJobSuccessResultInputRequestTypeDef",
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionTypesInputListActionTypesPaginateTypeDef",
     "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
@@ -153,46 +151,53 @@
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
     "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
     "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
+    "ActionRevisionUnionTypeDef",
+    "PutActionRevisionInputRequestTypeDef",
+    "PutJobSuccessResultInputRequestTypeDef",
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
     "GetPipelineExecutionOutputTypeDef",
     "ActionTypeExecutorOutputTypeDef",
     "ActionTypeExecutorTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
+    "WebhookDefinitionUnionTypeDef",
     "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
     "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
     "UpdatePipelineOutputTypeDef",
     "CreatePipelineInputRequestTypeDef",
+    "PipelineDeclarationUnionTypeDef",
     "UpdatePipelineInputRequestTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
+    "ActionTypeDeclarationUnionTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
     "GetJobDetailsOutputTypeDef",
     "PollForJobsOutputTypeDef",
     "GetThirdPartyJobDetailsOutputTypeDef",
 )
 
 AWSSessionCredentialsTypeDef = TypedDict(
@@ -331,23 +336,15 @@
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": datetime,
     },
 )
 
-ActionRevisionTypeDef = TypedDict(
-    "ActionRevisionTypeDef",
-    {
-        "revisionId": str,
-        "revisionChangeId": str,
-        "created": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
@@ -489,35 +486,14 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-_RequiredCurrentRevisionTypeDef = TypedDict(
-    "_RequiredCurrentRevisionTypeDef",
-    {
-        "revision": str,
-        "changeIdentifier": str,
-    },
-)
-_OptionalCurrentRevisionTypeDef = TypedDict(
-    "_OptionalCurrentRevisionTypeDef",
-    {
-        "created": Union[datetime, str],
-        "revisionSummary": str,
-    },
-    total=False,
-)
-
-
-class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
-    pass
-
-
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -1162,23 +1138,43 @@
         "externalExecutionUrl": str,
         "percentComplete": int,
         "errorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-PutActionRevisionInputRequestTypeDef = TypedDict(
-    "PutActionRevisionInputRequestTypeDef",
+ActionRevisionTypeDef = TypedDict(
+    "ActionRevisionTypeDef",
     {
-        "pipelineName": str,
-        "stageName": str,
-        "actionName": str,
-        "actionRevision": ActionRevisionTypeDef,
+        "revisionId": str,
+        "revisionChangeId": str,
+        "created": TimestampTypeDef,
+    },
+)
+
+_RequiredCurrentRevisionTypeDef = TypedDict(
+    "_RequiredCurrentRevisionTypeDef",
+    {
+        "revision": str,
+        "changeIdentifier": str,
     },
 )
+_OptionalCurrentRevisionTypeDef = TypedDict(
+    "_OptionalCurrentRevisionTypeDef",
+    {
+        "created": TimestampTypeDef,
+        "revisionSummary": str,
+    },
+    total=False,
+)
+
+
+class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
+    pass
+
 
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
         "id": ActionTypeIdTypeDef,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
         "outputArtifactDetails": ArtifactDetailsTypeDef,
@@ -1301,63 +1297,14 @@
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-    },
-)
-_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutJobSuccessResultInputRequestTypeDef",
-    {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-        "outputVariables": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class PutJobSuccessResultInputRequestTypeDef(
-    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
-):
-    pass
-
-
-_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-        "clientToken": str,
-    },
-)
-_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
-    {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-    },
-    total=False,
-)
-
-
-class PutThirdPartyJobSuccessResultInputRequestTypeDef(
-    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
-    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
-):
-    pass
-
-
 ExecutorConfigurationOutputTypeDef = TypedDict(
     "ExecutorConfigurationOutputTypeDef",
     {
         "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
     },
     total=False,
@@ -1599,14 +1546,74 @@
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
+ActionRevisionUnionTypeDef = Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
+PutActionRevisionInputRequestTypeDef = TypedDict(
+    "PutActionRevisionInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "stageName": str,
+        "actionName": str,
+        "actionRevision": ActionRevisionTypeDef,
+    },
+)
+
+_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+    },
+)
+_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+        "outputVariables": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class PutJobSuccessResultInputRequestTypeDef(
+    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
+):
+    pass
+
+
+_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+        "clientToken": str,
+    },
+)
+_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+    },
+    total=False,
+)
+
+
+class PutThirdPartyJobSuccessResultInputRequestTypeDef(
+    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
+    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
+):
+    pass
+
+
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1759,14 +1766,15 @@
 
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
 
+WebhookDefinitionUnionTypeDef = Union[WebhookDefinitionTypeDef, WebhookDefinitionOutputTypeDef]
 _RequiredPipelineDeclarationOutputTypeDef = TypedDict(
     "_RequiredPipelineDeclarationOutputTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": List[StageDeclarationOutputTypeDef],
     },
@@ -1986,14 +1994,17 @@
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
 
+PipelineDeclarationUnionTypeDef = Union[
+    PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef
+]
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
@@ -2053,14 +2064,17 @@
     "GetActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeDeclarationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActionTypeDeclarationUnionTypeDef = Union[
+    ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef
+]
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline/type_defs.pyi` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codepipeline.type_defs import AWSSessionCredentialsTypeDef
 
-    data: AWSSessionCredentialsTypeDef = {...}
+    data: AWSSessionCredentialsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -51,15 +51,15 @@
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
     "ActionRevisionOutputTypeDef",
-    "ActionRevisionTypeDef",
+    "TimestampTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
     "ActionTypeIdentifierTypeDef",
     "ActionTypePermissionsOutputTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
     "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
@@ -67,15 +67,14 @@
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
     "EncryptionKeyTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
-    "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
@@ -121,26 +120,25 @@
     "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
     "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
-    "PutActionRevisionInputRequestTypeDef",
+    "ActionRevisionTypeDef",
+    "CurrentRevisionTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "PutJobSuccessResultInputRequestTypeDef",
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionTypesInputListActionTypesPaginateTypeDef",
     "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
@@ -152,46 +150,53 @@
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
     "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
     "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
+    "ActionRevisionUnionTypeDef",
+    "PutActionRevisionInputRequestTypeDef",
+    "PutJobSuccessResultInputRequestTypeDef",
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
     "GetPipelineExecutionOutputTypeDef",
     "ActionTypeExecutorOutputTypeDef",
     "ActionTypeExecutorTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
+    "WebhookDefinitionUnionTypeDef",
     "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
     "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
     "UpdatePipelineOutputTypeDef",
     "CreatePipelineInputRequestTypeDef",
+    "PipelineDeclarationUnionTypeDef",
     "UpdatePipelineInputRequestTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
+    "ActionTypeDeclarationUnionTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
     "GetJobDetailsOutputTypeDef",
     "PollForJobsOutputTypeDef",
     "GetThirdPartyJobDetailsOutputTypeDef",
 )
 
 AWSSessionCredentialsTypeDef = TypedDict(
@@ -328,23 +333,15 @@
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": datetime,
     },
 )
 
-ActionRevisionTypeDef = TypedDict(
-    "ActionRevisionTypeDef",
-    {
-        "revisionId": str,
-        "revisionChangeId": str,
-        "created": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
@@ -484,33 +481,14 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-_RequiredCurrentRevisionTypeDef = TypedDict(
-    "_RequiredCurrentRevisionTypeDef",
-    {
-        "revision": str,
-        "changeIdentifier": str,
-    },
-)
-_OptionalCurrentRevisionTypeDef = TypedDict(
-    "_OptionalCurrentRevisionTypeDef",
-    {
-        "created": Union[datetime, str],
-        "revisionSummary": str,
-    },
-    total=False,
-)
-
-class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
-    pass
-
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -1129,24 +1107,42 @@
         "externalExecutionUrl": str,
         "percentComplete": int,
         "errorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-PutActionRevisionInputRequestTypeDef = TypedDict(
-    "PutActionRevisionInputRequestTypeDef",
+ActionRevisionTypeDef = TypedDict(
+    "ActionRevisionTypeDef",
     {
-        "pipelineName": str,
-        "stageName": str,
-        "actionName": str,
-        "actionRevision": ActionRevisionTypeDef,
+        "revisionId": str,
+        "revisionChangeId": str,
+        "created": TimestampTypeDef,
     },
 )
 
+_RequiredCurrentRevisionTypeDef = TypedDict(
+    "_RequiredCurrentRevisionTypeDef",
+    {
+        "revision": str,
+        "changeIdentifier": str,
+    },
+)
+_OptionalCurrentRevisionTypeDef = TypedDict(
+    "_OptionalCurrentRevisionTypeDef",
+    {
+        "created": TimestampTypeDef,
+        "revisionSummary": str,
+    },
+    total=False,
+)
+
+class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
+    pass
+
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
         "id": ActionTypeIdTypeDef,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
         "outputArtifactDetails": ArtifactDetailsTypeDef,
     },
@@ -1262,59 +1258,14 @@
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-    },
-)
-_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutJobSuccessResultInputRequestTypeDef",
-    {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-        "outputVariables": Mapping[str, str],
-    },
-    total=False,
-)
-
-class PutJobSuccessResultInputRequestTypeDef(
-    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
-):
-    pass
-
-_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-        "clientToken": str,
-    },
-)
-_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
-    {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-    },
-    total=False,
-)
-
-class PutThirdPartyJobSuccessResultInputRequestTypeDef(
-    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
-    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
-):
-    pass
-
 ExecutorConfigurationOutputTypeDef = TypedDict(
     "ExecutorConfigurationOutputTypeDef",
     {
         "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
     },
     total=False,
@@ -1546,14 +1497,70 @@
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
+ActionRevisionUnionTypeDef = Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
+PutActionRevisionInputRequestTypeDef = TypedDict(
+    "PutActionRevisionInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "stageName": str,
+        "actionName": str,
+        "actionRevision": ActionRevisionTypeDef,
+    },
+)
+
+_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+    },
+)
+_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+        "outputVariables": Mapping[str, str],
+    },
+    total=False,
+)
+
+class PutJobSuccessResultInputRequestTypeDef(
+    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
+):
+    pass
+
+_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+        "clientToken": str,
+    },
+)
+_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+    },
+    total=False,
+)
+
+class PutThirdPartyJobSuccessResultInputRequestTypeDef(
+    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
+    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
+):
+    pass
+
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1698,14 +1705,15 @@
 )
 
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
+WebhookDefinitionUnionTypeDef = Union[WebhookDefinitionTypeDef, WebhookDefinitionOutputTypeDef]
 _RequiredPipelineDeclarationOutputTypeDef = TypedDict(
     "_RequiredPipelineDeclarationOutputTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": List[StageDeclarationOutputTypeDef],
     },
@@ -1915,14 +1923,17 @@
 )
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
+PipelineDeclarationUnionTypeDef = Union[
+    PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef
+]
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
@@ -1982,14 +1993,17 @@
     "GetActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeDeclarationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActionTypeDeclarationUnionTypeDef = Union[
+    ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef
+]
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline.egg-info/PKG-INFO` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodePipeline 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodePipeline 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codepipeline type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codepipeline type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
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
@@ -351,20 +351,20 @@
 )
 
 
 def check_value(value: ActionCategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codepipeline.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
     ResponseMetadataTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
@@ -374,15 +374,15 @@
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
     ActionRevisionOutputTypeDef,
-    ActionRevisionTypeDef,
+    TimestampTypeDef,
     ActionTypeArtifactDetailsTypeDef,
     ActionTypeIdentifierTypeDef,
     ActionTypePermissionsOutputTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
     ActionTypePermissionsTypeDef,
     ActionTypeSettingsTypeDef,
@@ -390,15 +390,14 @@
     ApprovalResultTypeDef,
     S3LocationTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
     EncryptionKeyTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
-    CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
@@ -444,26 +443,25 @@
     StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
     ActionDeclarationOutputTypeDef,
     ActionDeclarationTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
-    PutActionRevisionInputRequestTypeDef,
+    ActionRevisionTypeDef,
+    CurrentRevisionTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
-    PutJobSuccessResultInputRequestTypeDef,
-    PutThirdPartyJobSuccessResultInputRequestTypeDef,
     ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
     ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionTypesInputListActionTypesPaginateTypeDef,
     ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
@@ -475,54 +473,61 @@
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
     StageDeclarationOutputTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
+    ActionRevisionUnionTypeDef,
+    PutActionRevisionInputRequestTypeDef,
+    PutJobSuccessResultInputRequestTypeDef,
+    PutThirdPartyJobSuccessResultInputRequestTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ActionExecutionInputTypeDef,
     ActionExecutionOutputTypeDef,
     ArtifactTypeDef,
     GetPipelineExecutionOutputTypeDef,
     ActionTypeExecutorOutputTypeDef,
     ActionTypeExecutorTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListWebhookItemTypeDef,
     PutWebhookInputRequestTypeDef,
+    WebhookDefinitionUnionTypeDef,
     PipelineDeclarationOutputTypeDef,
     PipelineDeclarationTypeDef,
     StageStateTypeDef,
     ActionExecutionDetailTypeDef,
     JobDataTypeDef,
     ThirdPartyJobDataTypeDef,
     ActionTypeDeclarationOutputTypeDef,
     ActionTypeDeclarationTypeDef,
     ListWebhooksOutputTypeDef,
     PutWebhookOutputTypeDef,
     CreatePipelineOutputTypeDef,
     GetPipelineOutputTypeDef,
     UpdatePipelineOutputTypeDef,
     CreatePipelineInputRequestTypeDef,
+    PipelineDeclarationUnionTypeDef,
     UpdatePipelineInputRequestTypeDef,
     GetPipelineStateOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     JobDetailsTypeDef,
     JobTypeDef,
     ThirdPartyJobDetailsTypeDef,
     GetActionTypeOutputTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     UpdateActionTypeInputRequestTypeDef,
     GetJobDetailsOutputTypeDef,
     PollForJobsOutputTypeDef,
     GetThirdPartyJobDetailsOutputTypeDef,
 )
 
 
-def get_structure() -> AWSSessionCredentialsTypeDef:
+def get_value() -> AWSSessionCredentialsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/mypy_boto3_codepipeline.egg-info/SOURCES.txt` & `mypy-boto3-codepipeline-1.28.16/mypy_boto3_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.15.post1/setup.py` & `mypy-boto3-codepipeline-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codepipeline",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodePipeline 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CodePipeline 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 codepipeline type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 codepipeline type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codepipeline": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

