# Comparing `tmp/mypy-boto3-elastictranscoder-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-elastictranscoder-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elastictranscoder-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:04 2023, max compression
+gzip compressed data, was "mypy-boto3-elastictranscoder-1.28.16.tar", last modified: Tue Aug  1 11:36:45 2023, max compression
```

## Comparing `mypy-boto3-elastictranscoder-1.28.15.post1.tar` & `mypy-boto3-elastictranscoder-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:04.685137 mypy-boto3-elastictranscoder-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-29 10:03:04.685137 mypy-boto3-elastictranscoder-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:04.685137 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25150 2023-07-29 09:44:47.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25131 2023-07-29 09:44:47.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:04.685137 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-29 10:03:04.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 10:03:04.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:04.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:04.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:04.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:03:04.000000 mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:04.685137 mypy-boto3-elastictranscoder-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-29 09:44:46.000000 mypy-boto3-elastictranscoder-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.116896 mypy-boto3-elastictranscoder-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-08-01 11:36:45.112896 mypy-boto3-elastictranscoder-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15256 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.104896 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-08-01 11:17:23.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-08-01 11:17:23.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25495 2023-08-01 11:17:24.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25477 2023-08-01 11:17:23.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-01 11:17:23.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-01 11:17:23.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.112896 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-08-01 11:36:44.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-01 11:36:44.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:44.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:44.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:44.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:36:44.000000 mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:45.116896 mypy-boto3-elastictranscoder-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-01 11:17:21.000000 mypy-boto3-elastictranscoder-1.28.16/setup.py
```

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/LICENSE` & `mypy-boto3-elastictranscoder-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/PKG-INFO` & `mypy-boto3-elastictranscoder-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastictranscoder
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ElasticTranscoder 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ElasticTranscoder 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 elastictranscoder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 elastictranscoder type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastictranscoder)](https://pepy.tech/project/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -349,20 +349,20 @@
 )
 
 
 def check_value(value: JobCompleteWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elastictranscoder.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elastictranscoder.type_defs import (
     EncryptionTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
     TimeSpanTypeDef,
@@ -413,40 +413,43 @@
     JobAlbumArtTypeDef,
     CaptionsOutputTypeDef,
     CaptionsTypeDef,
     InputCaptionsOutputTypeDef,
     InputCaptionsTypeDef,
     PipelineTypeDef,
     CreatePipelineRequestRequestTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     PresetTypeDef,
     CreatePresetRequestRequestTypeDef,
+    VideoParametersUnionTypeDef,
     JobOutputTypeDef,
     CreateJobOutputTypeDef,
     JobInputOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
     CreatePresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     ReadPresetResponseTypeDef,
     JobTypeDef,
-    CreateJobRequestRequestTypeDef,
+    JobInputUnionTypeDef,
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
+    CreateJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> EncryptionTypeDef:
+def get_value() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/README.md` & `mypy-boto3-elastictranscoder-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastictranscoder)](https://pepy.tech/project/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -317,20 +317,20 @@
 )
 
 
 def check_value(value: JobCompleteWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elastictranscoder.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elastictranscoder.type_defs import (
     EncryptionTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
     TimeSpanTypeDef,
@@ -381,40 +381,43 @@
     JobAlbumArtTypeDef,
     CaptionsOutputTypeDef,
     CaptionsTypeDef,
     InputCaptionsOutputTypeDef,
     InputCaptionsTypeDef,
     PipelineTypeDef,
     CreatePipelineRequestRequestTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     PresetTypeDef,
     CreatePresetRequestRequestTypeDef,
+    VideoParametersUnionTypeDef,
     JobOutputTypeDef,
     CreateJobOutputTypeDef,
     JobInputOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
     CreatePresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     ReadPresetResponseTypeDef,
     JobTypeDef,
-    CreateJobRequestRequestTypeDef,
+    JobInputUnionTypeDef,
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
+    CreateJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> EncryptionTypeDef:
+def get_value() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/__init__.py` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/__init__.pyi` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/__main__.py` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticTranscoder 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ElasticTranscoder 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder\nOther"
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

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/client.py` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_elastictranscoder.client import ElasticTranscoderClient
 
     session = Session()
     client: ElasticTranscoderClient = session.client("elastictranscoder")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListJobsByPipelinePaginator,
     ListJobsByStatusPaginator,
     ListPipelinesPaginator,
@@ -27,64 +27,57 @@
 from .type_defs import (
     AudioParametersTypeDef,
     CreateJobOutputTypeDef,
     CreateJobPlaylistTypeDef,
     CreateJobResponseTypeDef,
     CreatePipelineResponseTypeDef,
     CreatePresetResponseTypeDef,
-    JobInputOutputTypeDef,
-    JobInputTypeDef,
+    JobInputUnionTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListPresetsResponseTypeDef,
     NotificationsTypeDef,
-    PipelineOutputConfigOutputTypeDef,
-    PipelineOutputConfigTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     ReadJobResponseTypeDef,
     ReadPipelineResponseTypeDef,
     ReadPresetResponseTypeDef,
     TestRoleResponseTypeDef,
     ThumbnailsTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
-    VideoParametersOutputTypeDef,
-    VideoParametersTypeDef,
+    VideoParametersUnionTypeDef,
 )
 from .waiter import JobCompleteWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ElasticTranscoderClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IncompatibleVersionException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class ElasticTranscoderClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/)
     """
 
     meta: ClientMeta
@@ -93,273 +86,248 @@
     def exceptions(self) -> Exceptions:
         """
         ElasticTranscoderClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#can_paginate)
         """
-
     def cancel_job(self, *, Id: str) -> Dict[str, Any]:
         """
         The CancelJob operation cancels an unfinished job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.cancel_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#cancel_job)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#close)
         """
-
     def create_job(
         self,
         *,
         PipelineId: str,
-        Input: Union[JobInputTypeDef, JobInputOutputTypeDef] = ...,
-        Inputs: Sequence[Union[JobInputTypeDef, JobInputOutputTypeDef]] = ...,
+        Input: JobInputUnionTypeDef = ...,
+        Inputs: Sequence[JobInputUnionTypeDef] = ...,
         Output: CreateJobOutputTypeDef = ...,
         Outputs: Sequence[CreateJobOutputTypeDef] = ...,
         OutputKeyPrefix: str = ...,
         Playlists: Sequence[CreateJobPlaylistTypeDef] = ...,
         UserMetadata: Mapping[str, str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         When you create a job, Elastic Transcoder returns JSON data that includes the
         values that you specified plus information about the job that is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#create_job)
         """
-
     def create_pipeline(
         self,
         *,
         Name: str,
         InputBucket: str,
         Role: str,
         OutputBucket: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: Union[PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef] = ...,
-        ThumbnailConfig: Union[PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef] = ...
+        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         The CreatePipeline operation creates a pipeline with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#create_pipeline)
         """
-
     def create_preset(
         self,
         *,
         Name: str,
         Container: str,
         Description: str = ...,
-        Video: Union[VideoParametersTypeDef, VideoParametersOutputTypeDef] = ...,
+        Video: VideoParametersUnionTypeDef = ...,
         Audio: AudioParametersTypeDef = ...,
         Thumbnails: ThumbnailsTypeDef = ...
     ) -> CreatePresetResponseTypeDef:
         """
         The CreatePreset operation creates a preset with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_preset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#create_preset)
         """
-
     def delete_pipeline(self, *, Id: str) -> Dict[str, Any]:
         """
         The DeletePipeline operation removes a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.delete_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#delete_pipeline)
         """
-
     def delete_preset(self, *, Id: str) -> Dict[str, Any]:
         """
         The DeletePreset operation removes a preset that you've added in an AWS region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.delete_preset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#delete_preset)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#generate_presigned_url)
         """
-
     def list_jobs_by_pipeline(
         self, *, PipelineId: str, Ascending: str = ..., PageToken: str = ...
     ) -> ListJobsByPipelineResponseTypeDef:
         """
         The ListJobsByPipeline operation gets a list of the jobs currently in a
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_jobs_by_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#list_jobs_by_pipeline)
         """
-
     def list_jobs_by_status(
         self, *, Status: str, Ascending: str = ..., PageToken: str = ...
     ) -> ListJobsByStatusResponseTypeDef:
         """
         The ListJobsByStatus operation gets a list of jobs that have a specified status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_jobs_by_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#list_jobs_by_status)
         """
-
     def list_pipelines(
         self, *, Ascending: str = ..., PageToken: str = ...
     ) -> ListPipelinesResponseTypeDef:
         """
         The ListPipelines operation gets a list of the pipelines associated with the
         current AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_pipelines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#list_pipelines)
         """
-
     def list_presets(
         self, *, Ascending: str = ..., PageToken: str = ...
     ) -> ListPresetsResponseTypeDef:
         """
         The ListPresets operation gets a list of the default presets included with
         Elastic Transcoder and the presets that you've added in an AWS region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_presets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#list_presets)
         """
-
     def read_job(self, *, Id: str) -> ReadJobResponseTypeDef:
         """
         The ReadJob operation returns detailed information about a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.read_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#read_job)
         """
-
     def read_pipeline(self, *, Id: str) -> ReadPipelineResponseTypeDef:
         """
         The ReadPipeline operation gets detailed information about a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.read_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#read_pipeline)
         """
-
     def read_preset(self, *, Id: str) -> ReadPresetResponseTypeDef:
         """
         The ReadPreset operation gets detailed information about a preset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.read_preset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#read_preset)
         """
-
     def test_role(
         self, *, Role: str, InputBucket: str, OutputBucket: str, Topics: Sequence[str]
     ) -> TestRoleResponseTypeDef:
         """
         The TestRole operation tests the IAM role used to create the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.test_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#test_role)
         """
-
     def update_pipeline(
         self,
         *,
         Id: str,
         Name: str = ...,
         InputBucket: str = ...,
         Role: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: Union[PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef] = ...,
-        ThumbnailConfig: Union[PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef] = ...
+        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
     ) -> UpdatePipelineResponseTypeDef:
         """
         Use the `UpdatePipeline` operation to update settings for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#update_pipeline)
         """
-
     def update_pipeline_notifications(
         self, *, Id: str, Notifications: NotificationsTypeDef
     ) -> UpdatePipelineNotificationsResponseTypeDef:
         """
         With the UpdatePipelineNotifications operation, you can update Amazon Simple
         Notification Service (Amazon SNS) notifications for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#update_pipeline_notifications)
         """
-
     def update_pipeline_status(
         self, *, Id: str, Status: str
     ) -> UpdatePipelineStatusResponseTypeDef:
         """
         The UpdatePipelineStatus operation pauses or reactivates a pipeline, so that the
         pipeline stops or restarts the processing of jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#update_pipeline_status)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_jobs_by_pipeline"]
     ) -> ListJobsByPipelinePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_jobs_by_status"]
     ) -> ListJobsByStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_pipelines"]) -> ListPipelinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_presets"]) -> ListPresetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_paginator)
         """
-
     def get_waiter(self, waiter_name: Literal["job_complete"]) -> JobCompleteWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/client.pyi` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_elastictranscoder.client import ElasticTranscoderClient
 
     session = Session()
     client: ElasticTranscoderClient = session.client("elastictranscoder")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListJobsByPipelinePaginator,
     ListJobsByStatusPaginator,
     ListPipelinesPaginator,
