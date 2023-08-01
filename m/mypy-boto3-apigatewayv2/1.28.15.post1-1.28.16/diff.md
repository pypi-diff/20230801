# Comparing `tmp/mypy-boto3-apigatewayv2-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-apigatewayv2-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigatewayv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:27 2023, max compression
+gzip compressed data, was "mypy-boto3-apigatewayv2-1.28.16.tar", last modified: Tue Aug  1 11:36:08 2023, max compression
```

## Comparing `mypy-boto3-apigatewayv2-1.28.15.post1.tar` & `mypy-boto3-apigatewayv2-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.800994 mypy-boto3-apigatewayv2-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20585 2023-07-29 10:02:27.800994 mypy-boto3-apigatewayv2-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19072 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.780993 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52061 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51972 2023-07-29 09:37:58.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    76448 2023-07-29 09:38:02.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    76337 2023-07-29 09:38:00.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.800994 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20585 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:27.800994 mypy-boto3-apigatewayv2-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.456956 mypy-boto3-apigatewayv2-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-08-01 11:36:08.456956 mypy-boto3-apigatewayv2-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.444956 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51737 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51648 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76754 2023-08-01 11:10:32.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76644 2023-08-01 11:10:31.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:29.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.456956 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-08-01 11:36:08.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:36:08.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:08.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:08.000000 mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:08.456956 mypy-boto3-apigatewayv2-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:10:28.000000 mypy-boto3-apigatewayv2-1.28.16/setup.py
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/LICENSE` & `mypy-boto3-apigatewayv2-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/PKG-INFO` & `mypy-boto3-apigatewayv2-1.28.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewayv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApiGatewayV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 apigatewayv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 apigatewayv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewayv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewayv2)](https://pepy.tech/project/mypy-boto3-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[boto3.ApiGatewayV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
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
@@ -359,35 +359,34 @@
 )
 
 
 def check_value(value: AuthorizationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_apigatewayv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_apigatewayv2.type_defs import (
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
     CorsOutputTypeDef,
     JWTConfigurationOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    DomainNameConfigurationOutputTypeDef,
-    DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
     ParameterConstraintsTypeDef,
     RouteSettingsTypeDef,
@@ -405,14 +404,15 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
+    TimestampTypeDef,
     ExportApiRequestRequestTypeDef,
     GetApiMappingRequestRequestTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
@@ -448,14 +448,15 @@
     UpdateApiMappingRequestRequestTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
     ApiTypeDef,
     AuthorizerTypeDef,
+    CorsUnionTypeDef,
     CreateApiRequestRequestTypeDef,
     UpdateApiRequestRequestTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
@@ -479,17 +480,16 @@
     UpdateApiResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
     UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseResponseTypeDef,
     UpdateModelResponseTypeDef,
     UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
+    JWTConfigurationUnionTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    CreateDomainNameRequestRequestTypeDef,
-    UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateIntegrationRequestRequestTypeDef,
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
@@ -511,14 +511,15 @@
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
     UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    DomainNameConfigurationTypeDef,
     GetApisRequestGetApisPaginateTypeDef,
     GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetModelsRequestGetModelsPaginateTypeDef,
@@ -531,18 +532,21 @@
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
+    DomainNameConfigurationUnionTypeDef,
+    CreateDomainNameRequestRequestTypeDef,
+    UpdateDomainNameRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsTypeDef:
+def get_value() -> AccessLogSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/README.md` & `mypy-boto3-apigatewayv2-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewayv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewayv2)](https://pepy.tech/project/mypy-boto3-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[boto3.ApiGatewayV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
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
@@ -327,35 +327,34 @@
 )
 
 
 def check_value(value: AuthorizationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_apigatewayv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_apigatewayv2.type_defs import (
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
     CorsOutputTypeDef,
     JWTConfigurationOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    DomainNameConfigurationOutputTypeDef,
-    DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
     ParameterConstraintsTypeDef,
     RouteSettingsTypeDef,
@@ -373,14 +372,15 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
+    TimestampTypeDef,
     ExportApiRequestRequestTypeDef,
     GetApiMappingRequestRequestTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
@@ -416,14 +416,15 @@
     UpdateApiMappingRequestRequestTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
     ApiTypeDef,
     AuthorizerTypeDef,
+    CorsUnionTypeDef,
     CreateApiRequestRequestTypeDef,
     UpdateApiRequestRequestTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
@@ -447,17 +448,16 @@
     UpdateApiResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
     UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseResponseTypeDef,
     UpdateModelResponseTypeDef,
     UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
+    JWTConfigurationUnionTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    CreateDomainNameRequestRequestTypeDef,
-    UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateIntegrationRequestRequestTypeDef,
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
@@ -479,14 +479,15 @@
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
     UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    DomainNameConfigurationTypeDef,
     GetApisRequestGetApisPaginateTypeDef,
     GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetModelsRequestGetModelsPaginateTypeDef,
@@ -499,18 +500,21 @@
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
+    DomainNameConfigurationUnionTypeDef,
+    CreateDomainNameRequestRequestTypeDef,
+    UpdateDomainNameRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsTypeDef:
+def get_value() -> AccessLogSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__init__.py` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__init__.pyi` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__main__.py` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApiGatewayV2 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ApiGatewayV2 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2\nOther"
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

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/client.py` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_apigatewayv2.client import ApiGatewayV2Client
 
     session = Session()
     client: ApiGatewayV2Client = session.client("apigatewayv2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthorizationTypeType,
     AuthorizerTypeType,
     ConnectionTypeType,
@@ -38,30 +38,28 @@
     GetModelsPaginator,
     GetRouteResponsesPaginator,
     GetRoutesPaginator,
     GetStagesPaginator,
 )
 from .type_defs import (
     AccessLogSettingsTypeDef,
-    CorsOutputTypeDef,
-    CorsTypeDef,
+    CorsUnionTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
     CreateIntegrationResultTypeDef,
     CreateModelResponseTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     CreateStageResponseTypeDef,
     CreateVpcLinkResponseTypeDef,
-    DomainNameConfigurationOutputTypeDef,
-    DomainNameConfigurationTypeDef,
+    DomainNameConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportApiResponseTypeDef,
     GetApiMappingResponseTypeDef,
     GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizerResponseTypeDef,
@@ -83,16 +81,15 @@
     GetRoutesResponseTypeDef,
     GetStageResponseTypeDef,
     GetStagesResponseTypeDef,
     GetTagsResponseTypeDef,
     GetVpcLinkResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     ImportApiResponseTypeDef,
-    JWTConfigurationOutputTypeDef,
-    JWTConfigurationTypeDef,
+    JWTConfigurationUnionTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     ParameterConstraintsTypeDef,
     ReimportApiResponseTypeDef,
     RouteSettingsTypeDef,
     TlsConfigInputTypeDef,
     UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
@@ -169,15 +166,15 @@
 
     def create_api(
         self,
         *,
         Name: str,
         ProtocolType: ProtocolTypeType,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
+        CorsConfiguration: CorsUnionTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -210,15 +207,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef] = ...
+        JwtConfiguration: JWTConfigurationUnionTypeDef = ...
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#create_authorizer)
         """
@@ -233,17 +230,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#create_deployment)
         """
 
     def create_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[
-            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
-        ] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
@@ -841,15 +836,15 @@
         """
 
     def update_api(
         self,
         *,
         ApiId: str,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
+        CorsConfiguration: CorsUnionTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
@@ -888,15 +883,15 @@
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef] = ...,
+        JwtConfiguration: JWTConfigurationUnionTypeDef = ...,
         Name: str = ...
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_authorizer)
@@ -912,17 +907,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_deployment)
         """
 
     def update_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[
-            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
-        ] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_domain_name)
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/client.pyi` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_apigatewayv2.client import ApiGatewayV2Client
 
     session = Session()
     client: ApiGatewayV2Client = session.client("apigatewayv2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthorizationTypeType,
     AuthorizerTypeType,
     ConnectionTypeType,
@@ -38,30 +38,28 @@
     GetModelsPaginator,
     GetRouteResponsesPaginator,
     GetRoutesPaginator,
     GetStagesPaginator,
 )
 from .type_defs import (
     AccessLogSettingsTypeDef,
-    CorsOutputTypeDef,
-    CorsTypeDef,
+    CorsUnionTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
     CreateIntegrationResultTypeDef,
     CreateModelResponseTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     CreateStageResponseTypeDef,
     CreateVpcLinkResponseTypeDef,
-    DomainNameConfigurationOutputTypeDef,
-    DomainNameConfigurationTypeDef,
+    DomainNameConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportApiResponseTypeDef,
     GetApiMappingResponseTypeDef,
     GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizerResponseTypeDef,
@@ -83,16 +81,15 @@
     GetRoutesResponseTypeDef,
     GetStageResponseTypeDef,
     GetStagesResponseTypeDef,
     GetTagsResponseTypeDef,
     GetVpcLinkResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     ImportApiResponseTypeDef,
-    JWTConfigurationOutputTypeDef,
-    JWTConfigurationTypeDef,
+    JWTConfigurationUnionTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     ParameterConstraintsTypeDef,
     ReimportApiResponseTypeDef,
     RouteSettingsTypeDef,
     TlsConfigInputTypeDef,
     UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
@@ -162,15 +159,15 @@
         """
     def create_api(
         self,
         *,
         Name: str,
         ProtocolType: ProtocolTypeType,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
+        CorsConfiguration: CorsUnionTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -201,15 +198,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef] = ...
+        JwtConfiguration: JWTConfigurationUnionTypeDef = ...
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#create_authorizer)
         """
@@ -222,17 +219,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#create_deployment)
         """
     def create_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[
-            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
-        ] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
@@ -773,15 +768,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#untag_resource)
         """
     def update_api(
         self,
         *,
         ApiId: str,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
+        CorsConfiguration: CorsUnionTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
@@ -818,15 +813,15 @@
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef] = ...,
+        JwtConfiguration: JWTConfigurationUnionTypeDef = ...,
         Name: str = ...
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_authorizer)
@@ -840,17 +835,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_deployment)
         """
     def update_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[
-            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
-        ] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_domain_name)
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/literals.py` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/literals.pyi` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/paginator.py` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/paginator.pyi` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/type_defs.py` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsTypeDef
 
-    data: AccessLogSettingsTypeDef = {...}
+    data: AccessLogSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -50,17 +50,16 @@
     "CorsOutputTypeDef",
     "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "DomainNameConfigurationOutputTypeDef",
-    "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
+    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "RouteSettingsTypeDef",
@@ -78,14 +77,15 @@
     "DeleteRouteRequestParameterRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseRequestRequestTypeDef",
     "DeleteRouteSettingsRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "DeploymentTypeDef",
+    "TimestampTypeDef",
     "ExportApiRequestRequestTypeDef",
     "GetApiMappingRequestRequestTypeDef",
     "GetApiMappingsRequestRequestTypeDef",
     "GetApiRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetApisRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
@@ -121,14 +121,15 @@
     "UpdateApiMappingRequestRequestTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
     "ApiTypeDef",
     "AuthorizerTypeDef",
+    "CorsUnionTypeDef",
     "CreateApiRequestRequestTypeDef",
     "UpdateApiRequestRequestTypeDef",
     "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
     "CreateAuthorizerResponseTypeDef",
     "CreateDeploymentResponseTypeDef",
     "CreateIntegrationResponseResponseTypeDef",
@@ -152,17 +153,16 @@
     "UpdateApiResponseTypeDef",
     "UpdateAuthorizerResponseTypeDef",
     "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelResponseTypeDef",
     "UpdateVpcLinkResponseTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
+    "JWTConfigurationUnionTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "CreateDomainNameRequestRequestTypeDef",
-    "UpdateDomainNameRequestRequestTypeDef",
     "CreateDomainNameResponseTypeDef",
     "DomainNameTypeDef",
     "GetDomainNameResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateIntegrationRequestRequestTypeDef",
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
@@ -184,14 +184,15 @@
     "CreateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "StageTypeDef",
     "UpdateStageRequestRequestTypeDef",
     "UpdateStageResponseTypeDef",
     "GetDeploymentsResponseTypeDef",
+    "DomainNameConfigurationTypeDef",
     "GetApisRequestGetApisPaginateTypeDef",
     "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
     "GetModelsRequestGetModelsPaginateTypeDef",
@@ -204,14 +205,17 @@
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
     "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
+    "DomainNameConfigurationUnionTypeDef",
+    "CreateDomainNameRequestRequestTypeDef",
+    "UpdateDomainNameRequestRequestTypeDef",
 )
 
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
@@ -336,57 +340,40 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-DomainNameConfigurationOutputTypeDef = TypedDict(
-    "DomainNameConfigurationOutputTypeDef",
+MutualTlsAuthenticationInputTypeDef = TypedDict(
+    "MutualTlsAuthenticationInputTypeDef",
     {
-        "ApiGatewayDomainName": str,
-        "CertificateArn": str,
-        "CertificateName": str,
-        "CertificateUploadDate": datetime,
-        "DomainNameStatus": DomainNameStatusType,
-        "DomainNameStatusMessage": str,
-        "EndpointType": EndpointTypeType,
-        "HostedZoneId": str,
-        "SecurityPolicy": SecurityPolicyType,
-        "OwnershipVerificationCertificateArn": str,
+        "TruststoreUri": str,
+        "TruststoreVersion": str,
     },
     total=False,
 )
 
-DomainNameConfigurationTypeDef = TypedDict(
-    "DomainNameConfigurationTypeDef",
+DomainNameConfigurationOutputTypeDef = TypedDict(
+    "DomainNameConfigurationOutputTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
-        "CertificateUploadDate": Union[datetime, str],
+        "CertificateUploadDate": datetime,
         "DomainNameStatus": DomainNameStatusType,
         "DomainNameStatusMessage": str,
         "EndpointType": EndpointTypeType,
         "HostedZoneId": str,
         "SecurityPolicy": SecurityPolicyType,
         "OwnershipVerificationCertificateArn": str,
     },
     total=False,
 )
 
-MutualTlsAuthenticationInputTypeDef = TypedDict(
-    "MutualTlsAuthenticationInputTypeDef",
-    {
-        "TruststoreUri": str,
-        "TruststoreVersion": str,
-    },
-    total=False,
-)
-
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
@@ -640,14 +627,15 @@
         "DeploymentStatus": DeploymentStatusType,
         "DeploymentStatusMessage": str,
         "Description": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredExportApiRequestRequestTypeDef = TypedDict(
     "_RequiredExportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "OutputType": JSONYAMLType,
         "Specification": Literal["OAS30"],
     },
@@ -1349,14 +1337,15 @@
 )
 
 
 class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
     pass
 
 
+CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
 _RequiredCreateApiRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiRequestRequestTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
     },
 )
