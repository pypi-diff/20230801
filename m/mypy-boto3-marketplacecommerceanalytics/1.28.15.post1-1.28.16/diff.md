# Comparing `tmp/mypy-boto3-marketplacecommerceanalytics-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-marketplacecommerceanalytics-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-marketplacecommerceanalytics-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:37 2023, max compression
+gzip compressed data, was "mypy-boto3-marketplacecommerceanalytics-1.28.16.tar", last modified: Tue Aug  1 11:37:17 2023, max compression
```

## Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1.tar` & `mypy-boto3-marketplacecommerceanalytics-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.473270 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-07-29 10:03:37.465270 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.465270 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-29 09:50:36.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-29 09:50:36.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-29 09:50:36.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:37.465270 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-07-29 10:03:37.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-29 10:03:37.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:37.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:37.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:37.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 10:03:37.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:37.473270 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-29 09:50:35.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.340828 mypy-boto3-marketplacecommerceanalytics-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-08-01 11:37:17.332828 mypy-boto3-marketplacecommerceanalytics-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.332828 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:17.332828 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-08-01 11:37:17.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-01 11:37:17.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:17.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:17.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:17.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 11:37:17.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:17.340828 mypy-boto3-marketplacecommerceanalytics-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-01 11:23:28.000000 mypy-boto3-marketplacecommerceanalytics-1.28.16/setup.py
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/LICENSE` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/PKG-INFO` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplacecommerceanalytics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 marketplacecommerceanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 marketplacecommerceanalytics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplacecommerceanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplacecommerceanalytics)](https://pepy.tech/project/mypy-boto3-marketplacecommerceanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCommerceAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
+[boto3.MarketplaceCommerceAnalytics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
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
 [mypy-boto3-marketplacecommerceanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -290,32 +290,34 @@
 )
 
 
 def check_value(value: DataSetTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_marketplacecommerceanalytics.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_marketplacecommerceanalytics.type_defs import (
-    GenerateDataSetRequestRequestTypeDef,
+    TimestampTypeDef,
     ResponseMetadataTypeDef,
+    GenerateDataSetRequestRequestTypeDef,
     StartSupportDataExportRequestRequestTypeDef,
     GenerateDataSetResultTypeDef,
     StartSupportDataExportResultTypeDef,
 )
 
 
-def get_structure() -> GenerateDataSetRequestRequestTypeDef:
+def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/README.md` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplacecommerceanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplacecommerceanalytics)](https://pepy.tech/project/mypy-boto3-marketplacecommerceanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCommerceAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
+[boto3.MarketplaceCommerceAnalytics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
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
 [mypy-boto3-marketplacecommerceanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -258,32 +258,34 @@
 )
 
 
 def check_value(value: DataSetTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_marketplacecommerceanalytics.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_marketplacecommerceanalytics.type_defs import (
-    GenerateDataSetRequestRequestTypeDef,
+    TimestampTypeDef,
     ResponseMetadataTypeDef,
+    GenerateDataSetRequestRequestTypeDef,
     StartSupportDataExportRequestRequestTypeDef,
     GenerateDataSetResultTypeDef,
     StartSupportDataExportResultTypeDef,
 )
 
 
-def get_structure() -> GenerateDataSetRequestRequestTypeDef:
+def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/__init__.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/__init__.pyi` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/__main__.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics\nOther"
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

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/client.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,24 @@
     from boto3.session import Session
     from mypy_boto3_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient
 
     session = Session()
     client: MarketplaceCommerceAnalyticsClient = session.client("marketplacecommerceanalytics")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DataSetTypeType, SupportDataSetTypeType
-from .type_defs import GenerateDataSetResultTypeDef, StartSupportDataExportResultTypeDef
+from .type_defs import (
+    GenerateDataSetResultTypeDef,
+    StartSupportDataExportResultTypeDef,
+    TimestampTypeDef,
+)
 
 __all__ = ("MarketplaceCommerceAnalyticsClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -70,15 +73,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/client/#close)
         """
 
     def generate_data_set(
         self,
         *,
         dataSetType: DataSetTypeType,
-        dataSetPublicationDate: Union[datetime, str],
+        dataSetPublicationDate: TimestampTypeDef,
         roleNameArn: str,
         destinationS3BucketName: str,
         snsTopicArn: str,
         destinationS3Prefix: str = ...,
         customerDefinedValues: Mapping[str, str] = ...
     ) -> GenerateDataSetResultTypeDef:
         """
@@ -104,15 +107,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/client/#generate_presigned_url)
         """
 
     def start_support_data_export(
         self,
         *,
         dataSetType: SupportDataSetTypeType,
-        fromDate: Union[datetime, str],
+        fromDate: TimestampTypeDef,
         roleNameArn: str,
         destinationS3BucketName: str,
         snsTopicArn: str,
         destinationS3Prefix: str = ...,
         customerDefinedValues: Mapping[str, str] = ...
     ) -> StartSupportDataExportResultTypeDef:
         """
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/client.pyi` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,24 @@
     from boto3.session import Session
     from mypy_boto3_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient
 
     session = Session()
     client: MarketplaceCommerceAnalyticsClient = session.client("marketplacecommerceanalytics")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DataSetTypeType, SupportDataSetTypeType
-from .type_defs import GenerateDataSetResultTypeDef, StartSupportDataExportResultTypeDef
+from .type_defs import (
+    GenerateDataSetResultTypeDef,
+    StartSupportDataExportResultTypeDef,
+    TimestampTypeDef,
+)
 
 __all__ = ("MarketplaceCommerceAnalyticsClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -64,15 +67,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/client/#close)
         """
     def generate_data_set(
         self,
         *,
         dataSetType: DataSetTypeType,
-        dataSetPublicationDate: Union[datetime, str],
+        dataSetPublicationDate: TimestampTypeDef,
         roleNameArn: str,
         destinationS3BucketName: str,
         snsTopicArn: str,
         destinationS3Prefix: str = ...,
         customerDefinedValues: Mapping[str, str] = ...
     ) -> GenerateDataSetResultTypeDef:
         """
@@ -96,15 +99,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/client/#generate_presigned_url)
         """
     def start_support_data_export(
         self,
         *,
         dataSetType: SupportDataSetTypeType,
-        fromDate: Union[datetime, str],
+        fromDate: TimestampTypeDef,
         roleNameArn: str,
         destinationS3BucketName: str,
         snsTopicArn: str,
         destinationS3Prefix: str = ...,
         customerDefinedValues: Mapping[str, str] = ...
     ) -> StartSupportDataExportResultTypeDef:
         """
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/literals.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/literals.pyi` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/type_defs.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,103 +2,100 @@
 Type annotations for marketplacecommerceanalytics service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_marketplacecommerceanalytics.type_defs import GenerateDataSetRequestRequestTypeDef
+    from mypy_boto3_marketplacecommerceanalytics.type_defs import TimestampTypeDef
 
-    data: GenerateDataSetRequestRequestTypeDef = {...}
+    data: TimestampTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Mapping, Union
 
 from .literals import DataSetTypeType, SupportDataSetTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "GenerateDataSetRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ResponseMetadataTypeDef",
+    "GenerateDataSetRequestRequestTypeDef",
     "StartSupportDataExportRequestRequestTypeDef",
     "GenerateDataSetResultTypeDef",
     "StartSupportDataExportResultTypeDef",
 )
 
+TimestampTypeDef = Union[datetime, str]
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredGenerateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataSetRequestRequestTypeDef",
     {
         "dataSetType": DataSetTypeType,
-        "dataSetPublicationDate": Union[datetime, str],
+        "dataSetPublicationDate": TimestampTypeDef,
         "roleNameArn": str,
         "destinationS3BucketName": str,
         "snsTopicArn": str,
     },
 )
 _OptionalGenerateDataSetRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataSetRequestRequestTypeDef",
     {
         "destinationS3Prefix": str,
         "customerDefinedValues": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GenerateDataSetRequestRequestTypeDef(
     _RequiredGenerateDataSetRequestRequestTypeDef, _OptionalGenerateDataSetRequestRequestTypeDef
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredStartSupportDataExportRequestRequestTypeDef = TypedDict(
     "_RequiredStartSupportDataExportRequestRequestTypeDef",
     {
         "dataSetType": SupportDataSetTypeType,
-        "fromDate": Union[datetime, str],
+        "fromDate": TimestampTypeDef,
         "roleNameArn": str,
         "destinationS3BucketName": str,
         "snsTopicArn": str,
     },
 )
 _OptionalStartSupportDataExportRequestRequestTypeDef = TypedDict(
     "_OptionalStartSupportDataExportRequestRequestTypeDef",
     {
         "destinationS3Prefix": str,
         "customerDefinedValues": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartSupportDataExportRequestRequestTypeDef(
     _RequiredStartSupportDataExportRequestRequestTypeDef,
     _OptionalStartSupportDataExportRequestRequestTypeDef,
 ):
     pass
 
-
 GenerateDataSetResultTypeDef = TypedDict(
     "GenerateDataSetResultTypeDef",
     {
         "dataSetRequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics/type_defs.pyi` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,98 +2,105 @@
 Type annotations for marketplacecommerceanalytics service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_marketplacecommerceanalytics.type_defs import GenerateDataSetRequestRequestTypeDef
+    from mypy_boto3_marketplacecommerceanalytics.type_defs import TimestampTypeDef
 
-    data: GenerateDataSetRequestRequestTypeDef = {...}
+    data: TimestampTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Mapping, Union
 
 from .literals import DataSetTypeType, SupportDataSetTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "GenerateDataSetRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ResponseMetadataTypeDef",
+    "GenerateDataSetRequestRequestTypeDef",
     "StartSupportDataExportRequestRequestTypeDef",
     "GenerateDataSetResultTypeDef",
     "StartSupportDataExportResultTypeDef",
 )
 
+TimestampTypeDef = Union[datetime, str]
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredGenerateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataSetRequestRequestTypeDef",
     {
         "dataSetType": DataSetTypeType,
-        "dataSetPublicationDate": Union[datetime, str],
+        "dataSetPublicationDate": TimestampTypeDef,
         "roleNameArn": str,
         "destinationS3BucketName": str,
         "snsTopicArn": str,
     },
 )
 _OptionalGenerateDataSetRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataSetRequestRequestTypeDef",
     {
         "destinationS3Prefix": str,
         "customerDefinedValues": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GenerateDataSetRequestRequestTypeDef(
     _RequiredGenerateDataSetRequestRequestTypeDef, _OptionalGenerateDataSetRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
 
 _RequiredStartSupportDataExportRequestRequestTypeDef = TypedDict(
     "_RequiredStartSupportDataExportRequestRequestTypeDef",
     {
         "dataSetType": SupportDataSetTypeType,
-        "fromDate": Union[datetime, str],
+        "fromDate": TimestampTypeDef,
         "roleNameArn": str,
         "destinationS3BucketName": str,
         "snsTopicArn": str,
     },
 )
 _OptionalStartSupportDataExportRequestRequestTypeDef = TypedDict(
     "_OptionalStartSupportDataExportRequestRequestTypeDef",
     {
         "destinationS3Prefix": str,
         "customerDefinedValues": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartSupportDataExportRequestRequestTypeDef(
     _RequiredStartSupportDataExportRequestRequestTypeDef,
     _OptionalStartSupportDataExportRequestRequestTypeDef,
 ):
     pass
 
+
 GenerateDataSetResultTypeDef = TypedDict(
     "GenerateDataSetResultTypeDef",
     {
         "dataSetRequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics.egg-info/PKG-INFO` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplacecommerceanalytics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 marketplacecommerceanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 marketplacecommerceanalytics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplacecommerceanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplacecommerceanalytics)](https://pepy.tech/project/mypy-boto3-marketplacecommerceanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCommerceAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
+[boto3.MarketplaceCommerceAnalytics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
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
 [mypy-boto3-marketplacecommerceanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -290,32 +290,34 @@
 )
 
 
 def check_value(value: DataSetTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_marketplacecommerceanalytics.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_marketplacecommerceanalytics.type_defs import (
-    GenerateDataSetRequestRequestTypeDef,
+    TimestampTypeDef,
     ResponseMetadataTypeDef,
+    GenerateDataSetRequestRequestTypeDef,
     StartSupportDataExportRequestRequestTypeDef,
     GenerateDataSetResultTypeDef,
     StartSupportDataExportResultTypeDef,
 )
 
 
-def get_structure() -> GenerateDataSetRequestRequestTypeDef:
+def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/mypy_boto3_marketplacecommerceanalytics.egg-info/SOURCES.txt` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/mypy_boto3_marketplacecommerceanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.15.post1/setup.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-marketplacecommerceanalytics",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_marketplacecommerceanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.16 service generated with"
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
-        "boto3 marketplacecommerceanalytics type-annotations boto3-stubs mypy typeshed autocomplete"
+        "boto3 marketplacecommerceanalytics type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_marketplacecommerceanalytics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
```

