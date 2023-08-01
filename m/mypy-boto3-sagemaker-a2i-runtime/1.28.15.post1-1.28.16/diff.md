# Comparing `tmp/mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-sagemaker-a2i-runtime-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:05 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-a2i-runtime-1.28.16.tar", last modified: Tue Aug  1 11:37:45 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1.tar` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:05.525380 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-29 10:04:05.525380 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:05.525380 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:05.525380 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:05.525380 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-29 09:58:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.120755 mypy-boto3-sagemaker-a2i-runtime-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-08-01 11:37:45.116755 mypy-boto3-sagemaker-a2i-runtime-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.116755 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.116755 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:45.120755 mypy-boto3-sagemaker-a2i-runtime-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 11:31:58.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.16/setup.py
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/LICENSE` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/PKG-INFO` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-a2i-runtime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AugmentedAIRuntime 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AugmentedAIRuntime 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-a2i-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-a2i-runtime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-a2i-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AugmentedAIRuntime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
+[boto3.AugmentedAIRuntime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [mypy-boto3-sagemaker-a2i-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/).
 
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
@@ -313,42 +313,43 @@
 )
 
 
 def check_value(value: ContentClassifierType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_a2i_runtime.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_a2i_runtime.type_defs import (
     DeleteHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopRequestRequestTypeDef,
     HumanLoopOutputTypeDef,
     ResponseMetadataTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     HumanLoopSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
+    TimestampTypeDef,
     StopHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopResponseTypeDef,
     StartHumanLoopResponseTypeDef,
     StartHumanLoopRequestRequestTypeDef,
     ListHumanLoopsResponseTypeDef,
     ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    ListHumanLoopsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> DeleteHumanLoopRequestRequestTypeDef:
+def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/README.md` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-a2i-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AugmentedAIRuntime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
+[boto3.AugmentedAIRuntime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [mypy-boto3-sagemaker-a2i-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/).
 
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
@@ -281,42 +281,43 @@
 )
 
 
 def check_value(value: ContentClassifierType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_a2i_runtime.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_a2i_runtime.type_defs import (
     DeleteHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopRequestRequestTypeDef,
     HumanLoopOutputTypeDef,
     ResponseMetadataTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     HumanLoopSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
+    TimestampTypeDef,
     StopHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopResponseTypeDef,
     StartHumanLoopResponseTypeDef,
     StartHumanLoopRequestRequestTypeDef,
     ListHumanLoopsResponseTypeDef,
     ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    ListHumanLoopsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> DeleteHumanLoopRequestRequestTypeDef:
+def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/__init__.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/__init__.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/__main__.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AugmentedAIRuntime 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AugmentedAIRuntime 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime\nOther"
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

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/client.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,56 +10,52 @@
     from mypy_boto3_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient
 
     session = Session()
     client: AugmentedAIRuntimeClient = session.client("sagemaker-a2i-runtime")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import SortOrderType
 from .paginator import ListHumanLoopsPaginator
 from .type_defs import (
     DescribeHumanLoopResponseTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     ListHumanLoopsResponseTypeDef,
     StartHumanLoopResponseTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AugmentedAIRuntimeClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class AugmentedAIRuntimeClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/)
     """
 
     meta: ClientMeta
@@ -68,99 +64,90 @@
     def exceptions(self) -> Exceptions:
         """
         AugmentedAIRuntimeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#close)
         """
-
     def delete_human_loop(self, *, HumanLoopName: str) -> Dict[str, Any]:
         """
         Deletes the specified human loop for a flow definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.delete_human_loop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#delete_human_loop)
         """
-
     def describe_human_loop(self, *, HumanLoopName: str) -> DescribeHumanLoopResponseTypeDef:
         """
         Returns information about the specified human loop.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.describe_human_loop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#describe_human_loop)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#generate_presigned_url)
         """
-
     def list_human_loops(
         self,
         *,
         FlowDefinitionArn: str,
-        CreationTimeAfter: Union[datetime, str] = ...,
-        CreationTimeBefore: Union[datetime, str] = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListHumanLoopsResponseTypeDef:
         """
         Returns information about human loops, given the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#list_human_loops)
         """
-
     def start_human_loop(
         self,
         *,
         HumanLoopName: str,
         FlowDefinitionArn: str,
         HumanLoopInput: HumanLoopInputTypeDef,
         DataAttributes: HumanLoopDataAttributesTypeDef = ...
     ) -> StartHumanLoopResponseTypeDef:
         """
         Starts a human loop, provided that at least one activation condition is met.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#start_human_loop)
         """
-
     def stop_human_loop(self, *, HumanLoopName: str) -> Dict[str, Any]:
         """
         Stops the specified human loop.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.stop_human_loop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#stop_human_loop)
         """
-
     def get_paginator(self, operation_name: Literal["list_human_loops"]) -> ListHumanLoopsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/client.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,52 +10,56 @@
     from mypy_boto3_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient
 
     session = Session()
     client: AugmentedAIRuntimeClient = session.client("sagemaker-a2i-runtime")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import SortOrderType
 from .paginator import ListHumanLoopsPaginator
 from .type_defs import (
     DescribeHumanLoopResponseTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     ListHumanLoopsResponseTypeDef,
     StartHumanLoopResponseTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("AugmentedAIRuntimeClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class AugmentedAIRuntimeClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/)
     """
 
     meta: ClientMeta
@@ -64,90 +68,99 @@
     def exceptions(self) -> Exceptions:
         """
         AugmentedAIRuntimeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#close)
         """
+
     def delete_human_loop(self, *, HumanLoopName: str) -> Dict[str, Any]:
         """
         Deletes the specified human loop for a flow definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.delete_human_loop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#delete_human_loop)
         """
+
     def describe_human_loop(self, *, HumanLoopName: str) -> DescribeHumanLoopResponseTypeDef:
         """
         Returns information about the specified human loop.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.describe_human_loop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#describe_human_loop)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#generate_presigned_url)
         """
+
     def list_human_loops(
         self,
         *,
         FlowDefinitionArn: str,
-        CreationTimeAfter: Union[datetime, str] = ...,
-        CreationTimeBefore: Union[datetime, str] = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListHumanLoopsResponseTypeDef:
         """
         Returns information about human loops, given the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#list_human_loops)
         """
+
     def start_human_loop(
         self,
         *,
         HumanLoopName: str,
         FlowDefinitionArn: str,
         HumanLoopInput: HumanLoopInputTypeDef,
         DataAttributes: HumanLoopDataAttributesTypeDef = ...
     ) -> StartHumanLoopResponseTypeDef:
         """
         Starts a human loop, provided that at least one activation condition is met.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#start_human_loop)
         """
+
     def stop_human_loop(self, *, HumanLoopName: str) -> Dict[str, Any]:
         """
         Stops the specified human loop.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.stop_human_loop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#stop_human_loop)
         """
+
     def get_paginator(self, operation_name: Literal["list_human_loops"]) -> ListHumanLoopsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/literals.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/literals.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/paginator.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/paginator.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 
     session = Session()
     client: AugmentedAIRuntimeClient = session.client("sagemaker-a2i-runtime")
 
     list_human_loops_paginator: ListHumanLoopsPaginator = client.get_paginator("list_human_loops")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SortOrderType
-from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListHumanLoopsPaginator",)
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
@@ -46,16 +45,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
     """
 
     def paginate(
         self,
         *,
         FlowDefinitionArn: str,
-        CreationTimeAfter: Union[datetime, str] = ...,
-        CreationTimeBefore: Union[datetime, str] = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHumanLoopsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
         """
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/paginator.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/paginator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 
     session = Session()
     client: AugmentedAIRuntimeClient = session.client("sagemaker-a2i-runtime")
 
     list_human_loops_paginator: ListHumanLoopsPaginator = client.get_paginator("list_human_loops")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SortOrderType
-from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListHumanLoopsPaginator",)
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
@@ -43,16 +42,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
     """
 
     def paginate(
         self,
         *,
         FlowDefinitionArn: str,
-        CreationTimeAfter: Union[datetime, str] = ...,
-        CreationTimeBefore: Union[datetime, str] = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHumanLoopsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
         """
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/type_defs.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_a2i_runtime.type_defs import DeleteHumanLoopRequestRequestTypeDef
 
-    data: DeleteHumanLoopRequestRequestTypeDef = {...}
+    data: DeleteHumanLoopRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ContentClassifierType, HumanLoopStatusType, SortOrderType
@@ -28,21 +28,22 @@
     "DescribeHumanLoopRequestRequestTypeDef",
     "HumanLoopOutputTypeDef",
     "ResponseMetadataTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "HumanLoopInputTypeDef",
     "HumanLoopSummaryTypeDef",
     "PaginatorConfigTypeDef",
-    "ListHumanLoopsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "StopHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopResponseTypeDef",
     "StartHumanLoopResponseTypeDef",
     "StartHumanLoopRequestRequestTypeDef",
     "ListHumanLoopsResponseTypeDef",
     "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    "ListHumanLoopsRequestRequestTypeDef",
 )
 
 DeleteHumanLoopRequestRequestTypeDef = TypedDict(
     "DeleteHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
@@ -105,39 +106,15 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
-    "_RequiredListHumanLoopsRequestRequestTypeDef",
-    {
-        "FlowDefinitionArn": str,
-    },
-)
-_OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
-    "_OptionalListHumanLoopsRequestRequestTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-        "SortOrder": SortOrderType,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListHumanLoopsRequestRequestTypeDef(
-    _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 StopHumanLoopRequestRequestTypeDef = TypedDict(
     "StopHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
 )
 
@@ -201,21 +178,46 @@
     {
         "FlowDefinitionArn": str,
     },
 )
 _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
     "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
     {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
         "SortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
     _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
     _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
 ):
     pass
+
+
+_RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
+    "_RequiredListHumanLoopsRequestRequestTypeDef",
+    {
+        "FlowDefinitionArn": str,
+    },
+)
+_OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
+    "_OptionalListHumanLoopsRequestRequestTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": SortOrderType,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListHumanLoopsRequestRequestTypeDef(
+    _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime/type_defs.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_a2i_runtime.type_defs import DeleteHumanLoopRequestRequestTypeDef
 
-    data: DeleteHumanLoopRequestRequestTypeDef = {...}
+    data: DeleteHumanLoopRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ContentClassifierType, HumanLoopStatusType, SortOrderType
@@ -27,21 +27,22 @@
     "DescribeHumanLoopRequestRequestTypeDef",
     "HumanLoopOutputTypeDef",
     "ResponseMetadataTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "HumanLoopInputTypeDef",
     "HumanLoopSummaryTypeDef",
     "PaginatorConfigTypeDef",
-    "ListHumanLoopsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "StopHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopResponseTypeDef",
     "StartHumanLoopResponseTypeDef",
     "StartHumanLoopRequestRequestTypeDef",
     "ListHumanLoopsResponseTypeDef",
     "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    "ListHumanLoopsRequestRequestTypeDef",
 )
 
 DeleteHumanLoopRequestRequestTypeDef = TypedDict(
     "DeleteHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
@@ -104,37 +105,15 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
-    "_RequiredListHumanLoopsRequestRequestTypeDef",
-    {
-        "FlowDefinitionArn": str,
-    },
-)
-_OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
-    "_OptionalListHumanLoopsRequestRequestTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-        "SortOrder": SortOrderType,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListHumanLoopsRequestRequestTypeDef(
-    _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 StopHumanLoopRequestRequestTypeDef = TypedDict(
     "StopHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
 )
 
@@ -196,20 +175,43 @@
     {
         "FlowDefinitionArn": str,
     },
 )
 _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
     "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
     {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
         "SortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
     _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
     _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
 ):
     pass
+
+_RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
+    "_RequiredListHumanLoopsRequestRequestTypeDef",
+    {
+        "FlowDefinitionArn": str,
+    },
+)
+_OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
+    "_OptionalListHumanLoopsRequestRequestTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": SortOrderType,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListHumanLoopsRequestRequestTypeDef(
+    _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-a2i-runtime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AugmentedAIRuntime 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AugmentedAIRuntime 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-a2i-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-a2i-runtime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-a2i-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AugmentedAIRuntime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
+[boto3.AugmentedAIRuntime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [mypy-boto3-sagemaker-a2i-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/).
 
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
@@ -313,42 +313,43 @@
 )
 
 
 def check_value(value: ContentClassifierType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_a2i_runtime.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_a2i_runtime.type_defs import (
     DeleteHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopRequestRequestTypeDef,
     HumanLoopOutputTypeDef,
     ResponseMetadataTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     HumanLoopSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
+    TimestampTypeDef,
     StopHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopResponseTypeDef,
     StartHumanLoopResponseTypeDef,
     StartHumanLoopRequestRequestTypeDef,
     ListHumanLoopsResponseTypeDef,
     ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    ListHumanLoopsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> DeleteHumanLoopRequestRequestTypeDef:
+def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/mypy_boto3_sagemaker_a2i_runtime.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/mypy_boto3_sagemaker_a2i_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.15.post1/setup.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-a2i-runtime",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_sagemaker_a2i_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AugmentedAIRuntime 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.AugmentedAIRuntime 1.28.16 service generated with"
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
-    keywords="boto3 sagemaker-a2i-runtime type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 sagemaker-a2i-runtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sagemaker_a2i_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/"
```

