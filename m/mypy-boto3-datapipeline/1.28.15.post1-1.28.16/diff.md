# Comparing `tmp/mypy-boto3-datapipeline-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-datapipeline-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datapipeline-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:55 2023, max compression
+gzip compressed data, was "mypy-boto3-datapipeline-1.28.16.tar", last modified: Tue Aug  1 11:36:35 2023, max compression
```

## Comparing `mypy-boto3-datapipeline-1.28.15.post1.tar` & `mypy-boto3-datapipeline-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-07-29 09:42:03.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-29 09:42:04.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-29 09:42:04.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-29 09:42:03.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-29 09:42:03.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-07-29 09:42:04.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18428 2023-07-29 09:42:04.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.540913 mypy-boto3-datapipeline-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:35.000000 mypy-boto3-datapipeline-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-08-01 11:36:35.536913 mypy-boto3-datapipeline-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-08-01 11:14:35.000000 mypy-boto3-datapipeline-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.528913 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-01 11:14:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-01 11:14:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:14:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-08-01 11:14:36.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-08-01 11:14:36.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-08-01 11:14:36.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-08-01 11:14:36.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-08-01 11:14:36.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-01 11:14:36.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18638 2023-08-01 11:14:36.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18606 2023-08-01 11:14:36.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.536913 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-08-01 11:36:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:36:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:35.000000 mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:35.540913 mypy-boto3-datapipeline-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:14:35.000000 mypy-boto3-datapipeline-1.28.16/setup.py
```

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/LICENSE` & `mypy-boto3-datapipeline-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/PKG-INFO` & `mypy-boto3-datapipeline-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DataPipeline 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 datapipeline type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 datapipeline type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datapipeline)](https://pepy.tech/project/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
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
@@ -320,24 +320,25 @@
 )
 
 
 def check_value(value: DescribeObjectsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_datapipeline.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_datapipeline.type_defs import (
     ParameterValueTypeDef,
+    TimestampTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeactivatePipelineInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
@@ -376,25 +377,27 @@
     ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
     DescribePipelinesOutputTypeDef,
     DescribeObjectsOutputTypeDef,
     TaskObjectTypeDef,
+    PipelineObjectUnionTypeDef,
     QueryTypeDef,
     GetPipelineDefinitionOutputTypeDef,
-    PutPipelineDefinitionInputRequestTypeDef,
-    ValidatePipelineDefinitionInputRequestTypeDef,
+    ParameterObjectUnionTypeDef,
     PollForTaskOutputTypeDef,
     QueryObjectsInputQueryObjectsPaginateTypeDef,
     QueryObjectsInputRequestTypeDef,
+    PutPipelineDefinitionInputRequestTypeDef,
+    ValidatePipelineDefinitionInputRequestTypeDef,
 )
 
 
-def get_structure() -> ParameterValueTypeDef:
+def get_value() -> ParameterValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/README.md` & `mypy-boto3-datapipeline-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datapipeline)](https://pepy.tech/project/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
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
@@ -288,24 +288,25 @@
 )
 
 
 def check_value(value: DescribeObjectsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_datapipeline.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_datapipeline.type_defs import (
     ParameterValueTypeDef,
+    TimestampTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeactivatePipelineInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
@@ -344,25 +345,27 @@
     ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
     DescribePipelinesOutputTypeDef,
     DescribeObjectsOutputTypeDef,
     TaskObjectTypeDef,
+    PipelineObjectUnionTypeDef,
     QueryTypeDef,
     GetPipelineDefinitionOutputTypeDef,
-    PutPipelineDefinitionInputRequestTypeDef,
-    ValidatePipelineDefinitionInputRequestTypeDef,
+    ParameterObjectUnionTypeDef,
     PollForTaskOutputTypeDef,
     QueryObjectsInputQueryObjectsPaginateTypeDef,
     QueryObjectsInputRequestTypeDef,
+    PutPipelineDefinitionInputRequestTypeDef,
+    ValidatePipelineDefinitionInputRequestTypeDef,
 )
 
 
-def get_structure() -> ParameterValueTypeDef:
+def get_value() -> ParameterValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__init__.py` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__init__.pyi` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__main__.py` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataPipeline 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.DataPipeline 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline\nOther"
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

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/client.py` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_datapipeline.client import DataPipelineClient
 
     session = Session()
     client: DataPipelineClient = session.client("datapipeline")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import TaskStatusType
 from .paginator import DescribeObjectsPaginator, ListPipelinesPaginator, QueryObjectsPaginator
 from .type_defs import (
     CreatePipelineOutputTypeDef,
@@ -27,55 +26,50 @@
     DescribePipelinesOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluateExpressionOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     InstanceIdentityTypeDef,
     ListPipelinesOutputTypeDef,
-    ParameterObjectOutputTypeDef,
-    ParameterObjectTypeDef,
+    ParameterObjectUnionTypeDef,
     ParameterValueTypeDef,
-    PipelineObjectOutputTypeDef,
-    PipelineObjectTypeDef,
+    PipelineObjectUnionTypeDef,
     PollForTaskOutputTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     QueryObjectsOutputTypeDef,
     QueryTypeDef,
     ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatOutputTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DataPipelineClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServiceError: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     PipelineDeletedException: Type[BotocoreClientError]
     PipelineNotFoundException: Type[BotocoreClientError]
     TaskNotFoundException: Type[BotocoreClientError]
 
-
 class DataPipelineClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/)
     """
 
     meta: ClientMeta
@@ -84,178 +78,160 @@
     def exceptions(self) -> Exceptions:
         """
         DataPipelineClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#exceptions)
         """
-
     def activate_pipeline(
         self,
         *,
         pipelineId: str,
         parameterValues: Sequence[ParameterValueTypeDef] = ...,
-        startTimestamp: Union[datetime, str] = ...
+        startTimestamp: TimestampTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Validates the specified pipeline and starts processing pipeline tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.activate_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#activate_pipeline)
         """
-
     def add_tags(self, *, pipelineId: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds or modifies tags for the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.add_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#add_tags)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#close)
         """
-
     def create_pipeline(
         self, *, name: str, uniqueId: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a new, empty pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#create_pipeline)
         """
-
     def deactivate_pipeline(self, *, pipelineId: str, cancelActive: bool = ...) -> Dict[str, Any]:
         """
         Deactivates the specified running pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.deactivate_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#deactivate_pipeline)
         """
-
     def delete_pipeline(self, *, pipelineId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a pipeline, its pipeline definition, and its run history.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.delete_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#delete_pipeline)
         """
-
     def describe_objects(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
         marker: str = ...
     ) -> DescribeObjectsOutputTypeDef:
         """
         Gets the object definitions for a set of objects associated with the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.describe_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#describe_objects)
         """
-
     def describe_pipelines(self, *, pipelineIds: Sequence[str]) -> DescribePipelinesOutputTypeDef:
         """
         Retrieves metadata about one or more pipelines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.describe_pipelines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#describe_pipelines)
         """
-
     def evaluate_expression(
         self, *, pipelineId: str, objectId: str, expression: str
     ) -> EvaluateExpressionOutputTypeDef:
         """
         Task runners call `EvaluateExpression` to evaluate a string in the context of
         the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.evaluate_expression)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#evaluate_expression)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#generate_presigned_url)
         """
-
     def get_pipeline_definition(
         self, *, pipelineId: str, version: str = ...
     ) -> GetPipelineDefinitionOutputTypeDef:
         """
         Gets the definition of the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.get_pipeline_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#get_pipeline_definition)
         """
-
     def list_pipelines(self, *, marker: str = ...) -> ListPipelinesOutputTypeDef:
         """
         Lists the pipeline identifiers for all active pipelines that you have permission
         to access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.list_pipelines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#list_pipelines)
         """
-
     def poll_for_task(
         self,
         *,
         workerGroup: str,
         hostname: str = ...,
         instanceIdentity: InstanceIdentityTypeDef = ...
     ) -> PollForTaskOutputTypeDef:
         """
         Task runners call `PollForTask` to receive a task to perform from AWS Data
         Pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.poll_for_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#poll_for_task)
         """
-
     def put_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
-        parameterObjects: Sequence[
-            Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
-        ] = ...,
+        pipelineObjects: Sequence[PipelineObjectUnionTypeDef],
+        parameterObjects: Sequence[ParameterObjectUnionTypeDef] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> PutPipelineDefinitionOutputTypeDef:
         """
         Adds tasks, schedules, and preconditions to the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.put_pipeline_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#put_pipeline_definition)
         """
-
     def query_objects(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
         marker: str = ...,
@@ -264,56 +240,51 @@
         """
         Queries the specified pipeline for the names of objects that match the specified
         set of conditions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.query_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#query_objects)
         """
-
     def remove_tags(self, *, pipelineId: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes existing tags from the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.remove_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#remove_tags)
         """
-
     def report_task_progress(
         self, *, taskId: str, fields: Sequence[FieldTypeDef] = ...
     ) -> ReportTaskProgressOutputTypeDef:
         """
         Task runners call `ReportTaskProgress` when assigned a task to acknowledge that
         it has the task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.report_task_progress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#report_task_progress)
         """
-
     def report_task_runner_heartbeat(
         self, *, taskrunnerId: str, workerGroup: str = ..., hostname: str = ...
     ) -> ReportTaskRunnerHeartbeatOutputTypeDef:
         """
         Task runners call `ReportTaskRunnerHeartbeat` every 15 minutes to indicate that
         they are operational.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.report_task_runner_heartbeat)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#report_task_runner_heartbeat)
         """
-
     def set_status(
         self, *, pipelineId: str, objectIds: Sequence[str], status: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Requests that the status of the specified physical or logical pipeline objects
         be updated in the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#set_status)
         """
-
     def set_task_status(
         self,
         *,
         taskId: str,
         taskStatus: TaskStatusType,
         errorId: str = ...,
         errorMessage: str = ...,
@@ -322,48 +293,42 @@
         """
         Task runners call `SetTaskStatus` to notify AWS Data Pipeline that a task is
         completed and provide information about the final status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_task_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#set_task_status)
         """
-
     def validate_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
-        parameterObjects: Sequence[
-            Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
-        ] = ...,
+        pipelineObjects: Sequence[PipelineObjectUnionTypeDef],
+        parameterObjects: Sequence[ParameterObjectUnionTypeDef] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> ValidatePipelineDefinitionOutputTypeDef:
         """
         Validates the specified pipeline definition to ensure that it is well formed and
         can be run without error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.validate_pipeline_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#validate_pipeline_definition)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_objects"]
     ) -> DescribeObjectsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_pipelines"]) -> ListPipelinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["query_objects"]) -> QueryObjectsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/client.pyi` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_datapipeline.client import DataPipelineClient
 
     session = Session()
     client: DataPipelineClient = session.client("datapipeline")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import TaskStatusType
 from .paginator import DescribeObjectsPaginator, ListPipelinesPaginator, QueryObjectsPaginator
 from .type_defs import (
     CreatePipelineOutputTypeDef,
@@ -27,51 +26,54 @@
     DescribePipelinesOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluateExpressionOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     InstanceIdentityTypeDef,
     ListPipelinesOutputTypeDef,
-    ParameterObjectOutputTypeDef,
-    ParameterObjectTypeDef,
+    ParameterObjectUnionTypeDef,
     ParameterValueTypeDef,
-    PipelineObjectOutputTypeDef,
-    PipelineObjectTypeDef,
+    PipelineObjectUnionTypeDef,
     PollForTaskOutputTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     QueryObjectsOutputTypeDef,
     QueryTypeDef,
     ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatOutputTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("DataPipelineClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServiceError: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     PipelineDeletedException: Type[BotocoreClientError]
     PipelineNotFoundException: Type[BotocoreClientError]
     TaskNotFoundException: Type[BotocoreClientError]
 
+
 class DataPipelineClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/)
     """
 
     meta: ClientMeta
@@ -80,162 +82,176 @@
     def exceptions(self) -> Exceptions:
         """
         DataPipelineClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#exceptions)
         """
+
     def activate_pipeline(
         self,
         *,
         pipelineId: str,
         parameterValues: Sequence[ParameterValueTypeDef] = ...,
-        startTimestamp: Union[datetime, str] = ...
+        startTimestamp: TimestampTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Validates the specified pipeline and starts processing pipeline tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.activate_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#activate_pipeline)
         """
+
     def add_tags(self, *, pipelineId: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds or modifies tags for the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.add_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#add_tags)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#close)
         """
+
     def create_pipeline(
         self, *, name: str, uniqueId: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a new, empty pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#create_pipeline)
         """
+
     def deactivate_pipeline(self, *, pipelineId: str, cancelActive: bool = ...) -> Dict[str, Any]:
         """
         Deactivates the specified running pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.deactivate_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#deactivate_pipeline)
         """
+
     def delete_pipeline(self, *, pipelineId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a pipeline, its pipeline definition, and its run history.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.delete_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#delete_pipeline)
         """
+
     def describe_objects(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
         marker: str = ...
     ) -> DescribeObjectsOutputTypeDef:
         """
         Gets the object definitions for a set of objects associated with the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.describe_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#describe_objects)
         """
+
     def describe_pipelines(self, *, pipelineIds: Sequence[str]) -> DescribePipelinesOutputTypeDef:
         """
         Retrieves metadata about one or more pipelines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.describe_pipelines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#describe_pipelines)
         """
+
     def evaluate_expression(
         self, *, pipelineId: str, objectId: str, expression: str
     ) -> EvaluateExpressionOutputTypeDef:
         """
         Task runners call `EvaluateExpression` to evaluate a string in the context of
         the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.evaluate_expression)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#evaluate_expression)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#generate_presigned_url)
         """
+
     def get_pipeline_definition(
         self, *, pipelineId: str, version: str = ...
     ) -> GetPipelineDefinitionOutputTypeDef:
         """
         Gets the definition of the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.get_pipeline_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#get_pipeline_definition)
         """
+
     def list_pipelines(self, *, marker: str = ...) -> ListPipelinesOutputTypeDef:
         """
         Lists the pipeline identifiers for all active pipelines that you have permission
         to access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.list_pipelines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#list_pipelines)
         """
+
     def poll_for_task(
         self,
         *,
         workerGroup: str,
         hostname: str = ...,
         instanceIdentity: InstanceIdentityTypeDef = ...
     ) -> PollForTaskOutputTypeDef:
         """
         Task runners call `PollForTask` to receive a task to perform from AWS Data
         Pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.poll_for_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#poll_for_task)
         """
+
     def put_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
-        parameterObjects: Sequence[
-            Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
-        ] = ...,
+        pipelineObjects: Sequence[PipelineObjectUnionTypeDef],
+        parameterObjects: Sequence[ParameterObjectUnionTypeDef] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> PutPipelineDefinitionOutputTypeDef:
         """
         Adds tasks, schedules, and preconditions to the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.put_pipeline_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#put_pipeline_definition)
         """
+
     def query_objects(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
         marker: str = ...,
@@ -244,51 +260,56 @@
         """
         Queries the specified pipeline for the names of objects that match the specified
         set of conditions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.query_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#query_objects)
         """
+
     def remove_tags(self, *, pipelineId: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes existing tags from the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.remove_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#remove_tags)
         """
+
     def report_task_progress(
         self, *, taskId: str, fields: Sequence[FieldTypeDef] = ...
     ) -> ReportTaskProgressOutputTypeDef:
         """
         Task runners call `ReportTaskProgress` when assigned a task to acknowledge that
         it has the task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.report_task_progress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#report_task_progress)
         """
+
     def report_task_runner_heartbeat(
         self, *, taskrunnerId: str, workerGroup: str = ..., hostname: str = ...
     ) -> ReportTaskRunnerHeartbeatOutputTypeDef:
         """
         Task runners call `ReportTaskRunnerHeartbeat` every 15 minutes to indicate that
         they are operational.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.report_task_runner_heartbeat)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#report_task_runner_heartbeat)
         """
+
     def set_status(
         self, *, pipelineId: str, objectIds: Sequence[str], status: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Requests that the status of the specified physical or logical pipeline objects
         be updated in the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#set_status)
         """
+
     def set_task_status(
         self,
         *,
         taskId: str,
         taskStatus: TaskStatusType,
         errorId: str = ...,
         errorMessage: str = ...,
@@ -297,44 +318,46 @@
         """
         Task runners call `SetTaskStatus` to notify AWS Data Pipeline that a task is
         completed and provide information about the final status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_task_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#set_task_status)
         """
+
     def validate_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
-        parameterObjects: Sequence[
-            Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
-        ] = ...,
+        pipelineObjects: Sequence[PipelineObjectUnionTypeDef],
+        parameterObjects: Sequence[ParameterObjectUnionTypeDef] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> ValidatePipelineDefinitionOutputTypeDef:
         """
         Validates the specified pipeline definition to ensure that it is well formed and
         can be run without error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.validate_pipeline_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#validate_pipeline_definition)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_objects"]
     ) -> DescribeObjectsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_pipelines"]) -> ListPipelinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["query_objects"]) -> QueryObjectsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/literals.py` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/literals.pyi` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/paginator.py` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/paginator.pyi` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/type_defs.py` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_datapipeline.type_defs import ParameterValueTypeDef
 
-    data: ParameterValueTypeDef = {...}
+    data: ParameterValueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import OperatorTypeType, TaskStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ParameterValueTypeDef",
+    "TimestampTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeactivatePipelineInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeObjectsInputRequestTypeDef",
     "DescribePipelinesInputRequestTypeDef",
@@ -67,31 +67,34 @@
     "ParameterObjectOutputTypeDef",
     "ParameterObjectTypeDef",
     "PutPipelineDefinitionOutputTypeDef",
     "ValidatePipelineDefinitionOutputTypeDef",
     "DescribePipelinesOutputTypeDef",
     "DescribeObjectsOutputTypeDef",
     "TaskObjectTypeDef",
+    "PipelineObjectUnionTypeDef",
     "QueryTypeDef",
     "GetPipelineDefinitionOutputTypeDef",
-    "PutPipelineDefinitionInputRequestTypeDef",
-    "ValidatePipelineDefinitionInputRequestTypeDef",
+    "ParameterObjectUnionTypeDef",
     "PollForTaskOutputTypeDef",
     "QueryObjectsInputQueryObjectsPaginateTypeDef",
     "QueryObjectsInputRequestTypeDef",
+    "PutPipelineDefinitionInputRequestTypeDef",
+    "ValidatePipelineDefinitionInputRequestTypeDef",
 )
 
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
     {
         "id": str,
         "stringValue": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -117,21 +120,19 @@
     "_OptionalDeactivatePipelineInputRequestTypeDef",
     {
         "cancelActive": bool,
     },
     total=False,
 )
 
-
 class DeactivatePipelineInputRequestTypeDef(
     _RequiredDeactivatePipelineInputRequestTypeDef, _OptionalDeactivatePipelineInputRequestTypeDef
 ):
     pass
 
-
 DeletePipelineInputRequestTypeDef = TypedDict(
     "DeletePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 
@@ -157,21 +158,19 @@
     {
         "evaluateExpressions": bool,
         "marker": str,
     },
     total=False,
 )
 
-
 class DescribeObjectsInputRequestTypeDef(
     _RequiredDescribeObjectsInputRequestTypeDef, _OptionalDescribeObjectsInputRequestTypeDef
 ):
     pass
 
-
 DescribePipelinesInputRequestTypeDef = TypedDict(
     "DescribePipelinesInputRequestTypeDef",
     {
         "pipelineIds": Sequence[str],
     },
 )
 
@@ -195,41 +194,37 @@
     {
         "stringValue": str,
         "refValue": str,
     },
     total=False,
 )
 