@@ -1846,14 +1835,15 @@
 
 class CreateAuthorizerRequestRequestTypeDef(
     _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
 ):
     pass
 
 
+JWTConfigurationUnionTypeDef = Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef]
 _RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
@@ -1877,63 +1867,14 @@
 
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDomainNameRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDomainNameRequestRequestTypeDef",
-    {
-        "DomainNameConfigurations": Sequence[
-            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
-        ],
-        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDomainNameRequestRequestTypeDef(
-    _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameRequestRequestTypeDef",
-    {
-        "DomainNameConfigurations": Sequence[
-            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
-        ],
-        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateDomainNameRequestRequestTypeDef(
-    _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
-):
-    pass
-
-
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
         "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
@@ -2593,14 +2534,31 @@
     {
         "Items": List[DeploymentTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DomainNameConfigurationTypeDef = TypedDict(
+    "DomainNameConfigurationTypeDef",
+    {
+        "ApiGatewayDomainName": str,
+        "CertificateArn": str,
+        "CertificateName": str,
+        "CertificateUploadDate": TimestampTypeDef,
+        "DomainNameStatus": DomainNameStatusType,
+        "DomainNameStatusMessage": str,
+        "EndpointType": EndpointTypeType,
+        "HostedZoneId": str,
+        "SecurityPolicy": SecurityPolicyType,
+        "OwnershipVerificationCertificateArn": str,
+    },
+    total=False,
+)
+
 GetApisRequestGetApisPaginateTypeDef = TypedDict(
     "GetApisRequestGetApisPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2876,7 +2834,54 @@
     "GetStagesResponseTypeDef",
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+DomainNameConfigurationUnionTypeDef = Union[
+    DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef
+]
+_RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDomainNameRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDomainNameRequestRequestTypeDef",
+    {
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDomainNameRequestRequestTypeDef(
+    _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameRequestRequestTypeDef",
+    {
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateDomainNameRequestRequestTypeDef(
+    _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/type_defs.pyi` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsTypeDef
 
-    data: AccessLogSettingsTypeDef = {...}
+    data: AccessLogSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -49,17 +49,16 @@
     "CorsOutputTypeDef",
     "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "DomainNameConfigurationOutputTypeDef",
-    "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
+    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "RouteSettingsTypeDef",
@@ -77,14 +76,15 @@
     "DeleteRouteRequestParameterRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseRequestRequestTypeDef",
     "DeleteRouteSettingsRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "DeploymentTypeDef",
+    "TimestampTypeDef",
     "ExportApiRequestRequestTypeDef",
     "GetApiMappingRequestRequestTypeDef",
     "GetApiMappingsRequestRequestTypeDef",
     "GetApiRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetApisRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
@@ -120,14 +120,15 @@
     "UpdateApiMappingRequestRequestTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
     "ApiTypeDef",
     "AuthorizerTypeDef",
+    "CorsUnionTypeDef",
     "CreateApiRequestRequestTypeDef",
     "UpdateApiRequestRequestTypeDef",
     "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
     "CreateAuthorizerResponseTypeDef",
     "CreateDeploymentResponseTypeDef",
     "CreateIntegrationResponseResponseTypeDef",
@@ -151,17 +152,16 @@
     "UpdateApiResponseTypeDef",
     "UpdateAuthorizerResponseTypeDef",
     "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelResponseTypeDef",
     "UpdateVpcLinkResponseTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
+    "JWTConfigurationUnionTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "CreateDomainNameRequestRequestTypeDef",
-    "UpdateDomainNameRequestRequestTypeDef",
     "CreateDomainNameResponseTypeDef",
     "DomainNameTypeDef",
     "GetDomainNameResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateIntegrationRequestRequestTypeDef",
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
@@ -183,14 +183,15 @@
     "CreateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "StageTypeDef",
     "UpdateStageRequestRequestTypeDef",
     "UpdateStageResponseTypeDef",
     "GetDeploymentsResponseTypeDef",
+    "DomainNameConfigurationTypeDef",
     "GetApisRequestGetApisPaginateTypeDef",
     "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
     "GetModelsRequestGetModelsPaginateTypeDef",
@@ -203,14 +204,17 @@
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
     "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
+    "DomainNameConfigurationUnionTypeDef",
+    "CreateDomainNameRequestRequestTypeDef",
+    "UpdateDomainNameRequestRequestTypeDef",
 )
 
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
@@ -329,57 +333,40 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-DomainNameConfigurationOutputTypeDef = TypedDict(
-    "DomainNameConfigurationOutputTypeDef",
+MutualTlsAuthenticationInputTypeDef = TypedDict(
+    "MutualTlsAuthenticationInputTypeDef",
     {
-        "ApiGatewayDomainName": str,
-        "CertificateArn": str,
-        "CertificateName": str,
-        "CertificateUploadDate": datetime,
-        "DomainNameStatus": DomainNameStatusType,
-        "DomainNameStatusMessage": str,
-        "EndpointType": EndpointTypeType,
-        "HostedZoneId": str,
-        "SecurityPolicy": SecurityPolicyType,
-        "OwnershipVerificationCertificateArn": str,
+        "TruststoreUri": str,
+        "TruststoreVersion": str,
     },
     total=False,
 )
 
-DomainNameConfigurationTypeDef = TypedDict(
-    "DomainNameConfigurationTypeDef",
+DomainNameConfigurationOutputTypeDef = TypedDict(
+    "DomainNameConfigurationOutputTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
-        "CertificateUploadDate": Union[datetime, str],
+        "CertificateUploadDate": datetime,
         "DomainNameStatus": DomainNameStatusType,
         "DomainNameStatusMessage": str,
         "EndpointType": EndpointTypeType,
         "HostedZoneId": str,
         "SecurityPolicy": SecurityPolicyType,
         "OwnershipVerificationCertificateArn": str,
     },
     total=False,
 )
 
-MutualTlsAuthenticationInputTypeDef = TypedDict(
-    "MutualTlsAuthenticationInputTypeDef",
-    {
-        "TruststoreUri": str,
-        "TruststoreVersion": str,
-    },
-    total=False,
-)
-
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
@@ -627,14 +614,15 @@
         "DeploymentStatus": DeploymentStatusType,
         "DeploymentStatusMessage": str,
         "Description": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredExportApiRequestRequestTypeDef = TypedDict(
     "_RequiredExportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "OutputType": JSONYAMLType,
         "Specification": Literal["OAS30"],
     },
@@ -1290,14 +1278,15 @@
     },
     total=False,
 )
 
 class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
     pass
 
+CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
 _RequiredCreateApiRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiRequestRequestTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
     },
 )
@@ -1781,14 +1770,15 @@
 )
 
 class CreateAuthorizerRequestRequestTypeDef(
     _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
 ):
     pass
 
+JWTConfigurationUnionTypeDef = Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef]
 _RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
@@ -1810,59 +1800,14 @@
 )
 
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDomainNameRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDomainNameRequestRequestTypeDef",
-    {
-        "DomainNameConfigurations": Sequence[
-            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
-        ],
-        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDomainNameRequestRequestTypeDef(
-    _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameRequestRequestTypeDef",
-    {
-        "DomainNameConfigurations": Sequence[
-            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
-        ],
-        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
-    },
-    total=False,
-)
-
-class UpdateDomainNameRequestRequestTypeDef(
-    _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
-):
-    pass
-
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
         "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
@@ -2498,14 +2443,31 @@
     {
         "Items": List[DeploymentTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DomainNameConfigurationTypeDef = TypedDict(
+    "DomainNameConfigurationTypeDef",
+    {
+        "ApiGatewayDomainName": str,
+        "CertificateArn": str,
+        "CertificateName": str,
+        "CertificateUploadDate": TimestampTypeDef,
+        "DomainNameStatus": DomainNameStatusType,
+        "DomainNameStatusMessage": str,
+        "EndpointType": EndpointTypeType,
+        "HostedZoneId": str,
+        "SecurityPolicy": SecurityPolicyType,
+        "OwnershipVerificationCertificateArn": str,
+    },
+    total=False,
+)
+
 GetApisRequestGetApisPaginateTypeDef = TypedDict(
     "GetApisRequestGetApisPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2765,7 +2727,51 @@
     "GetStagesResponseTypeDef",
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+DomainNameConfigurationUnionTypeDef = Union[
+    DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef
+]
+_RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDomainNameRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDomainNameRequestRequestTypeDef",
+    {
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDomainNameRequestRequestTypeDef(
+    _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameRequestRequestTypeDef",
+    {
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
+    },
+    total=False,
+)
+
+class UpdateDomainNameRequestRequestTypeDef(
+    _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/PKG-INFO` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewayv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApiGatewayV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 apigatewayv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 apigatewayv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewayv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewayv2)](https://pepy.tech/project/mypy-boto3-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[boto3.ApiGatewayV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
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
@@ -359,35 +359,34 @@
 )
 
 
 def check_value(value: AuthorizationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_apigatewayv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_apigatewayv2.type_defs import (
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
     CorsOutputTypeDef,
     JWTConfigurationOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    DomainNameConfigurationOutputTypeDef,
-    DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
     ParameterConstraintsTypeDef,
     RouteSettingsTypeDef,
@@ -405,14 +404,15 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
+    TimestampTypeDef,
     ExportApiRequestRequestTypeDef,
     GetApiMappingRequestRequestTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
@@ -448,14 +448,15 @@
     UpdateApiMappingRequestRequestTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
     ApiTypeDef,
     AuthorizerTypeDef,
+    CorsUnionTypeDef,
     CreateApiRequestRequestTypeDef,
     UpdateApiRequestRequestTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
@@ -479,17 +480,16 @@
     UpdateApiResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
     UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseResponseTypeDef,
     UpdateModelResponseTypeDef,
     UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
+    JWTConfigurationUnionTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    CreateDomainNameRequestRequestTypeDef,
-    UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateIntegrationRequestRequestTypeDef,
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
@@ -511,14 +511,15 @@
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
     UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    DomainNameConfigurationTypeDef,
     GetApisRequestGetApisPaginateTypeDef,
     GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetModelsRequestGetModelsPaginateTypeDef,
@@ -531,18 +532,21 @@
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
+    DomainNameConfigurationUnionTypeDef,
+    CreateDomainNameRequestRequestTypeDef,
+    UpdateDomainNameRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsTypeDef:
+def get_value() -> AccessLogSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt` & `mypy-boto3-apigatewayv2-1.28.16/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15.post1/setup.py` & `mypy-boto3-apigatewayv2-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigatewayv2",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_apigatewayv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.ApiGatewayV2 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 apigatewayv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 apigatewayv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_apigatewayv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

