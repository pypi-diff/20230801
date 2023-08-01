# Comparing `tmp/mypy-boto3-lambda-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-lambda-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lambda-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:30 2023, max compression
+gzip compressed data, was "mypy-boto3-lambda-1.28.16.tar", last modified: Tue Aug  1 11:37:10 2023, max compression
```

## Comparing `mypy-boto3-lambda-1.28.15.post1.tar` & `mypy-boto3-lambda-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.493232 mypy-boto3-lambda-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25007 2023-07-29 10:03:30.493232 mypy-boto3-lambda-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23518 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.485231 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60385 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    60295 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79959 2023-07-29 09:49:15.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79852 2023-07-29 09:49:14.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.493232 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25007 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:30.493232 mypy-boto3-lambda-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.364844 mypy-boto3-lambda-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25237 2023-08-01 11:37:10.364844 mypy-boto3-lambda-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23757 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.356844 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59621 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59531 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    80686 2023-08-01 11:22:03.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80579 2023-08-01 11:22:02.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.364844 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25237 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:10.364844 mypy-boto3-lambda-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/setup.py
```

### Comparing `mypy-boto3-lambda-1.28.15.post1/LICENSE` & `mypy-boto3-lambda-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/PKG-INFO` & `mypy-boto3-lambda-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Lambda 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lambda type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lambda type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
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
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -76,15 +76,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -449,47 +449,48 @@
 )
 
 
 def check_value(value: ArchitectureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lambda.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lambda.type_defs import (
     AccountLimitTypeDef,
     AccountUsageTypeDef,
     AddLayerVersionPermissionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AddPermissionRequestRequestTypeDef,
     AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
+    BlobTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyTypeDef,
     CorsOutputTypeDef,
     CorsTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SourceAccessConfigurationTypeDef,
+    TimestampTypeDef,
     DeadLetterConfigTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     FileSystemConfigTypeDef,
-    FunctionCodeTypeDef,
     ImageConfigTypeDef,
     SnapStartTypeDef,
     TracingConfigTypeDef,
     VpcConfigTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCodeSigningConfigRequestRequestTypeDef,
     DeleteEventSourceMappingRequestRequestTypeDef,
@@ -525,20 +526,16 @@
     GetLayerVersionRequestRequestTypeDef,
     LayerVersionContentOutputTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProvisionedConcurrencyConfigRequestRequestTypeDef,
     GetRuntimeManagementConfigRequestRequestTypeDef,
     ImageConfigErrorTypeDef,
     ImageConfigOutputTypeDef,
-    InvocationRequestRequestTypeDef,
-    InvokeAsyncRequestRequestTypeDef,
     InvokeResponseStreamUpdateTypeDef,
     InvokeWithResponseStreamCompleteEventTypeDef,
-    InvokeWithResponseStreamRequestRequestTypeDef,
-    LayerVersionContentInputTypeDef,
     LayerVersionsListItemTypeDef,
     PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListCodeSigningConfigsRequestRequestTypeDef,
     ListEventSourceMappingsRequestRequestTypeDef,
     ListFunctionEventInvokeConfigsRequestRequestTypeDef,
     ListFunctionUrlConfigsRequestRequestTypeDef,
@@ -556,15 +553,14 @@
     PutProvisionedConcurrencyConfigRequestRequestTypeDef,
     PutRuntimeManagementConfigRequestRequestTypeDef,
     RemoveLayerVersionPermissionRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RuntimeVersionErrorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateFunctionCodeRequestRequestTypeDef,
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
     ConcurrencyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyResponseTypeDef,
@@ -577,42 +573,51 @@
     ListFunctionsByCodeSigningConfigResponseTypeDef,
     ListTagsResponseTypeDef,
     PutFunctionCodeSigningConfigResponseTypeDef,
     PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigResponseTypeDef,
     AliasConfigurationResponseTypeDef,
     AliasConfigurationTypeDef,
+    AliasRoutingConfigurationUnionTypeDef,
     CreateAliasRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
+    AllowedPublishersUnionTypeDef,
+    FunctionCodeTypeDef,
+    InvocationRequestRequestTypeDef,
+    InvokeAsyncRequestRequestTypeDef,
+    InvokeWithResponseStreamRequestRequestTypeDef,
+    LayerVersionContentInputTypeDef,
+    UpdateFunctionCodeRequestRequestTypeDef,
     CodeSigningConfigTypeDef,
     CreateCodeSigningConfigRequestRequestTypeDef,
     UpdateCodeSigningConfigRequestRequestTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     FunctionUrlConfigTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
+    CorsUnionTypeDef,
     CreateFunctionUrlConfigRequestRequestTypeDef,
     UpdateFunctionUrlConfigRequestRequestTypeDef,
-    CreateFunctionRequestRequestTypeDef,
     UpdateFunctionConfigurationRequestRequestTypeDef,
     DestinationConfigTypeDef,
     EnvironmentResponseTypeDef,
+    SelfManagedEventSourceUnionTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     GetFunctionConfigurationRequestFunctionActiveWaitTypeDef,
     GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef,
     GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef,
     GetFunctionRequestFunctionActiveV2WaitTypeDef,
     GetFunctionRequestFunctionExistsWaitTypeDef,
     GetFunctionRequestFunctionUpdatedV2WaitTypeDef,
     GetLayerVersionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     ImageConfigResponseTypeDef,
+    ImageConfigUnionTypeDef,
     InvokeWithResponseStreamResponseEventTypeDef,
-    PublishLayerVersionRequestRequestTypeDef,
     LayersListItemTypeDef,
     ListLayerVersionsResponseTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
     ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
     ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
     ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
@@ -621,40 +626,43 @@
     ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
     ListLayersRequestListLayersPaginateTypeDef,
     ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
     ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListProvisionedConcurrencyConfigsResponseTypeDef,
     RuntimeVersionConfigTypeDef,
     ListAliasesResponseTypeDef,
+    CreateFunctionRequestRequestTypeDef,
+    PublishLayerVersionRequestRequestTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     ListFunctionUrlConfigsResponseTypeDef,
     FunctionEventInvokeConfigResponseTypeDef,
     FunctionEventInvokeConfigTypeDef,
     PutFunctionEventInvokeConfigRequestRequestTypeDef,
     UpdateFunctionEventInvokeConfigRequestRequestTypeDef,
     EventSourceMappingConfigurationResponseTypeDef,
     EventSourceMappingConfigurationTypeDef,
     CreateEventSourceMappingRequestRequestTypeDef,
+    FilterCriteriaUnionTypeDef,
     UpdateEventSourceMappingRequestRequestTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     ListLayersResponseTypeDef,
     FunctionConfigurationResponseTypeDef,
     FunctionConfigurationTypeDef,
     ListFunctionEventInvokeConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
     GetFunctionResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
 )
 
 
-def get_structure() -> AccountLimitTypeDef:
+def get_value() -> AccountLimitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lambda-1.28.15.post1/README.md` & `mypy-boto3-lambda-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
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
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -44,15 +44,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -417,47 +417,48 @@
 )
 
 
 def check_value(value: ArchitectureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lambda.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lambda.type_defs import (
     AccountLimitTypeDef,
     AccountUsageTypeDef,
     AddLayerVersionPermissionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AddPermissionRequestRequestTypeDef,
     AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
+    BlobTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyTypeDef,
     CorsOutputTypeDef,
     CorsTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SourceAccessConfigurationTypeDef,
+    TimestampTypeDef,
     DeadLetterConfigTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     FileSystemConfigTypeDef,
-    FunctionCodeTypeDef,
     ImageConfigTypeDef,
     SnapStartTypeDef,
     TracingConfigTypeDef,
     VpcConfigTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCodeSigningConfigRequestRequestTypeDef,
     DeleteEventSourceMappingRequestRequestTypeDef,
@@ -493,20 +494,16 @@
     GetLayerVersionRequestRequestTypeDef,
     LayerVersionContentOutputTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProvisionedConcurrencyConfigRequestRequestTypeDef,
     GetRuntimeManagementConfigRequestRequestTypeDef,
     ImageConfigErrorTypeDef,
     ImageConfigOutputTypeDef,
-    InvocationRequestRequestTypeDef,
-    InvokeAsyncRequestRequestTypeDef,
     InvokeResponseStreamUpdateTypeDef,
     InvokeWithResponseStreamCompleteEventTypeDef,
-    InvokeWithResponseStreamRequestRequestTypeDef,
-    LayerVersionContentInputTypeDef,
     LayerVersionsListItemTypeDef,
     PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListCodeSigningConfigsRequestRequestTypeDef,
     ListEventSourceMappingsRequestRequestTypeDef,
     ListFunctionEventInvokeConfigsRequestRequestTypeDef,
     ListFunctionUrlConfigsRequestRequestTypeDef,
@@ -524,15 +521,14 @@
     PutProvisionedConcurrencyConfigRequestRequestTypeDef,
     PutRuntimeManagementConfigRequestRequestTypeDef,
     RemoveLayerVersionPermissionRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RuntimeVersionErrorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateFunctionCodeRequestRequestTypeDef,
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
     ConcurrencyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyResponseTypeDef,
@@ -545,42 +541,51 @@
     ListFunctionsByCodeSigningConfigResponseTypeDef,
     ListTagsResponseTypeDef,
     PutFunctionCodeSigningConfigResponseTypeDef,
     PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigResponseTypeDef,
     AliasConfigurationResponseTypeDef,
     AliasConfigurationTypeDef,
+    AliasRoutingConfigurationUnionTypeDef,
     CreateAliasRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
+    AllowedPublishersUnionTypeDef,
+    FunctionCodeTypeDef,
+    InvocationRequestRequestTypeDef,
+    InvokeAsyncRequestRequestTypeDef,
+    InvokeWithResponseStreamRequestRequestTypeDef,
+    LayerVersionContentInputTypeDef,
+    UpdateFunctionCodeRequestRequestTypeDef,
     CodeSigningConfigTypeDef,
     CreateCodeSigningConfigRequestRequestTypeDef,
     UpdateCodeSigningConfigRequestRequestTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     FunctionUrlConfigTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
+    CorsUnionTypeDef,
     CreateFunctionUrlConfigRequestRequestTypeDef,
     UpdateFunctionUrlConfigRequestRequestTypeDef,
-    CreateFunctionRequestRequestTypeDef,
     UpdateFunctionConfigurationRequestRequestTypeDef,
     DestinationConfigTypeDef,
     EnvironmentResponseTypeDef,
+    SelfManagedEventSourceUnionTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     GetFunctionConfigurationRequestFunctionActiveWaitTypeDef,
     GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef,
     GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef,
     GetFunctionRequestFunctionActiveV2WaitTypeDef,
     GetFunctionRequestFunctionExistsWaitTypeDef,
     GetFunctionRequestFunctionUpdatedV2WaitTypeDef,
     GetLayerVersionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     ImageConfigResponseTypeDef,
+    ImageConfigUnionTypeDef,
     InvokeWithResponseStreamResponseEventTypeDef,
-    PublishLayerVersionRequestRequestTypeDef,
     LayersListItemTypeDef,
     ListLayerVersionsResponseTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
     ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
     ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
     ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
@@ -589,40 +594,43 @@
     ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
     ListLayersRequestListLayersPaginateTypeDef,
     ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
     ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListProvisionedConcurrencyConfigsResponseTypeDef,
     RuntimeVersionConfigTypeDef,
     ListAliasesResponseTypeDef,
+    CreateFunctionRequestRequestTypeDef,
+    PublishLayerVersionRequestRequestTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     ListFunctionUrlConfigsResponseTypeDef,
     FunctionEventInvokeConfigResponseTypeDef,
     FunctionEventInvokeConfigTypeDef,
     PutFunctionEventInvokeConfigRequestRequestTypeDef,
     UpdateFunctionEventInvokeConfigRequestRequestTypeDef,
     EventSourceMappingConfigurationResponseTypeDef,
     EventSourceMappingConfigurationTypeDef,
     CreateEventSourceMappingRequestRequestTypeDef,
+    FilterCriteriaUnionTypeDef,
     UpdateEventSourceMappingRequestRequestTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     ListLayersResponseTypeDef,
     FunctionConfigurationResponseTypeDef,
     FunctionConfigurationTypeDef,
     ListFunctionEventInvokeConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
     GetFunctionResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
 )
 
 
-def get_structure() -> AccountLimitTypeDef:
+def get_value() -> AccountLimitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__init__.py` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__init__.pyi` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__main__.py` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lambda 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Lambda 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda\nOther"
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

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/client.py` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,17 @@
     from mypy_boto3_lambda.client import LambdaClient
 
     session = Session()
     client: LambdaClient = session.client("lambda")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ArchitectureType,
     EventSourcePositionType,
     FunctionUrlAuthTypeType,
     InvocationTypeType,
     InvokeModeType,
@@ -45,51 +43,47 @@
     ListProvisionedConcurrencyConfigsPaginator,
     ListVersionsByFunctionPaginator,
 )
 from .type_defs import (
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
     AliasConfigurationResponseTypeDef,
-    AliasRoutingConfigurationOutputTypeDef,
-    AliasRoutingConfigurationTypeDef,
-    AllowedPublishersOutputTypeDef,
-    AllowedPublishersTypeDef,
+    AliasRoutingConfigurationUnionTypeDef,
+    AllowedPublishersUnionTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
+    BlobTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyResponseTypeDef,
-    CorsOutputTypeDef,
-    CorsTypeDef,
+    CorsUnionTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     EventSourceMappingConfigurationResponseTypeDef,
     FileSystemConfigTypeDef,
-    FilterCriteriaOutputTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     FunctionCodeTypeDef,
     FunctionConfigurationResponseTypeDef,
     FunctionEventInvokeConfigResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigResponseTypeDef,
-    ImageConfigOutputTypeDef,
-    ImageConfigTypeDef,
+    ImageConfigUnionTypeDef,
     InvocationResponseTypeDef,
     InvokeAsyncResponseTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     LayerVersionContentInputTypeDef,
     ListAliasesResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
@@ -103,19 +97,19 @@
     ListTagsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     PutFunctionCodeSigningConfigResponseTypeDef,
     PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigResponseTypeDef,
     ScalingConfigTypeDef,
-    SelfManagedEventSourceOutputTypeDef,
-    SelfManagedEventSourceTypeDef,
+    SelfManagedEventSourceUnionTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SnapStartTypeDef,
     SourceAccessConfigurationTypeDef,
+    TimestampTypeDef,
     TracingConfigTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
     VpcConfigTypeDef,
 )
 from .waiter import (
     FunctionActiveV2Waiter,
@@ -263,30 +257,28 @@
     def create_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
-        RoutingConfig: Union[
-            AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
-        ] = ...
+        RoutingConfig: AliasRoutingConfigurationUnionTypeDef = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_ for a Lambda function version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_alias)
         """
 
     def create_code_signing_config(
         self,
         *,
-        AllowedPublishers: Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef],
+        AllowedPublishers: AllowedPublishersUnionTypeDef,
         Description: str = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> CreateCodeSigningConfigResponseTypeDef:
         """
         Creates a code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_code_signing_config)
