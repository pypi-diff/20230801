# Comparing `tmp/mypy-boto3-vpc-lattice-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-vpc-lattice-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-vpc-lattice-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:23 2023, max compression
+gzip compressed data, was "mypy-boto3-vpc-lattice-1.28.16.tar", last modified: Tue Aug  1 11:38:02 2023, max compression
```

## Comparing `mypy-boto3-vpc-lattice-1.28.15.post1.tar` & `mypy-boto3-vpc-lattice-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.849449 mypy-boto3-vpc-lattice-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20328 2023-07-29 10:04:23.845449 mypy-boto3-vpc-lattice-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18820 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.837449 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39132 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39064 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-07-29 10:01:10.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-29 10:01:10.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49473 2023-07-29 10:01:11.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-07-29 10:01:10.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.845449 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20328 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:23.849449 mypy-boto3-vpc-lattice-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:02.944683 mypy-boto3-vpc-lattice-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20373 2023-08-01 11:38:02.944683 mypy-boto3-vpc-lattice-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18874 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:02.944683 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38918 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38850 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49684 2023-08-01 11:34:50.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49635 2023-08-01 11:34:49.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:02.944683 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20373 2023-08-01 11:38:02.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-01 11:38:02.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:02.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:02.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:02.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:38:02.000000 mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:02.944683 mypy-boto3-vpc-lattice-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-01 11:34:48.000000 mypy-boto3-vpc-lattice-1.28.16/setup.py
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/LICENSE` & `mypy-boto3-vpc-lattice-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/PKG-INFO` & `mypy-boto3-vpc-lattice-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.VPCLattice 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 vpc-lattice type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 vpc-lattice type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
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
@@ -356,20 +356,20 @@
 )
 
 
 def check_value(value: AuthPolicyStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_vpc_lattice.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
     ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
@@ -487,34 +487,36 @@
     UpdateTargetGroupRequestRequestTypeDef,
     HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
     UpdateListenerResponseTypeDef,
     CreateListenerRequestRequestTypeDef,
+    RuleActionUnionTypeDef,
     UpdateListenerRequestRequestTypeDef,
     CreateTargetGroupRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
     RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
     UpdateRuleResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     UpdateRuleRequestRequestTypeDef,
     BatchUpdateRuleResponseTypeDef,
     BatchUpdateRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSubscriptionSummaryTypeDef:
+def get_value() -> AccessLogSubscriptionSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/README.md` & `mypy-boto3-vpc-lattice-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
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
@@ -324,20 +324,20 @@
 )
 
 
 def check_value(value: AuthPolicyStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_vpc_lattice.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
     ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
@@ -455,34 +455,36 @@
     UpdateTargetGroupRequestRequestTypeDef,
     HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
     UpdateListenerResponseTypeDef,
     CreateListenerRequestRequestTypeDef,
+    RuleActionUnionTypeDef,
     UpdateListenerRequestRequestTypeDef,
     CreateTargetGroupRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
     RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
     UpdateRuleResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     UpdateRuleRequestRequestTypeDef,
     BatchUpdateRuleResponseTypeDef,
     BatchUpdateRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSubscriptionSummaryTypeDef:
+def get_value() -> AccessLogSubscriptionSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__init__.py` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__init__.pyi` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__main__.py` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VPCLattice 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.VPCLattice 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice\nOther"
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

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/client.py` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_vpc_lattice.client import VPCLatticeClient
 
     session = Session()
     client: VPCLatticeClient = session.client("vpc-lattice")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AuthTypeType, ListenerProtocolType, TargetGroupTypeType
 from .paginator import (
     ListAccessLogSubscriptionsPaginator,
     ListListenersPaginator,
@@ -64,18 +64,16 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
-    RuleActionOutputTypeDef,
-    RuleActionTypeDef,
-    RuleMatchOutputTypeDef,
-    RuleMatchTypeDef,
+    RuleActionUnionTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateServiceNetworkResponseTypeDef,
@@ -170,15 +168,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_access_log_subscription)
         """
 
     def create_listener(
         self,
         *,
-        defaultAction: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
+        defaultAction: RuleActionUnionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateListenerResponseTypeDef:
@@ -188,17 +186,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_listener)
         """
 
     def create_rule(
         self,
         *,
-        action: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
+        action: RuleActionUnionTypeDef,
         listenerIdentifier: str,
-        match: Union[RuleMatchTypeDef, RuleMatchOutputTypeDef],
+        match: RuleMatchUnionTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleResponseTypeDef:
         """
@@ -674,15 +672,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_access_log_subscription)
         """
 
     def update_listener(
         self,
         *,
-        defaultAction: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
+        defaultAction: RuleActionUnionTypeDef,
         listenerIdentifier: str,
         serviceIdentifier: str
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
@@ -691,16 +689,16 @@
 
     def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: Union[RuleActionTypeDef, RuleActionOutputTypeDef] = ...,
-        match: Union[RuleMatchTypeDef, RuleMatchOutputTypeDef] = ...,
+        action: RuleActionUnionTypeDef = ...,
+        match: RuleMatchUnionTypeDef = ...,
         priority: int = ...
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_rule)
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/client.pyi` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_vpc_lattice.client import VPCLatticeClient
 
     session = Session()
     client: VPCLatticeClient = session.client("vpc-lattice")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AuthTypeType, ListenerProtocolType, TargetGroupTypeType
 from .paginator import (
     ListAccessLogSubscriptionsPaginator,
     ListListenersPaginator,
@@ -64,18 +64,16 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
-    RuleActionOutputTypeDef,
-    RuleActionTypeDef,
-    RuleMatchOutputTypeDef,
-    RuleMatchTypeDef,
+    RuleActionUnionTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateServiceNetworkResponseTypeDef,
@@ -161,15 +159,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_access_log_subscription)
         """
     def create_listener(
         self,
         *,
-        defaultAction: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
+        defaultAction: RuleActionUnionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateListenerResponseTypeDef:
@@ -178,17 +176,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_listener)
         """
     def create_rule(
         self,
         *,
-        action: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
+        action: RuleActionUnionTypeDef,
         listenerIdentifier: str,
-        match: Union[RuleMatchTypeDef, RuleMatchOutputTypeDef],
+        match: RuleMatchUnionTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleResponseTypeDef:
         """
@@ -620,15 +618,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_access_log_subscription)
         """
     def update_listener(
         self,
         *,
-        defaultAction: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
+        defaultAction: RuleActionUnionTypeDef,
         listenerIdentifier: str,
         serviceIdentifier: str
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
@@ -636,16 +634,16 @@
         """
     def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: Union[RuleActionTypeDef, RuleActionOutputTypeDef] = ...,
-        match: Union[RuleMatchTypeDef, RuleMatchOutputTypeDef] = ...,
+        action: RuleActionUnionTypeDef = ...,
+        match: RuleMatchUnionTypeDef = ...,
         priority: int = ...
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_rule)
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/literals.py` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/literals.pyi` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/paginator.py` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/paginator.pyi` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/type_defs.py` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_vpc_lattice.type_defs import AccessLogSubscriptionSummaryTypeDef
 
-    data: AccessLogSubscriptionSummaryTypeDef = {...}
+    data: AccessLogSubscriptionSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthPolicyStateType,
     AuthTypeType,
     HealthCheckProtocolVersionType,
     IpAddressTypeType,
     ListenerProtocolType,
@@ -156,26 +156,28 @@
     "UpdateTargetGroupRequestRequestTypeDef",
     "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
     "UpdateListenerResponseTypeDef",
     "CreateListenerRequestRequestTypeDef",
+    "RuleActionUnionTypeDef",
     "UpdateListenerRequestRequestTypeDef",
     "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
     "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
     "UpdateRuleResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
+    "RuleMatchUnionTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
@@ -1676,14 +1678,15 @@
 
 class CreateListenerRequestRequestTypeDef(
     _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
 ):
     pass
 
 
+RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
 UpdateListenerRequestRequestTypeDef = TypedDict(
     "UpdateListenerRequestRequestTypeDef",
     {
         "defaultAction": RuleActionTypeDef,
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
@@ -1853,14 +1856,15 @@
 
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
 
+RuleMatchUnionTypeDef = Union[RuleMatchTypeDef, RuleMatchOutputTypeDef]
 _RequiredRuleUpdateTypeDef = TypedDict(
     "_RequiredRuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
     },
 )
 _OptionalRuleUpdateTypeDef = TypedDict(
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/type_defs.pyi` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_vpc_lattice.type_defs import AccessLogSubscriptionSummaryTypeDef
 
-    data: AccessLogSubscriptionSummaryTypeDef = {...}
+    data: AccessLogSubscriptionSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthPolicyStateType,
     AuthTypeType,
     HealthCheckProtocolVersionType,
     IpAddressTypeType,
     ListenerProtocolType,
@@ -155,26 +155,28 @@
     "UpdateTargetGroupRequestRequestTypeDef",
     "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
     "UpdateListenerResponseTypeDef",
     "CreateListenerRequestRequestTypeDef",
+    "RuleActionUnionTypeDef",
     "UpdateListenerRequestRequestTypeDef",
     "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
     "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
     "UpdateRuleResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
+    "RuleMatchUnionTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
@@ -1635,14 +1637,15 @@
 )
 
 class CreateListenerRequestRequestTypeDef(
     _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
 ):
     pass
 
+RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
 UpdateListenerRequestRequestTypeDef = TypedDict(
     "UpdateListenerRequestRequestTypeDef",
     {
         "defaultAction": RuleActionTypeDef,
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
@@ -1808,14 +1811,15 @@
 )
 
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
+RuleMatchUnionTypeDef = Union[RuleMatchTypeDef, RuleMatchOutputTypeDef]
 _RequiredRuleUpdateTypeDef = TypedDict(
     "_RequiredRuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
     },
 )
 _OptionalRuleUpdateTypeDef = TypedDict(
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/PKG-INFO` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.VPCLattice 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 vpc-lattice type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 vpc-lattice type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
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
@@ -356,20 +356,20 @@
 )
 
 
 def check_value(value: AuthPolicyStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_vpc_lattice.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
     ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
@@ -487,34 +487,36 @@
     UpdateTargetGroupRequestRequestTypeDef,
     HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
     UpdateListenerResponseTypeDef,
     CreateListenerRequestRequestTypeDef,
+    RuleActionUnionTypeDef,
     UpdateListenerRequestRequestTypeDef,
     CreateTargetGroupRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
     RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
     UpdateRuleResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     UpdateRuleRequestRequestTypeDef,
     BatchUpdateRuleResponseTypeDef,
     BatchUpdateRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSubscriptionSummaryTypeDef:
+def get_value() -> AccessLogSubscriptionSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt` & `mypy-boto3-vpc-lattice-1.28.16/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15.post1/setup.py` & `mypy-boto3-vpc-lattice-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-vpc-lattice",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.VPCLattice 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 vpc-lattice type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 vpc-lattice type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_vpc_lattice": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

