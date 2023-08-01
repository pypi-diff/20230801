# Comparing `tmp/mypy-boto3-rbin-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-rbin-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rbin-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:57 2023, max compression
+gzip compressed data, was "mypy-boto3-rbin-1.28.16.tar", last modified: Tue Aug  1 11:37:37 2023, max compression
```

## Comparing `mypy-boto3-rbin-1.28.15.post1.tar` & `mypy-boto3-rbin-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:57.869354 mypy-boto3-rbin-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-07-29 10:03:57.869354 mypy-boto3-rbin-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:57.869354 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:56:15.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:57.869354 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-07-29 10:03:57.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-29 10:03:57.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:57.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:57.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:57.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:03:57.000000 mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:57.869354 mypy-boto3-rbin-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-29 09:56:14.000000 mypy-boto3-rbin-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:37.584778 mypy-boto3-rbin-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:29:34.000000 mypy-boto3-rbin-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-08-01 11:37:37.580778 mypy-boto3-rbin-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-08-01 11:29:34.000000 mypy-boto3-rbin-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:37.576778 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 11:29:34.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-01 11:29:34.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:29:34.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-08-01 11:29:35.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-08-01 11:29:35.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-08-01 11:29:35.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-08-01 11:29:35.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-01 11:29:35.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-01 11:29:35.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:29:34.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-08-01 11:29:35.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-08-01 11:29:35.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:29:34.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:37.580778 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-08-01 11:37:37.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-01 11:37:37.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:37.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:37.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:37.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 11:37:37.000000 mypy-boto3-rbin-1.28.16/mypy_boto3_rbin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:37.584778 mypy-boto3-rbin-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-01 11:29:34.000000 mypy-boto3-rbin-1.28.16/setup.py
```

### Comparing `mypy-boto3-rbin-1.28.15.post1/LICENSE` & `mypy-boto3-rbin-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/PKG-INFO` & `mypy-boto3-rbin-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rbin
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.RecycleBin 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.RecycleBin 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rbin type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 rbin type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rbin)](https://pepy.tech/project/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: ListRulesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rbin.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
@@ -352,15 +352,15 @@
     GetRuleResponseTypeDef,
     LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
     UnlockRuleResponseTypeDef,
 )
 
 
-def get_structure() -> ResourceTagTypeDef:
+def get_value() -> ResourceTagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rbin-1.28.15.post1/README.md` & `mypy-boto3-rbin-1.28.16/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rbin)](https://pepy.tech/project/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
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
@@ -282,20 +282,20 @@
 )
 
 
 def check_value(value: ListRulesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rbin.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
@@ -320,15 +320,15 @@
     GetRuleResponseTypeDef,
     LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
     UnlockRuleResponseTypeDef,
 )
 
 
-def get_structure() -> ResourceTagTypeDef:
+def get_value() -> ResourceTagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/__init__.py` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/__init__.pyi` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/__main__.py` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RecycleBin 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.RecycleBin 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin\nOther"
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

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/client.py` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/client.pyi` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/literals.py` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/literals.pyi` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/paginator.py` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/paginator.pyi` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/type_defs.py` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_rbin.type_defs import ResourceTagTypeDef
 
-    data: ResourceTagTypeDef = {...}
+    data: ResourceTagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import LockStateType, ResourceTypeType, RuleStatusType
```

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin/type_defs.pyi` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_rbin.type_defs import ResourceTagTypeDef
 
-    data: ResourceTagTypeDef = {...}
+    data: ResourceTagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import LockStateType, ResourceTypeType, RuleStatusType
```

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin.egg-info/PKG-INFO` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rbin
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.RecycleBin 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.RecycleBin 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rbin type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 rbin type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rbin)](https://pepy.tech/project/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: ListRulesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_rbin.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
@@ -352,15 +352,15 @@
     GetRuleResponseTypeDef,
     LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
     UnlockRuleResponseTypeDef,
 )
 
 
-def get_structure() -> ResourceTagTypeDef:
+def get_value() -> ResourceTagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rbin-1.28.15.post1/mypy_boto3_rbin.egg-info/SOURCES.txt` & `mypy-boto3-rbin-1.28.16/mypy_boto3_rbin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.15.post1/setup.py` & `mypy-boto3-rbin-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rbin",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_rbin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RecycleBin 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.RecycleBin 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 rbin type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 rbin type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_rbin": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

