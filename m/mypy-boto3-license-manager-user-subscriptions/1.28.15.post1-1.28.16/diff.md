# Comparing `tmp/mypy-boto3-license-manager-user-subscriptions-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-license-manager-user-subscriptions-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:33 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.28.16.tar", last modified: Tue Aug  1 11:37:13 2023, max compression
```

## Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1.tar` & `mypy-boto3-license-manager-user-subscriptions-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-07-29 09:49:49.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-07-29 09:49:49.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.404837 mypy-boto3-license-manager-user-subscriptions-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-08-01 11:37:13.392837 mypy-boto3-license-manager-user-subscriptions-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.384837 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-08-01 11:22:38.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-08-01 11:22:38.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-08-01 11:22:38.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-08-01 11:22:38.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-08-01 11:22:38.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-08-01 11:22:40.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-08-01 11:22:38.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.392837 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-08-01 11:37:13.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-01 11:37:13.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:13.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 11:37:13.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:13.404837 mypy-boto3-license-manager-user-subscriptions-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-user-subscriptions-1.28.16/setup.py
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/LICENSE` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 license-manager-user-subscriptions type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-license-manager-user-subscriptions"></a>
 
 # mypy-boto3-license-manager-user-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-user-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-user-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
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
@@ -336,21 +304,21 @@
 )
 
 
 def check_value(value: ListIdentityProvidersPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
     ResponseMetadataTypeDef,
     FilterTypeDef,
     SettingsOutputTypeDef,
@@ -360,14 +328,15 @@
     SettingsTypeDef,
     UpdateSettingsTypeDef,
     IdentityProviderTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
+    SettingsUnionTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
     IdentityProviderSummaryTypeDef,
     InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
@@ -387,15 +356,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
+def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/README.md` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-license-manager-user-subscriptions
+Version: 1.28.16
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 license-manager-user-subscriptions type-annotations botocore mypy typeshed autocomplete
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
 <a id="mypy-boto3-license-manager-user-subscriptions"></a>
 
 # mypy-boto3-license-manager-user-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-user-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-user-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
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
@@ -304,21 +336,21 @@
 )
 
 
 def check_value(value: ListIdentityProvidersPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
     ResponseMetadataTypeDef,
     FilterTypeDef,
     SettingsOutputTypeDef,
@@ -328,14 +360,15 @@
     SettingsTypeDef,
     UpdateSettingsTypeDef,
     IdentityProviderTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
+    SettingsUnionTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
     IdentityProviderSummaryTypeDef,
     InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
@@ -355,15 +388,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
+def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__init__.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__init__.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__main__.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions\nOther"
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/client.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient
 
     session = Session()
     client: LicenseManagerUserSubscriptionsClient = session.client("license-manager-user-subscriptions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListIdentityProvidersPaginator,
     ListInstancesPaginator,
     ListProductSubscriptionsPaginator,
@@ -31,16 +31,15 @@
     FilterTypeDef,
     IdentityProviderTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     ListUserAssociationsResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
-    SettingsOutputTypeDef,
-    SettingsTypeDef,
+    SettingsUnionTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
     UpdateIdentityProviderSettingsResponseTypeDef,
     UpdateSettingsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -211,15 +210,15 @@
         """
 
     def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: Union[SettingsTypeDef, SettingsOutputTypeDef] = ...
+        Settings: SettingsUnionTypeDef = ...
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/client/#register_identity_provider)
         """
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/client.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient
 
     session = Session()
     client: LicenseManagerUserSubscriptionsClient = session.client("license-manager-user-subscriptions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListIdentityProvidersPaginator,
     ListInstancesPaginator,
     ListProductSubscriptionsPaginator,
@@ -31,16 +31,15 @@
     FilterTypeDef,
     IdentityProviderTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     ListUserAssociationsResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
-    SettingsOutputTypeDef,
-    SettingsTypeDef,
+    SettingsUnionTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
     UpdateIdentityProviderSettingsResponseTypeDef,
     UpdateSettingsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -196,15 +195,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/client/#list_user_associations)
         """
     def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: Union[SettingsTypeDef, SettingsOutputTypeDef] = ...
+        Settings: SettingsUnionTypeDef = ...
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/client/#register_identity_provider)
         """
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/literals.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/literals.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/paginator.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/paginator.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/type_defs.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
 
-    data: ActiveDirectoryIdentityProviderTypeDef = {...}
+    data: ActiveDirectoryIdentityProviderTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
@@ -31,14 +31,15 @@
     "SettingsTypeDef",
     "UpdateSettingsTypeDef",
     "IdentityProviderTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
+    "SettingsUnionTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
     "IdentityProviderSummaryTypeDef",
     "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
@@ -207,14 +208,15 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+SettingsUnionTypeDef = Union[SettingsTypeDef, SettingsOutputTypeDef]
 _RequiredAssociateUserRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Username": str,
     },
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
 
-    data: ActiveDirectoryIdentityProviderTypeDef = {...}
+    data: ActiveDirectoryIdentityProviderTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
@@ -30,14 +30,15 @@
     "SettingsTypeDef",
     "UpdateSettingsTypeDef",
     "IdentityProviderTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
+    "SettingsUnionTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
     "IdentityProviderSummaryTypeDef",
     "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
@@ -202,14 +203,15 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+SettingsUnionTypeDef = Union[SettingsTypeDef, SettingsOutputTypeDef]
 _RequiredAssociateUserRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Username": str,
     },
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 license-manager-user-subscriptions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 license-manager-user-subscriptions type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-user-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
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
@@ -336,21 +336,21 @@
 )
 
 
 def check_value(value: ListIdentityProvidersPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
     ResponseMetadataTypeDef,
     FilterTypeDef,
     SettingsOutputTypeDef,
@@ -360,14 +360,15 @@
     SettingsTypeDef,
     UpdateSettingsTypeDef,
     IdentityProviderTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
+    SettingsUnionTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
     IdentityProviderSummaryTypeDef,
     InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
@@ -387,15 +388,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
+def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/setup.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager-user-subscriptions",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_license_manager_user_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.16 service generated with"
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
-        "boto3 license-manager-user-subscriptions type-annotations boto3-stubs mypy typeshed"
+        "boto3 license-manager-user-subscriptions type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_license_manager_user_subscriptions": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
```

