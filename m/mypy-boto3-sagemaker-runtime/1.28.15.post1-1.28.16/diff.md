# Comparing `tmp/mypy-boto3-sagemaker-runtime-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-sagemaker-runtime-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-runtime-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:08 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-runtime-1.28.16.tar", last modified: Tue Aug  1 11:37:47 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1.tar` & `mypy-boto3-sagemaker-runtime-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:08.037388 mypy-boto3-sagemaker-runtime-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-07-29 10:04:08.037388 mypy-boto3-sagemaker-runtime-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:08.029388 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-29 09:58:41.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-29 09:58:41.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-29 09:58:41.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-29 09:58:41.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:08.033388 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-07-29 10:04:07.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-29 10:04:07.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:07.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:07.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:07.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:04:07.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:08.037388 mypy-boto3-sagemaker-runtime-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:58:40.000000 mypy-boto3-sagemaker-runtime-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:47.420745 mypy-boto3-sagemaker-runtime-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-08-01 11:37:47.416745 mypy-boto3-sagemaker-runtime-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:47.408745 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:47.416745 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-08-01 11:37:47.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-01 11:37:47.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:47.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:47.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:47.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:37:47.000000 mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:47.420745 mypy-boto3-sagemaker-runtime-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 11:32:08.000000 mypy-boto3-sagemaker-runtime-1.28.16/setup.py
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/LICENSE` & `mypy-boto3-sagemaker-runtime-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/PKG-INFO` & `mypy-boto3-sagemaker-runtime-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-runtime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SageMakerRuntime 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SageMakerRuntime 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-runtime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerRuntime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
+[boto3.SageMakerRuntime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
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
 [mypy-boto3-sagemaker-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/).
 
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
@@ -288,32 +288,33 @@
 )
 
 
 def check_value(value: SageMakerRuntimeServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_runtime.type_defs import (
+    BlobTypeDef,
     InvokeEndpointAsyncInputRequestTypeDef,
     ResponseMetadataTypeDef,
     InvokeEndpointInputRequestTypeDef,
     InvokeEndpointAsyncOutputTypeDef,
     InvokeEndpointOutputTypeDef,
 )
 
 
-def get_structure() -> InvokeEndpointAsyncInputRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/README.md` & `mypy-boto3-sagemaker-runtime-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerRuntime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
+[boto3.SageMakerRuntime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
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
 [mypy-boto3-sagemaker-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/).
 
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
@@ -256,32 +256,33 @@
 )
 
 
 def check_value(value: SageMakerRuntimeServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_runtime.type_defs import (
+    BlobTypeDef,
     InvokeEndpointAsyncInputRequestTypeDef,
     ResponseMetadataTypeDef,
     InvokeEndpointInputRequestTypeDef,
     InvokeEndpointAsyncOutputTypeDef,
     InvokeEndpointOutputTypeDef,
 )
 
 
-def get_structure() -> InvokeEndpointAsyncInputRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/__main__.py` & `mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerRuntime 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.SageMakerRuntime 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime\nOther"
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

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/client.py` & `mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,19 @@
     from boto3.session import Session
     from mypy_boto3_sagemaker_runtime.client import SageMakerRuntimeClient
 
     session = Session()
     client: SageMakerRuntimeClient = session.client("sagemaker-runtime")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
-from .type_defs import InvokeEndpointAsyncOutputTypeDef, InvokeEndpointOutputTypeDef
+from .type_defs import BlobTypeDef, InvokeEndpointAsyncOutputTypeDef, InvokeEndpointOutputTypeDef
 
 __all__ = ("SageMakerRuntimeClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -88,15 +87,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/client/#generate_presigned_url)
         """
 
     def invoke_endpoint(
         self,
         *,
         EndpointName: str,
-        Body: Union[str, bytes, IO[Any], StreamingBody],
+        Body: BlobTypeDef,
         ContentType: str = ...,
         Accept: str = ...,
         CustomAttributes: str = ...,
         TargetModel: str = ...,
         TargetVariant: str = ...,
         TargetContainerHostname: str = ...,
         InferenceId: str = ...,
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/client.pyi` & `mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,19 @@
     from boto3.session import Session
     from mypy_boto3_sagemaker_runtime.client import SageMakerRuntimeClient
 
     session = Session()
     client: SageMakerRuntimeClient = session.client("sagemaker-runtime")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
-from .type_defs import InvokeEndpointAsyncOutputTypeDef, InvokeEndpointOutputTypeDef
+from .type_defs import BlobTypeDef, InvokeEndpointAsyncOutputTypeDef, InvokeEndpointOutputTypeDef
 
 __all__ = ("SageMakerRuntimeClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -81,15 +80,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/client/#generate_presigned_url)
         """
     def invoke_endpoint(
         self,
         *,
         EndpointName: str,
-        Body: Union[str, bytes, IO[Any], StreamingBody],
+        Body: BlobTypeDef,
         ContentType: str = ...,
         Accept: str = ...,
         CustomAttributes: str = ...,
         TargetModel: str = ...,
         TargetVariant: str = ...,
         TargetContainerHostname: str = ...,
         InferenceId: str = ...,
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/literals.py` & `mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/literals.pyi` & `mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/type_defs.py` & `mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 Type annotations for sagemaker-runtime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sagemaker_runtime.type_defs import InvokeEndpointAsyncInputRequestTypeDef
+    from mypy_boto3_sagemaker_runtime.type_defs import BlobTypeDef
 
-    data: InvokeEndpointAsyncInputRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, Union
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "InvokeEndpointAsyncInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "InvokeEndpointInputRequestTypeDef",
     "InvokeEndpointAsyncOutputTypeDef",
     "InvokeEndpointOutputTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredInvokeEndpointAsyncInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointAsyncInputRequestTypeDef",
     {
         "EndpointName": str,
         "InputLocation": str,
     },
 )
@@ -68,15 +70,15 @@
     },
 )
 
 _RequiredInvokeEndpointInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
-        "Body": Union[str, bytes, IO[Any], StreamingBody],
+        "Body": BlobTypeDef,
     },
 )
 _OptionalInvokeEndpointInputRequestTypeDef = TypedDict(
     "_OptionalInvokeEndpointInputRequestTypeDef",
     {
         "ContentType": str,
         "Accept": str,
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime/type_defs.pyi` & `mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,39 @@
 Type annotations for sagemaker-runtime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sagemaker_runtime.type_defs import InvokeEndpointAsyncInputRequestTypeDef
+    from mypy_boto3_sagemaker_runtime.type_defs import BlobTypeDef
 
-    data: InvokeEndpointAsyncInputRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, Union
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "InvokeEndpointAsyncInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "InvokeEndpointInputRequestTypeDef",
     "InvokeEndpointAsyncOutputTypeDef",
     "InvokeEndpointOutputTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredInvokeEndpointAsyncInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointAsyncInputRequestTypeDef",
     {
         "EndpointName": str,
         "InputLocation": str,
     },
 )
@@ -65,15 +67,15 @@
     },
 )
 
 _RequiredInvokeEndpointInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
