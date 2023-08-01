# Comparing `tmp/mypy-boto3-mediastore-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-mediastore-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediastore-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:40 2023, max compression
+gzip compressed data, was "mypy-boto3-mediastore-1.28.16.tar", last modified: Tue Aug  1 11:37:20 2023, max compression
```

## Comparing `mypy-boto3-mediastore-1.28.15.post1.tar` & `mypy-boto3-mediastore-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:51:17.000000 mypy-boto3-mediastore-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.644821 mypy-boto3-mediastore-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-08-01 11:37:20.644821 mypy-boto3-mediastore-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.644821 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.644821 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:20.644821 mypy-boto3-mediastore-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:24:16.000000 mypy-boto3-mediastore-1.28.16/setup.py
```

### Comparing `mypy-boto3-mediastore-1.28.15.post1/LICENSE` & `mypy-boto3-mediastore-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15.post1/PKG-INFO` & `mypy-boto3-mediastore-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaStore 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediastore type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediastore type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore)](https://pepy.tech/project/mypy-boto3-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStore 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[boto3.MediaStore 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
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
@@ -312,20 +312,20 @@
 )
 
 
 def check_value(value: ContainerLevelMetricsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediastore.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediastore.type_defs import (
     ContainerTypeDef,
     CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     TagTypeDef,
@@ -345,33 +345,35 @@
     ListTagsForResourceInputRequestTypeDef,
     MetricPolicyRuleTypeDef,
     PutContainerPolicyInputRequestTypeDef,
     PutLifecyclePolicyInputRequestTypeDef,
     StartAccessLoggingInputRequestTypeDef,
     StopAccessLoggingInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    PutCorsPolicyInputRequestTypeDef,
+    CorsRuleUnionTypeDef,
     CreateContainerInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     GetContainerPolicyOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListContainersInputListContainersPaginateTypeDef,
     MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
+    PutCorsPolicyInputRequestTypeDef,
     GetMetricPolicyOutputTypeDef,
+    MetricPolicyUnionTypeDef,
     PutMetricPolicyInputRequestTypeDef,
 )
 
 
-def get_structure() -> ContainerTypeDef:
+def get_value() -> ContainerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediastore-1.28.15.post1/README.md` & `mypy-boto3-mediastore-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore)](https://pepy.tech/project/mypy-boto3-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStore 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[boto3.MediaStore 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
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
@@ -280,20 +280,20 @@
 )
 
 
 def check_value(value: ContainerLevelMetricsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediastore.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediastore.type_defs import (
     ContainerTypeDef,
     CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     TagTypeDef,
@@ -313,33 +313,35 @@
     ListTagsForResourceInputRequestTypeDef,
     MetricPolicyRuleTypeDef,
     PutContainerPolicyInputRequestTypeDef,
     PutLifecyclePolicyInputRequestTypeDef,
     StartAccessLoggingInputRequestTypeDef,
     StopAccessLoggingInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    PutCorsPolicyInputRequestTypeDef,
+    CorsRuleUnionTypeDef,
     CreateContainerInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     GetContainerPolicyOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListContainersInputListContainersPaginateTypeDef,
     MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
+    PutCorsPolicyInputRequestTypeDef,
     GetMetricPolicyOutputTypeDef,
+    MetricPolicyUnionTypeDef,
     PutMetricPolicyInputRequestTypeDef,
 )
 
 
-def get_structure() -> ContainerTypeDef:
+def get_value() -> ContainerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__init__.py` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__init__.pyi` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__main__.py` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaStore 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MediaStore 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore\nOther"
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

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/client.py` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,30 @@
     from mypy_boto3_mediastore.client import MediaStoreClient
 
     session = Session()
     client: MediaStoreClient = session.client("mediastore")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListContainersPaginator
 from .type_defs import (
-    CorsRuleOutputTypeDef,
-    CorsRuleTypeDef,
+    CorsRuleUnionTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     GetContainerPolicyOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyOutputTypeDef,
     ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    MetricPolicyOutputTypeDef,
-    MetricPolicyTypeDef,
+    MetricPolicyUnionTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -225,18 +223,15 @@
         clients that can access it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_container_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_container_policy)
         """
 
     def put_cors_policy(
-        self,
-        *,
-        ContainerName: str,
-        CorsPolicy: Sequence[Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]]
+        self, *, ContainerName: str, CorsPolicy: Sequence[CorsRuleUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Sets the cross-origin resource sharing (CORS) configuration on a container so
         that the container can service cross-origin requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_cors_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_cors_policy)
@@ -247,18 +242,15 @@
         Writes an object lifecycle policy to a container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_lifecycle_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_lifecycle_policy)
         """
 
     def put_metric_policy(
-        self,
-        *,
-        ContainerName: str,
-        MetricPolicy: Union[MetricPolicyTypeDef, MetricPolicyOutputTypeDef]
+        self, *, ContainerName: str, MetricPolicy: MetricPolicyUnionTypeDef
     ) -> Dict[str, Any]:
         """
         The metric policy that you want to add to the container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_metric_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_metric_policy)
         """
```

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/client.pyi` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,30 @@
     from mypy_boto3_mediastore.client import MediaStoreClient
 
     session = Session()
     client: MediaStoreClient = session.client("mediastore")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListContainersPaginator
 from .type_defs import (
-    CorsRuleOutputTypeDef,
-    CorsRuleTypeDef,
+    CorsRuleUnionTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     GetContainerPolicyOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyOutputTypeDef,
     ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    MetricPolicyOutputTypeDef,
-    MetricPolicyTypeDef,
+    MetricPolicyUnionTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -203,18 +201,15 @@
         Creates an access policy for the specified container to restrict the users and
         clients that can access it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_container_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_container_policy)
         """
     def put_cors_policy(
-        self,
-        *,
-        ContainerName: str,
-        CorsPolicy: Sequence[Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]]
+        self, *, ContainerName: str, CorsPolicy: Sequence[CorsRuleUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Sets the cross-origin resource sharing (CORS) configuration on a container so
         that the container can service cross-origin requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_cors_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_cors_policy)
@@ -223,18 +218,15 @@
         """
         Writes an object lifecycle policy to a container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_lifecycle_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_lifecycle_policy)
         """
     def put_metric_policy(
-        self,
-        *,
-        ContainerName: str,
-        MetricPolicy: Union[MetricPolicyTypeDef, MetricPolicyOutputTypeDef]
+        self, *, ContainerName: str, MetricPolicy: MetricPolicyUnionTypeDef
     ) -> Dict[str, Any]:
         """
         The metric policy that you want to add to the container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_metric_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_metric_policy)
         """
```

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/literals.py` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/literals.pyi` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/paginator.py` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/paginator.pyi` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/type_defs.py` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mediastore.type_defs import ContainerTypeDef
 
-    data: ContainerTypeDef = {...}
+    data: ContainerTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ContainerLevelMetricsType, ContainerStatusType, MethodNameType
@@ -44,28 +44,30 @@
     "ListTagsForResourceInputRequestTypeDef",
     "MetricPolicyRuleTypeDef",
     "PutContainerPolicyInputRequestTypeDef",
     "PutLifecyclePolicyInputRequestTypeDef",
     "StartAccessLoggingInputRequestTypeDef",
     "StopAccessLoggingInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "PutCorsPolicyInputRequestTypeDef",
+    "CorsRuleUnionTypeDef",
     "CreateContainerInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateContainerOutputTypeDef",
     "DescribeContainerOutputTypeDef",
     "GetContainerPolicyOutputTypeDef",
     "GetCorsPolicyOutputTypeDef",
     "GetLifecyclePolicyOutputTypeDef",
     "ListContainersOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListContainersInputListContainersPaginateTypeDef",
     "MetricPolicyOutputTypeDef",
     "MetricPolicyTypeDef",
+    "PutCorsPolicyInputRequestTypeDef",
     "GetMetricPolicyOutputTypeDef",
+    "MetricPolicyUnionTypeDef",
     "PutMetricPolicyInputRequestTypeDef",
 )
 
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
     {
         "Endpoint": str,
@@ -291,22 +293,15 @@
     "UntagResourceInputRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": Sequence[str],
     },
 )
 
-PutCorsPolicyInputRequestTypeDef = TypedDict(
-    "PutCorsPolicyInputRequestTypeDef",
-    {
-        "ContainerName": str,
-        "CorsPolicy": Sequence[Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]],
-    },
-)
-
+CorsRuleUnionTypeDef = Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]
 _RequiredCreateContainerInputRequestTypeDef = TypedDict(
     "_RequiredCreateContainerInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 _OptionalCreateContainerInputRequestTypeDef = TypedDict(
@@ -433,22 +428,31 @@
 )
 
 
 class MetricPolicyTypeDef(_RequiredMetricPolicyTypeDef, _OptionalMetricPolicyTypeDef):
     pass
 
 
+PutCorsPolicyInputRequestTypeDef = TypedDict(
+    "PutCorsPolicyInputRequestTypeDef",
+    {
+        "ContainerName": str,
+        "CorsPolicy": Sequence[CorsRuleUnionTypeDef],
+    },
+)
+
 GetMetricPolicyOutputTypeDef = TypedDict(
     "GetMetricPolicyOutputTypeDef",
     {
         "MetricPolicy": MetricPolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MetricPolicyUnionTypeDef = Union[MetricPolicyTypeDef, MetricPolicyOutputTypeDef]
 PutMetricPolicyInputRequestTypeDef = TypedDict(
     "PutMetricPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "MetricPolicy": MetricPolicyTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/type_defs.pyi` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mediastore.type_defs import ContainerTypeDef
 
-    data: ContainerTypeDef = {...}
+    data: ContainerTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ContainerLevelMetricsType, ContainerStatusType, MethodNameType
@@ -43,28 +43,30 @@
     "ListTagsForResourceInputRequestTypeDef",
     "MetricPolicyRuleTypeDef",
     "PutContainerPolicyInputRequestTypeDef",
     "PutLifecyclePolicyInputRequestTypeDef",
     "StartAccessLoggingInputRequestTypeDef",
     "StopAccessLoggingInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "PutCorsPolicyInputRequestTypeDef",
+    "CorsRuleUnionTypeDef",
     "CreateContainerInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateContainerOutputTypeDef",
     "DescribeContainerOutputTypeDef",
     "GetContainerPolicyOutputTypeDef",
     "GetCorsPolicyOutputTypeDef",
     "GetLifecyclePolicyOutputTypeDef",
     "ListContainersOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListContainersInputListContainersPaginateTypeDef",
     "MetricPolicyOutputTypeDef",
     "MetricPolicyTypeDef",
+    "PutCorsPolicyInputRequestTypeDef",
     "GetMetricPolicyOutputTypeDef",
+    "MetricPolicyUnionTypeDef",
     "PutMetricPolicyInputRequestTypeDef",
 )
 
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
     {
         "Endpoint": str,
@@ -284,22 +286,15 @@
     "UntagResourceInputRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": Sequence[str],
     },
 )
 
-PutCorsPolicyInputRequestTypeDef = TypedDict(
-    "PutCorsPolicyInputRequestTypeDef",
-    {
-        "ContainerName": str,
-        "CorsPolicy": Sequence[Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]],
-    },
-)
-
+CorsRuleUnionTypeDef = Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]
 _RequiredCreateContainerInputRequestTypeDef = TypedDict(
     "_RequiredCreateContainerInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 _OptionalCreateContainerInputRequestTypeDef = TypedDict(
@@ -420,22 +415,31 @@
     },
     total=False,
 )
 
 class MetricPolicyTypeDef(_RequiredMetricPolicyTypeDef, _OptionalMetricPolicyTypeDef):
     pass
 
+PutCorsPolicyInputRequestTypeDef = TypedDict(
+    "PutCorsPolicyInputRequestTypeDef",
+    {
+        "ContainerName": str,
+        "CorsPolicy": Sequence[CorsRuleUnionTypeDef],
+    },
+)
+
 GetMetricPolicyOutputTypeDef = TypedDict(
     "GetMetricPolicyOutputTypeDef",
     {
         "MetricPolicy": MetricPolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MetricPolicyUnionTypeDef = Union[MetricPolicyTypeDef, MetricPolicyOutputTypeDef]
 PutMetricPolicyInputRequestTypeDef = TypedDict(
     "PutMetricPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "MetricPolicy": MetricPolicyTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/PKG-INFO` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaStore 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediastore type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediastore type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore)](https://pepy.tech/project/mypy-boto3-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStore 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[boto3.MediaStore 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
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
@@ -312,20 +312,20 @@
 )
 
 
 def check_value(value: ContainerLevelMetricsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediastore.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediastore.type_defs import (
     ContainerTypeDef,
     CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     TagTypeDef,
@@ -345,33 +345,35 @@
     ListTagsForResourceInputRequestTypeDef,
     MetricPolicyRuleTypeDef,
     PutContainerPolicyInputRequestTypeDef,
     PutLifecyclePolicyInputRequestTypeDef,
     StartAccessLoggingInputRequestTypeDef,
     StopAccessLoggingInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    PutCorsPolicyInputRequestTypeDef,
+    CorsRuleUnionTypeDef,
     CreateContainerInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     GetContainerPolicyOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListContainersInputListContainersPaginateTypeDef,
     MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
+    PutCorsPolicyInputRequestTypeDef,
     GetMetricPolicyOutputTypeDef,
+    MetricPolicyUnionTypeDef,
     PutMetricPolicyInputRequestTypeDef,
 )
 
 
-def get_structure() -> ContainerTypeDef:
+def get_value() -> ContainerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/SOURCES.txt` & `mypy-boto3-mediastore-1.28.16/mypy_boto3_mediastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15.post1/setup.py` & `mypy-boto3-mediastore-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediastore",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_mediastore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.MediaStore 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 mediastore type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 mediastore type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mediastore": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

