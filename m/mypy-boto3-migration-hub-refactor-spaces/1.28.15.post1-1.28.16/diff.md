# Comparing `tmp/mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-migration-hub-refactor-spaces-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:43 2023, max compression
+gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.28.16.tar", last modified: Tue Aug  1 11:37:23 2023, max compression
```

## Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1.tar` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:43.609297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-29 10:03:43.601297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:43.593297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22886 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28978 2023-07-29 09:51:40.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28947 2023-07-29 09:51:40.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:43.601297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:43.609297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.652813 mypy-boto3-migration-hub-refactor-spaces-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:38.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-08-01 11:37:23.652813 mypy-boto3-migration-hub-refactor-spaces-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-08-01 11:24:38.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.648813 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-01 11:24:38.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-01 11:24:38.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-01 11:24:38.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22814 2023-08-01 11:24:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-08-01 11:24:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-08-01 11:24:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-08-01 11:24:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-01 11:24:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-08-01 11:24:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:38.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29116 2023-08-01 11:24:40.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29085 2023-08-01 11:24:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:38.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.652813 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-08-01 11:37:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-01 11:37:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 11:37:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:23.652813 mypy-boto3-migration-hub-refactor-spaces-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-01 11:24:38.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.16/setup.py
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/LICENSE` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 migration-hub-refactor-spaces type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 migration-hub-refactor-spaces type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migration-hub-refactor-spaces)](https://pepy.tech/project/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
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
@@ -339,20 +339,21 @@
 )
 
 
 def check_value(value: ApiGatewayEndpointTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migration_hub_refactor_spaces.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
@@ -403,14 +404,15 @@
     GetEnvironmentResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     GetRouteResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateRouteResponseTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseTypeDef,
+    UriPathRouteInputUnionTypeDef,
     CreateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     GetServiceResponseTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
@@ -420,15 +422,15 @@
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
 )
 
 
-def get_structure() -> ApiGatewayProxyConfigTypeDef:
+def get_value() -> ApiGatewayProxyConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/README.md` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migration-hub-refactor-spaces)](https://pepy.tech/project/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
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
@@ -307,20 +307,21 @@
 )
 
 
 def check_value(value: ApiGatewayEndpointTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migration_hub_refactor_spaces.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
@@ -371,14 +372,15 @@
     GetEnvironmentResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     GetRouteResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateRouteResponseTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseTypeDef,
+    UriPathRouteInputUnionTypeDef,
     CreateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     GetServiceResponseTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
@@ -388,15 +390,15 @@
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
 )
 
 
-def get_structure() -> ApiGatewayProxyConfigTypeDef:
+def get_value() -> ApiGatewayProxyConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__init__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__main__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces\nOther"
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/client.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migration_hub_refactor_spaces.client import MigrationHubRefactorSpacesClient
 
     session = Session()
     client: MigrationHubRefactorSpacesClient = session.client("migration-hub-refactor-spaces")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     NetworkFabricTypeType,
     RouteActivationStateType,
     RouteTypeType,
@@ -51,16 +51,15 @@
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateRouteResponseTypeDef,
-    UriPathRouteInputOutputTypeDef,
-    UriPathRouteInputTypeDef,
+    UriPathRouteInputUnionTypeDef,
     UrlEndpointInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -162,15 +161,15 @@
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteType: RouteTypeType,
         ServiceIdentifier: str,
         ClientToken: str = ...,
         DefaultRoute: DefaultRouteInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        UriPathRoute: Union[UriPathRouteInputTypeDef, UriPathRouteInputOutputTypeDef] = ...