-        "Body": Union[str, bytes, IO[Any], StreamingBody],
+        "Body": BlobTypeDef,
     },
 )
 _OptionalInvokeEndpointInputRequestTypeDef = TypedDict(
     "_OptionalInvokeEndpointInputRequestTypeDef",
     {
         "ContentType": str,
         "Accept": str,
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-runtime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SageMakerRuntime 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SageMakerRuntime 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-runtime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerRuntime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
+[boto3.SageMakerRuntime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
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
 [mypy-boto3-sagemaker-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/).
 
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
@@ -288,32 +288,33 @@
 )
 
 
 def check_value(value: SageMakerRuntimeServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_runtime.type_defs import (
+    BlobTypeDef,
     InvokeEndpointAsyncInputRequestTypeDef,
     ResponseMetadataTypeDef,
     InvokeEndpointInputRequestTypeDef,
     InvokeEndpointAsyncOutputTypeDef,
     InvokeEndpointOutputTypeDef,
 )
 
 
-def get_structure() -> InvokeEndpointAsyncInputRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-runtime-1.28.16/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.28.15.post1/setup.py` & `mypy-boto3-sagemaker-runtime-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-runtime",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_sagemaker_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerRuntime 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SageMakerRuntime 1.28.16 service generated with"
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
-    keywords="boto3 sagemaker-runtime type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 sagemaker-runtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sagemaker_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