@@ -296,30 +288,28 @@
     def create_event_source_mapping(
         self,
         *,
         FunctionName: str,
         EventSourceArn: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        FilterCriteria: FilterCriteriaUnionTypeDef = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         ParallelizationFactor: int = ...,
         StartingPosition: EventSourcePositionType = ...,
-        StartingPositionTimestamp: Union[datetime, str] = ...,
+        StartingPositionTimestamp: TimestampTypeDef = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         TumblingWindowInSeconds: int = ...,
         Topics: Sequence[str] = ...,
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
-        SelfManagedEventSource: Union[
-            SelfManagedEventSourceTypeDef, SelfManagedEventSourceOutputTypeDef
-        ] = ...,
+        SelfManagedEventSource: SelfManagedEventSourceUnionTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
@@ -346,15 +336,15 @@
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         Environment: EnvironmentTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: Union[ImageConfigTypeDef, ImageConfigOutputTypeDef] = ...,
+        ImageConfig: ImageConfigUnionTypeDef = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
@@ -365,15 +355,15 @@
 
     def create_function_url_config(
         self,
         *,
         FunctionName: str,
         AuthType: FunctionUrlAuthTypeType,
         Qualifier: str = ...,
-        Cors: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
+        Cors: CorsUnionTypeDef = ...,
         InvokeMode: InvokeModeType = ...
     ) -> CreateFunctionUrlConfigResponseTypeDef:
         """
         Creates a Lambda function URL with the specified configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function_url_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_function_url_config)
@@ -662,26 +652,26 @@
     def invoke(
         self,
         *,
         FunctionName: str,
         InvocationType: InvocationTypeType = ...,
         LogType: LogTypeType = ...,
         ClientContext: str = ...,
-        Payload: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        Payload: BlobTypeDef = ...,
         Qualifier: str = ...
     ) -> InvocationResponseTypeDef:
         """
         Invokes a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#invoke)
         """
 
     def invoke_async(
-        self, *, FunctionName: str, InvokeArgs: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, FunctionName: str, InvokeArgs: BlobTypeDef
     ) -> InvokeAsyncResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke_async)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#invoke_async)
         """
@@ -690,15 +680,15 @@
         self,
         *,
         FunctionName: str,
         InvocationType: ResponseStreamingInvocationTypeType = ...,
         LogType: LogTypeType = ...,
         ClientContext: str = ...,
         Qualifier: str = ...,
-        Payload: Union[str, bytes, IO[Any], StreamingBody] = ...
+        Payload: BlobTypeDef = ...
     ) -> InvokeWithResponseStreamResponseTypeDef:
         """
         Configure your Lambda functions to stream response payloads back to clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke_with_response_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#invoke_with_response_stream)
         """
@@ -1003,17 +993,15 @@
     def update_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
-        RoutingConfig: Union[
-            AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
-        ] = ...,
+        RoutingConfig: AliasRoutingConfigurationUnionTypeDef = ...,
         RevisionId: str = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
@@ -1022,15 +1010,15 @@
         """
 
     def update_code_signing_config(
         self,
         *,
         CodeSigningConfigArn: str,
         Description: str = ...,
-        AllowedPublishers: Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef] = ...,
+        AllowedPublishers: AllowedPublishersUnionTypeDef = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> UpdateCodeSigningConfigResponseTypeDef:
         """
         Update the code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_code_signing_config)
