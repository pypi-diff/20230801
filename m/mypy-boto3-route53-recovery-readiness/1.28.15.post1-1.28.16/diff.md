# Comparing `tmp/mypy-boto3-route53-recovery-readiness-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-route53-recovery-readiness-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:02 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.28.16.tar", last modified: Tue Aug  1 11:37:42 2023, max compression
```

## Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1.tar` & `mypy-boto3-route53-recovery-readiness-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:02.785371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-07-29 10:04:02.785371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17487 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:02.769371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28609 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30121 2023-07-29 09:57:23.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30084 2023-07-29 09:57:23.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:02.785371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:02.785371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-29 09:57:21.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:42.652763 mypy-boto3-route53-recovery-readiness-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-08-01 11:37:42.644763 mypy-boto3-route53-recovery-readiness-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:42.636763 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28530 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-08-01 11:30:46.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-08-01 11:30:46.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-08-01 11:30:46.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-08-01 11:30:46.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30166 2023-08-01 11:30:47.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30129 2023-08-01 11:30:46.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:42.644763 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-08-01 11:37:42.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-01 11:37:42.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:42.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:42.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:42.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:42.000000 mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:42.652763 mypy-boto3-route53-recovery-readiness-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-01 11:30:45.000000 mypy-boto3-route53-recovery-readiness-1.28.16/setup.py
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/LICENSE` & `mypy-boto3-route53-recovery-readiness-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 route53-recovery-readiness type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 route53-recovery-readiness type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-readiness)](https://pepy.tech/project/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
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
@@ -354,20 +354,21 @@
 )
 
 
 def check_value(value: GetCellReadinessSummaryPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_route53_recovery_readiness.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_route53_recovery_readiness.type_defs import (
     CellOutputTypeDef,
     CreateCellRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateCrossAccountAuthorizationRequestRequestTypeDef,
@@ -446,21 +447,22 @@
     DNSTargetResourceTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     CreateResourceSetResponseTypeDef,
     GetResourceSetResponseTypeDef,
     ResourceSetOutputTypeDef,
     UpdateResourceSetResponseTypeDef,
+    ResourceUnionTypeDef,
+    ListResourceSetsResponseTypeDef,
     CreateResourceSetRequestRequestTypeDef,
     UpdateResourceSetRequestRequestTypeDef,
-    ListResourceSetsResponseTypeDef,
 )
 
 
-def get_structure() -> CellOutputTypeDef:
+def get_value() -> CellOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/README.md` & `mypy-boto3-route53-recovery-readiness-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-readiness)](https://pepy.tech/project/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
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
@@ -322,20 +322,21 @@
 )
 
 
 def check_value(value: GetCellReadinessSummaryPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_route53_recovery_readiness.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_route53_recovery_readiness.type_defs import (
     CellOutputTypeDef,
     CreateCellRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateCrossAccountAuthorizationRequestRequestTypeDef,
@@ -414,21 +415,22 @@
     DNSTargetResourceTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     CreateResourceSetResponseTypeDef,
     GetResourceSetResponseTypeDef,
     ResourceSetOutputTypeDef,
     UpdateResourceSetResponseTypeDef,
+    ResourceUnionTypeDef,
+    ListResourceSetsResponseTypeDef,
     CreateResourceSetRequestRequestTypeDef,
     UpdateResourceSetRequestRequestTypeDef,
-    ListResourceSetsResponseTypeDef,
 )
 
 
-def get_structure() -> CellOutputTypeDef:
+def get_value() -> CellOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__init__.py` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__init__.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__main__.py` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53RecoveryReadiness 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Route53RecoveryReadiness 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness\nOther"
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/client.py` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_route53_recovery_readiness.client import Route53RecoveryReadinessClient
 
     session = Session()
     client: Route53RecoveryReadinessClient = session.client("route53-recovery-readiness")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     GetCellReadinessSummaryPaginator,
     GetReadinessCheckResourceStatusPaginator,
     GetReadinessCheckStatusPaginator,
@@ -49,16 +49,15 @@
     ListCellsResponseTypeDef,
     ListCrossAccountAuthorizationsResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListRulesResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
-    ResourceOutputTypeDef,
-    ResourceTypeDef,
+    ResourceUnionTypeDef,
     UpdateCellResponseTypeDef,
     UpdateReadinessCheckResponseTypeDef,
     UpdateRecoveryGroupResponseTypeDef,
     UpdateResourceSetResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -162,15 +161,15 @@
         """
 
     def create_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
-        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
+        Resources: Sequence[ResourceUnionTypeDef],
         Tags: Mapping[str, str] = ...
     ) -> CreateResourceSetResponseTypeDef:
         """
         Creates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#create_resource_set)
@@ -442,15 +441,15 @@
         """
 
     def update_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
-        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]]
+        Resources: Sequence[ResourceUnionTypeDef]
     ) -> UpdateResourceSetResponseTypeDef:
         """
         Updates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#update_resource_set)
         """
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/client.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_route53_recovery_readiness.client import Route53RecoveryReadinessClient
 
     session = Session()
     client: Route53RecoveryReadinessClient = session.client("route53-recovery-readiness")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     GetCellReadinessSummaryPaginator,
     GetReadinessCheckResourceStatusPaginator,
     GetReadinessCheckStatusPaginator,
@@ -49,16 +49,15 @@
     ListCellsResponseTypeDef,
     ListCrossAccountAuthorizationsResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListRulesResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
-    ResourceOutputTypeDef,
-    ResourceTypeDef,
+    ResourceUnionTypeDef,
     UpdateCellResponseTypeDef,
     UpdateReadinessCheckResponseTypeDef,
     UpdateRecoveryGroupResponseTypeDef,
     UpdateResourceSetResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -151,15 +150,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#create_recovery_group)
         """
     def create_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
