# Comparing `tmp/mypy-boto3-managedblockchain-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-managedblockchain-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-managedblockchain-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:37 2023, max compression
+gzip compressed data, was "mypy-boto3-managedblockchain-1.28.16.tar", last modified: Tue Aug  1 11:37:17 2023, max compression
```

## Comparing `mypy-boto3-managedblockchain-1.28.15.post1.tar` & `mypy-boto3-managedblockchain-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.177269 mypy-boto3-managedblockchain-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:28.000000 mypy-boto3-managedblockchain-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16181 2023-07-29 10:03:37.173269 mypy-boto3-managedblockchain-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-07-29 09:50:28.000000 mypy-boto3-managedblockchain-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.161269 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-29 09:50:28.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-29 09:50:28.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-29 09:50:28.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20672 2023-07-29 09:50:29.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20637 2023-07-29 09:50:29.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-07-29 09:50:29.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-07-29 09:50:29.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-29 09:50:29.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-29 09:50:29.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:28.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26645 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:28.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.173269 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16181 2023-07-29 10:03:36.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 10:03:36.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:36.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:36.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:36.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:03:36.000000 mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:37.177269 mypy-boto3-managedblockchain-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-29 09:50:28.000000 mypy-boto3-managedblockchain-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.148829 mypy-boto3-managedblockchain-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-08-01 11:37:17.148829 mypy-boto3-managedblockchain-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.144829 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20604 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20569 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-08-01 11:23:24.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26804 2023-08-01 11:23:24.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26775 2023-08-01 11:23:24.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.148829 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-08-01 11:37:16.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 11:37:16.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:16.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:16.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:16.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:37:16.000000 mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:17.148829 mypy-boto3-managedblockchain-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-01 11:23:23.000000 mypy-boto3-managedblockchain-1.28.16/setup.py
```

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/LICENSE` & `mypy-boto3-managedblockchain-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/PKG-INFO` & `mypy-boto3-managedblockchain-1.28.16/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-managedblockchain
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ManagedBlockchain 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +42,15 @@
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
@@ -323,20 +291,20 @@
 )
 
 
 def check_value(value: AccessorStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_managedblockchain.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
@@ -403,14 +371,15 @@
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
     ProposalTypeDef,
     CreateProposalInputRequestTypeDef,
+    ProposalActionsUnionTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
     MemberConfigurationTypeDef,
     MemberTypeDef,
     UpdateMemberInputRequestTypeDef,
@@ -421,15 +390,15 @@
     CreateNetworkInputRequestTypeDef,
     GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
     GetNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AccessorSummaryTypeDef:
+def get_value() -> AccessorSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/README.md` & `mypy-boto3-managedblockchain-1.28.16/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-managedblockchain
+Version: 1.28.16
+Summary: Type annotations for boto3.ManagedBlockchain 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 managedblockchain type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +74,15 @@
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
@@ -291,20 +323,20 @@
 )
 
 
 def check_value(value: AccessorStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_managedblockchain.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
@@ -371,14 +403,15 @@
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
     ProposalTypeDef,
     CreateProposalInputRequestTypeDef,
+    ProposalActionsUnionTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
     MemberConfigurationTypeDef,
     MemberTypeDef,
     UpdateMemberInputRequestTypeDef,
@@ -389,15 +422,15 @@
     CreateNetworkInputRequestTypeDef,
     GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
     GetNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AccessorSummaryTypeDef:
+def get_value() -> AccessorSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/__init__.py` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/__init__.pyi` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/__main__.py` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedBlockchain 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ManagedBlockchain 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
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

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/client.py` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_managedblockchain.client import ManagedBlockchainClient
 
     session = Session()
     client: ManagedBlockchainClient = session.client("managedblockchain")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     FrameworkType,
     MemberStatusType,
     NetworkStatusType,
@@ -46,16 +46,15 @@
     ListProposalVotesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberConfigurationTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
-    ProposalActionsOutputTypeDef,
-    ProposalActionsTypeDef,
+    ProposalActionsUnionTypeDef,
     VotingPolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -186,15 +185,15 @@
 
     def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
-        Actions: Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef],
+        Actions: ProposalActionsUnionTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the network
         can vote on, for example, a proposal to add a new member to the network.
```

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/client.pyi` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_managedblockchain.client import ManagedBlockchainClient
 
     session = Session()
     client: ManagedBlockchainClient = session.client("managedblockchain")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     FrameworkType,
     MemberStatusType,
     NetworkStatusType,
@@ -46,16 +46,15 @@
     ListProposalVotesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberConfigurationTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
-    ProposalActionsOutputTypeDef,
-    ProposalActionsTypeDef,
+    ProposalActionsUnionTypeDef,
     VotingPolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -175,15 +174,15 @@
         """
     def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
-        Actions: Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef],
+        Actions: ProposalActionsUnionTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the network
         can vote on, for example, a proposal to add a new member to the network.
```

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/literals.py` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/literals.pyi` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/paginator.py` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/paginator.pyi` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/type_defs.py` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_managedblockchain.type_defs import AccessorSummaryTypeDef
 
-    data: AccessorSummaryTypeDef = {...}
+    data: AccessorSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessorStatusType,
     EditionType,
     FrameworkType,
     InvitationStatusType,
     MemberStatusType,
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
@@ -107,14 +106,15 @@
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
     "ProposalTypeDef",
     "CreateProposalInputRequestTypeDef",
+    "ProposalActionsUnionTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
     "MemberConfigurationTypeDef",
     "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
@@ -175,21 +175,19 @@
     "_OptionalCreateAccessorInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -223,21 +221,19 @@
     "_OptionalDeleteNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
-
 class DeleteNodeInputRequestTypeDef(
     _RequiredDeleteNodeInputRequestTypeDef, _OptionalDeleteNodeInputRequestTypeDef
 ):
     pass
 
-
 GetAccessorInputRequestTypeDef = TypedDict(
     "GetAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
     },
 )
 
@@ -267,21 +263,19 @@
     "_OptionalGetNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
-
 class GetNodeInputRequestTypeDef(
     _RequiredGetNodeInputRequestTypeDef, _OptionalGetNodeInputRequestTypeDef
 ):
     pass
 
-
 GetProposalInputRequestTypeDef = TypedDict(
     "GetProposalInputRequestTypeDef",
     {
         "NetworkId": str,
         "ProposalId": str,
     },
 )
@@ -350,21 +344,19 @@
         "IsOwned": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListMembersInputRequestTypeDef(
     _RequiredListMembersInputRequestTypeDef, _OptionalListMembersInputRequestTypeDef
 ):
     pass
 
-
 MemberSummaryTypeDef = TypedDict(
     "MemberSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": MemberStatusType,
@@ -400,21 +392,19 @@
         "Status": NodeStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListNodesInputRequestTypeDef(
     _RequiredListNodesInputRequestTypeDef, _OptionalListNodesInputRequestTypeDef
 ):
     pass
 
-
 NodeSummaryTypeDef = TypedDict(
     "NodeSummaryTypeDef",
     {
         "Id": str,
         "Status": NodeStatusType,
         "CreationDate": datetime,
         "AvailabilityZone": str,
@@ -436,21 +426,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProposalVotesInputRequestTypeDef(
     _RequiredListProposalVotesInputRequestTypeDef, _OptionalListProposalVotesInputRequestTypeDef
 ):
     pass
 
-
 VoteSummaryTypeDef = TypedDict(
     "VoteSummaryTypeDef",
     {
         "Vote": VoteValueType,
         "MemberName": str,
         "MemberId": str,
     },
@@ -468,21 +456,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProposalsInputRequestTypeDef(
     _RequiredListProposalsInputRequestTypeDef, _OptionalListProposalsInputRequestTypeDef
 ):
     pass
 
-
 ProposalSummaryTypeDef = TypedDict(
     "ProposalSummaryTypeDef",
     {
         "ProposalId": str,
         "Description": str,
         "ProposedByMemberId": str,
         "ProposedByMemberName": str,
@@ -897,21 +883,20 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
-
+ProposalActionsUnionTypeDef = Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef]
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": MemberFabricLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
@@ -954,21 +939,19 @@
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
         "Tags": Mapping[str, str],
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-
 class MemberConfigurationTypeDef(
     _RequiredMemberConfigurationTypeDef, _OptionalMemberConfigurationTypeDef
 ):
     pass
 
-
 MemberTypeDef = TypedDict(
     "MemberTypeDef",
     {
         "NetworkId": str,
         "Id": str,
         "Name": str,
         "Description": str,
@@ -994,21 +977,19 @@
     "_OptionalUpdateMemberInputRequestTypeDef",
     {
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMemberInputRequestTypeDef(
     _RequiredUpdateMemberInputRequestTypeDef, _OptionalUpdateMemberInputRequestTypeDef
 ):
     pass
 
-
 _RequiredNodeConfigurationTypeDef = TypedDict(
     "_RequiredNodeConfigurationTypeDef",
     {
         "InstanceType": str,
     },
 )
 _OptionalNodeConfigurationTypeDef = TypedDict(
@@ -1017,21 +998,19 @@
         "AvailabilityZone": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
         "StateDB": StateDBTypeType,
     },
     total=False,
 )
 
-
 class NodeConfigurationTypeDef(
     _RequiredNodeConfigurationTypeDef, _OptionalNodeConfigurationTypeDef
 ):
     pass
 
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NetworkId": str,
         "MemberId": str,
         "Id": str,
         "InstanceType": str,
@@ -1060,21 +1039,19 @@
     {
         "MemberId": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateNodeInputRequestTypeDef(
     _RequiredUpdateNodeInputRequestTypeDef, _OptionalUpdateNodeInputRequestTypeDef
 ):
     pass
 
-
 CreateMemberInputRequestTypeDef = TypedDict(
     "CreateMemberInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "InvitationId": str,
         "NetworkId": str,
         "MemberConfiguration": MemberConfigurationTypeDef,
@@ -1098,21 +1075,19 @@
         "Description": str,
         "FrameworkConfiguration": NetworkFrameworkConfigurationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateNetworkInputRequestTypeDef(
     _RequiredCreateNetworkInputRequestTypeDef, _OptionalCreateNetworkInputRequestTypeDef
 ):
     pass
 
-
 GetMemberOutputTypeDef = TypedDict(
     "GetMemberOutputTypeDef",
     {
         "Member": MemberTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1130,21 +1105,19 @@
     {
         "MemberId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateNodeInputRequestTypeDef(
     _RequiredCreateNodeInputRequestTypeDef, _OptionalCreateNodeInputRequestTypeDef
 ):
     pass
 
-
 GetNodeOutputTypeDef = TypedDict(
     "GetNodeOutputTypeDef",
     {
         "Node": NodeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain/type_defs.pyi` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_managedblockchain.type_defs import AccessorSummaryTypeDef
 