@@ -1039,15 +1027,15 @@
     def update_event_source_mapping(
         self,
         *,
         UUID: str,
         FunctionName: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        FilterCriteria: FilterCriteriaUnionTypeDef = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
@@ -1063,15 +1051,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_event_source_mapping)
         """
 
     def update_function_code(
         self,
         *,
         FunctionName: str,
-        ZipFile: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        ZipFile: BlobTypeDef = ...,
         S3Bucket: str = ...,
         S3Key: str = ...,
         S3ObjectVersion: str = ...,
         ImageUri: str = ...,
         Publish: bool = ...,
         DryRun: bool = ...,
         RevisionId: str = ...,
@@ -1098,15 +1086,15 @@
         Runtime: RuntimeType = ...,
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: Union[ImageConfigTypeDef, ImageConfigOutputTypeDef] = ...,
+        ImageConfig: ImageConfigUnionTypeDef = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
@@ -1132,15 +1120,15 @@
 
     def update_function_url_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         AuthType: FunctionUrlAuthTypeType = ...,
-        Cors: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
+        Cors: CorsUnionTypeDef = ...,
         InvokeMode: InvokeModeType = ...
     ) -> UpdateFunctionUrlConfigResponseTypeDef:
         """
         Updates the configuration for a Lambda function URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_url_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_url_config)
```

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/client.pyi` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,17 @@
     from mypy_boto3_lambda.client import LambdaClient
 
     session = Session()
     client: LambdaClient = session.client("lambda")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ArchitectureType,
     EventSourcePositionType,
     FunctionUrlAuthTypeType,
     InvocationTypeType,
     InvokeModeType,
@@ -45,51 +43,47 @@
     ListProvisionedConcurrencyConfigsPaginator,
     ListVersionsByFunctionPaginator,
 )
 from .type_defs import (
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
     AliasConfigurationResponseTypeDef,
-    AliasRoutingConfigurationOutputTypeDef,
-    AliasRoutingConfigurationTypeDef,
-    AllowedPublishersOutputTypeDef,
-    AllowedPublishersTypeDef,
+    AliasRoutingConfigurationUnionTypeDef,
+    AllowedPublishersUnionTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
+    BlobTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyResponseTypeDef,
-    CorsOutputTypeDef,
-    CorsTypeDef,
+    CorsUnionTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     EventSourceMappingConfigurationResponseTypeDef,
     FileSystemConfigTypeDef,
-    FilterCriteriaOutputTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     FunctionCodeTypeDef,
     FunctionConfigurationResponseTypeDef,
     FunctionEventInvokeConfigResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigResponseTypeDef,
-    ImageConfigOutputTypeDef,
-    ImageConfigTypeDef,
+    ImageConfigUnionTypeDef,
     InvocationResponseTypeDef,
     InvokeAsyncResponseTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     LayerVersionContentInputTypeDef,
     ListAliasesResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
@@ -103,19 +97,19 @@
     ListTagsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     PutFunctionCodeSigningConfigResponseTypeDef,
     PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigResponseTypeDef,
     ScalingConfigTypeDef,
-    SelfManagedEventSourceOutputTypeDef,
-    SelfManagedEventSourceTypeDef,
+    SelfManagedEventSourceUnionTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SnapStartTypeDef,
     SourceAccessConfigurationTypeDef,
+    TimestampTypeDef,
     TracingConfigTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
     VpcConfigTypeDef,
 )
 from .waiter import (
     FunctionActiveV2Waiter,
@@ -254,29 +248,27 @@
     def create_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
-        RoutingConfig: Union[
-            AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
-        ] = ...
+        RoutingConfig: AliasRoutingConfigurationUnionTypeDef = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_ for a Lambda function version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_alias)
         """
     def create_code_signing_config(
         self,
         *,
-        AllowedPublishers: Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef],
+        AllowedPublishers: AllowedPublishersUnionTypeDef,
         Description: str = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> CreateCodeSigningConfigResponseTypeDef:
         """
         Creates a code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_code_signing_config)
@@ -285,30 +277,28 @@
     def create_event_source_mapping(
         self,
         *,
         FunctionName: str,
         EventSourceArn: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        FilterCriteria: FilterCriteriaUnionTypeDef = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         ParallelizationFactor: int = ...,
         StartingPosition: EventSourcePositionType = ...,
-        StartingPositionTimestamp: Union[datetime, str] = ...,
+        StartingPositionTimestamp: TimestampTypeDef = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         TumblingWindowInSeconds: int = ...,
         Topics: Sequence[str] = ...,
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
-        SelfManagedEventSource: Union[
-            SelfManagedEventSourceTypeDef, SelfManagedEventSourceOutputTypeDef
-        ] = ...,
+        SelfManagedEventSource: SelfManagedEventSourceUnionTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
@@ -334,15 +324,15 @@
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         Environment: EnvironmentTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: Union[ImageConfigTypeDef, ImageConfigOutputTypeDef] = ...,
+        ImageConfig: ImageConfigUnionTypeDef = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
@@ -352,15 +342,15 @@
         """
     def create_function_url_config(
         self,
         *,
         FunctionName: str,
         AuthType: FunctionUrlAuthTypeType,
         Qualifier: str = ...,
-        Cors: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
+        Cors: CorsUnionTypeDef = ...,
         InvokeMode: InvokeModeType = ...
     ) -> CreateFunctionUrlConfigResponseTypeDef:
         """
         Creates a Lambda function URL with the specified configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function_url_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_function_url_config)
@@ -621,25 +611,25 @@
     def invoke(
         self,
         *,
         FunctionName: str,
         InvocationType: InvocationTypeType = ...,
         LogType: LogTypeType = ...,
         ClientContext: str = ...,
-        Payload: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        Payload: BlobTypeDef = ...,
         Qualifier: str = ...
     ) -> InvocationResponseTypeDef:
         """
         Invokes a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#invoke)
         """
     def invoke_async(
-        self, *, FunctionName: str, InvokeArgs: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, FunctionName: str, InvokeArgs: BlobTypeDef
     ) -> InvokeAsyncResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke_async)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#invoke_async)
         """
@@ -647,15 +637,15 @@
         self,
         *,
         FunctionName: str,
         InvocationType: ResponseStreamingInvocationTypeType = ...,
         LogType: LogTypeType = ...,
         ClientContext: str = ...,
         Qualifier: str = ...,
-        Payload: Union[str, bytes, IO[Any], StreamingBody] = ...
+        Payload: BlobTypeDef = ...
     ) -> InvokeWithResponseStreamResponseTypeDef:
         """
         Configure your Lambda functions to stream response payloads back to clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke_with_response_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#invoke_with_response_stream)
         """
@@ -936,17 +926,15 @@
     def update_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
-        RoutingConfig: Union[
-            AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
-        ] = ...,
+        RoutingConfig: AliasRoutingConfigurationUnionTypeDef = ...,
         RevisionId: str = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
@@ -954,15 +942,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_alias)
         """
     def update_code_signing_config(
         self,
         *,
         CodeSigningConfigArn: str,
         Description: str = ...,
-        AllowedPublishers: Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef] = ...,
+        AllowedPublishers: AllowedPublishersUnionTypeDef = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> UpdateCodeSigningConfigResponseTypeDef:
         """
         Update the code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_code_signing_config)
@@ -970,15 +958,15 @@
     def update_event_source_mapping(
         self,
         *,
         UUID: str,
         FunctionName: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        FilterCriteria: FilterCriteriaUnionTypeDef = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
@@ -993,15 +981,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_event_source_mapping)
         """
     def update_function_code(
         self,
         *,
         FunctionName: str,
-        ZipFile: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        ZipFile: BlobTypeDef = ...,
         S3Bucket: str = ...,
         S3Key: str = ...,
         S3ObjectVersion: str = ...,
         ImageUri: str = ...,
         Publish: bool = ...,
         DryRun: bool = ...,
         RevisionId: str = ...,
@@ -1027,15 +1015,15 @@
         Runtime: RuntimeType = ...,
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: Union[ImageConfigTypeDef, ImageConfigOutputTypeDef] = ...,
+        ImageConfig: ImageConfigUnionTypeDef = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
@@ -1059,15 +1047,15 @@
         """
     def update_function_url_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         AuthType: FunctionUrlAuthTypeType = ...,
-        Cors: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
+        Cors: CorsUnionTypeDef = ...,
         InvokeMode: InvokeModeType = ...
     ) -> UpdateFunctionUrlConfigResponseTypeDef:
         """
         Updates the configuration for a Lambda function URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_url_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_url_config)
```

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/literals.py` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/literals.pyi` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/paginator.py` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/paginator.pyi` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/type_defs.py` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lambda.type_defs import AccountLimitTypeDef
 
-    data: AccountLimitTypeDef = {...}
+    data: AccountLimitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.eventstream import EventStream
@@ -59,28 +59,29 @@
     "ResponseMetadataTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "AliasRoutingConfigurationOutputTypeDef",
     "AliasRoutingConfigurationTypeDef",
     "AllowedPublishersOutputTypeDef",
     "AllowedPublishersTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
+    "BlobTypeDef",
     "CodeSigningPoliciesTypeDef",
     "ConcurrencyTypeDef",
     "CorsOutputTypeDef",
     "CorsTypeDef",
     "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
     "SourceAccessConfigurationTypeDef",
+    "TimestampTypeDef",
     "DeadLetterConfigTypeDef",
     "EnvironmentTypeDef",
     "EphemeralStorageTypeDef",
     "FileSystemConfigTypeDef",
-    "FunctionCodeTypeDef",
     "ImageConfigTypeDef",
     "SnapStartTypeDef",
     "TracingConfigTypeDef",
     "VpcConfigTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCodeSigningConfigRequestRequestTypeDef",
     "DeleteEventSourceMappingRequestRequestTypeDef",
