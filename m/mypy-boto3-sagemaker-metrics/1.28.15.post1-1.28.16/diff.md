# Comparing `tmp/mypy-boto3-sagemaker-metrics-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-sagemaker-metrics-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-metrics-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:06 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-metrics-1.28.16.tar", last modified: Tue Aug  1 11:37:47 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1.tar` & `mypy-boto3-sagemaker-metrics-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:06.629383 mypy-boto3-sagemaker-metrics-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-29 10:04:06.629383 mypy-boto3-sagemaker-metrics-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:06.629383 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-29 09:58:36.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-29 09:58:36.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:06.629383 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-29 10:04:06.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-29 10:04:06.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:06.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:06.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:06.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:04:06.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:06.629383 mypy-boto3-sagemaker-metrics-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-metrics-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:47.032746 mypy-boto3-sagemaker-metrics-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-08-01 11:37:47.024747 mypy-boto3-sagemaker-metrics-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:47.024747 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:47.024747 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-08-01 11:37:46.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-01 11:37:46.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:46.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:46.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:46.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:37:46.000000 mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:47.032746 mypy-boto3-sagemaker-metrics-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-metrics-1.28.16/setup.py
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/LICENSE` & `mypy-boto3-sagemaker-metrics-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/PKG-INFO` & `mypy-boto3-sagemaker-metrics-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-metrics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SageMakerMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SageMakerMetrics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-metrics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-metrics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-metrics)](https://pepy.tech/project/mypy-boto3-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerMetrics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[boto3.SageMakerMetrics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
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
 [mypy-boto3-sagemaker-metrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/).
 
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
@@ -289,32 +289,33 @@
 )
 
 
 def check_value(value: PutMetricsErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_metrics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_metrics.type_defs import (
     BatchPutMetricsErrorTypeDef,
-    RawMetricDataTypeDef,
     ResponseMetadataTypeDef,
-    BatchPutMetricsRequestRequestTypeDef,
+    TimestampTypeDef,
     BatchPutMetricsResponseTypeDef,
+    RawMetricDataTypeDef,
+    BatchPutMetricsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BatchPutMetricsErrorTypeDef:
+def get_value() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/README.md` & `mypy-boto3-sagemaker-metrics-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-metrics)](https://pepy.tech/project/mypy-boto3-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerMetrics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[boto3.SageMakerMetrics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
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
 [mypy-boto3-sagemaker-metrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/).
 
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
@@ -257,32 +257,33 @@
 )
 
 
 def check_value(value: PutMetricsErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_metrics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_metrics.type_defs import (
     BatchPutMetricsErrorTypeDef,
-    RawMetricDataTypeDef,
     ResponseMetadataTypeDef,
-    BatchPutMetricsRequestRequestTypeDef,
+    TimestampTypeDef,
     BatchPutMetricsResponseTypeDef,
+    RawMetricDataTypeDef,
+    BatchPutMetricsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BatchPutMetricsErrorTypeDef:
+def get_value() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/__main__.py` & `mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerMetrics 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.SageMakerMetrics 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics\nOther"
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

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/client.py` & `mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/client.pyi` & `mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/literals.py` & `mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/literals.pyi` & `mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/type_defs.py` & `mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_metrics.type_defs import BatchPutMetricsErrorTypeDef
 
-    data: BatchPutMetricsErrorTypeDef = {...}
+    data: BatchPutMetricsErrorTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import PutMetricsErrorCodeType
@@ -21,34 +21,55 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchPutMetricsErrorTypeDef",
-    "RawMetricDataTypeDef",
     "ResponseMetadataTypeDef",
-    "BatchPutMetricsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "BatchPutMetricsResponseTypeDef",
+    "RawMetricDataTypeDef",
+    "BatchPutMetricsRequestRequestTypeDef",
 )
 
 BatchPutMetricsErrorTypeDef = TypedDict(
     "BatchPutMetricsErrorTypeDef",
     {
         "Code": PutMetricsErrorCodeType,
         "MetricIndex": int,
     },
     total=False,
 )
 
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
+TimestampTypeDef = Union[datetime, str]
+BatchPutMetricsResponseTypeDef = TypedDict(
+    "BatchPutMetricsResponseTypeDef",
+    {
+        "Errors": List[BatchPutMetricsErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredRawMetricDataTypeDef = TypedDict(
     "_RequiredRawMetricDataTypeDef",
     {
         "MetricName": str,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
         "Value": float,
     },
 )
 _OptionalRawMetricDataTypeDef = TypedDict(
     "_OptionalRawMetricDataTypeDef",
     {
         "Step": int,
@@ -57,33 +78,14 @@
 )
 
 
 class RawMetricDataTypeDef(_RequiredRawMetricDataTypeDef, _OptionalRawMetricDataTypeDef):
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
-
 BatchPutMetricsRequestRequestTypeDef = TypedDict(
     "BatchPutMetricsRequestRequestTypeDef",
     {
         "TrialComponentName": str,
         "MetricData": Sequence[RawMetricDataTypeDef],
     },
 )
-
-BatchPutMetricsResponseTypeDef = TypedDict(
-    "BatchPutMetricsResponseTypeDef",
-    {
-        "Errors": List[BatchPutMetricsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics/type_defs.pyi` & `mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_metrics.type_defs import BatchPutMetricsErrorTypeDef
 
-    data: BatchPutMetricsErrorTypeDef = {...}
+    data: BatchPutMetricsErrorTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import PutMetricsErrorCodeType
@@ -20,67 +20,69 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchPutMetricsErrorTypeDef",
-    "RawMetricDataTypeDef",
     "ResponseMetadataTypeDef",
-    "BatchPutMetricsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "BatchPutMetricsResponseTypeDef",
+    "RawMetricDataTypeDef",
+    "BatchPutMetricsRequestRequestTypeDef",
 )
 
 BatchPutMetricsErrorTypeDef = TypedDict(
     "BatchPutMetricsErrorTypeDef",
     {
         "Code": PutMetricsErrorCodeType,
         "MetricIndex": int,
     },
     total=False,
 )
 
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
+TimestampTypeDef = Union[datetime, str]
+BatchPutMetricsResponseTypeDef = TypedDict(
+    "BatchPutMetricsResponseTypeDef",
+    {
+        "Errors": List[BatchPutMetricsErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredRawMetricDataTypeDef = TypedDict(
     "_RequiredRawMetricDataTypeDef",
     {
         "MetricName": str,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
         "Value": float,
     },
 )
 _OptionalRawMetricDataTypeDef = TypedDict(
     "_OptionalRawMetricDataTypeDef",
     {
         "Step": int,
     },
     total=False,
 )
 
 class RawMetricDataTypeDef(_RequiredRawMetricDataTypeDef, _OptionalRawMetricDataTypeDef):
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
-
 BatchPutMetricsRequestRequestTypeDef = TypedDict(
     "BatchPutMetricsRequestRequestTypeDef",
     {
         "TrialComponentName": str,
         "MetricData": Sequence[RawMetricDataTypeDef],
     },
 )
-
-BatchPutMetricsResponseTypeDef = TypedDict(
-    "BatchPutMetricsResponseTypeDef",
-    {
-        "Errors": List[BatchPutMetricsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-metrics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SageMakerMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SageMakerMetrics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-metrics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-metrics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-metrics)](https://pepy.tech/project/mypy-boto3-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerMetrics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[boto3.SageMakerMetrics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
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
 [mypy-boto3-sagemaker-metrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/).
 
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
@@ -289,32 +289,33 @@
 )
 
 
 def check_value(value: PutMetricsErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_metrics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_metrics.type_defs import (
     BatchPutMetricsErrorTypeDef,
-    RawMetricDataTypeDef,
     ResponseMetadataTypeDef,
-    BatchPutMetricsRequestRequestTypeDef,
+    TimestampTypeDef,
     BatchPutMetricsResponseTypeDef,
+    RawMetricDataTypeDef,
+    BatchPutMetricsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BatchPutMetricsErrorTypeDef:
+def get_value() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-metrics-1.28.16/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.15.post1/setup.py` & `mypy-boto3-sagemaker-metrics-1.28.16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-metrics",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_sagemaker_metrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerMetrics 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SageMakerMetrics 1.28.16 service generated with"
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
-    keywords="boto3 sagemaker-metrics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 sagemaker-metrics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sagemaker_metrics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