@@ -27,60 +27,61 @@
 from .type_defs import (
     AudioParametersTypeDef,
     CreateJobOutputTypeDef,
     CreateJobPlaylistTypeDef,
     CreateJobResponseTypeDef,
     CreatePipelineResponseTypeDef,
     CreatePresetResponseTypeDef,
-    JobInputOutputTypeDef,
-    JobInputTypeDef,
+    JobInputUnionTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListPresetsResponseTypeDef,
     NotificationsTypeDef,
-    PipelineOutputConfigOutputTypeDef,
-    PipelineOutputConfigTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     ReadJobResponseTypeDef,
     ReadPipelineResponseTypeDef,
     ReadPresetResponseTypeDef,
     TestRoleResponseTypeDef,
     ThumbnailsTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
-    VideoParametersOutputTypeDef,
-    VideoParametersTypeDef,
+    VideoParametersUnionTypeDef,
 )
 from .waiter import JobCompleteWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ElasticTranscoderClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IncompatibleVersionException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class ElasticTranscoderClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/)
     """
 
     meta: ClientMeta
@@ -89,248 +90,273 @@
     def exceptions(self) -> Exceptions:
         """
         ElasticTranscoderClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#can_paginate)
         """
+
     def cancel_job(self, *, Id: str) -> Dict[str, Any]:
         """
         The CancelJob operation cancels an unfinished job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.cancel_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#cancel_job)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#close)
         """
+
     def create_job(
         self,
         *,
         PipelineId: str,
-        Input: Union[JobInputTypeDef, JobInputOutputTypeDef] = ...,
-        Inputs: Sequence[Union[JobInputTypeDef, JobInputOutputTypeDef]] = ...,
+        Input: JobInputUnionTypeDef = ...,
+        Inputs: Sequence[JobInputUnionTypeDef] = ...,
         Output: CreateJobOutputTypeDef = ...,
         Outputs: Sequence[CreateJobOutputTypeDef] = ...,
         OutputKeyPrefix: str = ...,
         Playlists: Sequence[CreateJobPlaylistTypeDef] = ...,
         UserMetadata: Mapping[str, str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         When you create a job, Elastic Transcoder returns JSON data that includes the
         values that you specified plus information about the job that is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#create_job)
         """