+        UriPathRoute: UriPathRouteInputUnionTypeDef = ...
     ) -> CreateRouteResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_route)
         """
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/client.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migration_hub_refactor_spaces.client import MigrationHubRefactorSpacesClient
 
     session = Session()
     client: MigrationHubRefactorSpacesClient = session.client("migration-hub-refactor-spaces")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     NetworkFabricTypeType,
     RouteActivationStateType,
     RouteTypeType,
@@ -51,16 +51,15 @@
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateRouteResponseTypeDef,
-    UriPathRouteInputOutputTypeDef,
-    UriPathRouteInputTypeDef,
+    UriPathRouteInputUnionTypeDef,
     UrlEndpointInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -153,15 +152,15 @@
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteType: RouteTypeType,
         ServiceIdentifier: str,
         ClientToken: str = ...,
         DefaultRoute: DefaultRouteInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        UriPathRoute: Union[UriPathRouteInputTypeDef, UriPathRouteInputOutputTypeDef] = ...
+        UriPathRoute: UriPathRouteInputUnionTypeDef = ...
     ) -> CreateRouteResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_route)
         """
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/literals.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/literals.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/paginator.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/type_defs.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_migration_hub_refactor_spaces.type_defs import ApiGatewayProxyConfigTypeDef
 
-    data: ApiGatewayProxyConfigTypeDef = {...}
+    data: ApiGatewayProxyConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApiGatewayEndpointTypeType,
     ApplicationStateType,
     EnvironmentStateType,
     ErrorCodeType,
     ErrorResourceTypeType,
@@ -92,14 +92,15 @@
     "GetEnvironmentResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "GetRouteResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateRouteResponseTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseTypeDef",
+    "UriPathRouteInputUnionTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "ListEnvironmentVpcsResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
@@ -874,14 +875,15 @@
         "State": RouteStateType,
         "Tags": Dict[str, str],
         "UriPathRoute": UriPathRouteInputOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UriPathRouteInputUnionTypeDef = Union[UriPathRouteInputTypeDef, UriPathRouteInputOutputTypeDef]
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EndpointType": ServiceEndpointTypeType,
         "EnvironmentIdentifier": str,
         "Name": str,
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_migration_hub_refactor_spaces.type_defs import ApiGatewayProxyConfigTypeDef
 
-    data: ApiGatewayProxyConfigTypeDef = {...}
+    data: ApiGatewayProxyConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApiGatewayEndpointTypeType,
     ApplicationStateType,
     EnvironmentStateType,
     ErrorCodeType,
     ErrorResourceTypeType,
@@ -91,14 +91,15 @@
     "GetEnvironmentResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "GetRouteResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateRouteResponseTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseTypeDef",
+    "UriPathRouteInputUnionTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "ListEnvironmentVpcsResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
@@ -853,14 +854,15 @@
         "State": RouteStateType,
         "Tags": Dict[str, str],
         "UriPathRoute": UriPathRouteInputOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UriPathRouteInputUnionTypeDef = Union[UriPathRouteInputTypeDef, UriPathRouteInputOutputTypeDef]
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EndpointType": ServiceEndpointTypeType,
         "EnvironmentIdentifier": str,
         "Name": str,
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 migration-hub-refactor-spaces type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 migration-hub-refactor-spaces type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migration-hub-refactor-spaces)](https://pepy.tech/project/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
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
@@ -339,20 +339,21 @@
 )
 
 
 def check_value(value: ApiGatewayEndpointTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migration_hub_refactor_spaces.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
@@ -403,14 +404,15 @@
     GetEnvironmentResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     GetRouteResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateRouteResponseTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseTypeDef,
+    UriPathRouteInputUnionTypeDef,
     CreateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     GetServiceResponseTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
@@ -420,15 +422,15 @@
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
 )
 
 
-def get_structure() -> ApiGatewayProxyConfigTypeDef:
+def get_value() -> ApiGatewayProxyConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/setup.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migration-hub-refactor-spaces",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_migration_hub_refactor_spaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -35,16 +35,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords=(
-        "boto3 migration-hub-refactor-spaces type-annotations boto3-stubs mypy typeshed"
-        " autocomplete"
+        "boto3 migration-hub-refactor-spaces type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_migration_hub_refactor_spaces": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
```