-        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
+        Resources: Sequence[ResourceUnionTypeDef],
         Tags: Mapping[str, str] = ...
     ) -> CreateResourceSetResponseTypeDef:
         """
         Creates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#create_resource_set)
@@ -403,15 +402,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#update_recovery_group)
         """
     def update_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
-        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]]
+        Resources: Sequence[ResourceUnionTypeDef]
     ) -> UpdateResourceSetResponseTypeDef:
         """
         Updates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#update_resource_set)
         """
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/literals.py` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/literals.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/paginator.py` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/paginator.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/type_defs.py` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_route53_recovery_readiness.type_defs import CellOutputTypeDef
 
-    data: CellOutputTypeDef = {...}
+    data: CellOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import ReadinessType
@@ -103,17 +103,18 @@
     "DNSTargetResourceTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "CreateResourceSetResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "ResourceSetOutputTypeDef",
     "UpdateResourceSetResponseTypeDef",
+    "ResourceUnionTypeDef",
+    "ListResourceSetsResponseTypeDef",
     "CreateResourceSetRequestRequestTypeDef",
     "UpdateResourceSetRequestRequestTypeDef",
-    "ListResourceSetsResponseTypeDef",
 )
 
 _RequiredCellOutputTypeDef = TypedDict(
     "_RequiredCellOutputTypeDef",
     {
         "CellArn": str,
         "CellName": str,
@@ -1096,20 +1097,30 @@
         "ResourceSetType": str,
         "Resources": List[ResourceOutputTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
+ListResourceSetsResponseTypeDef = TypedDict(
+    "ListResourceSetsResponseTypeDef",
+    {
+        "NextToken": str,
+        "ResourceSets": List[ResourceSetOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
+        "Resources": Sequence[ResourceUnionTypeDef],
     },
 )
 _OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResourceSetRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
@@ -1124,19 +1135,10 @@
 
 
 UpdateResourceSetRequestRequestTypeDef = TypedDict(
     "UpdateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
-    },
-)
-
-ListResourceSetsResponseTypeDef = TypedDict(
-    "ListResourceSetsResponseTypeDef",
-    {
-        "NextToken": str,
-        "ResourceSets": List[ResourceSetOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Resources": Sequence[ResourceUnionTypeDef],
     },
 )
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/type_defs.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_route53_recovery_readiness.type_defs import CellOutputTypeDef
 
-    data: CellOutputTypeDef = {...}
+    data: CellOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import ReadinessType
@@ -102,17 +102,18 @@
     "DNSTargetResourceTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "CreateResourceSetResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "ResourceSetOutputTypeDef",
     "UpdateResourceSetResponseTypeDef",
+    "ResourceUnionTypeDef",
+    "ListResourceSetsResponseTypeDef",
     "CreateResourceSetRequestRequestTypeDef",
     "UpdateResourceSetRequestRequestTypeDef",
-    "ListResourceSetsResponseTypeDef",
 )
 
 _RequiredCellOutputTypeDef = TypedDict(
     "_RequiredCellOutputTypeDef",
     {
         "CellArn": str,
         "CellName": str,
@@ -1061,20 +1062,30 @@
         "ResourceSetType": str,
         "Resources": List[ResourceOutputTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
+ListResourceSetsResponseTypeDef = TypedDict(
+    "ListResourceSetsResponseTypeDef",
+    {
+        "NextToken": str,
+        "ResourceSets": List[ResourceSetOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
+        "Resources": Sequence[ResourceUnionTypeDef],
     },
 )
 _OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResourceSetRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
@@ -1087,19 +1098,10 @@
     pass
 
 UpdateResourceSetRequestRequestTypeDef = TypedDict(
     "UpdateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
-    },
-)
-
-ListResourceSetsResponseTypeDef = TypedDict(
-    "ListResourceSetsResponseTypeDef",
-    {
-        "NextToken": str,
-        "ResourceSets": List[ResourceSetOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Resources": Sequence[ResourceUnionTypeDef],
     },
 )
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 route53-recovery-readiness type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 route53-recovery-readiness type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-readiness)](https://pepy.tech/project/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
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
@@ -354,20 +354,21 @@
 )
 
 
 def check_value(value: GetCellReadinessSummaryPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_route53_recovery_readiness.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_route53_recovery_readiness.type_defs import (
     CellOutputTypeDef,
     CreateCellRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateCrossAccountAuthorizationRequestRequestTypeDef,
@@ -446,21 +447,22 @@
     DNSTargetResourceTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     CreateResourceSetResponseTypeDef,
     GetResourceSetResponseTypeDef,
     ResourceSetOutputTypeDef,
     UpdateResourceSetResponseTypeDef,
+    ResourceUnionTypeDef,
+    ListResourceSetsResponseTypeDef,
     CreateResourceSetRequestRequestTypeDef,
     UpdateResourceSetRequestRequestTypeDef,
-    ListResourceSetsResponseTypeDef,
 )
 
 
-def get_structure() -> CellOutputTypeDef:
+def get_value() -> CellOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt` & `mypy-boto3-route53-recovery-readiness-1.28.16/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.post1/setup.py` & `mypy-boto3-route53-recovery-readiness-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53-recovery-readiness",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_route53_recovery_readiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Route53RecoveryReadiness 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -35,15 +35,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords=(
-        "boto3 route53-recovery-readiness type-annotations boto3-stubs mypy typeshed autocomplete"
+        "boto3 route53-recovery-readiness type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_route53_recovery_readiness": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
```

