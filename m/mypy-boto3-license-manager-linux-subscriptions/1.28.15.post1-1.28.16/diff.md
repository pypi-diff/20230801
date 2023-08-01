# Comparing `tmp/mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-license-manager-linux-subscriptions-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:31 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-linux-subscriptions-1.28.16.tar", last modified: Tue Aug  1 11:37:12 2023, max compression
```

## Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1.tar` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:31.861240 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-07-29 10:03:31.861240 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:31.849240 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:31.861240 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:31.861240 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:12.576839 mypy-boto3-license-manager-linux-subscriptions-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:36.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-08-01 11:37:12.576839 mypy-boto3-license-manager-linux-subscriptions-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-08-01 11:22:36.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:12.572839 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-01 11:22:36.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-01 11:22:36.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 11:22:36.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:36.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-08-01 11:22:37.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:36.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:12.576839 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:12.576839 mypy-boto3-license-manager-linux-subscriptions-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-01 11:22:36.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.16/setup.py
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/LICENSE` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/PKG-INFO` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-linux-subscriptions
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 license-manager-linux-subscriptions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 license-manager-linux-subscriptions type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-linux-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
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
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
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
@@ -333,21 +333,21 @@
 )
 
 
 def check_value(value: LinuxSubscriptionsDiscoveryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_license_manager_linux_subscriptions.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
     LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
     ResponseMetadataTypeDef,
     InstanceTypeDef,
@@ -355,22 +355,23 @@
     PaginatorConfigTypeDef,
     SubscriptionTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
+    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
     ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
     ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
-def get_structure() -> FilterTypeDef:
+def get_value() -> FilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/README.md` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-linux-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
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
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
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
@@ -301,21 +301,21 @@
 )
 
 
 def check_value(value: LinuxSubscriptionsDiscoveryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_license_manager_linux_subscriptions.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
     LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
     ResponseMetadataTypeDef,
     InstanceTypeDef,
@@ -323,22 +323,23 @@
     PaginatorConfigTypeDef,
     SubscriptionTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
+    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
     ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
     ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
-def get_structure() -> FilterTypeDef:
+def get_value() -> FilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/__init__.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/__main__.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions\nOther"
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/client.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,24 @@
     from mypy_boto3_license_manager_linux_subscriptions.client import LicenseManagerLinuxSubscriptionsClient
 
     session = Session()
     client: LicenseManagerLinuxSubscriptionsClient = session.client("license-manager-linux-subscriptions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import LinuxSubscriptionsDiscoveryType
 from .paginator import ListLinuxSubscriptionInstancesPaginator, ListLinuxSubscriptionsPaginator
 from .type_defs import (
     FilterTypeDef,
     GetServiceSettingsResponseTypeDef,
-    LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
-    LinuxSubscriptionsDiscoverySettingsTypeDef,
+    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -130,18 +129,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/client/#list_linux_subscriptions)
         """
 
     def update_service_settings(
         self,
         *,
         LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,
-        LinuxSubscriptionsDiscoverySettings: Union[
-            LinuxSubscriptionsDiscoverySettingsTypeDef,
-            LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
-        ],
+        LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
         AllowUpdate: bool = ...
     ) -> UpdateServiceSettingsResponseTypeDef:
         """
         Updates the service settings for Linux subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.update_service_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/client/#update_service_settings)
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/client.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,24 @@
     from mypy_boto3_license_manager_linux_subscriptions.client import LicenseManagerLinuxSubscriptionsClient
 
     session = Session()
     client: LicenseManagerLinuxSubscriptionsClient = session.client("license-manager-linux-subscriptions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import LinuxSubscriptionsDiscoveryType
 from .paginator import ListLinuxSubscriptionInstancesPaginator, ListLinuxSubscriptionsPaginator
 from .type_defs import (
     FilterTypeDef,
     GetServiceSettingsResponseTypeDef,
-    LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
-    LinuxSubscriptionsDiscoverySettingsTypeDef,
+    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -119,18 +118,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.list_linux_subscriptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/client/#list_linux_subscriptions)
         """
     def update_service_settings(
         self,
         *,
         LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,
-        LinuxSubscriptionsDiscoverySettings: Union[
-            LinuxSubscriptionsDiscoverySettingsTypeDef,
-            LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
-        ],
+        LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
         AllowUpdate: bool = ...
     ) -> UpdateServiceSettingsResponseTypeDef:
         """
         Updates the service settings for Linux subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.update_service_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/client/#update_service_settings)
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/literals.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/literals.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/paginator.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/type_defs.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_license_manager_linux_subscriptions.type_defs import FilterTypeDef
 
-    data: FilterTypeDef = {...}
+    data: FilterTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     LinuxSubscriptionsDiscoveryType,
     OperatorType,
     OrganizationIntegrationType,
     StatusType,
 )
@@ -36,14 +36,15 @@
     "PaginatorConfigTypeDef",
     "SubscriptionTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
+    "LinuxSubscriptionsDiscoverySettingsUnionTypeDef",
     "UpdateServiceSettingsRequestRequestTypeDef",
     "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
@@ -169,14 +170,17 @@
     {
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LinuxSubscriptionsDiscoverySettingsUnionTypeDef = Union[
+    LinuxSubscriptionsDiscoverySettingsTypeDef, LinuxSubscriptionsDiscoverySettingsOutputTypeDef
+]
 _RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
     {
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_license_manager_linux_subscriptions.type_defs import FilterTypeDef
 
-    data: FilterTypeDef = {...}
+    data: FilterTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     LinuxSubscriptionsDiscoveryType,
     OperatorType,
     OrganizationIntegrationType,
     StatusType,
 )
@@ -35,14 +35,15 @@
     "PaginatorConfigTypeDef",
     "SubscriptionTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
+    "LinuxSubscriptionsDiscoverySettingsUnionTypeDef",
     "UpdateServiceSettingsRequestRequestTypeDef",
     "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
@@ -168,14 +169,17 @@
     {
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LinuxSubscriptionsDiscoverySettingsUnionTypeDef = Union[
+    LinuxSubscriptionsDiscoverySettingsTypeDef, LinuxSubscriptionsDiscoverySettingsOutputTypeDef
+]
 _RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
     {
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-linux-subscriptions
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 license-manager-linux-subscriptions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 license-manager-linux-subscriptions type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-linux-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
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
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
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
@@ -333,21 +333,21 @@
 )
 
 
 def check_value(value: LinuxSubscriptionsDiscoveryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_license_manager_linux_subscriptions.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
     LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
     ResponseMetadataTypeDef,
     InstanceTypeDef,
@@ -355,22 +355,23 @@
     PaginatorConfigTypeDef,
     SubscriptionTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
+    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
     ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
     ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
-def get_structure() -> FilterTypeDef:
+def get_value() -> FilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.15.post1/setup.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager-linux-subscriptions",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_license_manager_linux_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.16 service generated with"
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
-        "boto3 license-manager-linux-subscriptions type-annotations boto3-stubs mypy typeshed"
+        "boto3 license-manager-linux-subscriptions type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_license_manager_linux_subscriptions": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
```

