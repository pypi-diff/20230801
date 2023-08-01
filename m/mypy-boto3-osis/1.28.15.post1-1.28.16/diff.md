# Comparing `tmp/mypy-boto3-osis-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-osis-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-osis-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:49 2023, max compression
+gzip compressed data, was "mypy-boto3-osis-1.28.16.tar", last modified: Tue Aug  1 11:37:30 2023, max compression
```

## Comparing `mypy-boto3-osis-1.28.15.post1.tar` & `mypy-boto3-osis-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:49.945324 mypy-boto3-osis-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-07-29 10:03:49.945324 mypy-boto3-osis-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:49.929324 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11168 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:49.929324 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:49.945324 mypy-boto3-osis-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:30.476796 mypy-boto3-osis-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-08-01 11:37:30.476796 mypy-boto3-osis-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:30.468796 mypy-boto3-osis-1.28.16/mypy_boto3_osis/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:30.476796 mypy-boto3-osis-1.28.16/mypy_boto3_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-08-01 11:37:30.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 11:37:30.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:30.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:30.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:30.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 11:37:30.000000 mypy-boto3-osis-1.28.16/mypy_boto3_osis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:30.476796 mypy-boto3-osis-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-01 11:25:45.000000 mypy-boto3-osis-1.28.16/setup.py
```

### Comparing `mypy-boto3-osis-1.28.15.post1/LICENSE` & `mypy-boto3-osis-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15.post1/PKG-INFO` & `mypy-boto3-osis-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.OpenSearchIngestion 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 osis type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 osis type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-osis)](https://pepy.tech/project/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
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
@@ -289,20 +289,20 @@
 )
 
 
 def check_value(value: ChangeProgressStageStatusesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_osis.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
@@ -327,28 +327,29 @@
     TagResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
     VpcEndpointTypeDef,
+    VpcOptionsUnionTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
     PipelineTypeDef,
     CreatePipelineResponseTypeDef,
     GetPipelineResponseTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     UpdatePipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ChangeProgressStageTypeDef:
+def get_value() -> ChangeProgressStageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-osis-1.28.15.post1/README.md` & `mypy-boto3-osis-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-osis)](https://pepy.tech/project/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
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
@@ -257,20 +257,20 @@
 )
 
 
 def check_value(value: ChangeProgressStageStatusesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_osis.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
@@ -295,28 +295,29 @@
     TagResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
     VpcEndpointTypeDef,
+    VpcOptionsUnionTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
     PipelineTypeDef,
     CreatePipelineResponseTypeDef,
     GetPipelineResponseTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     UpdatePipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ChangeProgressStageTypeDef:
+def get_value() -> ChangeProgressStageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/__main__.py` & `mypy-boto3-osis-1.28.16/mypy_boto3_osis/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchIngestion 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.OpenSearchIngestion 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion\nOther"
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

### Comparing `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/client.py` & `mypy-boto3-osis-1.28.16/mypy_boto3_osis/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_osis.client import OpenSearchIngestionClient
 
     session = Session()
     client: OpenSearchIngestionClient = session.client("osis")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     CreatePipelineResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
@@ -27,16 +27,15 @@
     ListTagsForResourceResponseTypeDef,
     LogPublishingOptionsTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     TagTypeDef,
     UpdatePipelineResponseTypeDef,
     ValidatePipelineResponseTypeDef,
-    VpcOptionsOutputTypeDef,
-    VpcOptionsTypeDef,
+    VpcOptionsUnionTypeDef,
 )
 
 __all__ = ("OpenSearchIngestionClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -95,15 +94,15 @@
         self,
         *,
         PipelineName: str,
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
-        VpcOptions: Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef] = ...,
+        VpcOptions: VpcOptionsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/client/#create_pipeline)
```

### Comparing `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/client.pyi` & `mypy-boto3-osis-1.28.16/mypy_boto3_osis/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_osis.client import OpenSearchIngestionClient
 
     session = Session()
     client: OpenSearchIngestionClient = session.client("osis")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     CreatePipelineResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
@@ -27,16 +27,15 @@
     ListTagsForResourceResponseTypeDef,
     LogPublishingOptionsTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     TagTypeDef,
     UpdatePipelineResponseTypeDef,
     ValidatePipelineResponseTypeDef,
-    VpcOptionsOutputTypeDef,
-    VpcOptionsTypeDef,
+    VpcOptionsUnionTypeDef,
 )
 
 __all__ = ("OpenSearchIngestionClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -89,15 +88,15 @@
         self,
         *,
         PipelineName: str,
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
-        VpcOptions: Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef] = ...,
+        VpcOptions: VpcOptionsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/client/#create_pipeline)
```

### Comparing `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/literals.py` & `mypy-boto3-osis-1.28.16/mypy_boto3_osis/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/literals.pyi` & `mypy-boto3-osis-1.28.16/mypy_boto3_osis/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/type_defs.py` & `mypy-boto3-osis-1.28.16/mypy_boto3_osis/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,32 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_osis.type_defs import ChangeProgressStageTypeDef
 