-    data: AccessorSummaryTypeDef = {...}
+    data: AccessorSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessorStatusType,
     EditionType,
     FrameworkType,
     InvitationStatusType,
     MemberStatusType,
@@ -34,14 +34,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
@@ -106,14 +107,15 @@
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
     "ProposalTypeDef",
     "CreateProposalInputRequestTypeDef",
+    "ProposalActionsUnionTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
     "MemberConfigurationTypeDef",
     "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
@@ -174,19 +176,21 @@
     "_OptionalCreateAccessorInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -220,19 +224,21 @@
     "_OptionalDeleteNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
+
 class DeleteNodeInputRequestTypeDef(
     _RequiredDeleteNodeInputRequestTypeDef, _OptionalDeleteNodeInputRequestTypeDef
 ):
     pass
 
+
 GetAccessorInputRequestTypeDef = TypedDict(
     "GetAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
     },
 )
 
@@ -262,19 +268,21 @@
     "_OptionalGetNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
+
 class GetNodeInputRequestTypeDef(
     _RequiredGetNodeInputRequestTypeDef, _OptionalGetNodeInputRequestTypeDef
 ):
     pass
 
+
 GetProposalInputRequestTypeDef = TypedDict(
     "GetProposalInputRequestTypeDef",
     {
         "NetworkId": str,
         "ProposalId": str,
     },
 )
