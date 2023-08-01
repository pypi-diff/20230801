# Comparing `tmp/mypy-boto3-appsync-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-appsync-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appsync-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
+gzip compressed data, was "mypy-boto3-appsync-1.28.16.tar", last modified: Tue Aug  1 11:36:15 2023, max compression
```

## Comparing `mypy-boto3-appsync-1.28.15.post1.tar` & `mypy-boto3-appsync-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.313020 mypy-boto3-appsync-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-07-29 10:02:34.305020 mypy-boto3-appsync-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.305020 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43595 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43521 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57726 2023-07-29 09:38:36.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57641 2023-07-29 09:38:36.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.305020 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.313020 mypy-boto3-appsync-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.080945 mypy-boto3-appsync-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-08-01 11:36:15.080945 mypy-boto3-appsync-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.068945 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43350 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43276 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-08-01 11:11:07.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-08-01 11:11:06.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58007 2023-08-01 11:11:08.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57922 2023-08-01 11:11:07.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.080945 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-08-01 11:36:14.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:36:14.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:14.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:14.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:14.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:36:14.000000 mypy-boto3-appsync-1.28.16/mypy_boto3_appsync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:15.080945 mypy-boto3-appsync-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:11:05.000000 mypy-boto3-appsync-1.28.16/setup.py
```

### Comparing `mypy-boto3-appsync-1.28.15.post1/LICENSE` & `mypy-boto3-appsync-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15.post1/PKG-INFO` & `mypy-boto3-appsync-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppSync 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppSync 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appsync type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appsync type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appsync)](https://pepy.tech/project/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
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
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
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
@@ -353,34 +353,35 @@
 )
 
 
 def check_value(value: ApiCacheStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appsync.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appsync.type_defs import (
     CognitoUserPoolConfigTypeDef,
     LambdaAuthorizerConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     ApiAssociationTypeDef,
     ApiCacheTypeDef,
     ApiKeyTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SourceApiAssociationConfigTypeDef,
     AwsIamConfigTypeDef,
+    BlobTypeDef,
     CachingConfigOutputTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EventBridgeDataSourceConfigTypeDef,
@@ -431,15 +432,14 @@
     ListSourceApiAssociationsRequestRequestTypeDef,
     SourceApiAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTypesByAssociationRequestRequestTypeDef,
     ListTypesRequestRequestTypeDef,
     PipelineConfigOutputTypeDef,
     RdsHttpEndpointConfigTypeDef,
-    StartSchemaCreationRequestRequestTypeDef,
     StartSchemaMergeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiCacheRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     UpdateTypeRequestRequestTypeDef,
@@ -461,14 +461,16 @@
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
     AssociateMergedGraphqlApiRequestRequestTypeDef,
     AssociateSourceGraphqlApiRequestRequestTypeDef,
     SourceApiAssociationTypeDef,
     UpdateSourceApiAssociationRequestRequestTypeDef,
     AuthorizationConfigTypeDef,
+    StartSchemaCreationRequestRequestTypeDef,
+    CachingConfigUnionTypeDef,
     CodeErrorTypeDef,
     CreateDomainNameResponseTypeDef,
     GetDomainNameResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateTypeResponseTypeDef,
     GetTypeResponseTypeDef,
@@ -482,14 +484,15 @@
     ListDataSourcesRequestListDataSourcesPaginateTypeDef,
     ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
     ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
     ListResolversRequestListResolversPaginateTypeDef,
     ListTypesRequestListTypesPaginateTypeDef,
     ListSourceApiAssociationsResponseTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     CreateGraphqlApiRequestRequestTypeDef,
     GraphqlApiTypeDef,
     UpdateGraphqlApiRequestRequestTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     GetSourceApiAssociationResponseTypeDef,
@@ -522,15 +525,15 @@
     CreateDataSourceResponseTypeDef,
     GetDataSourceResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     UpdateDataSourceResponseTypeDef,
 )
 
 
-def get_structure() -> CognitoUserPoolConfigTypeDef:
+def get_value() -> CognitoUserPoolConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appsync-1.28.15.post1/README.md` & `mypy-boto3-appsync-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appsync)](https://pepy.tech/project/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
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
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
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
@@ -321,34 +321,35 @@
 )
 
 
 def check_value(value: ApiCacheStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appsync.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appsync.type_defs import (
     CognitoUserPoolConfigTypeDef,
     LambdaAuthorizerConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     ApiAssociationTypeDef,
     ApiCacheTypeDef,
     ApiKeyTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SourceApiAssociationConfigTypeDef,
     AwsIamConfigTypeDef,
+    BlobTypeDef,
     CachingConfigOutputTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EventBridgeDataSourceConfigTypeDef,
@@ -399,15 +400,14 @@
     ListSourceApiAssociationsRequestRequestTypeDef,
     SourceApiAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTypesByAssociationRequestRequestTypeDef,
     ListTypesRequestRequestTypeDef,
     PipelineConfigOutputTypeDef,
     RdsHttpEndpointConfigTypeDef,
-    StartSchemaCreationRequestRequestTypeDef,
     StartSchemaMergeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiCacheRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     UpdateTypeRequestRequestTypeDef,
@@ -429,14 +429,16 @@
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
     AssociateMergedGraphqlApiRequestRequestTypeDef,
     AssociateSourceGraphqlApiRequestRequestTypeDef,
     SourceApiAssociationTypeDef,
     UpdateSourceApiAssociationRequestRequestTypeDef,
     AuthorizationConfigTypeDef,
+    StartSchemaCreationRequestRequestTypeDef,
+    CachingConfigUnionTypeDef,
     CodeErrorTypeDef,
     CreateDomainNameResponseTypeDef,
     GetDomainNameResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateTypeResponseTypeDef,
     GetTypeResponseTypeDef,
@@ -450,14 +452,15 @@
     ListDataSourcesRequestListDataSourcesPaginateTypeDef,
     ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
     ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
     ListResolversRequestListResolversPaginateTypeDef,
     ListTypesRequestListTypesPaginateTypeDef,
     ListSourceApiAssociationsResponseTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     CreateGraphqlApiRequestRequestTypeDef,
     GraphqlApiTypeDef,
     UpdateGraphqlApiRequestRequestTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     GetSourceApiAssociationResponseTypeDef,
@@ -490,15 +493,15 @@
     CreateDataSourceResponseTypeDef,
     GetDataSourceResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     UpdateDataSourceResponseTypeDef,
 )
 
 
-def get_structure() -> CognitoUserPoolConfigTypeDef:
+def get_value() -> CognitoUserPoolConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__init__.py` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__init__.pyi` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__main__.py` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppSync 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AppSync 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync\nOther"
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

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/client.py` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_appsync.client import AppSyncClient
 
     session = Session()
     client: AppSyncClient = session.client("appsync")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ApiCacheTypeType,
     ApiCachingBehaviorType,
     AuthenticationTypeType,
     DataSourceTypeType,
     GraphQLApiTypeType,
@@ -42,16 +41,16 @@
 )
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
-    CachingConfigOutputTypeDef,
-    CachingConfigTypeDef,
+    BlobTypeDef,
+    CachingConfigUnionTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
@@ -87,16 +86,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
-    PipelineConfigOutputTypeDef,
-    PipelineConfigTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
@@ -327,17 +325,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef] = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: Union[CachingConfigTypeDef, CachingConfigOutputTypeDef] = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
@@ -708,15 +706,15 @@
         Lists `Type` objects by the source API association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types_by_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_types_by_association)
         """
 
     def start_schema_creation(
-        self, *, apiId: str, definition: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, apiId: str, definition: BlobTypeDef
     ) -> StartSchemaCreationResponseTypeDef:
         """
         Adds a new schema to your GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_creation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#start_schema_creation)
         """
@@ -856,17 +854,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef] = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: Union[CachingConfigTypeDef, CachingConfigOutputTypeDef] = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/client.pyi` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_appsync.client import AppSyncClient
 
     session = Session()
     client: AppSyncClient = session.client("appsync")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ApiCacheTypeType,
     ApiCachingBehaviorType,
     AuthenticationTypeType,
     DataSourceTypeType,
     GraphQLApiTypeType,
@@ -42,16 +41,16 @@
 )
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
-    CachingConfigOutputTypeDef,
-    CachingConfigTypeDef,
+    BlobTypeDef,
+    CachingConfigUnionTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
@@ -87,16 +86,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
-    PipelineConfigOutputTypeDef,
-    PipelineConfigTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
@@ -311,17 +309,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef] = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: Union[CachingConfigTypeDef, CachingConfigOutputTypeDef] = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
@@ -653,15 +651,15 @@
         """
         Lists `Type` objects by the source API association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types_by_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_types_by_association)
         """
     def start_schema_creation(
-        self, *, apiId: str, definition: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, apiId: str, definition: BlobTypeDef
     ) -> StartSchemaCreationResponseTypeDef:
         """
         Adds a new schema to your GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_creation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#start_schema_creation)
         """
@@ -791,17 +789,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef] = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: Union[CachingConfigTypeDef, CachingConfigOutputTypeDef] = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/literals.py` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/literals.pyi` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/paginator.py` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/paginator.pyi` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/type_defs.py` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appsync.type_defs import CognitoUserPoolConfigTypeDef
 
-    data: CognitoUserPoolConfigTypeDef = {...}
+    data: CognitoUserPoolConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -57,14 +57,15 @@
     "ApiCacheTypeDef",
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
+    "BlobTypeDef",
     "CachingConfigOutputTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
@@ -115,15 +116,14 @@
     "ListSourceApiAssociationsRequestRequestTypeDef",
     "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTypesByAssociationRequestRequestTypeDef",
     "ListTypesRequestRequestTypeDef",
     "PipelineConfigOutputTypeDef",
     "RdsHttpEndpointConfigTypeDef",
-    "StartSchemaCreationRequestRequestTypeDef",
     "StartSchemaMergeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "UpdateTypeRequestRequestTypeDef",
@@ -145,14 +145,16 @@
     "UpdateApiCacheResponseTypeDef",
     "UpdateApiKeyResponseTypeDef",
     "AssociateMergedGraphqlApiRequestRequestTypeDef",
     "AssociateSourceGraphqlApiRequestRequestTypeDef",
     "SourceApiAssociationTypeDef",
     "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
+    "StartSchemaCreationRequestRequestTypeDef",
+    "CachingConfigUnionTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
@@ -166,14 +168,15 @@
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversRequestListResolversPaginateTypeDef",
     "ListTypesRequestListTypesPaginateTypeDef",
     "ListSourceApiAssociationsResponseTypeDef",
+    "PipelineConfigUnionTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
     "AssociateMergedGraphqlApiResponseTypeDef",
     "AssociateSourceGraphqlApiResponseTypeDef",
     "GetSourceApiAssociationResponseTypeDef",
@@ -351,14 +354,15 @@
     {
         "signingRegion": str,
         "signingServiceName": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCachingConfigOutputTypeDef = TypedDict(
     "_RequiredCachingConfigOutputTypeDef",
     {
         "ttl": int,
     },
 )
 _OptionalCachingConfigOutputTypeDef = TypedDict(
@@ -1063,22 +1067,14 @@
         "databaseName": str,
         "schema": str,
         "awsSecretStoreArn": str,
     },
     total=False,
 )
 
-StartSchemaCreationRequestRequestTypeDef = TypedDict(
-    "StartSchemaCreationRequestRequestTypeDef",
-    {
-        "apiId": str,
-        "definition": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 StartSchemaMergeRequestRequestTypeDef = TypedDict(
     "StartSchemaMergeRequestRequestTypeDef",
     {
         "associationId": str,
         "mergedApiIdentifier": str,
     },
 )
@@ -1439,14 +1435,23 @@
 
 class AuthorizationConfigTypeDef(
     _RequiredAuthorizationConfigTypeDef, _OptionalAuthorizationConfigTypeDef
 ):
     pass
 
 
+StartSchemaCreationRequestRequestTypeDef = TypedDict(
+    "StartSchemaCreationRequestRequestTypeDef",
+    {
+        "apiId": str,
+        "definition": BlobTypeDef,
+    },
+)
+
+CachingConfigUnionTypeDef = Union[CachingConfigTypeDef, CachingConfigOutputTypeDef]
 CodeErrorTypeDef = TypedDict(
     "CodeErrorTypeDef",
     {
         "errorType": str,
         "value": str,
         "location": CodeErrorLocationTypeDef,
     },
@@ -1722,14 +1727,15 @@
     {
         "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PipelineConfigUnionTypeDef = Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef]
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
     "RelationalDatabaseDataSourceConfigTypeDef",
     {
         "relationalDatabaseSourceType": Literal["RDS_HTTP_ENDPOINT"],
         "rdsHttpEndpointConfig": RdsHttpEndpointConfigTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/type_defs.pyi` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appsync.type_defs import CognitoUserPoolConfigTypeDef
 
-    data: CognitoUserPoolConfigTypeDef = {...}
+    data: CognitoUserPoolConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -56,14 +56,15 @@
     "ApiCacheTypeDef",
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
+    "BlobTypeDef",
     "CachingConfigOutputTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
@@ -114,15 +115,14 @@
     "ListSourceApiAssociationsRequestRequestTypeDef",
     "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTypesByAssociationRequestRequestTypeDef",
     "ListTypesRequestRequestTypeDef",
     "PipelineConfigOutputTypeDef",
     "RdsHttpEndpointConfigTypeDef",
-    "StartSchemaCreationRequestRequestTypeDef",
     "StartSchemaMergeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "UpdateTypeRequestRequestTypeDef",
@@ -144,14 +144,16 @@
     "UpdateApiCacheResponseTypeDef",
     "UpdateApiKeyResponseTypeDef",
     "AssociateMergedGraphqlApiRequestRequestTypeDef",
     "AssociateSourceGraphqlApiRequestRequestTypeDef",
     "SourceApiAssociationTypeDef",
     "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
+    "StartSchemaCreationRequestRequestTypeDef",
+    "CachingConfigUnionTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
@@ -165,14 +167,15 @@
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversRequestListResolversPaginateTypeDef",
     "ListTypesRequestListTypesPaginateTypeDef",
     "ListSourceApiAssociationsResponseTypeDef",
+    "PipelineConfigUnionTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
     "AssociateMergedGraphqlApiResponseTypeDef",
     "AssociateSourceGraphqlApiResponseTypeDef",
     "GetSourceApiAssociationResponseTypeDef",
@@ -344,14 +347,15 @@
     {
         "signingRegion": str,
         "signingServiceName": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCachingConfigOutputTypeDef = TypedDict(
     "_RequiredCachingConfigOutputTypeDef",
     {
         "ttl": int,
     },
 )
 _OptionalCachingConfigOutputTypeDef = TypedDict(
@@ -1024,22 +1028,14 @@
         "databaseName": str,
         "schema": str,
         "awsSecretStoreArn": str,
     },
     total=False,
 )
 
-StartSchemaCreationRequestRequestTypeDef = TypedDict(
-    "StartSchemaCreationRequestRequestTypeDef",
-    {
-        "apiId": str,
-        "definition": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 StartSchemaMergeRequestRequestTypeDef = TypedDict(
     "StartSchemaMergeRequestRequestTypeDef",
     {
         "associationId": str,
         "mergedApiIdentifier": str,
     },
 )
@@ -1384,14 +1380,23 @@
 )
 
 class AuthorizationConfigTypeDef(
     _RequiredAuthorizationConfigTypeDef, _OptionalAuthorizationConfigTypeDef
 ):
     pass
 
+StartSchemaCreationRequestRequestTypeDef = TypedDict(
+    "StartSchemaCreationRequestRequestTypeDef",
+    {
+        "apiId": str,
+        "definition": BlobTypeDef,
+    },
+)
+
+CachingConfigUnionTypeDef = Union[CachingConfigTypeDef, CachingConfigOutputTypeDef]
 CodeErrorTypeDef = TypedDict(
     "CodeErrorTypeDef",
     {
         "errorType": str,
         "value": str,
         "location": CodeErrorLocationTypeDef,
     },
@@ -1653,14 +1658,15 @@
     {
         "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PipelineConfigUnionTypeDef = Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef]
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
     "RelationalDatabaseDataSourceConfigTypeDef",
     {
         "relationalDatabaseSourceType": Literal["RDS_HTTP_ENDPOINT"],
         "rdsHttpEndpointConfig": RdsHttpEndpointConfigTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/PKG-INFO` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppSync 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppSync 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appsync type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appsync type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appsync)](https://pepy.tech/project/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
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
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
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
@@ -353,34 +353,35 @@
 )
 
 
 def check_value(value: ApiCacheStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appsync.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appsync.type_defs import (
     CognitoUserPoolConfigTypeDef,
     LambdaAuthorizerConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     ApiAssociationTypeDef,
     ApiCacheTypeDef,
     ApiKeyTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SourceApiAssociationConfigTypeDef,
     AwsIamConfigTypeDef,
+    BlobTypeDef,
     CachingConfigOutputTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EventBridgeDataSourceConfigTypeDef,
@@ -431,15 +432,14 @@
     ListSourceApiAssociationsRequestRequestTypeDef,
     SourceApiAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTypesByAssociationRequestRequestTypeDef,
     ListTypesRequestRequestTypeDef,
     PipelineConfigOutputTypeDef,
     RdsHttpEndpointConfigTypeDef,
-    StartSchemaCreationRequestRequestTypeDef,
     StartSchemaMergeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiCacheRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     UpdateTypeRequestRequestTypeDef,
@@ -461,14 +461,16 @@
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
     AssociateMergedGraphqlApiRequestRequestTypeDef,
     AssociateSourceGraphqlApiRequestRequestTypeDef,
     SourceApiAssociationTypeDef,
     UpdateSourceApiAssociationRequestRequestTypeDef,
     AuthorizationConfigTypeDef,
+    StartSchemaCreationRequestRequestTypeDef,
+    CachingConfigUnionTypeDef,
     CodeErrorTypeDef,
     CreateDomainNameResponseTypeDef,
     GetDomainNameResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateTypeResponseTypeDef,
     GetTypeResponseTypeDef,
@@ -482,14 +484,15 @@
     ListDataSourcesRequestListDataSourcesPaginateTypeDef,
     ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
     ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
     ListResolversRequestListResolversPaginateTypeDef,
     ListTypesRequestListTypesPaginateTypeDef,
     ListSourceApiAssociationsResponseTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     CreateGraphqlApiRequestRequestTypeDef,
     GraphqlApiTypeDef,
     UpdateGraphqlApiRequestRequestTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     GetSourceApiAssociationResponseTypeDef,
@@ -522,15 +525,15 @@
     CreateDataSourceResponseTypeDef,
     GetDataSourceResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     UpdateDataSourceResponseTypeDef,
 )
 
 
-def get_structure() -> CognitoUserPoolConfigTypeDef:
+def get_value() -> CognitoUserPoolConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/SOURCES.txt` & `mypy-boto3-appsync-1.28.16/mypy_boto3_appsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15.post1/setup.py` & `mypy-boto3-appsync-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appsync",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_appsync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppSync 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.AppSync 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 appsync type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 appsync type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_appsync": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