@@ -116,20 +117,16 @@
     "GetLayerVersionRequestRequestTypeDef",
     "LayerVersionContentOutputTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
     "GetRuntimeManagementConfigRequestRequestTypeDef",
     "ImageConfigErrorTypeDef",
     "ImageConfigOutputTypeDef",
-    "InvocationRequestRequestTypeDef",
-    "InvokeAsyncRequestRequestTypeDef",
     "InvokeResponseStreamUpdateTypeDef",
     "InvokeWithResponseStreamCompleteEventTypeDef",
-    "InvokeWithResponseStreamRequestRequestTypeDef",
-    "LayerVersionContentInputTypeDef",
     "LayerVersionsListItemTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListCodeSigningConfigsRequestRequestTypeDef",
     "ListEventSourceMappingsRequestRequestTypeDef",
     "ListFunctionEventInvokeConfigsRequestRequestTypeDef",
     "ListFunctionUrlConfigsRequestRequestTypeDef",
@@ -147,15 +144,14 @@
     "PutProvisionedConcurrencyConfigRequestRequestTypeDef",
     "PutRuntimeManagementConfigRequestRequestTypeDef",
     "RemoveLayerVersionPermissionRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RuntimeVersionErrorTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateFunctionCodeRequestRequestTypeDef",
     "AddLayerVersionPermissionResponseTypeDef",
     "AddPermissionResponseTypeDef",
     "ConcurrencyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAccountSettingsResponseTypeDef",
     "GetFunctionCodeSigningConfigResponseTypeDef",
     "GetFunctionConcurrencyResponseTypeDef",
@@ -168,42 +164,51 @@
     "ListFunctionsByCodeSigningConfigResponseTypeDef",
     "ListTagsResponseTypeDef",
     "PutFunctionCodeSigningConfigResponseTypeDef",
     "PutProvisionedConcurrencyConfigResponseTypeDef",
     "PutRuntimeManagementConfigResponseTypeDef",
     "AliasConfigurationResponseTypeDef",
     "AliasConfigurationTypeDef",
+    "AliasRoutingConfigurationUnionTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
+    "AllowedPublishersUnionTypeDef",
+    "FunctionCodeTypeDef",
+    "InvocationRequestRequestTypeDef",
+    "InvokeAsyncRequestRequestTypeDef",
+    "InvokeWithResponseStreamRequestRequestTypeDef",
+    "LayerVersionContentInputTypeDef",
+    "UpdateFunctionCodeRequestRequestTypeDef",
     "CodeSigningConfigTypeDef",
     "CreateCodeSigningConfigRequestRequestTypeDef",
     "UpdateCodeSigningConfigRequestRequestTypeDef",
     "CreateFunctionUrlConfigResponseTypeDef",
     "FunctionUrlConfigTypeDef",
     "GetFunctionUrlConfigResponseTypeDef",
     "UpdateFunctionUrlConfigResponseTypeDef",
+    "CorsUnionTypeDef",
     "CreateFunctionUrlConfigRequestRequestTypeDef",
     "UpdateFunctionUrlConfigRequestRequestTypeDef",
-    "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionConfigurationRequestRequestTypeDef",
     "DestinationConfigTypeDef",
     "EnvironmentResponseTypeDef",
+    "SelfManagedEventSourceUnionTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "GetFunctionConfigurationRequestFunctionActiveWaitTypeDef",
     "GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef",
     "GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef",
     "GetFunctionRequestFunctionActiveV2WaitTypeDef",
     "GetFunctionRequestFunctionExistsWaitTypeDef",
     "GetFunctionRequestFunctionUpdatedV2WaitTypeDef",
     "GetLayerVersionResponseTypeDef",
     "PublishLayerVersionResponseTypeDef",
     "ImageConfigResponseTypeDef",
+    "ImageConfigUnionTypeDef",
     "InvokeWithResponseStreamResponseEventTypeDef",
-    "PublishLayerVersionRequestRequestTypeDef",
     "LayersListItemTypeDef",
     "ListLayerVersionsResponseTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
     "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
     "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
     "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
@@ -212,26 +217,29 @@
     "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
     "ListLayersRequestListLayersPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
     "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     "RuntimeVersionConfigTypeDef",
     "ListAliasesResponseTypeDef",
+    "CreateFunctionRequestRequestTypeDef",
+    "PublishLayerVersionRequestRequestTypeDef",
     "CreateCodeSigningConfigResponseTypeDef",
     "GetCodeSigningConfigResponseTypeDef",
     "ListCodeSigningConfigsResponseTypeDef",
     "UpdateCodeSigningConfigResponseTypeDef",
     "ListFunctionUrlConfigsResponseTypeDef",
     "FunctionEventInvokeConfigResponseTypeDef",
     "FunctionEventInvokeConfigTypeDef",
     "PutFunctionEventInvokeConfigRequestRequestTypeDef",
     "UpdateFunctionEventInvokeConfigRequestRequestTypeDef",
     "EventSourceMappingConfigurationResponseTypeDef",
     "EventSourceMappingConfigurationTypeDef",
     "CreateEventSourceMappingRequestRequestTypeDef",
+    "FilterCriteriaUnionTypeDef",
     "UpdateEventSourceMappingRequestRequestTypeDef",
     "InvokeWithResponseStreamResponseTypeDef",
     "ListLayersResponseTypeDef",
     "FunctionConfigurationResponseTypeDef",
     "FunctionConfigurationTypeDef",
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     "ListEventSourceMappingsResponseTypeDef",
@@ -363,14 +371,15 @@
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     {
         "ConsumerGroupId": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CodeSigningPoliciesTypeDef = TypedDict(
     "CodeSigningPoliciesTypeDef",
     {
         "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
     },
     total=False,
 )
@@ -448,14 +457,15 @@
     {
         "Type": SourceAccessTypeType,
         "URI": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "TargetArn": str,
     },
     total=False,
 )
@@ -479,26 +489,14 @@
     "FileSystemConfigTypeDef",
     {
         "Arn": str,
         "LocalMountPath": str,
     },
 )
 
-FunctionCodeTypeDef = TypedDict(
-    "FunctionCodeTypeDef",
-    {
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3ObjectVersion": str,
-        "ImageUri": str,
-    },
-    total=False,
-)
-
 ImageConfigTypeDef = TypedDict(
     "ImageConfigTypeDef",
     {
         "EntryPoint": Sequence[str],
         "Command": Sequence[str],
         "WorkingDirectory": str,
     },
@@ -970,47 +968,14 @@
         "EntryPoint": List[str],
         "Command": List[str],
         "WorkingDirectory": str,
     },
     total=False,
 )
 
-_RequiredInvocationRequestRequestTypeDef = TypedDict(
-    "_RequiredInvocationRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalInvocationRequestRequestTypeDef = TypedDict(
-    "_OptionalInvocationRequestRequestTypeDef",
-    {
-        "InvocationType": InvocationTypeType,
-        "LogType": LogTypeType,
-        "ClientContext": str,
-        "Payload": Union[str, bytes, IO[Any], StreamingBody],
-        "Qualifier": str,
-    },
-    total=False,
-)
-
-
-class InvocationRequestRequestTypeDef(
-    _RequiredInvocationRequestRequestTypeDef, _OptionalInvocationRequestRequestTypeDef
-):
-    pass
-
-
-InvokeAsyncRequestRequestTypeDef = TypedDict(
-    "InvokeAsyncRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-        "InvokeArgs": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 InvokeResponseStreamUpdateTypeDef = TypedDict(
     "InvokeResponseStreamUpdateTypeDef",
     {
         "Payload": bytes,
     },
     total=False,
 )
@@ -1021,51 +986,14 @@
         "ErrorCode": str,
         "ErrorDetails": str,
         "LogResult": str,
     },
     total=False,
 )
 
