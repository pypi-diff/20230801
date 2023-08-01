# Comparing `tmp/mypy-boto3-savingsplans-1.28.16.tar.gz` & `tmp/mypy-boto3-savingsplans-1.28.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-savingsplans-1.28.16.tar", last modified: Tue Aug  1 11:37:47 2023, max compression
+gzip compressed data, was "mypy-boto3-savingsplans-1.28.7.tar", last modified: Thu Jul 20 05:24:39 2023, max compression
```

## Comparing `mypy-boto3-savingsplans-1.28.16.tar` & `mypy-boto3-savingsplans-1.28.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:47.864743 mypy-boto3-savingsplans-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-08-01 11:37:47.840743 mypy-boto3-savingsplans-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:47.840743 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-08-01 11:32:10.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-08-01 11:32:10.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:47.840743 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-08-01 11:37:47.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 11:37:47.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:47.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:47.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:47.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:37:47.000000 mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:47.864743 mypy-boto3-savingsplans-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:32:09.000000 mypy-boto3-savingsplans-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:24:39.240568 mypy-boto3-savingsplans-1.28.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 05:24:30.000000 mypy-boto3-savingsplans-1.28.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-07-20 05:24:39.236568 mypy-boto3-savingsplans-1.28.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-07-20 05:24:30.000000 mypy-boto3-savingsplans-1.28.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:24:39.232568 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-07-20 05:24:31.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 05:24:30.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:24:39.236568 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-07-20 05:24:39.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-20 05:24:39.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 05:24:39.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 05:24:39.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 05:24:39.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 05:24:39.000000 mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 05:24:39.240568 mypy-boto3-savingsplans-1.28.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 05:24:30.000000 mypy-boto3-savingsplans-1.28.7/setup.py
```

### Comparing `mypy-boto3-savingsplans-1.28.16/LICENSE` & `mypy-boto3-savingsplans-1.28.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-savingsplans-1.28.16/PKG-INFO` & `mypy-boto3-savingsplans-1.28.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-savingsplans
-Version: 1.28.16
-Summary: Type annotations for boto3.SavingsPlans 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.7
+Summary: Type annotations for boto3.SavingsPlans 1.28.7 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 savingsplans type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 savingsplans type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-savingsplans"></a>
 
 # mypy-boto3-savingsplans
 
 [![PyPI - mypy-boto3-savingsplans](https://img.shields.io/pypi/v/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-savingsplans)](https://pepy.tech/project/mypy-boto3-savingsplans)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-savingsplans?color=blue)](https://pypistats.org/packages/mypy-boto3-savingsplans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SavingsPlans 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
+[boto3.SavingsPlans 1.28.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-savingsplans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -299,39 +299,38 @@
 )
 
 
 def check_value(value: CurrencyCodeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_savingsplans.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_savingsplans.type_defs import (
-    TimestampTypeDef,
+    CreateSavingsPlanRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DeleteQueuedSavingsPlanRequestRequestTypeDef,
     SavingsPlanRateFilterTypeDef,
     SavingsPlanOfferingRateFilterElementTypeDef,
     SavingsPlanOfferingFilterElementTypeDef,
     SavingsPlanFilterTypeDef,
     SavingsPlanTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ParentSavingsPlanOfferingTypeDef,
     SavingsPlanOfferingPropertyTypeDef,
     SavingsPlanOfferingRatePropertyTypeDef,
     SavingsPlanRatePropertyTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateSavingsPlanRequestRequestTypeDef,
     CreateSavingsPlanResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     DescribeSavingsPlanRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingsRequestRequestTypeDef,
     DescribeSavingsPlansRequestRequestTypeDef,
     DescribeSavingsPlansResponseTypeDef,
@@ -340,15 +339,15 @@
     SavingsPlanRateTypeDef,
     DescribeSavingsPlansOfferingsResponseTypeDef,
     DescribeSavingsPlansOfferingRatesResponseTypeDef,
     DescribeSavingsPlanRatesResponseTypeDef,
 )
 
 
-def get_value() -> TimestampTypeDef:
+def get_structure() -> CreateSavingsPlanRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-savingsplans-1.28.16/README.md` & `mypy-boto3-savingsplans-1.28.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-savingsplans"></a>
 
 # mypy-boto3-savingsplans
 
 [![PyPI - mypy-boto3-savingsplans](https://img.shields.io/pypi/v/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-savingsplans)](https://pepy.tech/project/mypy-boto3-savingsplans)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-savingsplans?color=blue)](https://pypistats.org/packages/mypy-boto3-savingsplans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SavingsPlans 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
+[boto3.SavingsPlans 1.28.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-savingsplans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -267,39 +267,38 @@
 )
 
 
 def check_value(value: CurrencyCodeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_savingsplans.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_savingsplans.type_defs import (
-    TimestampTypeDef,
+    CreateSavingsPlanRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DeleteQueuedSavingsPlanRequestRequestTypeDef,
     SavingsPlanRateFilterTypeDef,
     SavingsPlanOfferingRateFilterElementTypeDef,
     SavingsPlanOfferingFilterElementTypeDef,
     SavingsPlanFilterTypeDef,
     SavingsPlanTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ParentSavingsPlanOfferingTypeDef,
     SavingsPlanOfferingPropertyTypeDef,
     SavingsPlanOfferingRatePropertyTypeDef,
     SavingsPlanRatePropertyTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateSavingsPlanRequestRequestTypeDef,
     CreateSavingsPlanResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     DescribeSavingsPlanRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingsRequestRequestTypeDef,
     DescribeSavingsPlansRequestRequestTypeDef,
     DescribeSavingsPlansResponseTypeDef,
@@ -308,15 +307,15 @@
     SavingsPlanRateTypeDef,
     DescribeSavingsPlansOfferingsResponseTypeDef,
     DescribeSavingsPlansOfferingRatesResponseTypeDef,
     DescribeSavingsPlanRatesResponseTypeDef,
 )
 
 
-def get_value() -> TimestampTypeDef:
+def get_structure() -> CreateSavingsPlanRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/__main__.py` & `mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SavingsPlans 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.SavingsPlans 1.28.7\nVersion:         1.28.7\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.7")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/client.py` & `mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     from boto3.session import Session
     from mypy_boto3_savingsplans.client import SavingsPlansClient
 
     session = Session()
     client: SavingsPlansClient = session.client("savingsplans")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CurrencyCodeType,
     SavingsPlanPaymentOptionType,
     SavingsPlanProductTypeType,
@@ -32,15 +33,14 @@
     DescribeSavingsPlansOfferingsResponseTypeDef,
     DescribeSavingsPlansResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SavingsPlanFilterTypeDef,
     SavingsPlanOfferingFilterElementTypeDef,
     SavingsPlanOfferingRateFilterElementTypeDef,
     SavingsPlanRateFilterTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = ("SavingsPlansClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -93,15 +93,15 @@
 
     def create_savings_plan(
         self,
         *,
         savingsPlanOfferingId: str,
         commitment: str,
         upfrontPaymentAmount: str = ...,
-        purchaseTime: TimestampTypeDef = ...,
+        purchaseTime: Union[datetime, str] = ...,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSavingsPlanResponseTypeDef:
         """
         Creates a Savings Plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.create_savings_plan)
```

### Comparing `mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/client.pyi` & `mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     from boto3.session import Session
     from mypy_boto3_savingsplans.client import SavingsPlansClient
 
     session = Session()
     client: SavingsPlansClient = session.client("savingsplans")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CurrencyCodeType,
     SavingsPlanPaymentOptionType,
     SavingsPlanProductTypeType,
@@ -32,15 +33,14 @@
     DescribeSavingsPlansOfferingsResponseTypeDef,
     DescribeSavingsPlansResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SavingsPlanFilterTypeDef,
     SavingsPlanOfferingFilterElementTypeDef,
     SavingsPlanOfferingRateFilterElementTypeDef,
     SavingsPlanRateFilterTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = ("SavingsPlansClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -87,15 +87,15 @@
         """
     def create_savings_plan(
         self,
         *,
         savingsPlanOfferingId: str,
         commitment: str,
         upfrontPaymentAmount: str = ...,
-        purchaseTime: TimestampTypeDef = ...,
+        purchaseTime: Union[datetime, str] = ...,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSavingsPlanResponseTypeDef:
         """
         Creates a Savings Plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.create_savings_plan)
```

### Comparing `mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/literals.py` & `mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -282,15 +281,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/literals.pyi` & `mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -280,15 +279,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/type_defs.py` & `mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for savingsplans service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_savingsplans.type_defs import TimestampTypeDef
+    from mypy_boto3_savingsplans.type_defs import CreateSavingsPlanRequestRequestTypeDef
 
-    data: TimestampTypeDef = ...
+    data: CreateSavingsPlanRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -34,30 +34,29 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "TimestampTypeDef",
+    "CreateSavingsPlanRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteQueuedSavingsPlanRequestRequestTypeDef",
     "SavingsPlanRateFilterTypeDef",
     "SavingsPlanOfferingRateFilterElementTypeDef",
     "SavingsPlanOfferingFilterElementTypeDef",
     "SavingsPlanFilterTypeDef",
     "SavingsPlanTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ParentSavingsPlanOfferingTypeDef",
     "SavingsPlanOfferingPropertyTypeDef",
     "SavingsPlanOfferingRatePropertyTypeDef",
     "SavingsPlanRatePropertyTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateSavingsPlanRequestRequestTypeDef",
     "CreateSavingsPlanResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "DescribeSavingsPlanRatesRequestRequestTypeDef",
     "DescribeSavingsPlansOfferingRatesRequestRequestTypeDef",
     "DescribeSavingsPlansOfferingsRequestRequestTypeDef",
     "DescribeSavingsPlansRequestRequestTypeDef",
     "DescribeSavingsPlansResponseTypeDef",
@@ -65,15 +64,39 @@
     "SavingsPlanOfferingRateTypeDef",
     "SavingsPlanRateTypeDef",
     "DescribeSavingsPlansOfferingsResponseTypeDef",
     "DescribeSavingsPlansOfferingRatesResponseTypeDef",
     "DescribeSavingsPlanRatesResponseTypeDef",
 )
 
-TimestampTypeDef = Union[datetime, str]
+_RequiredCreateSavingsPlanRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSavingsPlanRequestRequestTypeDef",
+    {
+        "savingsPlanOfferingId": str,
+        "commitment": str,
+    },
+)
+_OptionalCreateSavingsPlanRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSavingsPlanRequestRequestTypeDef",
+    {
+        "upfrontPaymentAmount": str,
+        "purchaseTime": Union[datetime, str],
+        "clientToken": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateSavingsPlanRequestRequestTypeDef(
+    _RequiredCreateSavingsPlanRequestRequestTypeDef, _OptionalCreateSavingsPlanRequestRequestTypeDef
+):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -142,15 +165,14 @@
         "currency": CurrencyCodeType,
         "commitment": str,
         "upfrontPaymentAmount": str,
         "recurringPaymentAmount": str,
         "termDurationInSeconds": int,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
@@ -162,42 +184,38 @@
         "offeringId": str,
         "paymentOption": SavingsPlanPaymentOptionType,
         "planType": SavingsPlanTypeType,
         "durationSeconds": int,
         "currency": CurrencyCodeType,
         "planDescription": str,
     },
-    total=False,
 )
 
 SavingsPlanOfferingPropertyTypeDef = TypedDict(
     "SavingsPlanOfferingPropertyTypeDef",
     {
         "name": SavingsPlanOfferingPropertyKeyType,
         "value": str,
     },
-    total=False,
 )
 
 SavingsPlanOfferingRatePropertyTypeDef = TypedDict(
     "SavingsPlanOfferingRatePropertyTypeDef",
     {
         "name": str,
         "value": str,
     },
-    total=False,
 )
 
 SavingsPlanRatePropertyTypeDef = TypedDict(
     "SavingsPlanRatePropertyTypeDef",
     {
         "name": SavingsPlanRatePropertyKeyType,
         "value": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -208,39 +226,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredCreateSavingsPlanRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSavingsPlanRequestRequestTypeDef",
-    {
-        "savingsPlanOfferingId": str,
-        "commitment": str,
-    },
-)
-_OptionalCreateSavingsPlanRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSavingsPlanRequestRequestTypeDef",
-    {
-        "upfrontPaymentAmount": str,
-        "purchaseTime": TimestampTypeDef,
-        "clientToken": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateSavingsPlanRequestRequestTypeDef(
-    _RequiredCreateSavingsPlanRequestRequestTypeDef, _OptionalCreateSavingsPlanRequestRequestTypeDef
-):
-    pass
-
-
 CreateSavingsPlanResponseTypeDef = TypedDict(
     "CreateSavingsPlanResponseTypeDef",
     {
         "savingsPlanId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -347,45 +340,42 @@
         "durationSeconds": int,
         "currency": CurrencyCodeType,
         "serviceCode": str,
         "usageType": str,
         "operation": str,
         "properties": List[SavingsPlanOfferingPropertyTypeDef],
     },
-    total=False,
 )
 
 SavingsPlanOfferingRateTypeDef = TypedDict(
     "SavingsPlanOfferingRateTypeDef",
     {
         "savingsPlanOffering": ParentSavingsPlanOfferingTypeDef,
         "rate": str,
         "unit": SavingsPlanRateUnitType,
         "productType": SavingsPlanProductTypeType,
         "serviceCode": SavingsPlanRateServiceCodeType,
         "usageType": str,
         "operation": str,
         "properties": List[SavingsPlanOfferingRatePropertyTypeDef],
     },
-    total=False,
 )
 
 SavingsPlanRateTypeDef = TypedDict(
     "SavingsPlanRateTypeDef",
     {
         "rate": str,
         "currency": CurrencyCodeType,
         "unit": SavingsPlanRateUnitType,
         "productType": SavingsPlanProductTypeType,
         "serviceCode": SavingsPlanRateServiceCodeType,
         "usageType": str,
         "operation": str,
         "properties": List[SavingsPlanRatePropertyTypeDef],
     },
-    total=False,
 )
 
 DescribeSavingsPlansOfferingsResponseTypeDef = TypedDict(
     "DescribeSavingsPlansOfferingsResponseTypeDef",
     {
         "searchResults": List[SavingsPlanOfferingTypeDef],
         "nextToken": str,
```

### Comparing `mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans/type_defs.pyi` & `mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for savingsplans service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_savingsplans.type_defs import TimestampTypeDef
+    from mypy_boto3_savingsplans.type_defs import CreateSavingsPlanRequestRequestTypeDef
 
-    data: TimestampTypeDef = ...
+    data: CreateSavingsPlanRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -33,30 +33,29 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "TimestampTypeDef",
+    "CreateSavingsPlanRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteQueuedSavingsPlanRequestRequestTypeDef",
     "SavingsPlanRateFilterTypeDef",
     "SavingsPlanOfferingRateFilterElementTypeDef",
     "SavingsPlanOfferingFilterElementTypeDef",
     "SavingsPlanFilterTypeDef",
     "SavingsPlanTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ParentSavingsPlanOfferingTypeDef",
     "SavingsPlanOfferingPropertyTypeDef",
     "SavingsPlanOfferingRatePropertyTypeDef",
     "SavingsPlanRatePropertyTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateSavingsPlanRequestRequestTypeDef",
     "CreateSavingsPlanResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "DescribeSavingsPlanRatesRequestRequestTypeDef",
     "DescribeSavingsPlansOfferingRatesRequestRequestTypeDef",
     "DescribeSavingsPlansOfferingsRequestRequestTypeDef",
     "DescribeSavingsPlansRequestRequestTypeDef",
     "DescribeSavingsPlansResponseTypeDef",
@@ -64,15 +63,37 @@
     "SavingsPlanOfferingRateTypeDef",
     "SavingsPlanRateTypeDef",
     "DescribeSavingsPlansOfferingsResponseTypeDef",
     "DescribeSavingsPlansOfferingRatesResponseTypeDef",
     "DescribeSavingsPlanRatesResponseTypeDef",
 )
 
-TimestampTypeDef = Union[datetime, str]
+_RequiredCreateSavingsPlanRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSavingsPlanRequestRequestTypeDef",
+    {
+        "savingsPlanOfferingId": str,
+        "commitment": str,
+    },
+)
+_OptionalCreateSavingsPlanRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSavingsPlanRequestRequestTypeDef",
+    {
+        "upfrontPaymentAmount": str,
+        "purchaseTime": Union[datetime, str],
+        "clientToken": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateSavingsPlanRequestRequestTypeDef(
+    _RequiredCreateSavingsPlanRequestRequestTypeDef, _OptionalCreateSavingsPlanRequestRequestTypeDef
+):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -141,15 +162,14 @@
         "currency": CurrencyCodeType,
         "commitment": str,
         "upfrontPaymentAmount": str,
         "recurringPaymentAmount": str,
         "termDurationInSeconds": int,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
@@ -161,42 +181,38 @@
         "offeringId": str,
         "paymentOption": SavingsPlanPaymentOptionType,
         "planType": SavingsPlanTypeType,
         "durationSeconds": int,
         "currency": CurrencyCodeType,
         "planDescription": str,
     },
-    total=False,
 )
 
 SavingsPlanOfferingPropertyTypeDef = TypedDict(
     "SavingsPlanOfferingPropertyTypeDef",
     {
         "name": SavingsPlanOfferingPropertyKeyType,
         "value": str,
     },
-    total=False,
 )
 
 SavingsPlanOfferingRatePropertyTypeDef = TypedDict(
     "SavingsPlanOfferingRatePropertyTypeDef",
     {
         "name": str,
         "value": str,
     },
-    total=False,
 )
 
 SavingsPlanRatePropertyTypeDef = TypedDict(
     "SavingsPlanRatePropertyTypeDef",
     {
         "name": SavingsPlanRatePropertyKeyType,
         "value": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -207,37 +223,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredCreateSavingsPlanRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSavingsPlanRequestRequestTypeDef",
-    {
-        "savingsPlanOfferingId": str,
-        "commitment": str,
-    },
-)
-_OptionalCreateSavingsPlanRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSavingsPlanRequestRequestTypeDef",
-    {
-        "upfrontPaymentAmount": str,
-        "purchaseTime": TimestampTypeDef,
-        "clientToken": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateSavingsPlanRequestRequestTypeDef(
-    _RequiredCreateSavingsPlanRequestRequestTypeDef, _OptionalCreateSavingsPlanRequestRequestTypeDef
-):
-    pass
-
 CreateSavingsPlanResponseTypeDef = TypedDict(
     "CreateSavingsPlanResponseTypeDef",
     {
         "savingsPlanId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -342,45 +335,42 @@
         "durationSeconds": int,
         "currency": CurrencyCodeType,
         "serviceCode": str,
         "usageType": str,
         "operation": str,
         "properties": List[SavingsPlanOfferingPropertyTypeDef],
     },
-    total=False,
 )
 
 SavingsPlanOfferingRateTypeDef = TypedDict(
     "SavingsPlanOfferingRateTypeDef",
     {
         "savingsPlanOffering": ParentSavingsPlanOfferingTypeDef,
         "rate": str,
         "unit": SavingsPlanRateUnitType,
         "productType": SavingsPlanProductTypeType,
         "serviceCode": SavingsPlanRateServiceCodeType,
         "usageType": str,
         "operation": str,
         "properties": List[SavingsPlanOfferingRatePropertyTypeDef],
     },
-    total=False,
 )
 
 SavingsPlanRateTypeDef = TypedDict(
     "SavingsPlanRateTypeDef",
     {
         "rate": str,
         "currency": CurrencyCodeType,
         "unit": SavingsPlanRateUnitType,
         "productType": SavingsPlanProductTypeType,
         "serviceCode": SavingsPlanRateServiceCodeType,
         "usageType": str,
         "operation": str,
         "properties": List[SavingsPlanRatePropertyTypeDef],
     },
-    total=False,
 )
 
 DescribeSavingsPlansOfferingsResponseTypeDef = TypedDict(
     "DescribeSavingsPlansOfferingsResponseTypeDef",
     {
         "searchResults": List[SavingsPlanOfferingTypeDef],
         "nextToken": str,
```

### Comparing `mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans.egg-info/PKG-INFO` & `mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-savingsplans
-Version: 1.28.16
-Summary: Type annotations for boto3.SavingsPlans 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.7
+Summary: Type annotations for boto3.SavingsPlans 1.28.7 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 savingsplans type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 savingsplans type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-savingsplans"></a>
 
 # mypy-boto3-savingsplans
 
 [![PyPI - mypy-boto3-savingsplans](https://img.shields.io/pypi/v/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-savingsplans)](https://pepy.tech/project/mypy-boto3-savingsplans)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-savingsplans?color=blue)](https://pypistats.org/packages/mypy-boto3-savingsplans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SavingsPlans 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
+[boto3.SavingsPlans 1.28.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-savingsplans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -299,39 +299,38 @@
 )
 
 
 def check_value(value: CurrencyCodeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_savingsplans.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_savingsplans.type_defs import (
-    TimestampTypeDef,
+    CreateSavingsPlanRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DeleteQueuedSavingsPlanRequestRequestTypeDef,
     SavingsPlanRateFilterTypeDef,
     SavingsPlanOfferingRateFilterElementTypeDef,
     SavingsPlanOfferingFilterElementTypeDef,
     SavingsPlanFilterTypeDef,
     SavingsPlanTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ParentSavingsPlanOfferingTypeDef,
     SavingsPlanOfferingPropertyTypeDef,
     SavingsPlanOfferingRatePropertyTypeDef,
     SavingsPlanRatePropertyTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateSavingsPlanRequestRequestTypeDef,
     CreateSavingsPlanResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     DescribeSavingsPlanRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingsRequestRequestTypeDef,
     DescribeSavingsPlansRequestRequestTypeDef,
     DescribeSavingsPlansResponseTypeDef,
@@ -340,15 +339,15 @@
     SavingsPlanRateTypeDef,
     DescribeSavingsPlansOfferingsResponseTypeDef,
     DescribeSavingsPlansOfferingRatesResponseTypeDef,
     DescribeSavingsPlanRatesResponseTypeDef,
 )
 
 
-def get_value() -> TimestampTypeDef:
+def get_structure() -> CreateSavingsPlanRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-savingsplans-1.28.16/mypy_boto3_savingsplans.egg-info/SOURCES.txt` & `mypy-boto3-savingsplans-1.28.7/mypy_boto3_savingsplans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-savingsplans-1.28.16/setup.py` & `mypy-boto3-savingsplans-1.28.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-savingsplans",
-    version="1.28.16",
+    version="1.28.7",
     packages=["mypy_boto3_savingsplans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SavingsPlans 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.SavingsPlans 1.28.7 service generated with mypy-boto3-builder"
+        " 7.15.1"
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
-    keywords="boto3 savingsplans type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 savingsplans type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_savingsplans": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