-
 class FieldTypeDef(_RequiredFieldTypeDef, _OptionalFieldTypeDef):
     pass
 
-
 _RequiredGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredGetPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalGetPipelineDefinitionInputRequestTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
-
 class GetPipelineDefinitionInputRequestTypeDef(
     _RequiredGetPipelineDefinitionInputRequestTypeDef,
     _OptionalGetPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
-
 InstanceIdentityTypeDef = TypedDict(
     "InstanceIdentityTypeDef",
     {
         "document": str,
         "signature": str,
     },
     total=False,
@@ -306,22 +301,20 @@
     {
         "workerGroup": str,
         "hostname": str,
     },
     total=False,
 )
 
-
 class ReportTaskRunnerHeartbeatInputRequestTypeDef(
     _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef,
     _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef,
 ):
     pass
 
-
 SetStatusInputRequestTypeDef = TypedDict(
     "SetStatusInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
         "status": str,
     },
@@ -340,43 +333,39 @@
         "errorId": str,
         "errorMessage": str,
         "errorStackTrace": str,
     },
     total=False,
 )
 
-
 class SetTaskStatusInputRequestTypeDef(
     _RequiredSetTaskStatusInputRequestTypeDef, _OptionalSetTaskStatusInputRequestTypeDef
 ):
     pass
 