+
     def create_pipeline(
         self,
         *,
         Name: str,
         InputBucket: str,
         Role: str,
         OutputBucket: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: Union[PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef] = ...,
-        ThumbnailConfig: Union[PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef] = ...
+        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         The CreatePipeline operation creates a pipeline with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#create_pipeline)
         """
+
     def create_preset(
         self,
         *,
         Name: str,
         Container: str,
         Description: str = ...,
-        Video: Union[VideoParametersTypeDef, VideoParametersOutputTypeDef] = ...,
+        Video: VideoParametersUnionTypeDef = ...,
         Audio: AudioParametersTypeDef = ...,
         Thumbnails: ThumbnailsTypeDef = ...
     ) -> CreatePresetResponseTypeDef:
         """
         The CreatePreset operation creates a preset with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_preset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#create_preset)
         """
+
     def delete_pipeline(self, *, Id: str) -> Dict[str, Any]:
         """
         The DeletePipeline operation removes a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.delete_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#delete_pipeline)
         """
+
     def delete_preset(self, *, Id: str) -> Dict[str, Any]:
         """
         The DeletePreset operation removes a preset that you've added in an AWS region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.delete_preset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#delete_preset)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#generate_presigned_url)
         """
+
     def list_jobs_by_pipeline(
         self, *, PipelineId: str, Ascending: str = ..., PageToken: str = ...
     ) -> ListJobsByPipelineResponseTypeDef:
         """
         The ListJobsByPipeline operation gets a list of the jobs currently in a
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_jobs_by_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#list_jobs_by_pipeline)
         """
+
     def list_jobs_by_status(
         self, *, Status: str, Ascending: str = ..., PageToken: str = ...
     ) -> ListJobsByStatusResponseTypeDef:
         """
         The ListJobsByStatus operation gets a list of jobs that have a specified status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_jobs_by_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#list_jobs_by_status)
         """
+
     def list_pipelines(
         self, *, Ascending: str = ..., PageToken: str = ...
     ) -> ListPipelinesResponseTypeDef:
         """
         The ListPipelines operation gets a list of the pipelines associated with the
         current AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_pipelines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#list_pipelines)
         """
+
     def list_presets(
         self, *, Ascending: str = ..., PageToken: str = ...
     ) -> ListPresetsResponseTypeDef:
         """
         The ListPresets operation gets a list of the default presets included with
         Elastic Transcoder and the presets that you've added in an AWS region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_presets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#list_presets)
         """
+
     def read_job(self, *, Id: str) -> ReadJobResponseTypeDef:
         """
         The ReadJob operation returns detailed information about a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.read_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#read_job)
         """
+
     def read_pipeline(self, *, Id: str) -> ReadPipelineResponseTypeDef:
         """
         The ReadPipeline operation gets detailed information about a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.read_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#read_pipeline)
         """
+
     def read_preset(self, *, Id: str) -> ReadPresetResponseTypeDef:
         """
         The ReadPreset operation gets detailed information about a preset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.read_preset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#read_preset)
         """
+
     def test_role(
         self, *, Role: str, InputBucket: str, OutputBucket: str, Topics: Sequence[str]
     ) -> TestRoleResponseTypeDef:
         """
         The TestRole operation tests the IAM role used to create the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.test_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#test_role)
         """
+
     def update_pipeline(
         self,
         *,
         Id: str,
         Name: str = ...,
         InputBucket: str = ...,
         Role: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: Union[PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef] = ...,
-        ThumbnailConfig: Union[PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef] = ...
+        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
     ) -> UpdatePipelineResponseTypeDef:
         """
         Use the `UpdatePipeline` operation to update settings for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#update_pipeline)
         """
+
     def update_pipeline_notifications(
         self, *, Id: str, Notifications: NotificationsTypeDef
     ) -> UpdatePipelineNotificationsResponseTypeDef:
         """
         With the UpdatePipelineNotifications operation, you can update Amazon Simple
         Notification Service (Amazon SNS) notifications for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#update_pipeline_notifications)
         """
+
     def update_pipeline_status(
         self, *, Id: str, Status: str
     ) -> UpdatePipelineStatusResponseTypeDef:
         """
         The UpdatePipelineStatus operation pauses or reactivates a pipeline, so that the
         pipeline stops or restarts the processing of jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#update_pipeline_status)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_jobs_by_pipeline"]
     ) -> ListJobsByPipelinePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_jobs_by_status"]
     ) -> ListJobsByStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_pipelines"]) -> ListPipelinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_presets"]) -> ListPresetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_paginator)
         """
+
     def get_waiter(self, waiter_name: Literal["job_complete"]) -> JobCompleteWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/literals.py` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/literals.pyi` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/paginator.py` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/paginator.pyi` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/type_defs.py` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_elastictranscoder.type_defs import EncryptionTypeDef
 
-    data: EncryptionTypeDef = {...}
+    data: EncryptionTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -72,36 +72,39 @@
     "JobAlbumArtTypeDef",
     "CaptionsOutputTypeDef",
     "CaptionsTypeDef",
     "InputCaptionsOutputTypeDef",
     "InputCaptionsTypeDef",
     "PipelineTypeDef",
     "CreatePipelineRequestRequestTypeDef",
+    "PipelineOutputConfigUnionTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "PresetTypeDef",
     "CreatePresetRequestRequestTypeDef",
+    "VideoParametersUnionTypeDef",
     "JobOutputTypeDef",
     "CreateJobOutputTypeDef",
     "JobInputOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
     "CreatePresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "ReadPresetResponseTypeDef",
     "JobTypeDef",
-    "CreateJobRequestRequestTypeDef",
+    "JobInputUnionTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
+    "CreateJobRequestRequestTypeDef",
 )
 
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
@@ -760,14 +763,17 @@
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
 
+PipelineOutputConfigUnionTypeDef = Union[
+    PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef
+]
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -828,14 +834,15 @@
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
 
+VideoParametersUnionTypeDef = Union[VideoParametersTypeDef, VideoParametersOutputTypeDef]
 JobOutputTypeDef = TypedDict(
     "JobOutputTypeDef",
     {
         "Id": str,
         "Key": str,
         "ThumbnailPattern": str,
         "ThumbnailEncryption": EncryptionTypeDef,
@@ -1005,41 +1012,15 @@
         "Status": str,
         "UserMetadata": Dict[str, str],
         "Timing": TimingTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "Input": JobInputTypeDef,
-        "Inputs": Sequence[Union[JobInputTypeDef, JobInputOutputTypeDef]],
-        "Output": CreateJobOutputTypeDef,
-        "Outputs": Sequence[CreateJobOutputTypeDef],
-        "OutputKeyPrefix": str,
-        "Playlists": Sequence[CreateJobPlaylistTypeDef],
-        "UserMetadata": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
-
+JobInputUnionTypeDef = Union[JobInputTypeDef, JobInputOutputTypeDef]
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1065,7 +1046,33 @@
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "Input": JobInputTypeDef,
+        "Inputs": Sequence[JobInputUnionTypeDef],
+        "Output": CreateJobOutputTypeDef,
+        "Outputs": Sequence[CreateJobOutputTypeDef],
+        "OutputKeyPrefix": str,
+        "Playlists": Sequence[CreateJobPlaylistTypeDef],
+        "UserMetadata": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/type_defs.pyi` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_elastictranscoder.type_defs import EncryptionTypeDef
 
-    data: EncryptionTypeDef = {...}
+    data: EncryptionTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -71,36 +71,39 @@
     "JobAlbumArtTypeDef",
     "CaptionsOutputTypeDef",
     "CaptionsTypeDef",
     "InputCaptionsOutputTypeDef",
     "InputCaptionsTypeDef",
     "PipelineTypeDef",
     "CreatePipelineRequestRequestTypeDef",
+    "PipelineOutputConfigUnionTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "PresetTypeDef",
     "CreatePresetRequestRequestTypeDef",
+    "VideoParametersUnionTypeDef",
     "JobOutputTypeDef",
     "CreateJobOutputTypeDef",
     "JobInputOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
     "CreatePresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "ReadPresetResponseTypeDef",
     "JobTypeDef",
-    "CreateJobRequestRequestTypeDef",
+    "JobInputUnionTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
+    "CreateJobRequestRequestTypeDef",
 )
 
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
@@ -747,14 +750,17 @@
 )
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
+PipelineOutputConfigUnionTypeDef = Union[
+    PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef
+]
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -811,14 +817,15 @@
 )
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
+VideoParametersUnionTypeDef = Union[VideoParametersTypeDef, VideoParametersOutputTypeDef]
 JobOutputTypeDef = TypedDict(
     "JobOutputTypeDef",
     {
         "Id": str,
         "Key": str,
         "ThumbnailPattern": str,
         "ThumbnailEncryption": EncryptionTypeDef,
@@ -988,39 +995,15 @@
         "Status": str,
         "UserMetadata": Dict[str, str],
         "Timing": TimingTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "Input": JobInputTypeDef,
-        "Inputs": Sequence[Union[JobInputTypeDef, JobInputOutputTypeDef]],
-        "Output": CreateJobOutputTypeDef,
-        "Outputs": Sequence[CreateJobOutputTypeDef],
-        "OutputKeyPrefix": str,
-        "Playlists": Sequence[CreateJobPlaylistTypeDef],
-        "UserMetadata": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
+JobInputUnionTypeDef = Union[JobInputTypeDef, JobInputOutputTypeDef]
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1046,7 +1029,32 @@
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "Input": JobInputTypeDef,
+        "Inputs": Sequence[JobInputUnionTypeDef],
+        "Output": CreateJobOutputTypeDef,
+        "Outputs": Sequence[CreateJobOutputTypeDef],
+        "OutputKeyPrefix": str,
+        "Playlists": Sequence[CreateJobPlaylistTypeDef],
+        "UserMetadata": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/waiter.py` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder/waiter.pyi` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder.egg-info/PKG-INFO` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastictranscoder
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ElasticTranscoder 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ElasticTranscoder 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 elastictranscoder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 elastictranscoder type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastictranscoder)](https://pepy.tech/project/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -349,20 +349,20 @@
 )
 
 
 def check_value(value: JobCompleteWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elastictranscoder.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elastictranscoder.type_defs import (
     EncryptionTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
     TimeSpanTypeDef,
@@ -413,40 +413,43 @@
     JobAlbumArtTypeDef,
     CaptionsOutputTypeDef,
     CaptionsTypeDef,
     InputCaptionsOutputTypeDef,
     InputCaptionsTypeDef,
     PipelineTypeDef,
     CreatePipelineRequestRequestTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     PresetTypeDef,
     CreatePresetRequestRequestTypeDef,
+    VideoParametersUnionTypeDef,
     JobOutputTypeDef,
     CreateJobOutputTypeDef,
     JobInputOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
     CreatePresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     ReadPresetResponseTypeDef,
     JobTypeDef,
-    CreateJobRequestRequestTypeDef,
+    JobInputUnionTypeDef,
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
+    CreateJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> EncryptionTypeDef:
+def get_value() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt` & `mypy-boto3-elastictranscoder-1.28.16/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.15.post1/setup.py` & `mypy-boto3-elastictranscoder-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elastictranscoder",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_elastictranscoder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticTranscoder 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ElasticTranscoder 1.28.16 service generated with"
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
-    keywords="boto3 elastictranscoder type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 elastictranscoder type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_elastictranscoder": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

