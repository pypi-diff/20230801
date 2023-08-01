# Comparing `tmp/mypy-boto3-meteringmarketplace-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-meteringmarketplace-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-meteringmarketplace-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:41 2023, max compression
+gzip compressed data, was "mypy-boto3-meteringmarketplace-1.28.16.tar", last modified: Tue Aug  1 11:37:22 2023, max compression
```

## Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1.tar` & `mypy-boto3-meteringmarketplace-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:41.801289 mypy-boto3-meteringmarketplace-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-29 10:03:41.801289 mypy-boto3-meteringmarketplace-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:41.793289 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-29 09:51:30.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-29 09:51:30.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-29 09:51:30.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-29 09:51:30.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:41.801289 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:41.801289 mypy-boto3-meteringmarketplace-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:22.228817 mypy-boto3-meteringmarketplace-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:28.000000 mypy-boto3-meteringmarketplace-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-08-01 11:37:22.224817 mypy-boto3-meteringmarketplace-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-08-01 11:24:28.000000 mypy-boto3-meteringmarketplace-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:22.216817 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 11:24:28.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 11:24:28.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-01 11:24:28.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-08-01 11:24:29.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-08-01 11:24:29.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-08-01 11:24:29.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-08-01 11:24:29.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:28.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-08-01 11:24:29.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-08-01 11:24:29.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:28.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:22.224817 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-08-01 11:37:21.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-01 11:37:22.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:21.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:21.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:21.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 11:37:21.000000 mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:22.228817 mypy-boto3-meteringmarketplace-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-01 11:24:28.000000 mypy-boto3-meteringmarketplace-1.28.16/setup.py
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/LICENSE` & `mypy-boto3-meteringmarketplace-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MarketplaceMetering 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 meteringmarketplace type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 meteringmarketplace type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-meteringmarketplace)](https://pepy.tech/project/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
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
@@ -289,42 +289,45 @@
 )
 
 
 def check_value(value: UsageRecordResultStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_meteringmarketplace.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_meteringmarketplace.type_defs import (
     ResponseMetadataTypeDef,
+    TimestampTypeDef,
     RegisterUsageRequestRequestTypeDef,
     ResolveCustomerRequestRequestTypeDef,
     TagTypeDef,
     MeterUsageResultTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerResultTypeDef,
     UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
     UsageRecordOutputTypeDef,
-    MeterUsageRequestRequestTypeDef,
+    UsageAllocationUnionTypeDef,
     UsageRecordTypeDef,
     UsageRecordResultTypeDef,
-    BatchMeterUsageRequestRequestTypeDef,
+    MeterUsageRequestRequestTypeDef,
+    UsageRecordUnionTypeDef,
     BatchMeterUsageResultTypeDef,
+    BatchMeterUsageRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/README.md` & `mypy-boto3-meteringmarketplace-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-meteringmarketplace)](https://pepy.tech/project/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
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
@@ -257,42 +257,45 @@
 )
 
 
 def check_value(value: UsageRecordResultStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_meteringmarketplace.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_meteringmarketplace.type_defs import (
     ResponseMetadataTypeDef,
+    TimestampTypeDef,
     RegisterUsageRequestRequestTypeDef,
     ResolveCustomerRequestRequestTypeDef,
     TagTypeDef,
     MeterUsageResultTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerResultTypeDef,
     UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
     UsageRecordOutputTypeDef,
-    MeterUsageRequestRequestTypeDef,
+    UsageAllocationUnionTypeDef,
     UsageRecordTypeDef,
     UsageRecordResultTypeDef,
-    BatchMeterUsageRequestRequestTypeDef,
+    MeterUsageRequestRequestTypeDef,
+    UsageRecordUnionTypeDef,
     BatchMeterUsageResultTypeDef,
+    BatchMeterUsageRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/__main__.py` & `mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceMetering 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MarketplaceMetering 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering\nOther"
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

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/client.py` & `mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,41 +9,37 @@
     from boto3.session import Session
     from mypy_boto3_meteringmarketplace.client import MarketplaceMeteringClient
 
     session = Session()
     client: MarketplaceMeteringClient = session.client("meteringmarketplace")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     BatchMeterUsageResultTypeDef,
     MeterUsageResultTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerResultTypeDef,
-    UsageAllocationOutputTypeDef,
-    UsageAllocationTypeDef,
-    UsageRecordOutputTypeDef,
-    UsageRecordTypeDef,
+    TimestampTypeDef,
+    UsageAllocationUnionTypeDef,
+    UsageRecordUnionTypeDef,
 )
 
 __all__ = ("MarketplaceMeteringClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     CustomerNotEntitledException: Type[BotocoreClientError]
     DisabledApiException: Type[BotocoreClientError]
     DuplicateRequestException: Type[BotocoreClientError]
     ExpiredTokenException: Type[BotocoreClientError]
     InternalServiceErrorException: Type[BotocoreClientError]
@@ -56,15 +52,14 @@
     InvalidTokenException: Type[BotocoreClientError]
     InvalidUsageAllocationsException: Type[BotocoreClientError]
     InvalidUsageDimensionException: Type[BotocoreClientError]
     PlatformNotSupportedException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TimestampOutOfBoundsException: Type[BotocoreClientError]
 
-
 class MarketplaceMeteringClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/)
     """
 
     meta: ClientMeta
@@ -73,90 +68,78 @@
     def exceptions(self) -> Exceptions:
         """
         MarketplaceMeteringClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#exceptions)
         """
-
     def batch_meter_usage(
-        self,
-        *,
-        UsageRecords: Sequence[Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]],
-        ProductCode: str
+        self, *, UsageRecords: Sequence[UsageRecordUnionTypeDef], ProductCode: str
     ) -> BatchMeterUsageResultTypeDef:
         """
         `BatchMeterUsage` is called from a SaaS application listed on AWS Marketplace to
         post metering records for a set of customers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.batch_meter_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#batch_meter_usage)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#close)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#generate_presigned_url)
         """
-
     def meter_usage(
         self,
         *,
         ProductCode: str,
-        Timestamp: Union[datetime, str],
+        Timestamp: TimestampTypeDef,
         UsageDimension: str,
         UsageQuantity: int = ...,
         DryRun: bool = ...,
-        UsageAllocations: Sequence[
-            Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]
-        ] = ...
+        UsageAllocations: Sequence[UsageAllocationUnionTypeDef] = ...
     ) -> MeterUsageResultTypeDef:
         """
         API to emit metering records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.meter_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#meter_usage)
         """
-
     def register_usage(
         self, *, ProductCode: str, PublicKeyVersion: int, Nonce: str = ...
     ) -> RegisterUsageResultTypeDef:
         """
         Paid container software products sold through AWS Marketplace must integrate
         with the AWS Marketplace Metering Service and call the `RegisterUsage` operation
         for software entitlement and metering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.register_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#register_usage)
         """
-
     def resolve_customer(self, *, RegistrationToken: str) -> ResolveCustomerResultTypeDef:
         """
         `ResolveCustomer` is called by a SaaS application during the registration
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.resolve_customer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#resolve_customer)
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/client.pyi` & `mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,39 +9,39 @@
     from boto3.session import Session
     from mypy_boto3_meteringmarketplace.client import MarketplaceMeteringClient
 
     session = Session()
     client: MarketplaceMeteringClient = session.client("meteringmarketplace")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     BatchMeterUsageResultTypeDef,
     MeterUsageResultTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerResultTypeDef,
-    UsageAllocationOutputTypeDef,
-    UsageAllocationTypeDef,
-    UsageRecordOutputTypeDef,
-    UsageRecordTypeDef,
+    TimestampTypeDef,
+    UsageAllocationUnionTypeDef,
+    UsageRecordUnionTypeDef,
 )
 
 __all__ = ("MarketplaceMeteringClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     CustomerNotEntitledException: Type[BotocoreClientError]
     DisabledApiException: Type[BotocoreClientError]
     DuplicateRequestException: Type[BotocoreClientError]
     ExpiredTokenException: Type[BotocoreClientError]
     InternalServiceErrorException: Type[BotocoreClientError]
@@ -54,14 +54,15 @@
     InvalidTokenException: Type[BotocoreClientError]
     InvalidUsageAllocationsException: Type[BotocoreClientError]
     InvalidUsageDimensionException: Type[BotocoreClientError]
     PlatformNotSupportedException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TimestampOutOfBoundsException: Type[BotocoreClientError]
 
+
 class MarketplaceMeteringClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/)
     """
 
     meta: ClientMeta
@@ -70,83 +71,85 @@
     def exceptions(self) -> Exceptions:
         """
         MarketplaceMeteringClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#exceptions)
         """
+
     def batch_meter_usage(
-        self,
-        *,
-        UsageRecords: Sequence[Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]],
-        ProductCode: str
+        self, *, UsageRecords: Sequence[UsageRecordUnionTypeDef], ProductCode: str
     ) -> BatchMeterUsageResultTypeDef:
         """
         `BatchMeterUsage` is called from a SaaS application listed on AWS Marketplace to
         post metering records for a set of customers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.batch_meter_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#batch_meter_usage)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#close)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#generate_presigned_url)
         """
+
     def meter_usage(
         self,
         *,
         ProductCode: str,
-        Timestamp: Union[datetime, str],
+        Timestamp: TimestampTypeDef,
         UsageDimension: str,
         UsageQuantity: int = ...,
         DryRun: bool = ...,
-        UsageAllocations: Sequence[
-            Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]
-        ] = ...
+        UsageAllocations: Sequence[UsageAllocationUnionTypeDef] = ...
     ) -> MeterUsageResultTypeDef:
         """
         API to emit metering records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.meter_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#meter_usage)
         """
+
     def register_usage(
         self, *, ProductCode: str, PublicKeyVersion: int, Nonce: str = ...
     ) -> RegisterUsageResultTypeDef:
         """
         Paid container software products sold through AWS Marketplace must integrate
         with the AWS Marketplace Metering Service and call the `RegisterUsage` operation
         for software entitlement and metering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.register_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#register_usage)
         """
+
     def resolve_customer(self, *, RegistrationToken: str) -> ResolveCustomerResultTypeDef:
         """
         `ResolveCustomer` is called by a SaaS application during the registration
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.resolve_customer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#resolve_customer)
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/literals.py` & `mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/literals.pyi` & `mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/type_defs.py` & `mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,58 +4,61 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_meteringmarketplace.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import UsageRecordResultStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "RegisterUsageRequestRequestTypeDef",
     "ResolveCustomerRequestRequestTypeDef",
     "TagTypeDef",
     "MeterUsageResultTypeDef",
     "RegisterUsageResultTypeDef",
     "ResolveCustomerResultTypeDef",
     "UsageAllocationOutputTypeDef",
     "UsageAllocationTypeDef",
     "UsageRecordOutputTypeDef",
-    "MeterUsageRequestRequestTypeDef",
+    "UsageAllocationUnionTypeDef",
     "UsageRecordTypeDef",
     "UsageRecordResultTypeDef",
-    "BatchMeterUsageRequestRequestTypeDef",
+    "MeterUsageRequestRequestTypeDef",
+    "UsageRecordUnionTypeDef",
     "BatchMeterUsageResultTypeDef",
+    "BatchMeterUsageRequestRequestTypeDef",
 )
 
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
 _RequiredRegisterUsageRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterUsageRequestRequestTypeDef",
     {
         "ProductCode": str,
         "PublicKeyVersion": int,
     },
 )
@@ -63,21 +66,19 @@
     "_OptionalRegisterUsageRequestRequestTypeDef",
     {
         "Nonce": str,
     },
     total=False,
 )
 
-
 class RegisterUsageRequestRequestTypeDef(
     _RequiredRegisterUsageRequestRequestTypeDef, _OptionalRegisterUsageRequestRequestTypeDef
 ):
     pass
 
-
 ResolveCustomerRequestRequestTypeDef = TypedDict(
     "ResolveCustomerRequestRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
@@ -126,40 +127,36 @@
     "_OptionalUsageAllocationOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class UsageAllocationOutputTypeDef(
     _RequiredUsageAllocationOutputTypeDef, _OptionalUsageAllocationOutputTypeDef
 ):
     pass
 
-
 _RequiredUsageAllocationTypeDef = TypedDict(
     "_RequiredUsageAllocationTypeDef",
     {
         "AllocatedUsageQuantity": int,
     },
 )
 _OptionalUsageAllocationTypeDef = TypedDict(
     "_OptionalUsageAllocationTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UsageAllocationTypeDef(_RequiredUsageAllocationTypeDef, _OptionalUsageAllocationTypeDef):
     pass
 
-
 _RequiredUsageRecordOutputTypeDef = TypedDict(
     "_RequiredUsageRecordOutputTypeDef",
     {
         "Timestamp": datetime,
         "CustomerIdentifier": str,
         "Dimension": str,
     },
@@ -169,87 +166,83 @@
     {
         "Quantity": int,
         "UsageAllocations": List[UsageAllocationOutputTypeDef],
     },
     total=False,
 )
 
-
 class UsageRecordOutputTypeDef(
     _RequiredUsageRecordOutputTypeDef, _OptionalUsageRecordOutputTypeDef
 ):
     pass
 
-
-_RequiredMeterUsageRequestRequestTypeDef = TypedDict(
-    "_RequiredMeterUsageRequestRequestTypeDef",
-    {
-        "ProductCode": str,
-        "Timestamp": Union[datetime, str],
-        "UsageDimension": str,
-    },
-)
-_OptionalMeterUsageRequestRequestTypeDef = TypedDict(
-    "_OptionalMeterUsageRequestRequestTypeDef",
-    {
-        "UsageQuantity": int,
-        "DryRun": bool,
-        "UsageAllocations": Sequence[Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]],
-    },
-    total=False,
-)
-
-
-class MeterUsageRequestRequestTypeDef(
-    _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
-):
-    pass
-
-
+UsageAllocationUnionTypeDef = Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]
 _RequiredUsageRecordTypeDef = TypedDict(
     "_RequiredUsageRecordTypeDef",
     {
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
         "CustomerIdentifier": str,
         "Dimension": str,
     },
 )
 _OptionalUsageRecordTypeDef = TypedDict(
     "_OptionalUsageRecordTypeDef",
     {
         "Quantity": int,
         "UsageAllocations": Sequence[UsageAllocationTypeDef],
     },
     total=False,
 )
 
-
 class UsageRecordTypeDef(_RequiredUsageRecordTypeDef, _OptionalUsageRecordTypeDef):
     pass
 
-
 UsageRecordResultTypeDef = TypedDict(
     "UsageRecordResultTypeDef",
     {
         "UsageRecord": UsageRecordOutputTypeDef,
         "MeteringRecordId": str,
         "Status": UsageRecordResultStatusType,
     },
     total=False,
 )
 
-BatchMeterUsageRequestRequestTypeDef = TypedDict(
-    "BatchMeterUsageRequestRequestTypeDef",
+_RequiredMeterUsageRequestRequestTypeDef = TypedDict(
+    "_RequiredMeterUsageRequestRequestTypeDef",
     {
-        "UsageRecords": Sequence[Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]],
         "ProductCode": str,
+        "Timestamp": TimestampTypeDef,
+        "UsageDimension": str,
     },
 )
+_OptionalMeterUsageRequestRequestTypeDef = TypedDict(
+    "_OptionalMeterUsageRequestRequestTypeDef",
+    {
+        "UsageQuantity": int,
+        "DryRun": bool,
+        "UsageAllocations": Sequence[UsageAllocationUnionTypeDef],
+    },
+    total=False,
+)
+
+class MeterUsageRequestRequestTypeDef(
+    _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
+):
+    pass
 
+UsageRecordUnionTypeDef = Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
         "UnprocessedRecords": List[UsageRecordOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+BatchMeterUsageRequestRequestTypeDef = TypedDict(
+    "BatchMeterUsageRequestRequestTypeDef",
+    {
+        "UsageRecords": Sequence[UsageRecordUnionTypeDef],
+        "ProductCode": str,
+    },
+)
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/type_defs.pyi` & `mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,57 +4,62 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_meteringmarketplace.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import UsageRecordResultStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "RegisterUsageRequestRequestTypeDef",
     "ResolveCustomerRequestRequestTypeDef",
     "TagTypeDef",
     "MeterUsageResultTypeDef",
     "RegisterUsageResultTypeDef",
     "ResolveCustomerResultTypeDef",
     "UsageAllocationOutputTypeDef",
     "UsageAllocationTypeDef",
     "UsageRecordOutputTypeDef",
-    "MeterUsageRequestRequestTypeDef",
+    "UsageAllocationUnionTypeDef",
     "UsageRecordTypeDef",
     "UsageRecordResultTypeDef",
-    "BatchMeterUsageRequestRequestTypeDef",
+    "MeterUsageRequestRequestTypeDef",
+    "UsageRecordUnionTypeDef",
     "BatchMeterUsageResultTypeDef",
+    "BatchMeterUsageRequestRequestTypeDef",
 )
 
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
 _RequiredRegisterUsageRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterUsageRequestRequestTypeDef",
     {
         "ProductCode": str,
         "PublicKeyVersion": int,
     },
 )
@@ -62,19 +67,21 @@
     "_OptionalRegisterUsageRequestRequestTypeDef",
     {
         "Nonce": str,
     },
     total=False,
 )
 
+
 class RegisterUsageRequestRequestTypeDef(
     _RequiredRegisterUsageRequestRequestTypeDef, _OptionalRegisterUsageRequestRequestTypeDef
 ):
     pass
 
+
 ResolveCustomerRequestRequestTypeDef = TypedDict(
     "ResolveCustomerRequestRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
@@ -123,36 +130,40 @@
     "_OptionalUsageAllocationOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class UsageAllocationOutputTypeDef(
     _RequiredUsageAllocationOutputTypeDef, _OptionalUsageAllocationOutputTypeDef
 ):
     pass
 
+
 _RequiredUsageAllocationTypeDef = TypedDict(
     "_RequiredUsageAllocationTypeDef",
     {
         "AllocatedUsageQuantity": int,
     },
 )
 _OptionalUsageAllocationTypeDef = TypedDict(
     "_OptionalUsageAllocationTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UsageAllocationTypeDef(_RequiredUsageAllocationTypeDef, _OptionalUsageAllocationTypeDef):
     pass
 
+
 _RequiredUsageRecordOutputTypeDef = TypedDict(
     "_RequiredUsageRecordOutputTypeDef",
     {
         "Timestamp": datetime,
         "CustomerIdentifier": str,
         "Dimension": str,
     },
@@ -162,81 +173,89 @@
     {
         "Quantity": int,
         "UsageAllocations": List[UsageAllocationOutputTypeDef],
     },
     total=False,
 )
 
+
 class UsageRecordOutputTypeDef(
     _RequiredUsageRecordOutputTypeDef, _OptionalUsageRecordOutputTypeDef
 ):
     pass
 
-_RequiredMeterUsageRequestRequestTypeDef = TypedDict(
-    "_RequiredMeterUsageRequestRequestTypeDef",
-    {
-        "ProductCode": str,
-        "Timestamp": Union[datetime, str],
-        "UsageDimension": str,
-    },
-)
-_OptionalMeterUsageRequestRequestTypeDef = TypedDict(
-    "_OptionalMeterUsageRequestRequestTypeDef",
-    {
-        "UsageQuantity": int,
-        "DryRun": bool,
-        "UsageAllocations": Sequence[Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]],
-    },
-    total=False,
-)
-
-class MeterUsageRequestRequestTypeDef(
-    _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
-):
-    pass
 
+UsageAllocationUnionTypeDef = Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]
 _RequiredUsageRecordTypeDef = TypedDict(
     "_RequiredUsageRecordTypeDef",
     {
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
         "CustomerIdentifier": str,
         "Dimension": str,
     },
 )
 _OptionalUsageRecordTypeDef = TypedDict(
     "_OptionalUsageRecordTypeDef",
     {
         "Quantity": int,
         "UsageAllocations": Sequence[UsageAllocationTypeDef],
     },
     total=False,
 )
 
+
 class UsageRecordTypeDef(_RequiredUsageRecordTypeDef, _OptionalUsageRecordTypeDef):
     pass
 
+
 UsageRecordResultTypeDef = TypedDict(
     "UsageRecordResultTypeDef",
     {
         "UsageRecord": UsageRecordOutputTypeDef,
         "MeteringRecordId": str,
         "Status": UsageRecordResultStatusType,
     },
     total=False,
 )
 
-BatchMeterUsageRequestRequestTypeDef = TypedDict(
-    "BatchMeterUsageRequestRequestTypeDef",
+_RequiredMeterUsageRequestRequestTypeDef = TypedDict(
+    "_RequiredMeterUsageRequestRequestTypeDef",
     {
-        "UsageRecords": Sequence[Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]],
         "ProductCode": str,
+        "Timestamp": TimestampTypeDef,
+        "UsageDimension": str,
+    },
+)
+_OptionalMeterUsageRequestRequestTypeDef = TypedDict(
+    "_OptionalMeterUsageRequestRequestTypeDef",
+    {
+        "UsageQuantity": int,
+        "DryRun": bool,
+        "UsageAllocations": Sequence[UsageAllocationUnionTypeDef],
     },
+    total=False,
 )
 
+
+class MeterUsageRequestRequestTypeDef(
+    _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
+):
+    pass
+
+
+UsageRecordUnionTypeDef = Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
         "UnprocessedRecords": List[UsageRecordOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+BatchMeterUsageRequestRequestTypeDef = TypedDict(
+    "BatchMeterUsageRequestRequestTypeDef",
+    {
+        "UsageRecords": Sequence[UsageRecordUnionTypeDef],
+        "ProductCode": str,
+    },
+)
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MarketplaceMetering 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 meteringmarketplace type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 meteringmarketplace type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-meteringmarketplace)](https://pepy.tech/project/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
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
@@ -289,42 +289,45 @@
 )
 
 
 def check_value(value: UsageRecordResultStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_meteringmarketplace.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_meteringmarketplace.type_defs import (
     ResponseMetadataTypeDef,
+    TimestampTypeDef,
     RegisterUsageRequestRequestTypeDef,
     ResolveCustomerRequestRequestTypeDef,
     TagTypeDef,
     MeterUsageResultTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerResultTypeDef,
     UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
     UsageRecordOutputTypeDef,
-    MeterUsageRequestRequestTypeDef,
+    UsageAllocationUnionTypeDef,
     UsageRecordTypeDef,
     UsageRecordResultTypeDef,
-    BatchMeterUsageRequestRequestTypeDef,
+    MeterUsageRequestRequestTypeDef,
+    UsageRecordUnionTypeDef,
     BatchMeterUsageResultTypeDef,
+    BatchMeterUsageRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt` & `mypy-boto3-meteringmarketplace-1.28.16/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.15.post1/setup.py` & `mypy-boto3-meteringmarketplace-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-meteringmarketplace",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_meteringmarketplace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MarketplaceMetering 1.28.16 service generated with"
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
-    keywords="boto3 meteringmarketplace type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 meteringmarketplace type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_meteringmarketplace": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/"
```