-
 _RequiredActivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredActivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalActivatePipelineInputRequestTypeDef = TypedDict(
     "_OptionalActivatePipelineInputRequestTypeDef",
     {
         "parameterValues": Sequence[ParameterValueTypeDef],
-        "startTimestamp": Union[datetime, str],
+        "startTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class ActivatePipelineInputRequestTypeDef(
     _RequiredActivatePipelineInputRequestTypeDef, _OptionalActivatePipelineInputRequestTypeDef
 ):
     pass
 
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -393,21 +382,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
-
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
         "pipelineId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -465,22 +452,20 @@
     {
         "evaluateExpressions": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
     _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
     _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
 ):
     pass
 
-
 ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -498,21 +483,19 @@
     {
         "description": str,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class PipelineDescriptionTypeDef(
     _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
 ):
     pass
 
-
 PipelineObjectOutputTypeDef = TypedDict(
     "PipelineObjectOutputTypeDef",
     {
         "id": str,
         "name": str,
         "fields": List[FieldTypeDef],
     },
@@ -537,21 +520,19 @@
     "_OptionalReportTaskProgressInputRequestTypeDef",
     {
         "fields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
-
 class ReportTaskProgressInputRequestTypeDef(
     _RequiredReportTaskProgressInputRequestTypeDef, _OptionalReportTaskProgressInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPollForTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForTaskInputRequestTypeDef",
     {
         "workerGroup": str,
     },
 )
 _OptionalPollForTaskInputRequestTypeDef = TypedDict(
@@ -559,21 +540,19 @@
     {
         "hostname": str,
         "instanceIdentity": InstanceIdentityTypeDef,
     },
     total=False,
 )
 
-
 class PollForTaskInputRequestTypeDef(
     _RequiredPollForTaskInputRequestTypeDef, _OptionalPollForTaskInputRequestTypeDef
 ):
     pass
 
-
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelineIdList": List[PipelineIdNameTypeDef],
         "marker": str,
         "hasMoreResults": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -650,14 +629,15 @@
         "pipelineId": str,
         "attemptId": str,
         "objects": Dict[str, PipelineObjectOutputTypeDef],
     },
     total=False,
 )
 
+PipelineObjectUnionTypeDef = Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
         "selectors": Sequence[SelectorTypeDef],
     },
     total=False,
 )