-    data: ChangeProgressStageTypeDef = {...}
+    data: ChangeProgressStageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ChangeProgressStageStatusesType,
     ChangeProgressStatusesType,
     PipelineStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ChangeProgressStageTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
     "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
@@ -53,14 +52,15 @@
     "TagResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
     "VpcEndpointTypeDef",
+    "VpcOptionsUnionTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
     "PipelineTypeDef",
     "CreatePipelineResponseTypeDef",
     "GetPipelineResponseTypeDef",
@@ -105,19 +105,17 @@
     "_OptionalVpcOptionsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class VpcOptionsTypeDef(_RequiredVpcOptionsTypeDef, _OptionalVpcOptionsTypeDef):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -241,19 +239,17 @@
     "_OptionalVpcOptionsOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
-
 class VpcOptionsOutputTypeDef(_RequiredVpcOptionsOutputTypeDef, _OptionalVpcOptionsOutputTypeDef):
     pass
 
-
 ChangeProgressStatusTypeDef = TypedDict(
     "ChangeProgressStatusTypeDef",
     {
         "StartTime": datetime,
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
@@ -332,14 +328,15 @@
         "VpcEndpointId": str,
         "VpcId": str,
         "VpcOptions": VpcOptionsOutputTypeDef,
     },
     total=False,
 )
 
+VpcOptionsUnionTypeDef = Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef]
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -359,21 +356,19 @@
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcOptions": VpcOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -383,21 +378,19 @@
         "MaxUnits": int,
         "PipelineConfigurationBody": str,
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
-
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "NextToken": str,
         "Pipelines": List[PipelineSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/type_defs.pyi` & `mypy-boto3-osis-1.28.16/mypy_boto3_osis/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_osis.type_defs import ChangeProgressStageTypeDef
 
-    data: ChangeProgressStageTypeDef = {...}
+    data: ChangeProgressStageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ChangeProgressStageStatusesType,
     ChangeProgressStatusesType,
     PipelineStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ChangeProgressStageTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
     "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
@@ -52,14 +53,15 @@
     "TagResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
     "VpcEndpointTypeDef",
+    "VpcOptionsUnionTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
     "PipelineTypeDef",
     "CreatePipelineResponseTypeDef",
     "GetPipelineResponseTypeDef",
@@ -104,17 +106,19 @@
     "_OptionalVpcOptionsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class VpcOptionsTypeDef(_RequiredVpcOptionsTypeDef, _OptionalVpcOptionsTypeDef):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -238,17 +242,19 @@
     "_OptionalVpcOptionsOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
+
 class VpcOptionsOutputTypeDef(_RequiredVpcOptionsOutputTypeDef, _OptionalVpcOptionsOutputTypeDef):
     pass
 
+
 ChangeProgressStatusTypeDef = TypedDict(
     "ChangeProgressStatusTypeDef",
     {
         "StartTime": datetime,
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
@@ -327,14 +333,15 @@
         "VpcEndpointId": str,
         "VpcId": str,
         "VpcOptions": VpcOptionsOutputTypeDef,
     },
     total=False,
 )
 
+VpcOptionsUnionTypeDef = Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef]
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -354,19 +361,21 @@
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcOptions": VpcOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -376,19 +385,21 @@
         "MaxUnits": int,
         "PipelineConfigurationBody": str,
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
+
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "NextToken": str,
         "Pipelines": List[PipelineSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/PKG-INFO` & `mypy-boto3-osis-1.28.16/mypy_boto3_osis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.OpenSearchIngestion 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 osis type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 osis type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-osis)](https://pepy.tech/project/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
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
@@ -289,20 +289,20 @@
 )
 
 
 def check_value(value: ChangeProgressStageStatusesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_osis.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
@@ -327,28 +327,29 @@
     TagResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
     VpcEndpointTypeDef,
+    VpcOptionsUnionTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
     PipelineTypeDef,
     CreatePipelineResponseTypeDef,
     GetPipelineResponseTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     UpdatePipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ChangeProgressStageTypeDef:
+def get_value() -> ChangeProgressStageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/SOURCES.txt` & `mypy-boto3-osis-1.28.16/mypy_boto3_osis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15.post1/setup.py` & `mypy-boto3-osis-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-osis",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_osis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.OpenSearchIngestion 1.28.16 service generated with"
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
-    keywords="boto3 osis type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 osis type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_osis": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

