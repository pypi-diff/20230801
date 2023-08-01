# Comparing `tmp/mypy-boto3-servicecatalog-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-servicecatalog-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicecatalog-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:11 2023, max compression
+gzip compressed data, was "mypy-boto3-servicecatalog-1.28.16.tar", last modified: Tue Aug  1 11:37:51 2023, max compression
```

## Comparing `mypy-boto3-servicecatalog-1.28.15.post1.tar` & `mypy-boto3-servicecatalog-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:11.905403 mypy-boto3-servicecatalog-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:18.000000 mypy-boto3-servicecatalog-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-07-29 10:04:11.901403 mypy-boto3-servicecatalog-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26139 2023-07-29 09:59:18.000000 mypy-boto3-servicecatalog-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:11.901403 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-29 09:59:18.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-29 09:59:18.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:59:18.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-07-29 09:59:19.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    76049 2023-07-29 09:59:18.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-07-29 09:59:24.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-07-29 09:59:23.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-07-29 09:59:23.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21828 2023-07-29 09:59:19.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:18.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   102689 2023-07-29 09:59:26.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102544 2023-07-29 09:59:25.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:18.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:11.901403 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:11.905403 mypy-boto3-servicecatalog-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:59:18.000000 mypy-boto3-servicecatalog-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.448729 mypy-boto3-servicecatalog-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:32:49.000000 mypy-boto3-servicecatalog-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27650 2023-08-01 11:37:51.448729 mypy-boto3-servicecatalog-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-08-01 11:32:49.000000 mypy-boto3-servicecatalog-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.440729 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-08-01 11:32:49.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-08-01 11:32:49.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:32:49.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-08-01 11:32:55.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76049 2023-08-01 11:32:54.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-08-01 11:32:55.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-08-01 11:32:55.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-08-01 11:32:55.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21828 2023-08-01 11:32:55.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:32:49.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   102687 2023-08-01 11:32:58.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102542 2023-08-01 11:32:56.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:32:49.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.448729 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27650 2023-08-01 11:37:51.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:37:51.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:51.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:37:51.000000 mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:51.448729 mypy-boto3-servicecatalog-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:32:49.000000 mypy-boto3-servicecatalog-1.28.16/setup.py
```

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/LICENSE` & `mypy-boto3-servicecatalog-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/PKG-INFO` & `mypy-boto3-servicecatalog-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ServiceCatalog 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ServiceCatalog 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 servicecatalog type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 servicecatalog type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog)](https://pepy.tech/project/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
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
@@ -421,20 +421,20 @@
 )
 
 
 def check_value(value: AccessLevelFilterKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_servicecatalog.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_servicecatalog.type_defs import (
     AcceptPortfolioShareInputRequestTypeDef,
     AccessLevelFilterTypeDef,
     AssociateBudgetWithResourceInputRequestTypeDef,
     AssociatePrincipalWithPortfolioInputRequestTypeDef,
@@ -664,15 +664,15 @@
     CreateProductOutputTypeDef,
     DescribeProductAsAdminOutputTypeDef,
     SearchProductsAsAdminOutputTypeDef,
     UpdateProductOutputTypeDef,
 )
 
 
-def get_structure() -> AcceptPortfolioShareInputRequestTypeDef:
+def get_value() -> AcceptPortfolioShareInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/README.md` & `mypy-boto3-servicecatalog-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog)](https://pepy.tech/project/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
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
@@ -389,20 +389,20 @@
 )
 
 
 def check_value(value: AccessLevelFilterKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_servicecatalog.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_servicecatalog.type_defs import (
     AcceptPortfolioShareInputRequestTypeDef,
     AccessLevelFilterTypeDef,
     AssociateBudgetWithResourceInputRequestTypeDef,
     AssociatePrincipalWithPortfolioInputRequestTypeDef,
@@ -632,15 +632,15 @@
     CreateProductOutputTypeDef,
     DescribeProductAsAdminOutputTypeDef,
     SearchProductsAsAdminOutputTypeDef,
     UpdateProductOutputTypeDef,
 )
 
 
-def get_structure() -> AcceptPortfolioShareInputRequestTypeDef:
+def get_value() -> AcceptPortfolioShareInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/__init__.py` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/__init__.pyi` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/__main__.py` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceCatalog 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ServiceCatalog 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog\nOther"
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

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/client.py` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/client.pyi` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/literals.py` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/literals.pyi` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/paginator.py` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/paginator.pyi` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/type_defs.py` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_servicecatalog.type_defs import AcceptPortfolioShareInputRequestTypeDef
 
-    data: AcceptPortfolioShareInputRequestTypeDef = {...}
+    data: AcceptPortfolioShareInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog/type_defs.pyi` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_servicecatalog.type_defs import AcceptPortfolioShareInputRequestTypeDef
 
-    data: AcceptPortfolioShareInputRequestTypeDef = {...}
+    data: AcceptPortfolioShareInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog.egg-info/PKG-INFO` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ServiceCatalog 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ServiceCatalog 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 servicecatalog type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 servicecatalog type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog)](https://pepy.tech/project/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
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
@@ -421,20 +421,20 @@
 )
 
 
 def check_value(value: AccessLevelFilterKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_servicecatalog.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_servicecatalog.type_defs import (
     AcceptPortfolioShareInputRequestTypeDef,
     AccessLevelFilterTypeDef,
     AssociateBudgetWithResourceInputRequestTypeDef,
     AssociatePrincipalWithPortfolioInputRequestTypeDef,
@@ -664,15 +664,15 @@
     CreateProductOutputTypeDef,
     DescribeProductAsAdminOutputTypeDef,
     SearchProductsAsAdminOutputTypeDef,
     UpdateProductOutputTypeDef,
 )
 
 
-def get_structure() -> AcceptPortfolioShareInputRequestTypeDef:
+def get_value() -> AcceptPortfolioShareInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/mypy_boto3_servicecatalog.egg-info/SOURCES.txt` & `mypy-boto3-servicecatalog-1.28.16/mypy_boto3_servicecatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.15.post1/setup.py` & `mypy-boto3-servicecatalog-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicecatalog",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_servicecatalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceCatalog 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ServiceCatalog 1.28.16 service generated with"
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
-    keywords="boto3 servicecatalog type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 servicecatalog type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_servicecatalog": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