@@ -668,62 +648,15 @@
         "pipelineObjects": List[PipelineObjectOutputTypeDef],
         "parameterObjects": List[ParameterObjectOutputTypeDef],
         "parameterValues": List[ParameterValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_RequiredPutPipelineDefinitionInputRequestTypeDef",
-    {
-        "pipelineId": str,
-        "pipelineObjects": Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
-    },
-)
-_OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_OptionalPutPipelineDefinitionInputRequestTypeDef",
-    {
-        "parameterObjects": Sequence[Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]],
-        "parameterValues": Sequence[ParameterValueTypeDef],
-    },
-    total=False,
-)
-
-
-class PutPipelineDefinitionInputRequestTypeDef(
-    _RequiredPutPipelineDefinitionInputRequestTypeDef,
-    _OptionalPutPipelineDefinitionInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
-    {
-        "pipelineId": str,
-        "pipelineObjects": Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
-    },
-)
-_OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
-    {
-        "parameterObjects": Sequence[Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]],
-        "parameterValues": Sequence[ParameterValueTypeDef],
-    },
-    total=False,
-)
-
-
-class ValidatePipelineDefinitionInputRequestTypeDef(
-    _RequiredValidatePipelineDefinitionInputRequestTypeDef,
-    _OptionalValidatePipelineDefinitionInputRequestTypeDef,
-):
-    pass
-
-
+ParameterObjectUnionTypeDef = Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -740,22 +673,20 @@
     {
         "query": QueryTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class QueryObjectsInputQueryObjectsPaginateTypeDef(
     _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef,
     _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredQueryObjectsInputRequestTypeDef = TypedDict(
     "_RequiredQueryObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
@@ -765,12 +696,55 @@
         "query": QueryTypeDef,
         "marker": str,
         "limit": int,
     },
     total=False,
 )
 
-
 class QueryObjectsInputRequestTypeDef(
     _RequiredQueryObjectsInputRequestTypeDef, _OptionalQueryObjectsInputRequestTypeDef
 ):
     pass
+
+_RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_RequiredPutPipelineDefinitionInputRequestTypeDef",
+    {
+        "pipelineId": str,
+        "pipelineObjects": Sequence[PipelineObjectUnionTypeDef],
+    },
+)
+_OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_OptionalPutPipelineDefinitionInputRequestTypeDef",
+    {
+        "parameterObjects": Sequence[ParameterObjectUnionTypeDef],
+        "parameterValues": Sequence[ParameterValueTypeDef],
+    },
+    total=False,
+)
+
+class PutPipelineDefinitionInputRequestTypeDef(
+    _RequiredPutPipelineDefinitionInputRequestTypeDef,
+    _OptionalPutPipelineDefinitionInputRequestTypeDef,
+):
+    pass
+
+_RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
+    {
+        "pipelineId": str,
+        "pipelineObjects": Sequence[PipelineObjectUnionTypeDef],
+    },
+)
+_OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
+    {
+        "parameterObjects": Sequence[ParameterObjectUnionTypeDef],
+        "parameterValues": Sequence[ParameterValueTypeDef],
+    },
+    total=False,
+)
+
+class ValidatePipelineDefinitionInputRequestTypeDef(
+    _RequiredValidatePipelineDefinitionInputRequestTypeDef,
+    _OptionalValidatePipelineDefinitionInputRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/type_defs.pyi` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_datapipeline.type_defs import ParameterValueTypeDef
 
-    data: ParameterValueTypeDef = {...}
+    data: ParameterValueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import OperatorTypeType, TaskStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ParameterValueTypeDef",
+    "TimestampTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeactivatePipelineInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeObjectsInputRequestTypeDef",
     "DescribePipelinesInputRequestTypeDef",
@@ -66,31 +68,34 @@
     "ParameterObjectOutputTypeDef",
     "ParameterObjectTypeDef",
     "PutPipelineDefinitionOutputTypeDef",
     "ValidatePipelineDefinitionOutputTypeDef",
     "DescribePipelinesOutputTypeDef",
     "DescribeObjectsOutputTypeDef",
     "TaskObjectTypeDef",
+    "PipelineObjectUnionTypeDef",
     "QueryTypeDef",
     "GetPipelineDefinitionOutputTypeDef",
-    "PutPipelineDefinitionInputRequestTypeDef",
-    "ValidatePipelineDefinitionInputRequestTypeDef",
+    "ParameterObjectUnionTypeDef",
     "PollForTaskOutputTypeDef",
     "QueryObjectsInputQueryObjectsPaginateTypeDef",
     "QueryObjectsInputRequestTypeDef",
+    "PutPipelineDefinitionInputRequestTypeDef",
+    "ValidatePipelineDefinitionInputRequestTypeDef",
 )
 
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
     {
         "id": str,
         "stringValue": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -116,19 +121,21 @@
     "_OptionalDeactivatePipelineInputRequestTypeDef",
     {
         "cancelActive": bool,
     },
     total=False,
 )
 
+
 class DeactivatePipelineInputRequestTypeDef(
     _RequiredDeactivatePipelineInputRequestTypeDef, _OptionalDeactivatePipelineInputRequestTypeDef
 ):
     pass
 
+
 DeletePipelineInputRequestTypeDef = TypedDict(
     "DeletePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 
@@ -154,19 +161,21 @@
     {
         "evaluateExpressions": bool,
         "marker": str,
     },
     total=False,
 )
 
+
 class DescribeObjectsInputRequestTypeDef(
     _RequiredDescribeObjectsInputRequestTypeDef, _OptionalDescribeObjectsInputRequestTypeDef
 ):
     pass
 
+
 DescribePipelinesInputRequestTypeDef = TypedDict(
     "DescribePipelinesInputRequestTypeDef",
     {
         "pipelineIds": Sequence[str],
     },
 )
 
@@ -190,37 +199,41 @@
     {
         "stringValue": str,
         "refValue": str,
     },
     total=False,
 )
 
+
 class FieldTypeDef(_RequiredFieldTypeDef, _OptionalFieldTypeDef):
     pass
 
+
 _RequiredGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredGetPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalGetPipelineDefinitionInputRequestTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
+
 class GetPipelineDefinitionInputRequestTypeDef(
     _RequiredGetPipelineDefinitionInputRequestTypeDef,
     _OptionalGetPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
+
 InstanceIdentityTypeDef = TypedDict(
     "InstanceIdentityTypeDef",
     {
         "document": str,
         "signature": str,
     },
     total=False,
@@ -297,20 +310,22 @@
     {
         "workerGroup": str,
         "hostname": str,
     },
     total=False,
 )
 
+
 class ReportTaskRunnerHeartbeatInputRequestTypeDef(
     _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef,
     _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef,
 ):
     pass
 
+
 SetStatusInputRequestTypeDef = TypedDict(
     "SetStatusInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
         "status": str,
     },
@@ -329,39 +344,43 @@
         "errorId": str,
         "errorMessage": str,
         "errorStackTrace": str,
     },
     total=False,
 )
 
+
 class SetTaskStatusInputRequestTypeDef(
     _RequiredSetTaskStatusInputRequestTypeDef, _OptionalSetTaskStatusInputRequestTypeDef
 ):
     pass
 
+
 _RequiredActivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredActivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalActivatePipelineInputRequestTypeDef = TypedDict(
     "_OptionalActivatePipelineInputRequestTypeDef",
     {
         "parameterValues": Sequence[ParameterValueTypeDef],
-        "startTimestamp": Union[datetime, str],
+        "startTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class ActivatePipelineInputRequestTypeDef(
     _RequiredActivatePipelineInputRequestTypeDef, _OptionalActivatePipelineInputRequestTypeDef
 ):
     pass
 
+
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -378,19 +397,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
+
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
         "pipelineId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -448,20 +469,22 @@
     {
         "evaluateExpressions": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
     _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
     _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
 ):
     pass
 
+
 ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -479,19 +502,21 @@
     {
         "description": str,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class PipelineDescriptionTypeDef(
     _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
 ):
     pass
 
+
 PipelineObjectOutputTypeDef = TypedDict(
     "PipelineObjectOutputTypeDef",
     {
         "id": str,
         "name": str,
         "fields": List[FieldTypeDef],
     },
@@ -516,19 +541,21 @@
     "_OptionalReportTaskProgressInputRequestTypeDef",
     {
         "fields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
+
 class ReportTaskProgressInputRequestTypeDef(
     _RequiredReportTaskProgressInputRequestTypeDef, _OptionalReportTaskProgressInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPollForTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForTaskInputRequestTypeDef",
     {
         "workerGroup": str,
     },
 )
 _OptionalPollForTaskInputRequestTypeDef = TypedDict(
@@ -536,19 +563,21 @@
     {
         "hostname": str,
         "instanceIdentity": InstanceIdentityTypeDef,
     },
     total=False,
 )
 
+
 class PollForTaskInputRequestTypeDef(
     _RequiredPollForTaskInputRequestTypeDef, _OptionalPollForTaskInputRequestTypeDef
 ):
     pass
 
+
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelineIdList": List[PipelineIdNameTypeDef],
         "marker": str,
         "hasMoreResults": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -625,14 +654,15 @@
         "pipelineId": str,
         "attemptId": str,
         "objects": Dict[str, PipelineObjectOutputTypeDef],
     },
     total=False,
 )
 
+PipelineObjectUnionTypeDef = Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
         "selectors": Sequence[SelectorTypeDef],
     },
     total=False,
 )
@@ -643,58 +673,15 @@
         "pipelineObjects": List[PipelineObjectOutputTypeDef],
         "parameterObjects": List[ParameterObjectOutputTypeDef],
         "parameterValues": List[ParameterValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_RequiredPutPipelineDefinitionInputRequestTypeDef",
-    {
-        "pipelineId": str,
-        "pipelineObjects": Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
-    },
-)
-_OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_OptionalPutPipelineDefinitionInputRequestTypeDef",
-    {
-        "parameterObjects": Sequence[Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]],
-        "parameterValues": Sequence[ParameterValueTypeDef],
-    },
-    total=False,
-)
-
-class PutPipelineDefinitionInputRequestTypeDef(
-    _RequiredPutPipelineDefinitionInputRequestTypeDef,
-    _OptionalPutPipelineDefinitionInputRequestTypeDef,
-):
-    pass
-
-_RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
-    {
-        "pipelineId": str,
-        "pipelineObjects": Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
-    },
-)
-_OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
-    {
-        "parameterObjects": Sequence[Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]],
-        "parameterValues": Sequence[ParameterValueTypeDef],
-    },
-    total=False,
-)
-
-class ValidatePipelineDefinitionInputRequestTypeDef(
-    _RequiredValidatePipelineDefinitionInputRequestTypeDef,
-    _OptionalValidatePipelineDefinitionInputRequestTypeDef,
-):
-    pass
-
+ParameterObjectUnionTypeDef = Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -711,20 +698,22 @@
     {
         "query": QueryTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class QueryObjectsInputQueryObjectsPaginateTypeDef(
     _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef,
     _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredQueryObjectsInputRequestTypeDef = TypedDict(
     "_RequiredQueryObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
@@ -734,11 +723,60 @@
         "query": QueryTypeDef,
         "marker": str,
         "limit": int,
     },
     total=False,
 )
 
+
 class QueryObjectsInputRequestTypeDef(
     _RequiredQueryObjectsInputRequestTypeDef, _OptionalQueryObjectsInputRequestTypeDef
 ):
     pass
+
+
+_RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_RequiredPutPipelineDefinitionInputRequestTypeDef",
+    {
+        "pipelineId": str,
+        "pipelineObjects": Sequence[PipelineObjectUnionTypeDef],
+    },
+)
+_OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_OptionalPutPipelineDefinitionInputRequestTypeDef",
+    {
+        "parameterObjects": Sequence[ParameterObjectUnionTypeDef],
+        "parameterValues": Sequence[ParameterValueTypeDef],
+    },
+    total=False,
+)
+
+
+class PutPipelineDefinitionInputRequestTypeDef(
+    _RequiredPutPipelineDefinitionInputRequestTypeDef,
+    _OptionalPutPipelineDefinitionInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
+    {
+        "pipelineId": str,
+        "pipelineObjects": Sequence[PipelineObjectUnionTypeDef],
+    },
+)
+_OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
+    {
+        "parameterObjects": Sequence[ParameterObjectUnionTypeDef],
+        "parameterValues": Sequence[ParameterValueTypeDef],
+    },
+    total=False,
+)
+
+
+class ValidatePipelineDefinitionInputRequestTypeDef(
+    _RequiredValidatePipelineDefinitionInputRequestTypeDef,
+    _OptionalValidatePipelineDefinitionInputRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/PKG-INFO` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DataPipeline 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 datapipeline type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 datapipeline type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datapipeline)](https://pepy.tech/project/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
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
@@ -320,24 +320,25 @@
 )
 
 
 def check_value(value: DescribeObjectsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_datapipeline.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_datapipeline.type_defs import (
     ParameterValueTypeDef,
+    TimestampTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeactivatePipelineInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
@@ -376,25 +377,27 @@
     ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
     DescribePipelinesOutputTypeDef,
     DescribeObjectsOutputTypeDef,
     TaskObjectTypeDef,
+    PipelineObjectUnionTypeDef,
     QueryTypeDef,
     GetPipelineDefinitionOutputTypeDef,
-    PutPipelineDefinitionInputRequestTypeDef,
-    ValidatePipelineDefinitionInputRequestTypeDef,
+    ParameterObjectUnionTypeDef,
     PollForTaskOutputTypeDef,
     QueryObjectsInputQueryObjectsPaginateTypeDef,
     QueryObjectsInputRequestTypeDef,
+    PutPipelineDefinitionInputRequestTypeDef,
+    ValidatePipelineDefinitionInputRequestTypeDef,
 )
 
 
-def get_structure() -> ParameterValueTypeDef:
+def get_value() -> ParameterValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/SOURCES.txt` & `mypy-boto3-datapipeline-1.28.16/mypy_boto3_datapipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15.post1/setup.py` & `mypy-boto3-datapipeline-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datapipeline",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_datapipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.DataPipeline 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 datapipeline type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 datapipeline type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_datapipeline": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

