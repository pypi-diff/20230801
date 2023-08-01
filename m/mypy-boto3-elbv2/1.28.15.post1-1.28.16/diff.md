# Comparing `tmp/mypy-boto3-elbv2-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-elbv2-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elbv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:05 2023, max compression
+gzip compressed data, was "mypy-boto3-elbv2-1.28.16.tar", last modified: Tue Aug  1 11:36:45 2023, max compression
```

## Comparing `mypy-boto3-elbv2-1.28.15.post1.tar` & `mypy-boto3-elbv2-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.713141 mypy-boto3-elbv2-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-07-29 10:03:05.705141 mypy-boto3-elbv2-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.705141 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34134 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34081 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-07-29 09:44:52.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-29 09:44:52.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43639 2023-07-29 09:44:53.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43592 2023-07-29 09:44:52.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.705141 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:05.713141 mypy-boto3-elbv2-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.572895 mypy-boto3-elbv2-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:27.000000 mypy-boto3-elbv2-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20386 2023-08-01 11:36:45.572895 mypy-boto3-elbv2-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-08-01 11:17:27.000000 mypy-boto3-elbv2-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.572895 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-08-01 11:17:27.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-08-01 11:17:27.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 11:17:27.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33928 2023-08-01 11:17:28.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33875 2023-08-01 11:17:27.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-08-01 11:17:28.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-08-01 11:17:28.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-08-01 11:17:28.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-08-01 11:17:28.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:27.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43690 2023-08-01 11:17:31.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43644 2023-08-01 11:17:30.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:27.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-08-01 11:17:28.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-08-01 11:17:28.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.572895 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20386 2023-08-01 11:36:45.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 11:36:45.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:45.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:36:45.000000 mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:45.572895 mypy-boto3-elbv2-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-01 11:17:27.000000 mypy-boto3-elbv2-1.28.16/setup.py
```

### Comparing `mypy-boto3-elbv2-1.28.15.post1/LICENSE` & `mypy-boto3-elbv2-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/PKG-INFO` & `mypy-boto3-elbv2-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 elbv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 elbv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
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
@@ -395,20 +395,20 @@
 )
 
 
 def check_value(value: ActionTypeEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elbv2.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elbv2.type_defs import (
     AuthenticateCognitoActionConfigOutputTypeDef,
     AuthenticateOidcActionConfigOutputTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
@@ -514,30 +514,32 @@
     ActionTypeDef,
     RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
     ListenerTypeDef,
-    CreateListenerInputRequestTypeDef,
-    ModifyListenerInputRequestTypeDef,
+    ActionUnionTypeDef,
     RuleTypeDef,
-    CreateRuleInputRequestTypeDef,
-    ModifyRuleInputRequestTypeDef,
+    RuleConditionUnionTypeDef,
     CreateListenerOutputTypeDef,
     DescribeListenersOutputTypeDef,
     ModifyListenerOutputTypeDef,
+    CreateListenerInputRequestTypeDef,
+    ModifyListenerInputRequestTypeDef,
     CreateRuleOutputTypeDef,
     DescribeRulesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
+    CreateRuleInputRequestTypeDef,
+    ModifyRuleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AuthenticateCognitoActionConfigOutputTypeDef:
+def get_value() -> AuthenticateCognitoActionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elbv2-1.28.15.post1/README.md` & `mypy-boto3-elbv2-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
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
@@ -363,20 +363,20 @@
 )
 
 
 def check_value(value: ActionTypeEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elbv2.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elbv2.type_defs import (
     AuthenticateCognitoActionConfigOutputTypeDef,
     AuthenticateOidcActionConfigOutputTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
@@ -482,30 +482,32 @@
     ActionTypeDef,
     RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
     ListenerTypeDef,
-    CreateListenerInputRequestTypeDef,
-    ModifyListenerInputRequestTypeDef,
+    ActionUnionTypeDef,
     RuleTypeDef,
-    CreateRuleInputRequestTypeDef,
-    ModifyRuleInputRequestTypeDef,
+    RuleConditionUnionTypeDef,
     CreateListenerOutputTypeDef,
     DescribeListenersOutputTypeDef,
     ModifyListenerOutputTypeDef,
+    CreateListenerInputRequestTypeDef,
+    ModifyListenerInputRequestTypeDef,
     CreateRuleOutputTypeDef,
     DescribeRulesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
+    CreateRuleInputRequestTypeDef,
+    ModifyRuleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AuthenticateCognitoActionConfigOutputTypeDef:
+def get_value() -> AuthenticateCognitoActionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__init__.py` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__init__.pyi` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__main__.py` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\nOther"
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

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/client.py` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_elbv2.client import ElasticLoadBalancingv2Client
 
     session = Session()
     client: ElasticLoadBalancingv2Client = session.client("elbv2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
     LoadBalancerTypeEnumType,
@@ -32,16 +32,15 @@
     DescribeListenersPaginator,
     DescribeLoadBalancersPaginator,
     DescribeRulesPaginator,
     DescribeSSLPoliciesPaginator,
     DescribeTargetGroupsPaginator,
 )
 from .type_defs import (
-    ActionOutputTypeDef,
-    ActionTypeDef,
+    ActionUnionTypeDef,
     AddListenerCertificatesOutputTypeDef,
     CertificateTypeDef,
     CreateListenerOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     CreateRuleOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
@@ -58,16 +57,15 @@
     LoadBalancerAttributeTypeDef,
     MatcherTypeDef,
     ModifyListenerOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
-    RuleConditionOutputTypeDef,
-    RuleConditionTypeDef,
+    RuleConditionUnionTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
     SetSecurityGroupsOutputTypeDef,
     SetSubnetsOutputTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
@@ -194,15 +192,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#close)
         """
 
     def create_listener(
         self,
         *,
         LoadBalancerArn: str,
-        DefaultActions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        DefaultActions: Sequence[ActionUnionTypeDef],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateListenerOutputTypeDef:
@@ -235,17 +233,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#create_load_balancer)
         """
 
     def create_rule(
         self,
         *,
         ListenerArn: str,
-        Conditions: Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
+        Conditions: Sequence[RuleConditionUnionTypeDef],
         Priority: int,
-        Actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        Actions: Sequence[ActionUnionTypeDef],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#create_rule)
@@ -478,15 +476,15 @@
         self,
         *,
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
-        DefaultActions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
+        DefaultActions: Sequence[ActionUnionTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_listener)
@@ -503,16 +501,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_load_balancer_attributes)
         """
 
     def modify_rule(
         self,
         *,
         RuleArn: str,
-        Conditions: Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]] = ...,
-        Actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...
+        Conditions: Sequence[RuleConditionUnionTypeDef] = ...,
+        Actions: Sequence[ActionUnionTypeDef] = ...
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_rule)
         """
```

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/client.pyi` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_elbv2.client import ElasticLoadBalancingv2Client
 
     session = Session()
     client: ElasticLoadBalancingv2Client = session.client("elbv2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
     LoadBalancerTypeEnumType,
@@ -32,16 +32,15 @@
     DescribeListenersPaginator,
     DescribeLoadBalancersPaginator,
     DescribeRulesPaginator,
     DescribeSSLPoliciesPaginator,
     DescribeTargetGroupsPaginator,
 )
 from .type_defs import (
-    ActionOutputTypeDef,
-    ActionTypeDef,
+    ActionUnionTypeDef,
     AddListenerCertificatesOutputTypeDef,
     CertificateTypeDef,
     CreateListenerOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     CreateRuleOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
@@ -58,16 +57,15 @@
     LoadBalancerAttributeTypeDef,
     MatcherTypeDef,
     ModifyListenerOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
-    RuleConditionOutputTypeDef,
-    RuleConditionTypeDef,
+    RuleConditionUnionTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
     SetSecurityGroupsOutputTypeDef,
     SetSubnetsOutputTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
@@ -185,15 +183,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#close)
         """
     def create_listener(
         self,
         *,
         LoadBalancerArn: str,
-        DefaultActions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        DefaultActions: Sequence[ActionUnionTypeDef],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateListenerOutputTypeDef:
@@ -224,17 +222,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_load_balancer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#create_load_balancer)
         """
     def create_rule(
         self,
         *,
         ListenerArn: str,
-        Conditions: Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
+        Conditions: Sequence[RuleConditionUnionTypeDef],
         Priority: int,
-        Actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        Actions: Sequence[ActionUnionTypeDef],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#create_rule)
@@ -448,15 +446,15 @@
         self,
         *,
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
-        DefaultActions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
+        DefaultActions: Sequence[ActionUnionTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_listener)
@@ -471,16 +469,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_load_balancer_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_load_balancer_attributes)
         """
     def modify_rule(
         self,
         *,
         RuleArn: str,
-        Conditions: Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]] = ...,
-        Actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...
+        Conditions: Sequence[RuleConditionUnionTypeDef] = ...,
+        Actions: Sequence[ActionUnionTypeDef] = ...
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_rule)
         """
```

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/literals.py` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/literals.pyi` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/paginator.py` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/paginator.pyi` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/type_defs.py` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
 
-    data: AuthenticateCognitoActionConfigOutputTypeDef = {...}
+    data: AuthenticateCognitoActionConfigOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -144,26 +144,28 @@
     "ActionTypeDef",
     "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
     "ListenerTypeDef",
-    "CreateListenerInputRequestTypeDef",
-    "ModifyListenerInputRequestTypeDef",
+    "ActionUnionTypeDef",
     "RuleTypeDef",
-    "CreateRuleInputRequestTypeDef",
-    "ModifyRuleInputRequestTypeDef",
+    "RuleConditionUnionTypeDef",
     "CreateListenerOutputTypeDef",
     "DescribeListenersOutputTypeDef",
     "ModifyListenerOutputTypeDef",
+    "CreateListenerInputRequestTypeDef",
+    "ModifyListenerInputRequestTypeDef",
     "CreateRuleOutputTypeDef",
     "DescribeRulesOutputTypeDef",
     "ModifyRuleOutputTypeDef",
     "SetRulePrioritiesOutputTypeDef",
+    "CreateRuleInputRequestTypeDef",
+    "ModifyRuleInputRequestTypeDef",
 )
 
 _RequiredAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
     "_RequiredAuthenticateCognitoActionConfigOutputTypeDef",
     {
         "UserPoolArn": str,
         "UserPoolClientId": str,
@@ -1497,19 +1499,58 @@
         "SslPolicy": str,
         "DefaultActions": List[ActionOutputTypeDef],
         "AlpnPolicy": List[str],
     },
     total=False,
 )
 
+ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "RuleArn": str,
+        "Priority": str,
+        "Conditions": List[RuleConditionOutputTypeDef],
+        "Actions": List[ActionOutputTypeDef],
+        "IsDefault": bool,
+    },
+    total=False,
+)
+
+RuleConditionUnionTypeDef = Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]
+CreateListenerOutputTypeDef = TypedDict(
+    "CreateListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeListenersOutputTypeDef = TypedDict(
+    "DescribeListenersOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyListenerOutputTypeDef = TypedDict(
+    "ModifyListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
-        "DefaultActions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "DefaultActions": Sequence[ActionUnionTypeDef],
     },
 )
 _OptionalCreateListenerInputRequestTypeDef = TypedDict(
     "_OptionalCreateListenerInputRequestTypeDef",
     {
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -1537,46 +1578,67 @@
 _OptionalModifyListenerInputRequestTypeDef = TypedDict(
     "_OptionalModifyListenerInputRequestTypeDef",
     {
         "Port": int,
         "Protocol": ProtocolEnumType,
         "SslPolicy": str,
         "Certificates": Sequence[CertificateTypeDef],
-        "DefaultActions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "DefaultActions": Sequence[ActionUnionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
 
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
 
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
+CreateRuleOutputTypeDef = TypedDict(
+    "CreateRuleOutputTypeDef",
     {
-        "RuleArn": str,
-        "Priority": str,
-        "Conditions": List[RuleConditionOutputTypeDef],
-        "Actions": List[ActionOutputTypeDef],
-        "IsDefault": bool,
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRulesOutputTypeDef = TypedDict(
+    "DescribeRulesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyRuleOutputTypeDef = TypedDict(
+    "ModifyRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetRulePrioritiesOutputTypeDef = TypedDict(
+    "SetRulePrioritiesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
-        "Conditions": Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
+        "Conditions": Sequence[RuleConditionUnionTypeDef],
         "Priority": int,
-        "Actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "Actions": Sequence[ActionUnionTypeDef],
     },
 )
 _OptionalCreateRuleInputRequestTypeDef = TypedDict(
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -1595,77 +1657,18 @@
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
     "_OptionalModifyRuleInputRequestTypeDef",
     {
-        "Conditions": Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
-        "Actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "Conditions": Sequence[RuleConditionUnionTypeDef],
+        "Actions": Sequence[ActionUnionTypeDef],
     },
     total=False,
 )
 
 
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
-
-
-CreateListenerOutputTypeDef = TypedDict(
-    "CreateListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeListenersOutputTypeDef = TypedDict(
-    "DescribeListenersOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyListenerOutputTypeDef = TypedDict(
-    "ModifyListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRuleOutputTypeDef = TypedDict(
-    "CreateRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRulesOutputTypeDef = TypedDict(
-    "DescribeRulesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyRuleOutputTypeDef = TypedDict(
-    "ModifyRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetRulePrioritiesOutputTypeDef = TypedDict(
-    "SetRulePrioritiesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/type_defs.pyi` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
 
-    data: AuthenticateCognitoActionConfigOutputTypeDef = {...}
+    data: AuthenticateCognitoActionConfigOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -143,26 +143,28 @@
     "ActionTypeDef",
     "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
     "ListenerTypeDef",
-    "CreateListenerInputRequestTypeDef",
-    "ModifyListenerInputRequestTypeDef",
+    "ActionUnionTypeDef",
     "RuleTypeDef",
-    "CreateRuleInputRequestTypeDef",
-    "ModifyRuleInputRequestTypeDef",
+    "RuleConditionUnionTypeDef",
     "CreateListenerOutputTypeDef",
     "DescribeListenersOutputTypeDef",
     "ModifyListenerOutputTypeDef",
+    "CreateListenerInputRequestTypeDef",
+    "ModifyListenerInputRequestTypeDef",
     "CreateRuleOutputTypeDef",
     "DescribeRulesOutputTypeDef",
     "ModifyRuleOutputTypeDef",
     "SetRulePrioritiesOutputTypeDef",
+    "CreateRuleInputRequestTypeDef",
+    "ModifyRuleInputRequestTypeDef",
 )
 
 _RequiredAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
     "_RequiredAuthenticateCognitoActionConfigOutputTypeDef",
     {
         "UserPoolArn": str,
         "UserPoolClientId": str,
@@ -1458,19 +1460,58 @@
         "SslPolicy": str,
         "DefaultActions": List[ActionOutputTypeDef],
         "AlpnPolicy": List[str],
     },
     total=False,
 )
 
+ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "RuleArn": str,
+        "Priority": str,
+        "Conditions": List[RuleConditionOutputTypeDef],
+        "Actions": List[ActionOutputTypeDef],
+        "IsDefault": bool,
+    },
+    total=False,
+)
+
+RuleConditionUnionTypeDef = Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]
+CreateListenerOutputTypeDef = TypedDict(
+    "CreateListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeListenersOutputTypeDef = TypedDict(
+    "DescribeListenersOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyListenerOutputTypeDef = TypedDict(
+    "ModifyListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
-        "DefaultActions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "DefaultActions": Sequence[ActionUnionTypeDef],
     },
 )
 _OptionalCreateListenerInputRequestTypeDef = TypedDict(
     "_OptionalCreateListenerInputRequestTypeDef",
     {
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -1496,44 +1537,65 @@
 _OptionalModifyListenerInputRequestTypeDef = TypedDict(
     "_OptionalModifyListenerInputRequestTypeDef",
     {
         "Port": int,
         "Protocol": ProtocolEnumType,
         "SslPolicy": str,
         "Certificates": Sequence[CertificateTypeDef],
-        "DefaultActions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "DefaultActions": Sequence[ActionUnionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
+CreateRuleOutputTypeDef = TypedDict(
+    "CreateRuleOutputTypeDef",
     {
-        "RuleArn": str,
-        "Priority": str,
-        "Conditions": List[RuleConditionOutputTypeDef],
-        "Actions": List[ActionOutputTypeDef],
-        "IsDefault": bool,
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRulesOutputTypeDef = TypedDict(
+    "DescribeRulesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyRuleOutputTypeDef = TypedDict(
+    "ModifyRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetRulePrioritiesOutputTypeDef = TypedDict(
+    "SetRulePrioritiesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
-        "Conditions": Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
+        "Conditions": Sequence[RuleConditionUnionTypeDef],
         "Priority": int,
-        "Actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "Actions": Sequence[ActionUnionTypeDef],
     },
 )
 _OptionalCreateRuleInputRequestTypeDef = TypedDict(
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -1550,75 +1612,17 @@
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
     "_OptionalModifyRuleInputRequestTypeDef",
     {
-        "Conditions": Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
-        "Actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "Conditions": Sequence[RuleConditionUnionTypeDef],
+        "Actions": Sequence[ActionUnionTypeDef],
     },
     total=False,
 )
 
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
-
-CreateListenerOutputTypeDef = TypedDict(
-    "CreateListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeListenersOutputTypeDef = TypedDict(
-    "DescribeListenersOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyListenerOutputTypeDef = TypedDict(
-    "ModifyListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRuleOutputTypeDef = TypedDict(
-    "CreateRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRulesOutputTypeDef = TypedDict(
-    "DescribeRulesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyRuleOutputTypeDef = TypedDict(
-    "ModifyRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetRulePrioritiesOutputTypeDef = TypedDict(
-    "SetRulePrioritiesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/waiter.py` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/waiter.pyi` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/PKG-INFO` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 elbv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 elbv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
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
@@ -395,20 +395,20 @@
 )
 
 
 def check_value(value: ActionTypeEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elbv2.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elbv2.type_defs import (
     AuthenticateCognitoActionConfigOutputTypeDef,
     AuthenticateOidcActionConfigOutputTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
@@ -514,30 +514,32 @@
     ActionTypeDef,
     RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
     ListenerTypeDef,
-    CreateListenerInputRequestTypeDef,
-    ModifyListenerInputRequestTypeDef,
+    ActionUnionTypeDef,
     RuleTypeDef,
-    CreateRuleInputRequestTypeDef,
-    ModifyRuleInputRequestTypeDef,
+    RuleConditionUnionTypeDef,
     CreateListenerOutputTypeDef,
     DescribeListenersOutputTypeDef,
     ModifyListenerOutputTypeDef,
+    CreateListenerInputRequestTypeDef,
+    ModifyListenerInputRequestTypeDef,
     CreateRuleOutputTypeDef,
     DescribeRulesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
+    CreateRuleInputRequestTypeDef,
+    ModifyRuleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AuthenticateCognitoActionConfigOutputTypeDef:
+def get_value() -> AuthenticateCognitoActionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/SOURCES.txt` & `mypy-boto3-elbv2-1.28.16/mypy_boto3_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15.post1/setup.py` & `mypy-boto3-elbv2-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elbv2",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.16 service generated with"
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
-    keywords="boto3 elbv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 elbv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_elbv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