@@ -343,19 +351,21 @@
         "IsOwned": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListMembersInputRequestTypeDef(
     _RequiredListMembersInputRequestTypeDef, _OptionalListMembersInputRequestTypeDef
 ):
     pass
 
+
 MemberSummaryTypeDef = TypedDict(
     "MemberSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": MemberStatusType,
@@ -391,19 +401,21 @@
         "Status": NodeStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListNodesInputRequestTypeDef(
     _RequiredListNodesInputRequestTypeDef, _OptionalListNodesInputRequestTypeDef
 ):
     pass
 
+
 NodeSummaryTypeDef = TypedDict(
     "NodeSummaryTypeDef",
     {
         "Id": str,
         "Status": NodeStatusType,
         "CreationDate": datetime,
         "AvailabilityZone": str,
@@ -425,19 +437,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProposalVotesInputRequestTypeDef(
     _RequiredListProposalVotesInputRequestTypeDef, _OptionalListProposalVotesInputRequestTypeDef
 ):
     pass
 
+
 VoteSummaryTypeDef = TypedDict(
     "VoteSummaryTypeDef",
     {
         "Vote": VoteValueType,
         "MemberName": str,
         "MemberId": str,
     },
@@ -455,19 +469,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProposalsInputRequestTypeDef(
     _RequiredListProposalsInputRequestTypeDef, _OptionalListProposalsInputRequestTypeDef
 ):
     pass
 
+
 ProposalSummaryTypeDef = TypedDict(
     "ProposalSummaryTypeDef",
     {
         "ProposalId": str,
         "Description": str,
         "ProposedByMemberId": str,
         "ProposedByMemberName": str,
@@ -882,19 +898,22 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
+
+ProposalActionsUnionTypeDef = Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef]
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": MemberFabricLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
@@ -937,19 +956,21 @@
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
         "Tags": Mapping[str, str],
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+
 class MemberConfigurationTypeDef(
     _RequiredMemberConfigurationTypeDef, _OptionalMemberConfigurationTypeDef
 ):
     pass
 
+
 MemberTypeDef = TypedDict(
     "MemberTypeDef",
     {
         "NetworkId": str,
         "Id": str,
         "Name": str,
         "Description": str,
@@ -975,19 +996,21 @@
     "_OptionalUpdateMemberInputRequestTypeDef",
     {
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMemberInputRequestTypeDef(
     _RequiredUpdateMemberInputRequestTypeDef, _OptionalUpdateMemberInputRequestTypeDef
 ):
     pass
 
+
 _RequiredNodeConfigurationTypeDef = TypedDict(
     "_RequiredNodeConfigurationTypeDef",
     {
         "InstanceType": str,
     },
 )
 _OptionalNodeConfigurationTypeDef = TypedDict(
@@ -996,19 +1019,21 @@
         "AvailabilityZone": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
         "StateDB": StateDBTypeType,
     },
     total=False,
 )
 
+
 class NodeConfigurationTypeDef(
     _RequiredNodeConfigurationTypeDef, _OptionalNodeConfigurationTypeDef
 ):
     pass
 
+
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NetworkId": str,
         "MemberId": str,
         "Id": str,
         "InstanceType": str,
@@ -1037,19 +1062,21 @@
     {
         "MemberId": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateNodeInputRequestTypeDef(
     _RequiredUpdateNodeInputRequestTypeDef, _OptionalUpdateNodeInputRequestTypeDef
 ):
     pass
 
+
 CreateMemberInputRequestTypeDef = TypedDict(
     "CreateMemberInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "InvitationId": str,
         "NetworkId": str,
         "MemberConfiguration": MemberConfigurationTypeDef,
@@ -1073,19 +1100,21 @@
         "Description": str,
         "FrameworkConfiguration": NetworkFrameworkConfigurationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateNetworkInputRequestTypeDef(
     _RequiredCreateNetworkInputRequestTypeDef, _OptionalCreateNetworkInputRequestTypeDef
 ):
     pass
 
+
 GetMemberOutputTypeDef = TypedDict(
     "GetMemberOutputTypeDef",
     {
         "Member": MemberTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1103,19 +1132,21 @@
     {
         "MemberId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateNodeInputRequestTypeDef(
     _RequiredCreateNodeInputRequestTypeDef, _OptionalCreateNodeInputRequestTypeDef
 ):
     pass
 
+
 GetNodeOutputTypeDef = TypedDict(
     "GetNodeOutputTypeDef",
     {
         "Node": NodeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain.egg-info/PKG-INFO` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ManagedBlockchain 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ManagedBlockchain 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 managedblockchain type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
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
@@ -323,20 +323,20 @@
 )
 
 
 def check_value(value: AccessorStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_managedblockchain.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
@@ -403,14 +403,15 @@
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
     ProposalTypeDef,
     CreateProposalInputRequestTypeDef,
+    ProposalActionsUnionTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
     MemberConfigurationTypeDef,
     MemberTypeDef,
     UpdateMemberInputRequestTypeDef,
@@ -421,15 +422,15 @@
     CreateNetworkInputRequestTypeDef,
     GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
     GetNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AccessorSummaryTypeDef:
+def get_value() -> AccessorSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/mypy_boto3_managedblockchain.egg-info/SOURCES.txt` & `mypy-boto3-managedblockchain-1.28.16/mypy_boto3_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.15.post1/setup.py` & `mypy-boto3-managedblockchain-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-managedblockchain",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedBlockchain 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ManagedBlockchain 1.28.16 service generated with"
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
-    keywords="boto3 managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 managedblockchain type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_managedblockchain": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

