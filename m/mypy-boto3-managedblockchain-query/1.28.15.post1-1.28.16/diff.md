# Comparing `tmp/mypy-boto3-managedblockchain-query-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-managedblockchain-query-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-managedblockchain-query-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:37 2023, max compression
+gzip compressed data, was "mypy-boto3-managedblockchain-query-1.28.16.tar", last modified: Tue Aug  1 11:37:17 2023, max compression
```

## Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1.tar` & `mypy-boto3-managedblockchain-query-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.441270 mypy-boto3-managedblockchain-query-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-07-29 10:03:37.441270 mypy-boto3-managedblockchain-query-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.437270 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-07-29 09:50:33.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-29 09:50:33.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-29 09:50:33.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-29 09:50:33.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-29 09:50:33.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-29 09:50:33.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-07-29 09:50:33.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.441270 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-07-29 10:03:37.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-29 10:03:37.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:37.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:37.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:37.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 10:03:37.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:37.441270 mypy-boto3-managedblockchain-query-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-29 09:50:32.000000 mypy-boto3-managedblockchain-query-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.276828 mypy-boto3-managedblockchain-query-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-08-01 11:37:17.276828 mypy-boto3-managedblockchain-query-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.268828 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-08-01 11:23:26.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.276828 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-08-01 11:37:17.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 11:37:17.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:17.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:17.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:17.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 11:37:17.000000 mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:17.276828 mypy-boto3-managedblockchain-query-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-01 11:23:25.000000 mypy-boto3-managedblockchain-query-1.28.16/setup.py
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/LICENSE` & `mypy-boto3-managedblockchain-query-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/PKG-INFO` & `mypy-boto3-managedblockchain-query-1.28.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain-query
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ManagedBlockchainQuery 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ManagedBlockchainQuery 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 managedblockchain-query type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 managedblockchain-query type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain-query)](https://pepy.tech/project/mypy-boto3-managedblockchain-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchainQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
+[boto3.ManagedBlockchainQuery 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
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
 [mypy-boto3-managedblockchain-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/).
 
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
@@ -328,58 +328,60 @@
 )
 
 
 def check_value(value: ErrorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_managedblockchain_query.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain_query.type_defs import (
     BlockchainInstantOutputTypeDef,
     OwnerIdentifierTypeDef,
     TokenIdentifierTypeDef,
-    BlockchainInstantTypeDef,
     ResponseMetadataTypeDef,
+    TimestampTypeDef,
     GetTransactionInputRequestTypeDef,
     TransactionTypeDef,
     OwnerFilterTypeDef,
     PaginatorConfigTypeDef,
     TokenFilterTypeDef,
     ListTransactionEventsInputRequestTypeDef,
     TransactionEventTypeDef,
     ListTransactionsSortTypeDef,
     TransactionOutputItemTypeDef,
     BatchGetTokenBalanceErrorItemTypeDef,
     BatchGetTokenBalanceOutputItemTypeDef,
     TokenBalanceTypeDef,
-    BatchGetTokenBalanceInputItemTypeDef,
-    GetTokenBalanceInputRequestTypeDef,
     GetTokenBalanceOutputTypeDef,
+    BlockchainInstantTypeDef,
     GetTransactionOutputTypeDef,
     ListTransactionEventsInputListTransactionEventsPaginateTypeDef,
     ListTokenBalancesInputListTokenBalancesPaginateTypeDef,
     ListTokenBalancesInputRequestTypeDef,
     ListTransactionEventsOutputTypeDef,
-    ListTransactionsInputListTransactionsPaginateTypeDef,
-    ListTransactionsInputRequestTypeDef,
     ListTransactionsOutputTypeDef,
     BatchGetTokenBalanceOutputTypeDef,
     ListTokenBalancesOutputTypeDef,
+    BatchGetTokenBalanceInputItemTypeDef,
+    BlockchainInstantUnionTypeDef,
+    GetTokenBalanceInputRequestTypeDef,
+    ListTransactionsInputListTransactionsPaginateTypeDef,
+    ListTransactionsInputRequestTypeDef,
     BatchGetTokenBalanceInputRequestTypeDef,
 )
 
 
-def get_structure() -> BlockchainInstantOutputTypeDef:
+def get_value() -> BlockchainInstantOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/README.md` & `mypy-boto3-managedblockchain-query-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain-query)](https://pepy.tech/project/mypy-boto3-managedblockchain-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchainQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
+[boto3.ManagedBlockchainQuery 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
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
 [mypy-boto3-managedblockchain-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/).
 
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
@@ -296,58 +296,60 @@
 )
 
 
 def check_value(value: ErrorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_managedblockchain_query.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain_query.type_defs import (
     BlockchainInstantOutputTypeDef,
     OwnerIdentifierTypeDef,
     TokenIdentifierTypeDef,
-    BlockchainInstantTypeDef,
     ResponseMetadataTypeDef,
+    TimestampTypeDef,
     GetTransactionInputRequestTypeDef,
     TransactionTypeDef,
     OwnerFilterTypeDef,
     PaginatorConfigTypeDef,
     TokenFilterTypeDef,
     ListTransactionEventsInputRequestTypeDef,
     TransactionEventTypeDef,
     ListTransactionsSortTypeDef,
     TransactionOutputItemTypeDef,
     BatchGetTokenBalanceErrorItemTypeDef,
     BatchGetTokenBalanceOutputItemTypeDef,
     TokenBalanceTypeDef,
-    BatchGetTokenBalanceInputItemTypeDef,
-    GetTokenBalanceInputRequestTypeDef,
     GetTokenBalanceOutputTypeDef,
+    BlockchainInstantTypeDef,
     GetTransactionOutputTypeDef,
     ListTransactionEventsInputListTransactionEventsPaginateTypeDef,
     ListTokenBalancesInputListTokenBalancesPaginateTypeDef,
     ListTokenBalancesInputRequestTypeDef,
     ListTransactionEventsOutputTypeDef,
-    ListTransactionsInputListTransactionsPaginateTypeDef,
-    ListTransactionsInputRequestTypeDef,
     ListTransactionsOutputTypeDef,
     BatchGetTokenBalanceOutputTypeDef,
     ListTokenBalancesOutputTypeDef,
+    BatchGetTokenBalanceInputItemTypeDef,
+    BlockchainInstantUnionTypeDef,
+    GetTokenBalanceInputRequestTypeDef,
+    ListTransactionsInputListTransactionsPaginateTypeDef,
+    ListTransactionsInputRequestTypeDef,
     BatchGetTokenBalanceInputRequestTypeDef,
 )
 
 
-def get_structure() -> BlockchainInstantOutputTypeDef:
+def get_value() -> BlockchainInstantOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/__init__.py` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/__init__.pyi` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/__main__.py` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedBlockchainQuery 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ManagedBlockchainQuery 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery\nOther"
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

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/client.py` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,28 @@
     from mypy_boto3_managedblockchain_query.client import ManagedBlockchainQueryClient
 
     session = Session()
     client: ManagedBlockchainQueryClient = session.client("managedblockchain-query")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import QueryNetworkType
 from .paginator import (
     ListTokenBalancesPaginator,
     ListTransactionEventsPaginator,
     ListTransactionsPaginator,
 )
 from .type_defs import (
     BatchGetTokenBalanceInputItemTypeDef,
     BatchGetTokenBalanceOutputTypeDef,
-    BlockchainInstantOutputTypeDef,
-    BlockchainInstantTypeDef,
+    BlockchainInstantUnionTypeDef,
     GetTokenBalanceOutputTypeDef,
     GetTransactionOutputTypeDef,
     ListTokenBalancesOutputTypeDef,
     ListTransactionEventsOutputTypeDef,
     ListTransactionsOutputTypeDef,
     ListTransactionsSortTypeDef,
     OwnerFilterTypeDef,
@@ -127,15 +126,15 @@
         """
 
     def get_token_balance(
         self,
         *,
         tokenIdentifier: TokenIdentifierTypeDef,
         ownerIdentifier: OwnerIdentifierTypeDef,
-        atBlockchainInstant: Union[BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef] = ...
+        atBlockchainInstant: BlockchainInstantUnionTypeDef = ...
     ) -> GetTokenBalanceOutputTypeDef:
         """
         Gets the balance of a specific token, including native tokens, for a given
         address (wallet or contract) on the blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.get_token_balance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/client/#get_token_balance)
@@ -184,18 +183,16 @@
         """
 
     def list_transactions(
         self,
         *,
         address: str,
         network: QueryNetworkType,
-        fromBlockchainInstant: Union[
-            BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef
-        ] = ...,
-        toBlockchainInstant: Union[BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef] = ...,
+        fromBlockchainInstant: BlockchainInstantUnionTypeDef = ...,
+        toBlockchainInstant: BlockchainInstantUnionTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListTransactionsOutputTypeDef:
         """
         Lists all of the transactions on a given wallet address or to a specific
         contract.
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/client.pyi` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,28 @@
     from mypy_boto3_managedblockchain_query.client import ManagedBlockchainQueryClient
 
     session = Session()
     client: ManagedBlockchainQueryClient = session.client("managedblockchain-query")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import QueryNetworkType
 from .paginator import (
     ListTokenBalancesPaginator,
     ListTransactionEventsPaginator,
     ListTransactionsPaginator,
 )
 from .type_defs import (
     BatchGetTokenBalanceInputItemTypeDef,
     BatchGetTokenBalanceOutputTypeDef,
-    BlockchainInstantOutputTypeDef,
-    BlockchainInstantTypeDef,
+    BlockchainInstantUnionTypeDef,
     GetTokenBalanceOutputTypeDef,
     GetTransactionOutputTypeDef,
     ListTokenBalancesOutputTypeDef,
     ListTransactionEventsOutputTypeDef,
     ListTransactionsOutputTypeDef,
     ListTransactionsSortTypeDef,
     OwnerFilterTypeDef,
@@ -118,15 +117,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/client/#generate_presigned_url)
         """
     def get_token_balance(
         self,
         *,
         tokenIdentifier: TokenIdentifierTypeDef,
         ownerIdentifier: OwnerIdentifierTypeDef,
-        atBlockchainInstant: Union[BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef] = ...
+        atBlockchainInstant: BlockchainInstantUnionTypeDef = ...
     ) -> GetTokenBalanceOutputTypeDef:
         """
         Gets the balance of a specific token, including native tokens, for a given
         address (wallet or contract) on the blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.get_token_balance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/client/#get_token_balance)
@@ -171,18 +170,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/client/#list_transaction_events)
         """
     def list_transactions(
         self,
         *,
         address: str,
         network: QueryNetworkType,
-        fromBlockchainInstant: Union[
-            BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef
-        ] = ...,
-        toBlockchainInstant: Union[BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef] = ...,
+        fromBlockchainInstant: BlockchainInstantUnionTypeDef = ...,
+        toBlockchainInstant: BlockchainInstantUnionTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListTransactionsOutputTypeDef:
         """
         Lists all of the transactions on a given wallet address or to a specific
         contract.
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/literals.py` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/literals.pyi` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/paginator.py` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,21 @@
     client: ManagedBlockchainQueryClient = session.client("managedblockchain-query")
 
     list_token_balances_paginator: ListTokenBalancesPaginator = client.get_paginator("list_token_balances")
     list_transaction_events_paginator: ListTransactionEventsPaginator = client.get_paginator("list_transaction_events")
     list_transactions_paginator: ListTransactionsPaginator = client.get_paginator("list_transactions")
     ```
 """
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import QueryNetworkType
 from .type_defs import (
-    BlockchainInstantOutputTypeDef,
-    BlockchainInstantTypeDef,
+    BlockchainInstantUnionTypeDef,
     ListTokenBalancesOutputTypeDef,
     ListTransactionEventsOutputTypeDef,
     ListTransactionsOutputTypeDef,
     ListTransactionsSortTypeDef,
     OwnerFilterTypeDef,
     PaginatorConfigTypeDef,
     TokenFilterTypeDef,
@@ -102,18 +101,16 @@
     """
 
     def paginate(
         self,
         *,
         address: str,
         network: QueryNetworkType,
-        fromBlockchainInstant: Union[
-            BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef
-        ] = ...,
-        toBlockchainInstant: Union[BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef] = ...,
+        fromBlockchainInstant: BlockchainInstantUnionTypeDef = ...,
+        toBlockchainInstant: BlockchainInstantUnionTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTransactionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/paginators/#listtransactionspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/paginator.pyi` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,21 @@
     client: ManagedBlockchainQueryClient = session.client("managedblockchain-query")
 
     list_token_balances_paginator: ListTokenBalancesPaginator = client.get_paginator("list_token_balances")
     list_transaction_events_paginator: ListTransactionEventsPaginator = client.get_paginator("list_transaction_events")
     list_transactions_paginator: ListTransactionsPaginator = client.get_paginator("list_transactions")
     ```
 """
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import QueryNetworkType
 from .type_defs import (
-    BlockchainInstantOutputTypeDef,
-    BlockchainInstantTypeDef,
+    BlockchainInstantUnionTypeDef,
     ListTokenBalancesOutputTypeDef,
     ListTransactionEventsOutputTypeDef,
     ListTransactionsOutputTypeDef,
     ListTransactionsSortTypeDef,
     OwnerFilterTypeDef,
     PaginatorConfigTypeDef,
     TokenFilterTypeDef,
@@ -97,18 +96,16 @@
     """
 
     def paginate(
         self,
         *,
         address: str,
         network: QueryNetworkType,
-        fromBlockchainInstant: Union[
-            BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef
-        ] = ...,
-        toBlockchainInstant: Union[BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef] = ...,
+        fromBlockchainInstant: BlockchainInstantUnionTypeDef = ...,
+        toBlockchainInstant: BlockchainInstantUnionTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTransactionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/paginators/#listtransactionspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/type_defs.py` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_managedblockchain_query.type_defs import BlockchainInstantOutputTypeDef
 
-    data: BlockchainInstantOutputTypeDef = {...}
+    data: BlockchainInstantOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -33,41 +33,43 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BlockchainInstantOutputTypeDef",
     "OwnerIdentifierTypeDef",
     "TokenIdentifierTypeDef",
-    "BlockchainInstantTypeDef",
     "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "GetTransactionInputRequestTypeDef",
     "TransactionTypeDef",
     "OwnerFilterTypeDef",
     "PaginatorConfigTypeDef",
     "TokenFilterTypeDef",
     "ListTransactionEventsInputRequestTypeDef",
     "TransactionEventTypeDef",
     "ListTransactionsSortTypeDef",
     "TransactionOutputItemTypeDef",
     "BatchGetTokenBalanceErrorItemTypeDef",
     "BatchGetTokenBalanceOutputItemTypeDef",
     "TokenBalanceTypeDef",
-    "BatchGetTokenBalanceInputItemTypeDef",
-    "GetTokenBalanceInputRequestTypeDef",
     "GetTokenBalanceOutputTypeDef",
+    "BlockchainInstantTypeDef",
     "GetTransactionOutputTypeDef",
     "ListTransactionEventsInputListTransactionEventsPaginateTypeDef",
     "ListTokenBalancesInputListTokenBalancesPaginateTypeDef",
     "ListTokenBalancesInputRequestTypeDef",
     "ListTransactionEventsOutputTypeDef",
-    "ListTransactionsInputListTransactionsPaginateTypeDef",
-    "ListTransactionsInputRequestTypeDef",
     "ListTransactionsOutputTypeDef",
     "BatchGetTokenBalanceOutputTypeDef",
     "ListTokenBalancesOutputTypeDef",
+    "BatchGetTokenBalanceInputItemTypeDef",
+    "BlockchainInstantUnionTypeDef",
+    "GetTokenBalanceInputRequestTypeDef",
+    "ListTransactionsInputListTransactionsPaginateTypeDef",
+    "ListTransactionsInputRequestTypeDef",
     "BatchGetTokenBalanceInputRequestTypeDef",
 )
 
 BlockchainInstantOutputTypeDef = TypedDict(
     "BlockchainInstantOutputTypeDef",
     {
         "time": datetime,
@@ -98,33 +100,26 @@
 )
 
 
 class TokenIdentifierTypeDef(_RequiredTokenIdentifierTypeDef, _OptionalTokenIdentifierTypeDef):
     pass
 
 
-BlockchainInstantTypeDef = TypedDict(
-    "BlockchainInstantTypeDef",
-    {
-        "time": Union[datetime, str],
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 GetTransactionInputRequestTypeDef = TypedDict(
     "GetTransactionInputRequestTypeDef",
     {
         "transactionHash": str,
         "network": QueryNetworkType,
     },
 )
@@ -338,70 +333,34 @@
 )
 
 
 class TokenBalanceTypeDef(_RequiredTokenBalanceTypeDef, _OptionalTokenBalanceTypeDef):
     pass
 
 
-_RequiredBatchGetTokenBalanceInputItemTypeDef = TypedDict(
-    "_RequiredBatchGetTokenBalanceInputItemTypeDef",
-    {
-        "tokenIdentifier": TokenIdentifierTypeDef,
-        "ownerIdentifier": OwnerIdentifierTypeDef,
-    },
-)
-_OptionalBatchGetTokenBalanceInputItemTypeDef = TypedDict(
-    "_OptionalBatchGetTokenBalanceInputItemTypeDef",
-    {
-        "atBlockchainInstant": BlockchainInstantTypeDef,
-    },
-    total=False,
-)
-
-
-class BatchGetTokenBalanceInputItemTypeDef(
-    _RequiredBatchGetTokenBalanceInputItemTypeDef, _OptionalBatchGetTokenBalanceInputItemTypeDef
-):
-    pass
-
-
-_RequiredGetTokenBalanceInputRequestTypeDef = TypedDict(
-    "_RequiredGetTokenBalanceInputRequestTypeDef",
-    {
-        "tokenIdentifier": TokenIdentifierTypeDef,
-        "ownerIdentifier": OwnerIdentifierTypeDef,
-    },
-)
-_OptionalGetTokenBalanceInputRequestTypeDef = TypedDict(
-    "_OptionalGetTokenBalanceInputRequestTypeDef",
-    {
-        "atBlockchainInstant": BlockchainInstantTypeDef,
-    },
-    total=False,
-)
-
-
-class GetTokenBalanceInputRequestTypeDef(
-    _RequiredGetTokenBalanceInputRequestTypeDef, _OptionalGetTokenBalanceInputRequestTypeDef
-):
-    pass
-
-
 GetTokenBalanceOutputTypeDef = TypedDict(
     "GetTokenBalanceOutputTypeDef",
     {
         "ownerIdentifier": OwnerIdentifierTypeDef,
         "tokenIdentifier": TokenIdentifierTypeDef,
         "balance": str,
         "atBlockchainInstant": BlockchainInstantOutputTypeDef,
         "lastUpdatedTime": BlockchainInstantOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BlockchainInstantTypeDef = TypedDict(
+    "BlockchainInstantTypeDef",
+    {
+        "time": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetTransactionOutputTypeDef = TypedDict(
     "GetTransactionOutputTypeDef",
     {
         "transaction": TransactionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -480,14 +439,86 @@
     {
         "events": List[TransactionEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTransactionsOutputTypeDef = TypedDict(
+    "ListTransactionsOutputTypeDef",
+    {
+        "transactions": List[TransactionOutputItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchGetTokenBalanceOutputTypeDef = TypedDict(
+    "BatchGetTokenBalanceOutputTypeDef",
+    {
+        "tokenBalances": List[BatchGetTokenBalanceOutputItemTypeDef],
+        "errors": List[BatchGetTokenBalanceErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTokenBalancesOutputTypeDef = TypedDict(
+    "ListTokenBalancesOutputTypeDef",
+    {
+        "tokenBalances": List[TokenBalanceTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBatchGetTokenBalanceInputItemTypeDef = TypedDict(
+    "_RequiredBatchGetTokenBalanceInputItemTypeDef",
+    {
+        "tokenIdentifier": TokenIdentifierTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+    },
+)
+_OptionalBatchGetTokenBalanceInputItemTypeDef = TypedDict(
+    "_OptionalBatchGetTokenBalanceInputItemTypeDef",
+    {
+        "atBlockchainInstant": BlockchainInstantTypeDef,
+    },
+    total=False,
+)
+
+
+class BatchGetTokenBalanceInputItemTypeDef(
+    _RequiredBatchGetTokenBalanceInputItemTypeDef, _OptionalBatchGetTokenBalanceInputItemTypeDef
+):
+    pass
+
+
+BlockchainInstantUnionTypeDef = Union[BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef]
+_RequiredGetTokenBalanceInputRequestTypeDef = TypedDict(
+    "_RequiredGetTokenBalanceInputRequestTypeDef",
+    {
+        "tokenIdentifier": TokenIdentifierTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+    },
+)
+_OptionalGetTokenBalanceInputRequestTypeDef = TypedDict(
+    "_OptionalGetTokenBalanceInputRequestTypeDef",
+    {
+        "atBlockchainInstant": BlockchainInstantTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTokenBalanceInputRequestTypeDef(
+    _RequiredGetTokenBalanceInputRequestTypeDef, _OptionalGetTokenBalanceInputRequestTypeDef
+):
+    pass
+
+
 _RequiredListTransactionsInputListTransactionsPaginateTypeDef = TypedDict(
     "_RequiredListTransactionsInputListTransactionsPaginateTypeDef",
     {
         "address": str,
         "network": QueryNetworkType,
     },
 )
@@ -532,41 +563,14 @@
 
 class ListTransactionsInputRequestTypeDef(
     _RequiredListTransactionsInputRequestTypeDef, _OptionalListTransactionsInputRequestTypeDef
 ):
     pass
 
 
-ListTransactionsOutputTypeDef = TypedDict(
-    "ListTransactionsOutputTypeDef",
-    {
-        "transactions": List[TransactionOutputItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchGetTokenBalanceOutputTypeDef = TypedDict(
-    "BatchGetTokenBalanceOutputTypeDef",
-    {
-        "tokenBalances": List[BatchGetTokenBalanceOutputItemTypeDef],
-        "errors": List[BatchGetTokenBalanceErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTokenBalancesOutputTypeDef = TypedDict(
-    "ListTokenBalancesOutputTypeDef",
-    {
-        "tokenBalances": List[TokenBalanceTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetTokenBalanceInputRequestTypeDef = TypedDict(
     "BatchGetTokenBalanceInputRequestTypeDef",
     {
         "getTokenBalanceInputs": Sequence[BatchGetTokenBalanceInputItemTypeDef],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query/type_defs.pyi` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_managedblockchain_query.type_defs import BlockchainInstantOutputTypeDef
 
-    data: BlockchainInstantOutputTypeDef = {...}
+    data: BlockchainInstantOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -32,41 +32,43 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BlockchainInstantOutputTypeDef",
     "OwnerIdentifierTypeDef",
     "TokenIdentifierTypeDef",
-    "BlockchainInstantTypeDef",
     "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "GetTransactionInputRequestTypeDef",
     "TransactionTypeDef",
     "OwnerFilterTypeDef",
     "PaginatorConfigTypeDef",
     "TokenFilterTypeDef",
     "ListTransactionEventsInputRequestTypeDef",
     "TransactionEventTypeDef",
     "ListTransactionsSortTypeDef",
     "TransactionOutputItemTypeDef",
     "BatchGetTokenBalanceErrorItemTypeDef",
     "BatchGetTokenBalanceOutputItemTypeDef",
     "TokenBalanceTypeDef",
-    "BatchGetTokenBalanceInputItemTypeDef",
-    "GetTokenBalanceInputRequestTypeDef",
     "GetTokenBalanceOutputTypeDef",
+    "BlockchainInstantTypeDef",
     "GetTransactionOutputTypeDef",
     "ListTransactionEventsInputListTransactionEventsPaginateTypeDef",
     "ListTokenBalancesInputListTokenBalancesPaginateTypeDef",
     "ListTokenBalancesInputRequestTypeDef",
     "ListTransactionEventsOutputTypeDef",
-    "ListTransactionsInputListTransactionsPaginateTypeDef",
-    "ListTransactionsInputRequestTypeDef",
     "ListTransactionsOutputTypeDef",
     "BatchGetTokenBalanceOutputTypeDef",
     "ListTokenBalancesOutputTypeDef",
+    "BatchGetTokenBalanceInputItemTypeDef",
+    "BlockchainInstantUnionTypeDef",
+    "GetTokenBalanceInputRequestTypeDef",
+    "ListTransactionsInputListTransactionsPaginateTypeDef",
+    "ListTransactionsInputRequestTypeDef",
     "BatchGetTokenBalanceInputRequestTypeDef",
 )
 
 BlockchainInstantOutputTypeDef = TypedDict(
     "BlockchainInstantOutputTypeDef",
     {
         "time": datetime,
@@ -95,33 +97,26 @@
     },
     total=False,
 )
 
 class TokenIdentifierTypeDef(_RequiredTokenIdentifierTypeDef, _OptionalTokenIdentifierTypeDef):
     pass
 
-BlockchainInstantTypeDef = TypedDict(
-    "BlockchainInstantTypeDef",
-    {
-        "time": Union[datetime, str],
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 GetTransactionInputRequestTypeDef = TypedDict(
     "GetTransactionInputRequestTypeDef",
     {
         "transactionHash": str,
         "network": QueryNetworkType,
     },
 )
@@ -321,66 +316,34 @@
     },
     total=False,
 )
 
 class TokenBalanceTypeDef(_RequiredTokenBalanceTypeDef, _OptionalTokenBalanceTypeDef):
     pass
 
-_RequiredBatchGetTokenBalanceInputItemTypeDef = TypedDict(
-    "_RequiredBatchGetTokenBalanceInputItemTypeDef",
-    {
-        "tokenIdentifier": TokenIdentifierTypeDef,
-        "ownerIdentifier": OwnerIdentifierTypeDef,
-    },
-)
-_OptionalBatchGetTokenBalanceInputItemTypeDef = TypedDict(
-    "_OptionalBatchGetTokenBalanceInputItemTypeDef",
-    {
-        "atBlockchainInstant": BlockchainInstantTypeDef,
-    },
-    total=False,
-)
-
-class BatchGetTokenBalanceInputItemTypeDef(
-    _RequiredBatchGetTokenBalanceInputItemTypeDef, _OptionalBatchGetTokenBalanceInputItemTypeDef
-):
-    pass
-
-_RequiredGetTokenBalanceInputRequestTypeDef = TypedDict(
-    "_RequiredGetTokenBalanceInputRequestTypeDef",
-    {
-        "tokenIdentifier": TokenIdentifierTypeDef,
-        "ownerIdentifier": OwnerIdentifierTypeDef,
-    },
-)
-_OptionalGetTokenBalanceInputRequestTypeDef = TypedDict(
-    "_OptionalGetTokenBalanceInputRequestTypeDef",
-    {
-        "atBlockchainInstant": BlockchainInstantTypeDef,
-    },
-    total=False,
-)
-
-class GetTokenBalanceInputRequestTypeDef(
-    _RequiredGetTokenBalanceInputRequestTypeDef, _OptionalGetTokenBalanceInputRequestTypeDef
-):
-    pass
-
 GetTokenBalanceOutputTypeDef = TypedDict(
     "GetTokenBalanceOutputTypeDef",
     {
         "ownerIdentifier": OwnerIdentifierTypeDef,
         "tokenIdentifier": TokenIdentifierTypeDef,
         "balance": str,
         "atBlockchainInstant": BlockchainInstantOutputTypeDef,
         "lastUpdatedTime": BlockchainInstantOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BlockchainInstantTypeDef = TypedDict(
+    "BlockchainInstantTypeDef",
+    {
+        "time": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetTransactionOutputTypeDef = TypedDict(
     "GetTransactionOutputTypeDef",
     {
         "transaction": TransactionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -453,14 +416,82 @@
     {
         "events": List[TransactionEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTransactionsOutputTypeDef = TypedDict(
+    "ListTransactionsOutputTypeDef",
+    {
+        "transactions": List[TransactionOutputItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchGetTokenBalanceOutputTypeDef = TypedDict(
+    "BatchGetTokenBalanceOutputTypeDef",
+    {
+        "tokenBalances": List[BatchGetTokenBalanceOutputItemTypeDef],
+        "errors": List[BatchGetTokenBalanceErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTokenBalancesOutputTypeDef = TypedDict(
+    "ListTokenBalancesOutputTypeDef",
+    {
+        "tokenBalances": List[TokenBalanceTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBatchGetTokenBalanceInputItemTypeDef = TypedDict(
+    "_RequiredBatchGetTokenBalanceInputItemTypeDef",
+    {
+        "tokenIdentifier": TokenIdentifierTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+    },
+)
+_OptionalBatchGetTokenBalanceInputItemTypeDef = TypedDict(
+    "_OptionalBatchGetTokenBalanceInputItemTypeDef",
+    {
+        "atBlockchainInstant": BlockchainInstantTypeDef,
+    },
+    total=False,
+)
+
+class BatchGetTokenBalanceInputItemTypeDef(
+    _RequiredBatchGetTokenBalanceInputItemTypeDef, _OptionalBatchGetTokenBalanceInputItemTypeDef
+):
+    pass
+
+BlockchainInstantUnionTypeDef = Union[BlockchainInstantTypeDef, BlockchainInstantOutputTypeDef]
+_RequiredGetTokenBalanceInputRequestTypeDef = TypedDict(
+    "_RequiredGetTokenBalanceInputRequestTypeDef",
+    {
+        "tokenIdentifier": TokenIdentifierTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+    },
+)
+_OptionalGetTokenBalanceInputRequestTypeDef = TypedDict(
+    "_OptionalGetTokenBalanceInputRequestTypeDef",
+    {
+        "atBlockchainInstant": BlockchainInstantTypeDef,
+    },
+    total=False,
+)
+
+class GetTokenBalanceInputRequestTypeDef(
+    _RequiredGetTokenBalanceInputRequestTypeDef, _OptionalGetTokenBalanceInputRequestTypeDef
+):
+    pass
+
 _RequiredListTransactionsInputListTransactionsPaginateTypeDef = TypedDict(
     "_RequiredListTransactionsInputListTransactionsPaginateTypeDef",
     {
         "address": str,
         "network": QueryNetworkType,
     },
 )
@@ -501,41 +532,14 @@
 )
 
 class ListTransactionsInputRequestTypeDef(
     _RequiredListTransactionsInputRequestTypeDef, _OptionalListTransactionsInputRequestTypeDef
 ):
     pass
 
-ListTransactionsOutputTypeDef = TypedDict(
-    "ListTransactionsOutputTypeDef",
-    {
-        "transactions": List[TransactionOutputItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchGetTokenBalanceOutputTypeDef = TypedDict(
-    "BatchGetTokenBalanceOutputTypeDef",
-    {
-        "tokenBalances": List[BatchGetTokenBalanceOutputItemTypeDef],
-        "errors": List[BatchGetTokenBalanceErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTokenBalancesOutputTypeDef = TypedDict(
-    "ListTokenBalancesOutputTypeDef",
-    {
-        "tokenBalances": List[TokenBalanceTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetTokenBalanceInputRequestTypeDef = TypedDict(
     "BatchGetTokenBalanceInputRequestTypeDef",
     {
         "getTokenBalanceInputs": Sequence[BatchGetTokenBalanceInputItemTypeDef],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query.egg-info/PKG-INFO` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain-query
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ManagedBlockchainQuery 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ManagedBlockchainQuery 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 managedblockchain-query type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 managedblockchain-query type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain-query)](https://pepy.tech/project/mypy-boto3-managedblockchain-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchainQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
+[boto3.ManagedBlockchainQuery 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
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
 [mypy-boto3-managedblockchain-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/).
 
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
@@ -328,58 +328,60 @@
 )
 
 
 def check_value(value: ErrorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_managedblockchain_query.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain_query.type_defs import (
     BlockchainInstantOutputTypeDef,
     OwnerIdentifierTypeDef,
     TokenIdentifierTypeDef,
-    BlockchainInstantTypeDef,
     ResponseMetadataTypeDef,
+    TimestampTypeDef,
     GetTransactionInputRequestTypeDef,
     TransactionTypeDef,
     OwnerFilterTypeDef,
     PaginatorConfigTypeDef,
     TokenFilterTypeDef,
     ListTransactionEventsInputRequestTypeDef,
     TransactionEventTypeDef,
     ListTransactionsSortTypeDef,
     TransactionOutputItemTypeDef,
     BatchGetTokenBalanceErrorItemTypeDef,
     BatchGetTokenBalanceOutputItemTypeDef,
     TokenBalanceTypeDef,
-    BatchGetTokenBalanceInputItemTypeDef,
-    GetTokenBalanceInputRequestTypeDef,
     GetTokenBalanceOutputTypeDef,
+    BlockchainInstantTypeDef,
     GetTransactionOutputTypeDef,
     ListTransactionEventsInputListTransactionEventsPaginateTypeDef,
     ListTokenBalancesInputListTokenBalancesPaginateTypeDef,
     ListTokenBalancesInputRequestTypeDef,
     ListTransactionEventsOutputTypeDef,
-    ListTransactionsInputListTransactionsPaginateTypeDef,
-    ListTransactionsInputRequestTypeDef,
     ListTransactionsOutputTypeDef,
     BatchGetTokenBalanceOutputTypeDef,
     ListTokenBalancesOutputTypeDef,
+    BatchGetTokenBalanceInputItemTypeDef,
+    BlockchainInstantUnionTypeDef,
+    GetTokenBalanceInputRequestTypeDef,
+    ListTransactionsInputListTransactionsPaginateTypeDef,
+    ListTransactionsInputRequestTypeDef,
     BatchGetTokenBalanceInputRequestTypeDef,
 )
 
 
-def get_structure() -> BlockchainInstantOutputTypeDef:
+def get_value() -> BlockchainInstantOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/mypy_boto3_managedblockchain_query.egg-info/SOURCES.txt` & `mypy-boto3-managedblockchain-query-1.28.16/mypy_boto3_managedblockchain_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.15.post1/setup.py` & `mypy-boto3-managedblockchain-query-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-managedblockchain-query",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_managedblockchain_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedBlockchainQuery 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ManagedBlockchainQuery 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,17 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords=(
-        "boto3 managedblockchain-query type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="boto3 managedblockchain-query type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_managedblockchain_query": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/"
```

