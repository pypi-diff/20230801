# Comparing `tmp/mypy-boto3-billingconductor-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-billingconductor-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-billingconductor-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:37 2023, max compression
+gzip compressed data, was "mypy-boto3-billingconductor-1.28.16.tar", last modified: Tue Aug  1 11:36:18 2023, max compression
```

## Comparing `mypy-boto3-billingconductor-1.28.15.post1.tar` & `mypy-boto3-billingconductor-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.821035 mypy-boto3-billingconductor-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:04.000000 mypy-boto3-billingconductor-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-07-29 10:02:37.813035 mypy-boto3-billingconductor-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-07-29 09:39:04.000000 mypy-boto3-billingconductor-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.813035 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-29 09:39:04.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-29 09:39:04.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:39:04.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31684 2023-07-29 09:39:05.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31636 2023-07-29 09:39:05.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-07-29 09:39:05.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-29 09:39:05.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-07-29 09:39:05.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-07-29 09:39:05.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:04.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43645 2023-07-29 09:39:07.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43596 2023-07-29 09:39:07.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:04.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.813035 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-07-29 10:02:37.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:02:37.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:37.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:02:37.000000 mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:37.821035 mypy-boto3-billingconductor-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:39:04.000000 mypy-boto3-billingconductor-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.764939 mypy-boto3-billingconductor-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:37.000000 mypy-boto3-billingconductor-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-08-01 11:36:18.764939 mypy-boto3-billingconductor-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-08-01 11:11:37.000000 mypy-boto3-billingconductor-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.760939 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-08-01 11:11:38.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-08-01 11:11:38.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-01 11:11:38.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31684 2023-08-01 11:11:39.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31636 2023-08-01 11:11:39.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-08-01 11:11:39.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-08-01 11:11:39.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-08-01 11:11:39.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-08-01 11:11:39.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:38.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43643 2023-08-01 11:11:40.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43594 2023-08-01 11:11:40.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:37.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.764939 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-08-01 11:36:18.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:36:18.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:18.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:36:18.000000 mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:18.764939 mypy-boto3-billingconductor-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 11:11:37.000000 mypy-boto3-billingconductor-1.28.16/setup.py
```

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/LICENSE` & `mypy-boto3-billingconductor-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/PKG-INFO` & `mypy-boto3-billingconductor-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-billingconductor
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.BillingConductor 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.BillingConductor 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 billingconductor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 billingconductor type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-billingconductor)](https://pepy.tech/project/mypy-boto3-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BillingConductor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[boto3.BillingConductor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [mypy-boto3-billingconductor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/).
 
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
@@ -362,20 +362,20 @@
 )
 
 
 def check_value(value: AssociateResourceErrorReasonType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_billingconductor.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -486,15 +486,15 @@
     UpdatePricingRuleOutputTypeDef,
     ListPricingRulesOutputTypeDef,
     ListCustomLineItemsOutputTypeDef,
     ListCustomLineItemVersionsOutputTypeDef,
 )
 
 
-def get_structure() -> AccountAssociationsListElementTypeDef:
+def get_value() -> AccountAssociationsListElementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/README.md` & `mypy-boto3-billingconductor-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-billingconductor)](https://pepy.tech/project/mypy-boto3-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BillingConductor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[boto3.BillingConductor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [mypy-boto3-billingconductor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/).
 
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
@@ -330,20 +330,20 @@
 )
 
 
 def check_value(value: AssociateResourceErrorReasonType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_billingconductor.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -454,15 +454,15 @@
     UpdatePricingRuleOutputTypeDef,
     ListPricingRulesOutputTypeDef,
     ListCustomLineItemsOutputTypeDef,
     ListCustomLineItemVersionsOutputTypeDef,
 )
 
 
-def get_structure() -> AccountAssociationsListElementTypeDef:
+def get_value() -> AccountAssociationsListElementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/__init__.py` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/__init__.pyi` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/client.py` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/client.pyi` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/literals.py` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/literals.pyi` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/paginator.py` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/paginator.pyi` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/type_defs.py` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_billingconductor.type_defs import AccountAssociationsListElementTypeDef
 
-    data: AccountAssociationsListElementTypeDef = {...}
+    data: AccountAssociationsListElementTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AssociateResourceErrorReasonType,
```

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor/type_defs.pyi` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_billingconductor.type_defs import AccountAssociationsListElementTypeDef
 
-    data: AccountAssociationsListElementTypeDef = {...}
+    data: AccountAssociationsListElementTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AssociateResourceErrorReasonType,
```

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor.egg-info/PKG-INFO` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-billingconductor
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.BillingConductor 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.BillingConductor 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 billingconductor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 billingconductor type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-billingconductor)](https://pepy.tech/project/mypy-boto3-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BillingConductor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[boto3.BillingConductor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [mypy-boto3-billingconductor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/).
 
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
@@ -362,20 +362,20 @@
 )
 
 
 def check_value(value: AssociateResourceErrorReasonType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_billingconductor.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -486,15 +486,15 @@
     UpdatePricingRuleOutputTypeDef,
     ListPricingRulesOutputTypeDef,
     ListCustomLineItemsOutputTypeDef,
     ListCustomLineItemVersionsOutputTypeDef,
 )
 
 
-def get_structure() -> AccountAssociationsListElementTypeDef:
+def get_value() -> AccountAssociationsListElementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/mypy_boto3_billingconductor.egg-info/SOURCES.txt` & `mypy-boto3-billingconductor-1.28.16/mypy_boto3_billingconductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.15.post1/setup.py` & `mypy-boto3-billingconductor-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-billingconductor",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_billingconductor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BillingConductor 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.BillingConductor 1.28.16 service generated with"
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
-    keywords="boto3 billingconductor type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 billingconductor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_billingconductor": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