-_RequiredInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
-    "_RequiredInvokeWithResponseStreamRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
-    "_OptionalInvokeWithResponseStreamRequestRequestTypeDef",
-    {
-        "InvocationType": ResponseStreamingInvocationTypeType,
-        "LogType": LogTypeType,
-        "ClientContext": str,
-        "Qualifier": str,
-        "Payload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class InvokeWithResponseStreamRequestRequestTypeDef(
-    _RequiredInvokeWithResponseStreamRequestRequestTypeDef,
-    _OptionalInvokeWithResponseStreamRequestRequestTypeDef,
-):
-    pass
-
-
-LayerVersionContentInputTypeDef = TypedDict(
-    "LayerVersionContentInputTypeDef",
-    {
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3ObjectVersion": str,
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 LayerVersionsListItemTypeDef = TypedDict(
     "LayerVersionsListItemTypeDef",
     {
         "LayerVersionArn": str,
         "Version": int,
         "Description": str,
         "CreatedDate": str,
@@ -1451,44 +1379,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateFunctionCodeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFunctionCodeRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalUpdateFunctionCodeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFunctionCodeRequestRequestTypeDef",
-    {
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3ObjectVersion": str,
-        "ImageUri": str,
-        "Publish": bool,
-        "DryRun": bool,
-        "RevisionId": str,
-        "Architectures": Sequence[ArchitectureType],
-    },
-    total=False,
-)
-
-
-class UpdateFunctionCodeRequestRequestTypeDef(
-    _RequiredUpdateFunctionCodeRequestRequestTypeDef,
-    _OptionalUpdateFunctionCodeRequestRequestTypeDef,
-):
-    pass
-
-
 AddLayerVersionPermissionResponseTypeDef = TypedDict(
     "AddLayerVersionPermissionResponseTypeDef",
     {
         "Statement": str,
         "RevisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1675,14 +1573,17 @@
         "Description": str,
         "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
         "RevisionId": str,
     },
     total=False,
 )
 
+AliasRoutingConfigurationUnionTypeDef = Union[
+    AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
+]
 _RequiredCreateAliasRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
         "FunctionVersion": str,
     },
@@ -1724,14 +1625,127 @@
 
 class UpdateAliasRequestRequestTypeDef(
     _RequiredUpdateAliasRequestRequestTypeDef, _OptionalUpdateAliasRequestRequestTypeDef
 ):
     pass
 
 
+AllowedPublishersUnionTypeDef = Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef]
+FunctionCodeTypeDef = TypedDict(
+    "FunctionCodeTypeDef",
+    {
+        "ZipFile": BlobTypeDef,
+        "S3Bucket": str,
+        "S3Key": str,
+        "S3ObjectVersion": str,
+        "ImageUri": str,
+    },
+    total=False,
+)
+
+_RequiredInvocationRequestRequestTypeDef = TypedDict(
+    "_RequiredInvocationRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalInvocationRequestRequestTypeDef = TypedDict(
+    "_OptionalInvocationRequestRequestTypeDef",
+    {
+        "InvocationType": InvocationTypeType,
+        "LogType": LogTypeType,
+        "ClientContext": str,
+        "Payload": BlobTypeDef,
+        "Qualifier": str,
+    },
+    total=False,
+)
+
+
+class InvocationRequestRequestTypeDef(
+    _RequiredInvocationRequestRequestTypeDef, _OptionalInvocationRequestRequestTypeDef
+):
+    pass
+
+
+InvokeAsyncRequestRequestTypeDef = TypedDict(
+    "InvokeAsyncRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+        "InvokeArgs": BlobTypeDef,
+    },
+)
+
+_RequiredInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
+    "_RequiredInvokeWithResponseStreamRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
+    "_OptionalInvokeWithResponseStreamRequestRequestTypeDef",
+    {
+        "InvocationType": ResponseStreamingInvocationTypeType,
+        "LogType": LogTypeType,
+        "ClientContext": str,
+        "Qualifier": str,
+        "Payload": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class InvokeWithResponseStreamRequestRequestTypeDef(
+    _RequiredInvokeWithResponseStreamRequestRequestTypeDef,
+    _OptionalInvokeWithResponseStreamRequestRequestTypeDef,
+):
+    pass
+
+
+LayerVersionContentInputTypeDef = TypedDict(
+    "LayerVersionContentInputTypeDef",
+    {
+        "S3Bucket": str,
+        "S3Key": str,
+        "S3ObjectVersion": str,
+        "ZipFile": BlobTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUpdateFunctionCodeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFunctionCodeRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalUpdateFunctionCodeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFunctionCodeRequestRequestTypeDef",
+    {
+        "ZipFile": BlobTypeDef,
+        "S3Bucket": str,
+        "S3Key": str,
+        "S3ObjectVersion": str,
+        "ImageUri": str,
+        "Publish": bool,
+        "DryRun": bool,
+        "RevisionId": str,
+        "Architectures": Sequence[ArchitectureType],
+    },
+    total=False,
+)
+
+
+class UpdateFunctionCodeRequestRequestTypeDef(
+    _RequiredUpdateFunctionCodeRequestRequestTypeDef,
+    _OptionalUpdateFunctionCodeRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCodeSigningConfigTypeDef = TypedDict(
     "_RequiredCodeSigningConfigTypeDef",
     {
         "CodeSigningConfigId": str,
         "CodeSigningConfigArn": str,
         "AllowedPublishers": AllowedPublishersOutputTypeDef,
         "CodeSigningPolicies": CodeSigningPoliciesTypeDef,
@@ -1863,14 +1877,15 @@
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
 _RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "AuthType": FunctionUrlAuthTypeType,
     },
 )
@@ -1913,56 +1928,14 @@
 class UpdateFunctionUrlConfigRequestRequestTypeDef(
     _RequiredUpdateFunctionUrlConfigRequestRequestTypeDef,
     _OptionalUpdateFunctionUrlConfigRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateFunctionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFunctionRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-        "Role": str,
-        "Code": FunctionCodeTypeDef,
-    },
-)
-_OptionalCreateFunctionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFunctionRequestRequestTypeDef",
-    {
-        "Runtime": RuntimeType,
-        "Handler": str,
-        "Description": str,
-        "Timeout": int,
-        "MemorySize": int,
-        "Publish": bool,
-        "VpcConfig": VpcConfigTypeDef,
-        "PackageType": PackageTypeType,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "Environment": EnvironmentTypeDef,
-        "KMSKeyArn": str,
-        "TracingConfig": TracingConfigTypeDef,
-        "Tags": Mapping[str, str],
-        "Layers": Sequence[str],
-        "FileSystemConfigs": Sequence[FileSystemConfigTypeDef],
-        "ImageConfig": ImageConfigTypeDef,
-        "CodeSigningConfigArn": str,
-        "Architectures": Sequence[ArchitectureType],
-        "EphemeralStorage": EphemeralStorageTypeDef,
-        "SnapStart": SnapStartTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateFunctionRequestRequestTypeDef(
-    _RequiredCreateFunctionRequestRequestTypeDef, _OptionalCreateFunctionRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateFunctionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionConfigurationRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalUpdateFunctionConfigurationRequestRequestTypeDef = TypedDict(
@@ -2011,14 +1984,17 @@
     {
         "Variables": Dict[str, str],
         "Error": EnvironmentErrorTypeDef,
     },
     total=False,
 )
 
+SelfManagedEventSourceUnionTypeDef = Union[
+    SelfManagedEventSourceTypeDef, SelfManagedEventSourceOutputTypeDef
+]
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
         "Filters": List[FilterTypeDef],
     },
     total=False,
 )
@@ -2206,49 +2182,24 @@
     {
         "ImageConfig": ImageConfigOutputTypeDef,
         "Error": ImageConfigErrorTypeDef,
     },
     total=False,
 )
 
+ImageConfigUnionTypeDef = Union[ImageConfigTypeDef, ImageConfigOutputTypeDef]
 InvokeWithResponseStreamResponseEventTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseEventTypeDef",
     {
         "PayloadChunk": InvokeResponseStreamUpdateTypeDef,
         "InvokeComplete": InvokeWithResponseStreamCompleteEventTypeDef,
     },
     total=False,
 )
 
