# Comparing `tmp/mypy-boto3-pricing-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-pricing-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pricing-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:54 2023, max compression
+gzip compressed data, was "mypy-boto3-pricing-1.28.16.tar", last modified: Tue Aug  1 11:37:34 2023, max compression
```

## Comparing `mypy-boto3-pricing-1.28.15.post1.tar` & `mypy-boto3-pricing-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.789344 mypy-boto3-pricing-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-29 10:03:54.789344 mypy-boto3-pricing-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.777344 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.789344 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-29 10:03:54.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:03:54.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:54.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:03:54.000000 mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:54.789344 mypy-boto3-pricing-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:53:29.000000 mypy-boto3-pricing-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.592786 mypy-boto3-pricing-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-08-01 11:37:34.592786 mypy-boto3-pricing-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.592786 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.592786 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-08-01 11:37:34.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:37:34.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:34.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:34.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:34.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:37:34.000000 mypy-boto3-pricing-1.28.16/mypy_boto3_pricing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:34.592786 mypy-boto3-pricing-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:26:32.000000 mypy-boto3-pricing-1.28.16/setup.py
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/LICENSE` & `mypy-boto3-pricing-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.15.post1/PKG-INFO` & `mypy-boto3-pricing-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pricing
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Pricing 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Pricing 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pricing type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pricing type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pricing)](https://pepy.tech/project/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
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
@@ -323,47 +323,48 @@
 )
 
 
 def check_value(value: DescribeServicesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pricing.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pricing.type_defs import (
     AttributeValueTypeDef,
     PaginatorConfigTypeDef,
     DescribeServicesRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ServiceTypeDef,
     FilterTypeDef,
     GetAttributeValuesRequestRequestTypeDef,
     GetPriceListFileUrlRequestRequestTypeDef,
-    ListPriceListsRequestRequestTypeDef,
+    TimestampTypeDef,
     PriceListTypeDef,
     DescribeServicesRequestDescribeServicesPaginateTypeDef,
     GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    ListPriceListsRequestListPriceListsPaginateTypeDef,
     GetAttributeValuesResponseTypeDef,
     GetPriceListFileUrlResponseTypeDef,
     GetProductsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     GetProductsRequestGetProductsPaginateTypeDef,
     GetProductsRequestRequestTypeDef,
+    ListPriceListsRequestListPriceListsPaginateTypeDef,
+    ListPriceListsRequestRequestTypeDef,
     ListPriceListsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeValueTypeDef:
+def get_value() -> AttributeValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/README.md` & `mypy-boto3-pricing-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pricing)](https://pepy.tech/project/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
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
@@ -291,47 +291,48 @@
 )
 
 
 def check_value(value: DescribeServicesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pricing.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pricing.type_defs import (
     AttributeValueTypeDef,
     PaginatorConfigTypeDef,
     DescribeServicesRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ServiceTypeDef,
     FilterTypeDef,
     GetAttributeValuesRequestRequestTypeDef,
     GetPriceListFileUrlRequestRequestTypeDef,
-    ListPriceListsRequestRequestTypeDef,
+    TimestampTypeDef,
     PriceListTypeDef,
     DescribeServicesRequestDescribeServicesPaginateTypeDef,
     GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    ListPriceListsRequestListPriceListsPaginateTypeDef,
     GetAttributeValuesResponseTypeDef,
     GetPriceListFileUrlResponseTypeDef,
     GetProductsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     GetProductsRequestGetProductsPaginateTypeDef,
     GetProductsRequestRequestTypeDef,
+    ListPriceListsRequestListPriceListsPaginateTypeDef,
+    ListPriceListsRequestRequestTypeDef,
     ListPriceListsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeValueTypeDef:
+def get_value() -> AttributeValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/__init__.py` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/__init__.pyi` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/__main__.py` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pricing 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Pricing 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing\nOther"
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

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/client.py` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_pricing.client import PricingClient
 
     session = Session()
     client: PricingClient = session.client("pricing")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     DescribeServicesPaginator,
     GetAttributeValuesPaginator,
     GetProductsPaginator,
@@ -28,14 +27,15 @@
 from .type_defs import (
     DescribeServicesResponseTypeDef,
     FilterTypeDef,
     GetAttributeValuesResponseTypeDef,
     GetPriceListFileUrlResponseTypeDef,
     GetProductsResponseTypeDef,
     ListPriceListsResponseTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -159,15 +159,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/client/#get_products)
         """
 
     def list_price_lists(
         self,
         *,
         ServiceCode: str,
-        EffectiveDate: Union[datetime, str],
+        EffectiveDate: TimestampTypeDef,
         CurrencyCode: str,
         RegionCode: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPriceListsResponseTypeDef:
         """
         This feature is in preview release and is subject to change.
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/client.pyi` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_pricing.client import PricingClient
 
     session = Session()
     client: PricingClient = session.client("pricing")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     DescribeServicesPaginator,
     GetAttributeValuesPaginator,
     GetProductsPaginator,
@@ -28,14 +27,15 @@
 from .type_defs import (
     DescribeServicesResponseTypeDef,
     FilterTypeDef,
     GetAttributeValuesResponseTypeDef,
     GetPriceListFileUrlResponseTypeDef,
     GetProductsResponseTypeDef,
     ListPriceListsResponseTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -147,15 +147,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.get_products)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/client/#get_products)
         """
     def list_price_lists(
         self,
         *,
         ServiceCode: str,
-        EffectiveDate: Union[datetime, str],
+        EffectiveDate: TimestampTypeDef,
         CurrencyCode: str,
         RegionCode: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPriceListsResponseTypeDef:
         """
         This feature is in preview release and is subject to change.
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/literals.py` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/literals.pyi` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/paginator.py` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
     describe_services_paginator: DescribeServicesPaginator = client.get_paginator("describe_services")
     get_attribute_values_paginator: GetAttributeValuesPaginator = client.get_paginator("get_attribute_values")
     get_products_paginator: GetProductsPaginator = client.get_paginator("get_products")
     list_price_lists_paginator: ListPriceListsPaginator = client.get_paginator("list_price_lists")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeServicesResponseTypeDef,
     FilterTypeDef,
     GetAttributeValuesResponseTypeDef,
     GetProductsResponseTypeDef,
     ListPriceListsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeServicesPaginator",
     "GetAttributeValuesPaginator",
     "GetProductsPaginator",
     "ListPriceListsPaginator",
@@ -121,15 +121,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#listpricelistspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
-        EffectiveDate: Union[datetime, str],
+        EffectiveDate: TimestampTypeDef,
         CurrencyCode: str,
         RegionCode: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPriceListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.ListPriceLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#listpricelistspaginator)
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/paginator.pyi` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
     describe_services_paginator: DescribeServicesPaginator = client.get_paginator("describe_services")
     get_attribute_values_paginator: GetAttributeValuesPaginator = client.get_paginator("get_attribute_values")
     get_products_paginator: GetProductsPaginator = client.get_paginator("get_products")
     list_price_lists_paginator: ListPriceListsPaginator = client.get_paginator("list_price_lists")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeServicesResponseTypeDef,
     FilterTypeDef,
     GetAttributeValuesResponseTypeDef,
     GetProductsResponseTypeDef,
     ListPriceListsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeServicesPaginator",
     "GetAttributeValuesPaginator",
     "GetProductsPaginator",
     "ListPriceListsPaginator",
@@ -115,15 +115,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#listpricelistspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
-        EffectiveDate: Union[datetime, str],
+        EffectiveDate: TimestampTypeDef,
         CurrencyCode: str,
         RegionCode: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPriceListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.ListPriceLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#listpricelistspaginator)
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/type_defs.py` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pricing.type_defs import AttributeValueTypeDef
 
-    data: AttributeValueTypeDef = {...}
+    data: AttributeValueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 if sys.version_info >= (3, 9):
@@ -30,25 +30,26 @@
     "PaginatorConfigTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ServiceTypeDef",
     "FilterTypeDef",
     "GetAttributeValuesRequestRequestTypeDef",
     "GetPriceListFileUrlRequestRequestTypeDef",
-    "ListPriceListsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PriceListTypeDef",
     "DescribeServicesRequestDescribeServicesPaginateTypeDef",
     "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
-    "ListPriceListsRequestListPriceListsPaginateTypeDef",
     "GetAttributeValuesResponseTypeDef",
     "GetPriceListFileUrlResponseTypeDef",
     "GetProductsResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "GetProductsRequestGetProductsPaginateTypeDef",
     "GetProductsRequestRequestTypeDef",
+    "ListPriceListsRequestListPriceListsPaginateTypeDef",
+    "ListPriceListsRequestRequestTypeDef",
     "ListPriceListsResponseTypeDef",
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "Value": str,
@@ -144,39 +145,15 @@
     "GetPriceListFileUrlRequestRequestTypeDef",
     {
         "PriceListArn": str,
         "FileFormat": str,
     },
 )
 
-_RequiredListPriceListsRequestRequestTypeDef = TypedDict(
-    "_RequiredListPriceListsRequestRequestTypeDef",
-    {
-        "ServiceCode": str,
-        "EffectiveDate": Union[datetime, str],
-        "CurrencyCode": str,
-    },
-)
-_OptionalListPriceListsRequestRequestTypeDef = TypedDict(
-    "_OptionalListPriceListsRequestRequestTypeDef",
-    {
-        "RegionCode": str,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListPriceListsRequestRequestTypeDef(
-    _RequiredListPriceListsRequestRequestTypeDef, _OptionalListPriceListsRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 PriceListTypeDef = TypedDict(
     "PriceListTypeDef",
     {
         "PriceListArn": str,
         "RegionCode": str,
         "CurrencyCode": str,
         "FileFormats": List[str],
@@ -213,39 +190,14 @@
 class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
     _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
     _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "EffectiveDate": Union[datetime, str],
-        "CurrencyCode": str,
-    },
-)
-_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
-    {
-        "RegionCode": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPriceListsRequestListPriceListsPaginateTypeDef(
-    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
-    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
-):
-    pass
-
-
 GetAttributeValuesResponseTypeDef = TypedDict(
     "GetAttributeValuesResponseTypeDef",
     {
         "AttributeValues": List[AttributeValueTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -323,14 +275,64 @@
 
 class GetProductsRequestRequestTypeDef(
     _RequiredGetProductsRequestRequestTypeDef, _OptionalGetProductsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "EffectiveDate": TimestampTypeDef,
+        "CurrencyCode": str,
+    },
+)
+_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "RegionCode": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPriceListsRequestListPriceListsPaginateTypeDef(
+    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
+    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPriceListsRequestRequestTypeDef = TypedDict(
+    "_RequiredListPriceListsRequestRequestTypeDef",
+    {
+        "ServiceCode": str,
+        "EffectiveDate": TimestampTypeDef,
+        "CurrencyCode": str,
+    },
+)
+_OptionalListPriceListsRequestRequestTypeDef = TypedDict(
+    "_OptionalListPriceListsRequestRequestTypeDef",
+    {
+        "RegionCode": str,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListPriceListsRequestRequestTypeDef(
+    _RequiredListPriceListsRequestRequestTypeDef, _OptionalListPriceListsRequestRequestTypeDef
+):
+    pass
+
+
 ListPriceListsResponseTypeDef = TypedDict(
     "ListPriceListsResponseTypeDef",
     {
         "PriceLists": List[PriceListTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing/type_defs.pyi` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pricing.type_defs import AttributeValueTypeDef
 
-    data: AttributeValueTypeDef = {...}
+    data: AttributeValueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 if sys.version_info >= (3, 9):
@@ -29,25 +29,26 @@
     "PaginatorConfigTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ServiceTypeDef",
     "FilterTypeDef",
     "GetAttributeValuesRequestRequestTypeDef",
     "GetPriceListFileUrlRequestRequestTypeDef",
-    "ListPriceListsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PriceListTypeDef",
     "DescribeServicesRequestDescribeServicesPaginateTypeDef",
     "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
-    "ListPriceListsRequestListPriceListsPaginateTypeDef",
     "GetAttributeValuesResponseTypeDef",
     "GetPriceListFileUrlResponseTypeDef",
     "GetProductsResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "GetProductsRequestGetProductsPaginateTypeDef",
     "GetProductsRequestRequestTypeDef",
+    "ListPriceListsRequestListPriceListsPaginateTypeDef",
+    "ListPriceListsRequestRequestTypeDef",
     "ListPriceListsResponseTypeDef",
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "Value": str,
@@ -139,37 +140,15 @@
     "GetPriceListFileUrlRequestRequestTypeDef",
     {
         "PriceListArn": str,
         "FileFormat": str,
     },
 )
 
-_RequiredListPriceListsRequestRequestTypeDef = TypedDict(
-    "_RequiredListPriceListsRequestRequestTypeDef",
-    {
-        "ServiceCode": str,
-        "EffectiveDate": Union[datetime, str],
-        "CurrencyCode": str,
-    },
-)
-_OptionalListPriceListsRequestRequestTypeDef = TypedDict(
-    "_OptionalListPriceListsRequestRequestTypeDef",
-    {
-        "RegionCode": str,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListPriceListsRequestRequestTypeDef(
-    _RequiredListPriceListsRequestRequestTypeDef, _OptionalListPriceListsRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 PriceListTypeDef = TypedDict(
     "PriceListTypeDef",
     {
         "PriceListArn": str,
         "RegionCode": str,
         "CurrencyCode": str,
         "FileFormats": List[str],
@@ -204,37 +183,14 @@
 
 class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
     _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
     _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
 ):
     pass
 
-_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "EffectiveDate": Union[datetime, str],
-        "CurrencyCode": str,
-    },
-)
-_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
-    {
-        "RegionCode": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPriceListsRequestListPriceListsPaginateTypeDef(
-    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
-    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
-):
-    pass
-
 GetAttributeValuesResponseTypeDef = TypedDict(
     "GetAttributeValuesResponseTypeDef",
     {
         "AttributeValues": List[AttributeValueTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -308,14 +264,60 @@
 )
 
 class GetProductsRequestRequestTypeDef(
     _RequiredGetProductsRequestRequestTypeDef, _OptionalGetProductsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "EffectiveDate": TimestampTypeDef,
+        "CurrencyCode": str,
+    },
+)
+_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "RegionCode": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPriceListsRequestListPriceListsPaginateTypeDef(
+    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
+    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPriceListsRequestRequestTypeDef = TypedDict(
+    "_RequiredListPriceListsRequestRequestTypeDef",
+    {
+        "ServiceCode": str,
+        "EffectiveDate": TimestampTypeDef,
+        "CurrencyCode": str,
+    },
+)
+_OptionalListPriceListsRequestRequestTypeDef = TypedDict(
+    "_OptionalListPriceListsRequestRequestTypeDef",
+    {
+        "RegionCode": str,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListPriceListsRequestRequestTypeDef(
+    _RequiredListPriceListsRequestRequestTypeDef, _OptionalListPriceListsRequestRequestTypeDef
+):
+    pass
+
 ListPriceListsResponseTypeDef = TypedDict(
     "ListPriceListsResponseTypeDef",
     {
         "PriceLists": List[PriceListTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing.egg-info/PKG-INFO` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pricing
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Pricing 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Pricing 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pricing type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pricing type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pricing)](https://pepy.tech/project/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
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
@@ -323,47 +323,48 @@
 )
 
 
 def check_value(value: DescribeServicesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pricing.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pricing.type_defs import (
     AttributeValueTypeDef,
     PaginatorConfigTypeDef,
     DescribeServicesRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ServiceTypeDef,
     FilterTypeDef,
     GetAttributeValuesRequestRequestTypeDef,
     GetPriceListFileUrlRequestRequestTypeDef,
-    ListPriceListsRequestRequestTypeDef,
+    TimestampTypeDef,
     PriceListTypeDef,
     DescribeServicesRequestDescribeServicesPaginateTypeDef,
     GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    ListPriceListsRequestListPriceListsPaginateTypeDef,
     GetAttributeValuesResponseTypeDef,
     GetPriceListFileUrlResponseTypeDef,
     GetProductsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     GetProductsRequestGetProductsPaginateTypeDef,
     GetProductsRequestRequestTypeDef,
+    ListPriceListsRequestListPriceListsPaginateTypeDef,
+    ListPriceListsRequestRequestTypeDef,
     ListPriceListsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeValueTypeDef:
+def get_value() -> AttributeValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pricing-1.28.15.post1/mypy_boto3_pricing.egg-info/SOURCES.txt` & `mypy-boto3-pricing-1.28.16/mypy_boto3_pricing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.15.post1/setup.py` & `mypy-boto3-pricing-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pricing",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_pricing"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pricing 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Pricing 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 pricing type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 pricing type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_pricing": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

