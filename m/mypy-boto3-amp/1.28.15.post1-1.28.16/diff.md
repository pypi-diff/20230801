# Comparing `tmp/mypy-boto3-amp-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-amp-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amp-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:24 2023, max compression
+gzip compressed data, was "mypy-boto3-amp-1.28.16.tar", last modified: Tue Aug  1 11:36:04 2023, max compression
```

## Comparing `mypy-boto3-amp-1.28.15.post1.tar` & `mypy-boto3-amp-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.008978 mypy-boto3-amp-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-07-29 10:02:24.008978 mypy-boto3-amp-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.004978 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22713 2023-07-29 09:37:38.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-07-29 09:37:38.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.008978 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-07-29 10:02:23.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:02:23.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:23.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:02:23.000000 mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:24.008978 mypy-boto3-amp-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-29 09:37:37.000000 mypy-boto3-amp-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.776961 mypy-boto3-amp-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-08-01 11:36:04.776961 mypy-boto3-amp-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.764961 mypy-boto3-amp-1.28.16/mypy_boto3_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16793 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22666 2023-08-01 11:10:08.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.768961 mypy-boto3-amp-1.28.16/mypy_boto3_amp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-08-01 11:36:04.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:36:04.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:04.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:04.000000 mypy-boto3-amp-1.28.16/mypy_boto3_amp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:04.776961 mypy-boto3-amp-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-01 11:10:07.000000 mypy-boto3-amp-1.28.16/setup.py
```

### Comparing `mypy-boto3-amp-1.28.15.post1/LICENSE` & `mypy-boto3-amp-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/PKG-INFO` & `mypy-boto3-amp-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amp
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PrometheusService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PrometheusService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amp type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 amp type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amp.svg?color=blue)](https://pypi.org/project/mypy-boto3-amp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amp)](https://pepy.tech/project/mypy-boto3-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PrometheusService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[boto3.PrometheusService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
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
 [mypy-boto3-amp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
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
@@ -340,29 +340,28 @@
 )
 
 
 def check_value(value: AlertManagerDefinitionStatusCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amp.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amp.type_defs import (
     AlertManagerDefinitionStatusTypeDef,
-    CreateAlertManagerDefinitionRequestRequestTypeDef,
+    BlobTypeDef,
     ResponseMetadataTypeDef,
     CreateLoggingConfigurationRequestRequestTypeDef,
     LoggingConfigurationStatusTypeDef,
-    CreateRuleGroupsNamespaceRequestRequestTypeDef,
     RuleGroupsNamespaceStatusTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     WorkspaceStatusTypeDef,
     DeleteAlertManagerDefinitionRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteRuleGroupsNamespaceRequestRequestTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
@@ -371,21 +370,23 @@
     DescribeRuleGroupsNamespaceRequestRequestTypeDef,
     DescribeWorkspaceRequestRequestTypeDef,
     WaiterConfigTypeDef,
     PaginatorConfigTypeDef,
     ListRuleGroupsNamespacesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkspacesRequestRequestTypeDef,
-    PutAlertManagerDefinitionRequestRequestTypeDef,
-    PutRuleGroupsNamespaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateWorkspaceAliasRequestRequestTypeDef,
     AlertManagerDefinitionDescriptionTypeDef,
+    CreateAlertManagerDefinitionRequestRequestTypeDef,
+    CreateRuleGroupsNamespaceRequestRequestTypeDef,
+    PutAlertManagerDefinitionRequestRequestTypeDef,
+    PutRuleGroupsNamespaceRequestRequestTypeDef,
     CreateAlertManagerDefinitionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutAlertManagerDefinitionResponseTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     LoggingConfigurationMetadataTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
@@ -405,15 +406,15 @@
     DescribeRuleGroupsNamespaceResponseTypeDef,
     ListRuleGroupsNamespacesResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
 )
 
 
-def get_structure() -> AlertManagerDefinitionStatusTypeDef:
+def get_value() -> AlertManagerDefinitionStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amp-1.28.15.post1/README.md` & `mypy-boto3-amp-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amp.svg?color=blue)](https://pypi.org/project/mypy-boto3-amp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amp)](https://pepy.tech/project/mypy-boto3-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PrometheusService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[boto3.PrometheusService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
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
 [mypy-boto3-amp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
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
@@ -308,29 +308,28 @@
 )
 
 
 def check_value(value: AlertManagerDefinitionStatusCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amp.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amp.type_defs import (
     AlertManagerDefinitionStatusTypeDef,
-    CreateAlertManagerDefinitionRequestRequestTypeDef,
+    BlobTypeDef,
     ResponseMetadataTypeDef,
     CreateLoggingConfigurationRequestRequestTypeDef,
     LoggingConfigurationStatusTypeDef,
-    CreateRuleGroupsNamespaceRequestRequestTypeDef,
     RuleGroupsNamespaceStatusTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     WorkspaceStatusTypeDef,
     DeleteAlertManagerDefinitionRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteRuleGroupsNamespaceRequestRequestTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
@@ -339,21 +338,23 @@
     DescribeRuleGroupsNamespaceRequestRequestTypeDef,
     DescribeWorkspaceRequestRequestTypeDef,
     WaiterConfigTypeDef,
     PaginatorConfigTypeDef,
     ListRuleGroupsNamespacesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkspacesRequestRequestTypeDef,
-    PutAlertManagerDefinitionRequestRequestTypeDef,
-    PutRuleGroupsNamespaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateWorkspaceAliasRequestRequestTypeDef,
     AlertManagerDefinitionDescriptionTypeDef,
+    CreateAlertManagerDefinitionRequestRequestTypeDef,
+    CreateRuleGroupsNamespaceRequestRequestTypeDef,
+    PutAlertManagerDefinitionRequestRequestTypeDef,
+    PutRuleGroupsNamespaceRequestRequestTypeDef,
     CreateAlertManagerDefinitionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutAlertManagerDefinitionResponseTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     LoggingConfigurationMetadataTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
@@ -373,15 +374,15 @@
     DescribeRuleGroupsNamespaceResponseTypeDef,
     ListRuleGroupsNamespacesResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
 )
 
 
-def get_structure() -> AlertManagerDefinitionStatusTypeDef:
+def get_value() -> AlertManagerDefinitionStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/__init__.py` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/__init__.pyi` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/__main__.py` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PrometheusService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.PrometheusService 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService\nOther"
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

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/client.py` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     from mypy_boto3_amp.client import PrometheusServiceClient
 
     session = Session()
     client: PrometheusServiceClient = session.client("amp")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import ListRuleGroupsNamespacesPaginator, ListWorkspacesPaginator
 from .type_defs import (
+    BlobTypeDef,
     CreateAlertManagerDefinitionResponseTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     CreateRuleGroupsNamespaceResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DescribeAlertManagerDefinitionResponseTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeRuleGroupsNamespaceResponseTypeDef,
@@ -97,19 +97,15 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#close)
         """
 
     def create_alert_manager_definition(
-        self,
-        *,
-        workspaceId: str,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        clientToken: str = ...
+        self, *, workspaceId: str, data: BlobTypeDef, clientToken: str = ...
     ) -> CreateAlertManagerDefinitionResponseTypeDef:
         """
         Create an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_alert_manager_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#create_alert_manager_definition)
         """
@@ -125,15 +121,15 @@
         """
 
     def create_rule_groups_namespace(
         self,
         *,
         workspaceId: str,
         name: str,
-        data: Union[str, bytes, IO[Any], StreamingBody],
+        data: BlobTypeDef,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleGroupsNamespaceResponseTypeDef:
         """
         Create a rule group namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_rule_groups_namespace)
@@ -267,34 +263,25 @@
         Lists all AMP workspaces, including workspaces being created or deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#list_workspaces)
         """
 
     def put_alert_manager_definition(
-        self,
-        *,
-        workspaceId: str,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        clientToken: str = ...
+        self, *, workspaceId: str, data: BlobTypeDef, clientToken: str = ...
     ) -> PutAlertManagerDefinitionResponseTypeDef:
         """
         Update an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_alert_manager_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#put_alert_manager_definition)
         """
 
     def put_rule_groups_namespace(
-        self,
-        *,
-        workspaceId: str,
-        name: str,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        clientToken: str = ...
+        self, *, workspaceId: str, name: str, data: BlobTypeDef, clientToken: str = ...
     ) -> PutRuleGroupsNamespaceResponseTypeDef:
         """
         Update a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_rule_groups_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#put_rule_groups_namespace)
         """
```

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/client.pyi` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     from mypy_boto3_amp.client import PrometheusServiceClient
 
     session = Session()
     client: PrometheusServiceClient = session.client("amp")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .paginator import ListRuleGroupsNamespacesPaginator, ListWorkspacesPaginator
 from .type_defs import (
+    BlobTypeDef,
     CreateAlertManagerDefinitionResponseTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     CreateRuleGroupsNamespaceResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DescribeAlertManagerDefinitionResponseTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeRuleGroupsNamespaceResponseTypeDef,
@@ -90,19 +90,15 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#close)
         """
     def create_alert_manager_definition(
-        self,
-        *,
-        workspaceId: str,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        clientToken: str = ...
+        self, *, workspaceId: str, data: BlobTypeDef, clientToken: str = ...
     ) -> CreateAlertManagerDefinitionResponseTypeDef:
         """
         Create an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_alert_manager_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#create_alert_manager_definition)
         """
@@ -116,15 +112,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#create_logging_configuration)
         """
     def create_rule_groups_namespace(
         self,
         *,
         workspaceId: str,
         name: str,
-        data: Union[str, bytes, IO[Any], StreamingBody],
+        data: BlobTypeDef,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleGroupsNamespaceResponseTypeDef:
         """
         Create a rule group namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_rule_groups_namespace)
@@ -244,33 +240,24 @@
         """
         Lists all AMP workspaces, including workspaces being created or deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#list_workspaces)
         """
     def put_alert_manager_definition(
-        self,
-        *,
-        workspaceId: str,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        clientToken: str = ...
+        self, *, workspaceId: str, data: BlobTypeDef, clientToken: str = ...
     ) -> PutAlertManagerDefinitionResponseTypeDef:
         """
         Update an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_alert_manager_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#put_alert_manager_definition)
         """
     def put_rule_groups_namespace(
-        self,
-        *,
-        workspaceId: str,
-        name: str,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        clientToken: str = ...
+        self, *, workspaceId: str, name: str, data: BlobTypeDef, clientToken: str = ...
     ) -> PutRuleGroupsNamespaceResponseTypeDef:
         """
         Update a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_rule_groups_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#put_rule_groups_namespace)
         """
```

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/literals.py` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/literals.pyi` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/paginator.py` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/paginator.pyi` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/type_defs.py` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_amp.type_defs import AlertManagerDefinitionStatusTypeDef
 
-    data: AlertManagerDefinitionStatusTypeDef = {...}
+    data: AlertManagerDefinitionStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -28,19 +28,18 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AlertManagerDefinitionStatusTypeDef",
-    "CreateAlertManagerDefinitionRequestRequestTypeDef",
+    "BlobTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLoggingConfigurationRequestRequestTypeDef",
     "LoggingConfigurationStatusTypeDef",
-    "CreateRuleGroupsNamespaceRequestRequestTypeDef",
     "RuleGroupsNamespaceStatusTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "WorkspaceStatusTypeDef",
     "DeleteAlertManagerDefinitionRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteRuleGroupsNamespaceRequestRequestTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
@@ -49,21 +48,23 @@
     "DescribeRuleGroupsNamespaceRequestRequestTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ListRuleGroupsNamespacesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
-    "PutAlertManagerDefinitionRequestRequestTypeDef",
-    "PutRuleGroupsNamespaceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateWorkspaceAliasRequestRequestTypeDef",
     "AlertManagerDefinitionDescriptionTypeDef",
+    "CreateAlertManagerDefinitionRequestRequestTypeDef",
+    "CreateRuleGroupsNamespaceRequestRequestTypeDef",
+    "PutAlertManagerDefinitionRequestRequestTypeDef",
+    "PutRuleGroupsNamespaceRequestRequestTypeDef",
     "CreateAlertManagerDefinitionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutAlertManagerDefinitionResponseTypeDef",
     "CreateLoggingConfigurationResponseTypeDef",
     "LoggingConfigurationMetadataTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
@@ -103,37 +104,15 @@
 
 class AlertManagerDefinitionStatusTypeDef(
     _RequiredAlertManagerDefinitionStatusTypeDef, _OptionalAlertManagerDefinitionStatusTypeDef
 ):
     pass
 
 
-_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateAlertManagerDefinitionRequestRequestTypeDef(
-    _RequiredCreateAlertManagerDefinitionRequestRequestTypeDef,
-    _OptionalCreateAlertManagerDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -181,39 +160,14 @@
 
 class LoggingConfigurationStatusTypeDef(
     _RequiredLoggingConfigurationStatusTypeDef, _OptionalLoggingConfigurationStatusTypeDef
 ):
     pass
 
 
-_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "name": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateRuleGroupsNamespaceRequestRequestTypeDef(
-    _RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef,
-    _OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredRuleGroupsNamespaceStatusTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceStatusTypeDef",
     {
         "statusCode": RuleGroupsNamespaceStatusCodeType,
     },
 )
 _OptionalRuleGroupsNamespaceStatusTypeDef = TypedDict(
@@ -421,61 +375,14 @@
         "nextToken": str,
         "alias": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutAlertManagerDefinitionRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutAlertManagerDefinitionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class PutAlertManagerDefinitionRequestRequestTypeDef(
-    _RequiredPutAlertManagerDefinitionRequestRequestTypeDef,
-    _OptionalPutAlertManagerDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "name": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class PutRuleGroupsNamespaceRequestRequestTypeDef(
-    _RequiredPutRuleGroupsNamespaceRequestRequestTypeDef,
-    _OptionalPutRuleGroupsNamespaceRequestRequestTypeDef,
-):
-    pass
-
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -540,14 +447,109 @@
         "status": AlertManagerDefinitionStatusTypeDef,
         "data": bytes,
         "createdAt": datetime,
         "modifiedAt": datetime,
     },
 )
 
+_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "data": BlobTypeDef,
+    },
+)
+_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateAlertManagerDefinitionRequestRequestTypeDef(
+    _RequiredCreateAlertManagerDefinitionRequestRequestTypeDef,
+    _OptionalCreateAlertManagerDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "name": str,
+        "data": BlobTypeDef,
+    },
+)
+_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateRuleGroupsNamespaceRequestRequestTypeDef(
+    _RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef,
+    _OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutAlertManagerDefinitionRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "data": BlobTypeDef,
+    },
+)
+_OptionalPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutAlertManagerDefinitionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class PutAlertManagerDefinitionRequestRequestTypeDef(
+    _RequiredPutAlertManagerDefinitionRequestRequestTypeDef,
+    _OptionalPutAlertManagerDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "name": str,
+        "data": BlobTypeDef,
+    },
+)
+_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class PutRuleGroupsNamespaceRequestRequestTypeDef(
+    _RequiredPutRuleGroupsNamespaceRequestRequestTypeDef,
+    _OptionalPutRuleGroupsNamespaceRequestRequestTypeDef,
+):
+    pass
+
+
 CreateAlertManagerDefinitionResponseTypeDef = TypedDict(
     "CreateAlertManagerDefinitionResponseTypeDef",
     {
         "status": AlertManagerDefinitionStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/type_defs.pyi` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_amp.type_defs import AlertManagerDefinitionStatusTypeDef
 
-    data: AlertManagerDefinitionStatusTypeDef = {...}
+    data: AlertManagerDefinitionStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -27,19 +27,18 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlertManagerDefinitionStatusTypeDef",
-    "CreateAlertManagerDefinitionRequestRequestTypeDef",
+    "BlobTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLoggingConfigurationRequestRequestTypeDef",
     "LoggingConfigurationStatusTypeDef",
-    "CreateRuleGroupsNamespaceRequestRequestTypeDef",
     "RuleGroupsNamespaceStatusTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "WorkspaceStatusTypeDef",
     "DeleteAlertManagerDefinitionRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteRuleGroupsNamespaceRequestRequestTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
@@ -48,21 +47,23 @@
     "DescribeRuleGroupsNamespaceRequestRequestTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ListRuleGroupsNamespacesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
-    "PutAlertManagerDefinitionRequestRequestTypeDef",
-    "PutRuleGroupsNamespaceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateWorkspaceAliasRequestRequestTypeDef",
     "AlertManagerDefinitionDescriptionTypeDef",
+    "CreateAlertManagerDefinitionRequestRequestTypeDef",
+    "CreateRuleGroupsNamespaceRequestRequestTypeDef",
+    "PutAlertManagerDefinitionRequestRequestTypeDef",
+    "PutRuleGroupsNamespaceRequestRequestTypeDef",
     "CreateAlertManagerDefinitionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutAlertManagerDefinitionResponseTypeDef",
     "CreateLoggingConfigurationResponseTypeDef",
     "LoggingConfigurationMetadataTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
@@ -100,35 +101,15 @@
 )
 
 class AlertManagerDefinitionStatusTypeDef(
     _RequiredAlertManagerDefinitionStatusTypeDef, _OptionalAlertManagerDefinitionStatusTypeDef
 ):
     pass
 
-_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreateAlertManagerDefinitionRequestRequestTypeDef(
-    _RequiredCreateAlertManagerDefinitionRequestRequestTypeDef,
-    _OptionalCreateAlertManagerDefinitionRequestRequestTypeDef,
-):
-    pass
-
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -172,37 +153,14 @@
 )
 
 class LoggingConfigurationStatusTypeDef(
     _RequiredLoggingConfigurationStatusTypeDef, _OptionalLoggingConfigurationStatusTypeDef
 ):
     pass
 
-_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "name": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateRuleGroupsNamespaceRequestRequestTypeDef(
-    _RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef,
-    _OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef,
-):
-    pass
-
 _RequiredRuleGroupsNamespaceStatusTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceStatusTypeDef",
     {
         "statusCode": RuleGroupsNamespaceStatusCodeType,
     },
 )
 _OptionalRuleGroupsNamespaceStatusTypeDef = TypedDict(
@@ -398,57 +356,14 @@
         "nextToken": str,
         "alias": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutAlertManagerDefinitionRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutAlertManagerDefinitionRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class PutAlertManagerDefinitionRequestRequestTypeDef(
-    _RequiredPutAlertManagerDefinitionRequestRequestTypeDef,
-    _OptionalPutAlertManagerDefinitionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "name": str,
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class PutRuleGroupsNamespaceRequestRequestTypeDef(
-    _RequiredPutRuleGroupsNamespaceRequestRequestTypeDef,
-    _OptionalPutRuleGroupsNamespaceRequestRequestTypeDef,
-):
-    pass
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -509,14 +424,101 @@
         "status": AlertManagerDefinitionStatusTypeDef,
         "data": bytes,
         "createdAt": datetime,
         "modifiedAt": datetime,
     },
 )
 
+_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "data": BlobTypeDef,
+    },
+)
+_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreateAlertManagerDefinitionRequestRequestTypeDef(
+    _RequiredCreateAlertManagerDefinitionRequestRequestTypeDef,
+    _OptionalCreateAlertManagerDefinitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "name": str,
+        "data": BlobTypeDef,
+    },
+)
+_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateRuleGroupsNamespaceRequestRequestTypeDef(
+    _RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef,
+    _OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef,
+):
+    pass
+
+_RequiredPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutAlertManagerDefinitionRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "data": BlobTypeDef,
+    },
+)
+_OptionalPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutAlertManagerDefinitionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class PutAlertManagerDefinitionRequestRequestTypeDef(
+    _RequiredPutAlertManagerDefinitionRequestRequestTypeDef,
+    _OptionalPutAlertManagerDefinitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "name": str,
+        "data": BlobTypeDef,
+    },
+)
+_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class PutRuleGroupsNamespaceRequestRequestTypeDef(
+    _RequiredPutRuleGroupsNamespaceRequestRequestTypeDef,
+    _OptionalPutRuleGroupsNamespaceRequestRequestTypeDef,
+):
+    pass
+
 CreateAlertManagerDefinitionResponseTypeDef = TypedDict(
     "CreateAlertManagerDefinitionResponseTypeDef",
     {
         "status": AlertManagerDefinitionStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/waiter.py` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp/waiter.pyi` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp.egg-info/PKG-INFO` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amp
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PrometheusService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PrometheusService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amp type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 amp type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amp.svg?color=blue)](https://pypi.org/project/mypy-boto3-amp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amp)](https://pepy.tech/project/mypy-boto3-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PrometheusService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[boto3.PrometheusService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
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
 [mypy-boto3-amp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
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
@@ -340,29 +340,28 @@
 )
 
 
 def check_value(value: AlertManagerDefinitionStatusCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amp.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amp.type_defs import (
     AlertManagerDefinitionStatusTypeDef,
-    CreateAlertManagerDefinitionRequestRequestTypeDef,
+    BlobTypeDef,
     ResponseMetadataTypeDef,
     CreateLoggingConfigurationRequestRequestTypeDef,
     LoggingConfigurationStatusTypeDef,
-    CreateRuleGroupsNamespaceRequestRequestTypeDef,
     RuleGroupsNamespaceStatusTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     WorkspaceStatusTypeDef,
     DeleteAlertManagerDefinitionRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteRuleGroupsNamespaceRequestRequestTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
@@ -371,21 +370,23 @@
     DescribeRuleGroupsNamespaceRequestRequestTypeDef,
     DescribeWorkspaceRequestRequestTypeDef,
     WaiterConfigTypeDef,
     PaginatorConfigTypeDef,
     ListRuleGroupsNamespacesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkspacesRequestRequestTypeDef,
-    PutAlertManagerDefinitionRequestRequestTypeDef,
-    PutRuleGroupsNamespaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateWorkspaceAliasRequestRequestTypeDef,
     AlertManagerDefinitionDescriptionTypeDef,
+    CreateAlertManagerDefinitionRequestRequestTypeDef,
+    CreateRuleGroupsNamespaceRequestRequestTypeDef,
+    PutAlertManagerDefinitionRequestRequestTypeDef,
+    PutRuleGroupsNamespaceRequestRequestTypeDef,
     CreateAlertManagerDefinitionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutAlertManagerDefinitionResponseTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     LoggingConfigurationMetadataTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
@@ -405,15 +406,15 @@
     DescribeRuleGroupsNamespaceResponseTypeDef,
     ListRuleGroupsNamespacesResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
 )
 
 
-def get_structure() -> AlertManagerDefinitionStatusTypeDef:
+def get_value() -> AlertManagerDefinitionStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amp-1.28.15.post1/mypy_boto3_amp.egg-info/SOURCES.txt` & `mypy-boto3-amp-1.28.16/mypy_boto3_amp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.28.15.post1/setup.py` & `mypy-boto3-amp-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amp",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_amp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PrometheusService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.PrometheusService 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 amp type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 amp type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_amp": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