-_RequiredPublishLayerVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredPublishLayerVersionRequestRequestTypeDef",
-    {
-        "LayerName": str,
-        "Content": LayerVersionContentInputTypeDef,
-    },
-)
-_OptionalPublishLayerVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalPublishLayerVersionRequestRequestTypeDef",
-    {
-        "Description": str,
-        "CompatibleRuntimes": Sequence[RuntimeType],
-        "LicenseInfo": str,
-        "CompatibleArchitectures": Sequence[ArchitectureType],
-    },
-    total=False,
-)
-
-
-class PublishLayerVersionRequestRequestTypeDef(
-    _RequiredPublishLayerVersionRequestRequestTypeDef,
-    _OptionalPublishLayerVersionRequestRequestTypeDef,
-):
-    pass
-
-
 LayersListItemTypeDef = TypedDict(
     "LayersListItemTypeDef",
     {
         "LayerName": str,
         "LayerArn": str,
         "LatestMatchingVersion": LayerVersionsListItemTypeDef,
     },
@@ -2482,14 +2433,82 @@
     {
         "NextMarker": str,
         "Aliases": List[AliasConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateFunctionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFunctionRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+        "Role": str,
+        "Code": FunctionCodeTypeDef,
+    },
+)
+_OptionalCreateFunctionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFunctionRequestRequestTypeDef",
+    {
+        "Runtime": RuntimeType,
+        "Handler": str,
+        "Description": str,
+        "Timeout": int,
+        "MemorySize": int,
+        "Publish": bool,
+        "VpcConfig": VpcConfigTypeDef,
+        "PackageType": PackageTypeType,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
+        "Environment": EnvironmentTypeDef,
+        "KMSKeyArn": str,
+        "TracingConfig": TracingConfigTypeDef,
+        "Tags": Mapping[str, str],
+        "Layers": Sequence[str],
+        "FileSystemConfigs": Sequence[FileSystemConfigTypeDef],
+        "ImageConfig": ImageConfigTypeDef,
+        "CodeSigningConfigArn": str,
+        "Architectures": Sequence[ArchitectureType],
+        "EphemeralStorage": EphemeralStorageTypeDef,
+        "SnapStart": SnapStartTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateFunctionRequestRequestTypeDef(
+    _RequiredCreateFunctionRequestRequestTypeDef, _OptionalCreateFunctionRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredPublishLayerVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishLayerVersionRequestRequestTypeDef",
+    {
+        "LayerName": str,
+        "Content": LayerVersionContentInputTypeDef,
+    },
+)
+_OptionalPublishLayerVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishLayerVersionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "CompatibleRuntimes": Sequence[RuntimeType],
+        "LicenseInfo": str,
+        "CompatibleArchitectures": Sequence[ArchitectureType],
+    },
+    total=False,
+)
+
+
+class PublishLayerVersionRequestRequestTypeDef(
+    _RequiredPublishLayerVersionRequestRequestTypeDef,
+    _OptionalPublishLayerVersionRequestRequestTypeDef,
+):
+    pass
+
+
 CreateCodeSigningConfigResponseTypeDef = TypedDict(
     "CreateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2682,15 +2701,15 @@
         "EventSourceArn": str,
         "Enabled": bool,
         "BatchSize": int,
         "FilterCriteria": FilterCriteriaTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "ParallelizationFactor": int,
         "StartingPosition": EventSourcePositionType,
-        "StartingPositionTimestamp": Union[datetime, str],
+        "StartingPositionTimestamp": TimestampTypeDef,
         "DestinationConfig": DestinationConfigTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "Topics": Sequence[str],
         "Queues": Sequence[str],
@@ -2709,14 +2728,15 @@
 class CreateEventSourceMappingRequestRequestTypeDef(
     _RequiredCreateEventSourceMappingRequestRequestTypeDef,
     _OptionalCreateEventSourceMappingRequestRequestTypeDef,
 ):
     pass
 
 
+FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
 _RequiredUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventSourceMappingRequestRequestTypeDef",
     {
         "UUID": str,
     },
 )
 _OptionalUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/type_defs.pyi` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lambda.type_defs import AccountLimitTypeDef
 
-    data: AccountLimitTypeDef = {...}
+    data: AccountLimitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.eventstream import EventStream
@@ -58,28 +58,29 @@
     "ResponseMetadataTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "AliasRoutingConfigurationOutputTypeDef",
     "AliasRoutingConfigurationTypeDef",
     "AllowedPublishersOutputTypeDef",
     "AllowedPublishersTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
+    "BlobTypeDef",
     "CodeSigningPoliciesTypeDef",
     "ConcurrencyTypeDef",
     "CorsOutputTypeDef",
     "CorsTypeDef",
     "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
     "SourceAccessConfigurationTypeDef",
+    "TimestampTypeDef",
     "DeadLetterConfigTypeDef",
     "EnvironmentTypeDef",
     "EphemeralStorageTypeDef",
     "FileSystemConfigTypeDef",
-    "FunctionCodeTypeDef",
     "ImageConfigTypeDef",
     "SnapStartTypeDef",
     "TracingConfigTypeDef",
     "VpcConfigTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCodeSigningConfigRequestRequestTypeDef",
     "DeleteEventSourceMappingRequestRequestTypeDef",
@@ -115,20 +116,16 @@
     "GetLayerVersionRequestRequestTypeDef",
     "LayerVersionContentOutputTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
     "GetRuntimeManagementConfigRequestRequestTypeDef",
     "ImageConfigErrorTypeDef",
     "ImageConfigOutputTypeDef",
-    "InvocationRequestRequestTypeDef",
-    "InvokeAsyncRequestRequestTypeDef",
     "InvokeResponseStreamUpdateTypeDef",
     "InvokeWithResponseStreamCompleteEventTypeDef",
-    "InvokeWithResponseStreamRequestRequestTypeDef",
-    "LayerVersionContentInputTypeDef",
     "LayerVersionsListItemTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListCodeSigningConfigsRequestRequestTypeDef",
     "ListEventSourceMappingsRequestRequestTypeDef",
     "ListFunctionEventInvokeConfigsRequestRequestTypeDef",
     "ListFunctionUrlConfigsRequestRequestTypeDef",
@@ -146,15 +143,14 @@
     "PutProvisionedConcurrencyConfigRequestRequestTypeDef",
     "PutRuntimeManagementConfigRequestRequestTypeDef",
     "RemoveLayerVersionPermissionRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RuntimeVersionErrorTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateFunctionCodeRequestRequestTypeDef",
     "AddLayerVersionPermissionResponseTypeDef",
     "AddPermissionResponseTypeDef",
     "ConcurrencyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAccountSettingsResponseTypeDef",
     "GetFunctionCodeSigningConfigResponseTypeDef",
     "GetFunctionConcurrencyResponseTypeDef",
@@ -167,42 +163,51 @@
     "ListFunctionsByCodeSigningConfigResponseTypeDef",
     "ListTagsResponseTypeDef",
     "PutFunctionCodeSigningConfigResponseTypeDef",
     "PutProvisionedConcurrencyConfigResponseTypeDef",
     "PutRuntimeManagementConfigResponseTypeDef",
     "AliasConfigurationResponseTypeDef",
     "AliasConfigurationTypeDef",
+    "AliasRoutingConfigurationUnionTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
+    "AllowedPublishersUnionTypeDef",
+    "FunctionCodeTypeDef",
+    "InvocationRequestRequestTypeDef",
+    "InvokeAsyncRequestRequestTypeDef",
+    "InvokeWithResponseStreamRequestRequestTypeDef",
+    "LayerVersionContentInputTypeDef",
+    "UpdateFunctionCodeRequestRequestTypeDef",
     "CodeSigningConfigTypeDef",
     "CreateCodeSigningConfigRequestRequestTypeDef",
     "UpdateCodeSigningConfigRequestRequestTypeDef",
     "CreateFunctionUrlConfigResponseTypeDef",
     "FunctionUrlConfigTypeDef",
     "GetFunctionUrlConfigResponseTypeDef",
     "UpdateFunctionUrlConfigResponseTypeDef",
+    "CorsUnionTypeDef",
     "CreateFunctionUrlConfigRequestRequestTypeDef",
     "UpdateFunctionUrlConfigRequestRequestTypeDef",
-    "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionConfigurationRequestRequestTypeDef",
     "DestinationConfigTypeDef",
     "EnvironmentResponseTypeDef",
+    "SelfManagedEventSourceUnionTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "GetFunctionConfigurationRequestFunctionActiveWaitTypeDef",
     "GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef",
     "GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef",
     "GetFunctionRequestFunctionActiveV2WaitTypeDef",
     "GetFunctionRequestFunctionExistsWaitTypeDef",
     "GetFunctionRequestFunctionUpdatedV2WaitTypeDef",
     "GetLayerVersionResponseTypeDef",
     "PublishLayerVersionResponseTypeDef",
     "ImageConfigResponseTypeDef",
+    "ImageConfigUnionTypeDef",
     "InvokeWithResponseStreamResponseEventTypeDef",
-    "PublishLayerVersionRequestRequestTypeDef",
     "LayersListItemTypeDef",
     "ListLayerVersionsResponseTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
     "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
     "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
     "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
@@ -211,26 +216,29 @@
     "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
     "ListLayersRequestListLayersPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
     "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     "RuntimeVersionConfigTypeDef",
     "ListAliasesResponseTypeDef",
+    "CreateFunctionRequestRequestTypeDef",
+    "PublishLayerVersionRequestRequestTypeDef",
     "CreateCodeSigningConfigResponseTypeDef",
     "GetCodeSigningConfigResponseTypeDef",
     "ListCodeSigningConfigsResponseTypeDef",
     "UpdateCodeSigningConfigResponseTypeDef",
     "ListFunctionUrlConfigsResponseTypeDef",
     "FunctionEventInvokeConfigResponseTypeDef",
     "FunctionEventInvokeConfigTypeDef",
     "PutFunctionEventInvokeConfigRequestRequestTypeDef",
     "UpdateFunctionEventInvokeConfigRequestRequestTypeDef",
     "EventSourceMappingConfigurationResponseTypeDef",
     "EventSourceMappingConfigurationTypeDef",
     "CreateEventSourceMappingRequestRequestTypeDef",
+    "FilterCriteriaUnionTypeDef",
     "UpdateEventSourceMappingRequestRequestTypeDef",
     "InvokeWithResponseStreamResponseTypeDef",
     "ListLayersResponseTypeDef",
     "FunctionConfigurationResponseTypeDef",
     "FunctionConfigurationTypeDef",
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     "ListEventSourceMappingsResponseTypeDef",
@@ -358,14 +366,15 @@
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     {
         "ConsumerGroupId": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CodeSigningPoliciesTypeDef = TypedDict(
     "CodeSigningPoliciesTypeDef",
     {
         "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
     },
     total=False,
 )
@@ -443,14 +452,15 @@
     {
         "Type": SourceAccessTypeType,
         "URI": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "TargetArn": str,
     },
     total=False,
 )
@@ -474,26 +484,14 @@
     "FileSystemConfigTypeDef",
     {
         "Arn": str,
         "LocalMountPath": str,
     },
 )
 
-FunctionCodeTypeDef = TypedDict(
-    "FunctionCodeTypeDef",
-    {
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3ObjectVersion": str,
-        "ImageUri": str,
-    },
-    total=False,
-)
-
 ImageConfigTypeDef = TypedDict(
     "ImageConfigTypeDef",
     {
         "EntryPoint": Sequence[str],
         "Command": Sequence[str],
         "WorkingDirectory": str,
     },
@@ -947,45 +945,14 @@
         "EntryPoint": List[str],
         "Command": List[str],
         "WorkingDirectory": str,
     },
     total=False,
 )
 
-_RequiredInvocationRequestRequestTypeDef = TypedDict(
-    "_RequiredInvocationRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalInvocationRequestRequestTypeDef = TypedDict(
-    "_OptionalInvocationRequestRequestTypeDef",
-    {
-        "InvocationType": InvocationTypeType,
-        "LogType": LogTypeType,
-        "ClientContext": str,
-        "Payload": Union[str, bytes, IO[Any], StreamingBody],
-        "Qualifier": str,
-    },
-    total=False,
-)
-
-class InvocationRequestRequestTypeDef(
-    _RequiredInvocationRequestRequestTypeDef, _OptionalInvocationRequestRequestTypeDef
-):
-    pass
-
-InvokeAsyncRequestRequestTypeDef = TypedDict(
-    "InvokeAsyncRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-        "InvokeArgs": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 InvokeResponseStreamUpdateTypeDef = TypedDict(
     "InvokeResponseStreamUpdateTypeDef",
     {
         "Payload": bytes,
     },
     total=False,
 )
@@ -996,49 +963,14 @@
         "ErrorCode": str,
         "ErrorDetails": str,
         "LogResult": str,
     },
     total=False,
 )
 
-_RequiredInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
-    "_RequiredInvokeWithResponseStreamRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
-    "_OptionalInvokeWithResponseStreamRequestRequestTypeDef",
-    {
-        "InvocationType": ResponseStreamingInvocationTypeType,
-        "LogType": LogTypeType,
-        "ClientContext": str,
-        "Qualifier": str,
-        "Payload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class InvokeWithResponseStreamRequestRequestTypeDef(
-    _RequiredInvokeWithResponseStreamRequestRequestTypeDef,
-    _OptionalInvokeWithResponseStreamRequestRequestTypeDef,
-):
-    pass
-
-LayerVersionContentInputTypeDef = TypedDict(
-    "LayerVersionContentInputTypeDef",
-    {
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3ObjectVersion": str,
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 LayerVersionsListItemTypeDef = TypedDict(
     "LayerVersionsListItemTypeDef",
     {
         "LayerVersionArn": str,
         "Version": int,
         "Description": str,
         "CreatedDate": str,
@@ -1402,42 +1334,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateFunctionCodeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFunctionCodeRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalUpdateFunctionCodeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFunctionCodeRequestRequestTypeDef",
-    {
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3ObjectVersion": str,
-        "ImageUri": str,
-        "Publish": bool,
-        "DryRun": bool,
-        "RevisionId": str,
-        "Architectures": Sequence[ArchitectureType],
-    },
-    total=False,
-)
-
-class UpdateFunctionCodeRequestRequestTypeDef(
-    _RequiredUpdateFunctionCodeRequestRequestTypeDef,
-    _OptionalUpdateFunctionCodeRequestRequestTypeDef,
-):
-    pass
-
 AddLayerVersionPermissionResponseTypeDef = TypedDict(
     "AddLayerVersionPermissionResponseTypeDef",
     {
         "Statement": str,
         "RevisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1624,14 +1528,17 @@
         "Description": str,
         "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
         "RevisionId": str,
     },
     total=False,
 )
 
+AliasRoutingConfigurationUnionTypeDef = Union[
+    AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
+]
 _RequiredCreateAliasRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
         "FunctionVersion": str,
     },
@@ -1669,14 +1576,121 @@
 )
 
 class UpdateAliasRequestRequestTypeDef(
     _RequiredUpdateAliasRequestRequestTypeDef, _OptionalUpdateAliasRequestRequestTypeDef
 ):
     pass
 
+AllowedPublishersUnionTypeDef = Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef]
+FunctionCodeTypeDef = TypedDict(
+    "FunctionCodeTypeDef",
+    {
+        "ZipFile": BlobTypeDef,
+        "S3Bucket": str,
+        "S3Key": str,
+        "S3ObjectVersion": str,
+        "ImageUri": str,
+    },
+    total=False,
+)
+
+_RequiredInvocationRequestRequestTypeDef = TypedDict(
+    "_RequiredInvocationRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalInvocationRequestRequestTypeDef = TypedDict(
+    "_OptionalInvocationRequestRequestTypeDef",
+    {
+        "InvocationType": InvocationTypeType,
+        "LogType": LogTypeType,
+        "ClientContext": str,
+        "Payload": BlobTypeDef,
+        "Qualifier": str,
+    },
+    total=False,
+)
+
+class InvocationRequestRequestTypeDef(
+    _RequiredInvocationRequestRequestTypeDef, _OptionalInvocationRequestRequestTypeDef
+):
+    pass
+
+InvokeAsyncRequestRequestTypeDef = TypedDict(
+    "InvokeAsyncRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+        "InvokeArgs": BlobTypeDef,
+    },
+)
+
+_RequiredInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
+    "_RequiredInvokeWithResponseStreamRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
+    "_OptionalInvokeWithResponseStreamRequestRequestTypeDef",
+    {
+        "InvocationType": ResponseStreamingInvocationTypeType,
+        "LogType": LogTypeType,
+        "ClientContext": str,
+        "Qualifier": str,
+        "Payload": BlobTypeDef,
+    },
+    total=False,
+)
+
+class InvokeWithResponseStreamRequestRequestTypeDef(
+    _RequiredInvokeWithResponseStreamRequestRequestTypeDef,
+    _OptionalInvokeWithResponseStreamRequestRequestTypeDef,
+):
+    pass
+
+LayerVersionContentInputTypeDef = TypedDict(
+    "LayerVersionContentInputTypeDef",
+    {
+        "S3Bucket": str,
+        "S3Key": str,
+        "S3ObjectVersion": str,
+        "ZipFile": BlobTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUpdateFunctionCodeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFunctionCodeRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalUpdateFunctionCodeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFunctionCodeRequestRequestTypeDef",
+    {
+        "ZipFile": BlobTypeDef,
+        "S3Bucket": str,
+        "S3Key": str,
+        "S3ObjectVersion": str,
+        "ImageUri": str,
+        "Publish": bool,
+        "DryRun": bool,
+        "RevisionId": str,
+        "Architectures": Sequence[ArchitectureType],
+    },
+    total=False,
+)
+
+class UpdateFunctionCodeRequestRequestTypeDef(
+    _RequiredUpdateFunctionCodeRequestRequestTypeDef,
+    _OptionalUpdateFunctionCodeRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCodeSigningConfigTypeDef = TypedDict(
     "_RequiredCodeSigningConfigTypeDef",
     {
         "CodeSigningConfigId": str,
         "CodeSigningConfigArn": str,
         "AllowedPublishers": AllowedPublishersOutputTypeDef,
         "CodeSigningPolicies": CodeSigningPoliciesTypeDef,
@@ -1800,14 +1814,15 @@
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
 _RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "AuthType": FunctionUrlAuthTypeType,
     },
 )
@@ -1846,54 +1861,14 @@
 
 class UpdateFunctionUrlConfigRequestRequestTypeDef(
     _RequiredUpdateFunctionUrlConfigRequestRequestTypeDef,
     _OptionalUpdateFunctionUrlConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateFunctionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFunctionRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-        "Role": str,
-        "Code": FunctionCodeTypeDef,
-    },
-)
-_OptionalCreateFunctionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFunctionRequestRequestTypeDef",
-    {
-        "Runtime": RuntimeType,
-        "Handler": str,
-        "Description": str,
-        "Timeout": int,
-        "MemorySize": int,
-        "Publish": bool,
-        "VpcConfig": VpcConfigTypeDef,
-        "PackageType": PackageTypeType,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "Environment": EnvironmentTypeDef,
-        "KMSKeyArn": str,
-        "TracingConfig": TracingConfigTypeDef,
-        "Tags": Mapping[str, str],
-        "Layers": Sequence[str],
-        "FileSystemConfigs": Sequence[FileSystemConfigTypeDef],
-        "ImageConfig": ImageConfigTypeDef,
-        "CodeSigningConfigArn": str,
-        "Architectures": Sequence[ArchitectureType],
-        "EphemeralStorage": EphemeralStorageTypeDef,
-        "SnapStart": SnapStartTypeDef,
-    },
-    total=False,
-)
-
-class CreateFunctionRequestRequestTypeDef(
-    _RequiredCreateFunctionRequestRequestTypeDef, _OptionalCreateFunctionRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateFunctionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionConfigurationRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalUpdateFunctionConfigurationRequestRequestTypeDef = TypedDict(
@@ -1940,14 +1915,17 @@
     {
         "Variables": Dict[str, str],
         "Error": EnvironmentErrorTypeDef,
     },
     total=False,
 )
 
+SelfManagedEventSourceUnionTypeDef = Union[
+    SelfManagedEventSourceTypeDef, SelfManagedEventSourceOutputTypeDef
+]
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
         "Filters": List[FilterTypeDef],
     },
     total=False,
 )
@@ -2123,47 +2101,24 @@
     {
         "ImageConfig": ImageConfigOutputTypeDef,
         "Error": ImageConfigErrorTypeDef,
     },
     total=False,
 )
 
+ImageConfigUnionTypeDef = Union[ImageConfigTypeDef, ImageConfigOutputTypeDef]
 InvokeWithResponseStreamResponseEventTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseEventTypeDef",
     {
         "PayloadChunk": InvokeResponseStreamUpdateTypeDef,
         "InvokeComplete": InvokeWithResponseStreamCompleteEventTypeDef,
     },
     total=False,
 )
 
-_RequiredPublishLayerVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredPublishLayerVersionRequestRequestTypeDef",
-    {
-        "LayerName": str,
-        "Content": LayerVersionContentInputTypeDef,
-    },
-)
-_OptionalPublishLayerVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalPublishLayerVersionRequestRequestTypeDef",
-    {
-        "Description": str,
-        "CompatibleRuntimes": Sequence[RuntimeType],
-        "LicenseInfo": str,
-        "CompatibleArchitectures": Sequence[ArchitectureType],
-    },
-    total=False,
-)
-
-class PublishLayerVersionRequestRequestTypeDef(
-    _RequiredPublishLayerVersionRequestRequestTypeDef,
-    _OptionalPublishLayerVersionRequestRequestTypeDef,
-):
-    pass
-
 LayersListItemTypeDef = TypedDict(
     "LayersListItemTypeDef",
     {
         "LayerName": str,
         "LayerArn": str,
         "LatestMatchingVersion": LayerVersionsListItemTypeDef,
     },
@@ -2383,14 +2338,78 @@
     {
         "NextMarker": str,
         "Aliases": List[AliasConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateFunctionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFunctionRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+        "Role": str,
+        "Code": FunctionCodeTypeDef,
+    },
+)
+_OptionalCreateFunctionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFunctionRequestRequestTypeDef",
+    {
+        "Runtime": RuntimeType,
+        "Handler": str,
+        "Description": str,
+        "Timeout": int,
+        "MemorySize": int,
+        "Publish": bool,
+        "VpcConfig": VpcConfigTypeDef,
+        "PackageType": PackageTypeType,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
+        "Environment": EnvironmentTypeDef,
+        "KMSKeyArn": str,
+        "TracingConfig": TracingConfigTypeDef,
+        "Tags": Mapping[str, str],
+        "Layers": Sequence[str],
+        "FileSystemConfigs": Sequence[FileSystemConfigTypeDef],
+        "ImageConfig": ImageConfigTypeDef,
+        "CodeSigningConfigArn": str,
+        "Architectures": Sequence[ArchitectureType],
+        "EphemeralStorage": EphemeralStorageTypeDef,
+        "SnapStart": SnapStartTypeDef,
+    },
+    total=False,
+)
+
+class CreateFunctionRequestRequestTypeDef(
+    _RequiredCreateFunctionRequestRequestTypeDef, _OptionalCreateFunctionRequestRequestTypeDef
+):
+    pass
+
+_RequiredPublishLayerVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishLayerVersionRequestRequestTypeDef",
+    {
+        "LayerName": str,
+        "Content": LayerVersionContentInputTypeDef,
+    },
+)
+_OptionalPublishLayerVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishLayerVersionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "CompatibleRuntimes": Sequence[RuntimeType],
+        "LicenseInfo": str,
+        "CompatibleArchitectures": Sequence[ArchitectureType],
+    },
+    total=False,
+)
+
+class PublishLayerVersionRequestRequestTypeDef(
+    _RequiredPublishLayerVersionRequestRequestTypeDef,
+    _OptionalPublishLayerVersionRequestRequestTypeDef,
+):
+    pass
+
 CreateCodeSigningConfigResponseTypeDef = TypedDict(
     "CreateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2579,15 +2598,15 @@
         "EventSourceArn": str,
         "Enabled": bool,
         "BatchSize": int,
         "FilterCriteria": FilterCriteriaTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "ParallelizationFactor": int,
         "StartingPosition": EventSourcePositionType,
-        "StartingPositionTimestamp": Union[datetime, str],
+        "StartingPositionTimestamp": TimestampTypeDef,
         "DestinationConfig": DestinationConfigTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "Topics": Sequence[str],
         "Queues": Sequence[str],
@@ -2604,14 +2623,15 @@
 
 class CreateEventSourceMappingRequestRequestTypeDef(
     _RequiredCreateEventSourceMappingRequestRequestTypeDef,
     _OptionalCreateEventSourceMappingRequestRequestTypeDef,
 ):
     pass
 
+FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
 _RequiredUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventSourceMappingRequestRequestTypeDef",
     {
         "UUID": str,
     },
 )
 _OptionalUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/waiter.py` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/waiter.pyi` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/PKG-INFO` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Lambda 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lambda type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lambda type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
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
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -76,15 +76,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -449,47 +449,48 @@
 )
 
 
 def check_value(value: ArchitectureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lambda.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lambda.type_defs import (
     AccountLimitTypeDef,
     AccountUsageTypeDef,
     AddLayerVersionPermissionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AddPermissionRequestRequestTypeDef,
     AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
+    BlobTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyTypeDef,
     CorsOutputTypeDef,
     CorsTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SourceAccessConfigurationTypeDef,
+    TimestampTypeDef,
     DeadLetterConfigTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     FileSystemConfigTypeDef,
-    FunctionCodeTypeDef,
     ImageConfigTypeDef,
     SnapStartTypeDef,
     TracingConfigTypeDef,
     VpcConfigTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCodeSigningConfigRequestRequestTypeDef,
     DeleteEventSourceMappingRequestRequestTypeDef,
@@ -525,20 +526,16 @@
     GetLayerVersionRequestRequestTypeDef,
     LayerVersionContentOutputTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProvisionedConcurrencyConfigRequestRequestTypeDef,
     GetRuntimeManagementConfigRequestRequestTypeDef,
     ImageConfigErrorTypeDef,
     ImageConfigOutputTypeDef,
-    InvocationRequestRequestTypeDef,
-    InvokeAsyncRequestRequestTypeDef,
     InvokeResponseStreamUpdateTypeDef,
     InvokeWithResponseStreamCompleteEventTypeDef,
-    InvokeWithResponseStreamRequestRequestTypeDef,
-    LayerVersionContentInputTypeDef,
     LayerVersionsListItemTypeDef,
     PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListCodeSigningConfigsRequestRequestTypeDef,
     ListEventSourceMappingsRequestRequestTypeDef,
     ListFunctionEventInvokeConfigsRequestRequestTypeDef,
     ListFunctionUrlConfigsRequestRequestTypeDef,
@@ -556,15 +553,14 @@
     PutProvisionedConcurrencyConfigRequestRequestTypeDef,
     PutRuntimeManagementConfigRequestRequestTypeDef,
     RemoveLayerVersionPermissionRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RuntimeVersionErrorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateFunctionCodeRequestRequestTypeDef,
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
     ConcurrencyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyResponseTypeDef,
@@ -577,42 +573,51 @@
     ListFunctionsByCodeSigningConfigResponseTypeDef,
     ListTagsResponseTypeDef,
     PutFunctionCodeSigningConfigResponseTypeDef,
     PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigResponseTypeDef,
     AliasConfigurationResponseTypeDef,
     AliasConfigurationTypeDef,
+    AliasRoutingConfigurationUnionTypeDef,
     CreateAliasRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
+    AllowedPublishersUnionTypeDef,
+    FunctionCodeTypeDef,
+    InvocationRequestRequestTypeDef,
+    InvokeAsyncRequestRequestTypeDef,
+    InvokeWithResponseStreamRequestRequestTypeDef,
+    LayerVersionContentInputTypeDef,
+    UpdateFunctionCodeRequestRequestTypeDef,
     CodeSigningConfigTypeDef,
     CreateCodeSigningConfigRequestRequestTypeDef,
     UpdateCodeSigningConfigRequestRequestTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     FunctionUrlConfigTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
+    CorsUnionTypeDef,
     CreateFunctionUrlConfigRequestRequestTypeDef,
     UpdateFunctionUrlConfigRequestRequestTypeDef,
-    CreateFunctionRequestRequestTypeDef,
     UpdateFunctionConfigurationRequestRequestTypeDef,
     DestinationConfigTypeDef,
     EnvironmentResponseTypeDef,
+    SelfManagedEventSourceUnionTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     GetFunctionConfigurationRequestFunctionActiveWaitTypeDef,
     GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef,
     GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef,
     GetFunctionRequestFunctionActiveV2WaitTypeDef,
     GetFunctionRequestFunctionExistsWaitTypeDef,
     GetFunctionRequestFunctionUpdatedV2WaitTypeDef,
     GetLayerVersionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     ImageConfigResponseTypeDef,
+    ImageConfigUnionTypeDef,
     InvokeWithResponseStreamResponseEventTypeDef,
-    PublishLayerVersionRequestRequestTypeDef,
     LayersListItemTypeDef,
     ListLayerVersionsResponseTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
     ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
     ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
     ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
@@ -621,40 +626,43 @@
     ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
     ListLayersRequestListLayersPaginateTypeDef,
     ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
     ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListProvisionedConcurrencyConfigsResponseTypeDef,
     RuntimeVersionConfigTypeDef,
     ListAliasesResponseTypeDef,
+    CreateFunctionRequestRequestTypeDef,
+    PublishLayerVersionRequestRequestTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     ListFunctionUrlConfigsResponseTypeDef,
     FunctionEventInvokeConfigResponseTypeDef,
     FunctionEventInvokeConfigTypeDef,
     PutFunctionEventInvokeConfigRequestRequestTypeDef,
     UpdateFunctionEventInvokeConfigRequestRequestTypeDef,
     EventSourceMappingConfigurationResponseTypeDef,
     EventSourceMappingConfigurationTypeDef,
     CreateEventSourceMappingRequestRequestTypeDef,
+    FilterCriteriaUnionTypeDef,
     UpdateEventSourceMappingRequestRequestTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     ListLayersResponseTypeDef,
     FunctionConfigurationResponseTypeDef,
     FunctionConfigurationTypeDef,
     ListFunctionEventInvokeConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
     GetFunctionResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
 )
 
 
-def get_structure() -> AccountLimitTypeDef:
+def get_value() -> AccountLimitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/SOURCES.txt` & `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15.post1/setup.py` & `mypy-boto3-lambda-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lambda",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_lambda"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Lambda 1.28.16 service generated with mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -33,15 +33,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 lambda type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 lambda type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_lambda": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

