# Comparing `tmp/mypy-boto3-ivs-1.28.16.tar.gz` & `tmp/mypy-boto3-ivs-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-1.28.16.tar", last modified: Tue Aug  1 11:37:03 2023, max compression
+gzip compressed data, was "mypy-boto3-ivs-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-ivs-1.28.16.tar` & `mypy-boto3-ivs-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.764858 mypy-boto3-ivs-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16750 2023-08-01 11:37:03.748858 mypy-boto3-ivs-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.748858 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22950 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22908 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-08-01 11:21:10.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-08-01 11:21:10.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-08-01 11:21:11.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27982 2023-08-01 11:21:10.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.748858 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16750 2023-08-01 11:37:03.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:37:03.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:03.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:03.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:03.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:03.000000 mypy-boto3-ivs-1.28.16/mypy_boto3_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:03.764858 mypy-boto3-ivs-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:21:09.000000 mypy-boto3-ivs-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16775 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.965310 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22888 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26821 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16775 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/setup.py
```

### Comparing `mypy-boto3-ivs-1.28.16/LICENSE` & `mypy-boto3-ivs-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.16/PKG-INFO` & `mypy-boto3-ivs-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.28.16
-Summary: Type annotations for boto3.IVS 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.4
+Summary: Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ivs type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 ivs type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -337,20 +337,20 @@
 )
 
 
 def check_value(value: ChannelLatencyModeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_ivs.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
@@ -364,14 +364,15 @@
     RenditionConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
@@ -408,14 +409,15 @@
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
@@ -423,28 +425,26 @@
     ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
-    RenditionConfigurationUnionTypeDef,
-    ThumbnailConfigurationUnionTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
     RecordingConfigurationSummaryTypeDef,
     RecordingConfigurationTypeDef,
+    CreateRecordingConfigurationRequestRequestTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     GetRecordingConfigurationResponseTypeDef,
     StreamSessionTypeDef,
     GetStreamSessionResponseTypeDef,
 )
 
 
-def get_value() -> AudioConfigurationTypeDef:
+def get_structure() -> AudioConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ivs-1.28.16/README.md` & `mypy-boto3-ivs-1.28.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -305,20 +305,20 @@
 )
 
 
 def check_value(value: ChannelLatencyModeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_ivs.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
@@ -332,14 +332,15 @@
     RenditionConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
@@ -376,14 +377,15 @@
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
@@ -391,28 +393,26 @@
     ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
-    RenditionConfigurationUnionTypeDef,
-    ThumbnailConfigurationUnionTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
     RecordingConfigurationSummaryTypeDef,
     RecordingConfigurationTypeDef,
+    CreateRecordingConfigurationRequestRequestTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     GetRecordingConfigurationResponseTypeDef,
     StreamSessionTypeDef,
     GetStreamSessionResponseTypeDef,
 )
 
 
-def get_value() -> AudioConfigurationTypeDef:
+def get_structure() -> AudioConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/__init__.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/__init__.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/__main__.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IVS 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.IVS 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/client.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     ListChannelsResponseTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    RenditionConfigurationUnionTypeDef,
+    RenditionConfigurationTypeDef,
     StreamFiltersTypeDef,
-    ThumbnailConfigurationUnionTypeDef,
+    ThumbnailConfigurationTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -168,17 +168,17 @@
 
     def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
-        renditionConfiguration: RenditionConfigurationUnionTypeDef = ...,
+        renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        thumbnailConfiguration: ThumbnailConfigurationUnionTypeDef = ...
+        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#create_recording_configuration)
         """
```

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/client.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     ListChannelsResponseTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    RenditionConfigurationUnionTypeDef,
+    RenditionConfigurationTypeDef,
     StreamFiltersTypeDef,
-    ThumbnailConfigurationUnionTypeDef,
+    ThumbnailConfigurationTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -157,17 +157,17 @@
         """
     def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
-        renditionConfiguration: RenditionConfigurationUnionTypeDef = ...,
+        renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        thumbnailConfiguration: ThumbnailConfigurationUnionTypeDef = ...
+        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#create_recording_configuration)
         """
```

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/literals.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -263,28 +262,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/literals.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -261,28 +260,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/paginator.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/paginator.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/type_defs.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ivs.type_defs import AudioConfigurationTypeDef
 
-    data: AudioConfigurationTypeDef = ...
+    data: AudioConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
     RenditionConfigurationRenditionSelectionType,
@@ -50,14 +50,15 @@
     "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
@@ -94,14 +95,15 @@
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
@@ -109,19 +111,17 @@
     "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
-    "RenditionConfigurationUnionTypeDef",
-    "ThumbnailConfigurationUnionTypeDef",
-    "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
+    "CreateRecordingConfigurationRequestRequestTypeDef",
     "ListRecordingConfigurationsResponseTypeDef",
     "CreateRecordingConfigurationResponseTypeDef",
     "GetRecordingConfigurationResponseTypeDef",
     "StreamSessionTypeDef",
     "GetStreamSessionResponseTypeDef",
 )
 
@@ -129,25 +129,23 @@
     "AudioConfigurationTypeDef",
     {
         "channels": int,
         "codec": str,
         "sampleRate": int,
         "targetBitrate": int,
     },
-    total=False,
 )
 
 BatchErrorTypeDef = TypedDict(
     "BatchErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
-    total=False,
 )
 
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -164,15 +162,14 @@
         "name": str,
         "playbackUrl": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -193,41 +190,26 @@
     "StreamKeyTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
-    total=False,
 )
 
-_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+BatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationErrorTypeDef",
     {
         "channelArn": str,
-        "viewerId": str,
-    },
-)
-_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
-    {
         "code": str,
         "message": str,
+        "viewerId": str,
     },
-    total=False,
 )
 
-
-class BatchStartViewerSessionRevocationErrorTypeDef(
-    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
-    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
-):
-    pass
-
-
 _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
     "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
     },
 )
@@ -256,15 +238,14 @@
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
         "insecureIngest": bool,
@@ -343,14 +324,21 @@
 DeleteStreamKeyRequestRequestTypeDef = TypedDict(
     "DeleteStreamKeyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
         "bucketName": str,
     },
 )
 
@@ -372,15 +360,14 @@
     "PlaybackKeyPairTypeDef",
     {
         "arn": str,
         "fingerprint": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 GetRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecordingConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
@@ -407,15 +394,14 @@
         "health": StreamHealthType,
         "playbackUrl": str,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 _RequiredGetStreamSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetStreamSessionRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -466,15 +452,14 @@
         "codec": str,
         "encoder": str,
         "targetBitrate": int,
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -506,15 +491,14 @@
 PlaybackKeyPairSummaryTypeDef = TypedDict(
     "PlaybackKeyPairSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
@@ -547,15 +531,14 @@
 StreamKeySummaryTypeDef = TypedDict(
     "StreamKeySummaryTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListStreamSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamSessionsRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -581,15 +564,14 @@
     "StreamSessionSummaryTypeDef",
     {
         "endTime": datetime,
         "hasErrorEvent": bool,
         "startTime": datetime,
         "streamId": str,
     },
-    total=False,
 )
 
 StreamFiltersTypeDef = TypedDict(
     "StreamFiltersTypeDef",
     {
         "health": StreamHealthType,
     },
@@ -602,15 +584,14 @@
         "channelArn": str,
         "health": StreamHealthType,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
@@ -626,26 +607,24 @@
 
 RenditionConfigurationOutputTypeDef = TypedDict(
     "RenditionConfigurationOutputTypeDef",
     {
         "renditionSelection": RenditionConfigurationRenditionSelectionType,
         "renditions": List[RenditionConfigurationRenditionType],
     },
-    total=False,
 )
 
 ThumbnailConfigurationOutputTypeDef = TypedDict(
     "ThumbnailConfigurationOutputTypeDef",
     {
         "recordingMode": RecordingModeType,
         "resolution": ThumbnailConfigurationResolutionType,
         "storage": List[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
-    total=False,
 )
 
 _RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
@@ -677,15 +656,14 @@
 StreamEventTypeDef = TypedDict(
     "StreamEventTypeDef",
     {
         "eventTime": datetime,
         "name": str,
         "type": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -821,14 +799,21 @@
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "s3": S3DestinationConfigurationOutputTypeDef,
+    },
+)
+
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
@@ -859,15 +844,14 @@
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
-    total=False,
 )
 
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "filterByName": str,
         "filterByRecordingConfigurationArn": str,
@@ -965,93 +949,61 @@
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RenditionConfigurationUnionTypeDef = Union[
-    RenditionConfigurationTypeDef, RenditionConfigurationOutputTypeDef
-]
-ThumbnailConfigurationUnionTypeDef = Union[
-    ThumbnailConfigurationTypeDef, ThumbnailConfigurationOutputTypeDef
-]
-_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
+RecordingConfigurationSummaryTypeDef = TypedDict(
+    "RecordingConfigurationSummaryTypeDef",
     {
+        "arn": str,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
-        "recordingReconnectWindowSeconds": int,
-        "renditionConfiguration": RenditionConfigurationTypeDef,
-        "tags": Mapping[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
+        "state": RecordingConfigurationStateType,
+        "tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class CreateRecordingConfigurationRequestRequestTypeDef(
-    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
-    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationSummaryTypeDef",
+RecordingConfigurationTypeDef = TypedDict(
+    "RecordingConfigurationTypeDef",
     {
         "arn": str,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationSummaryTypeDef",
-    {
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
+        "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-
-class RecordingConfigurationSummaryTypeDef(
-    _RequiredRecordingConfigurationSummaryTypeDef, _OptionalRecordingConfigurationSummaryTypeDef
-):
-    pass
-
-
-_RequiredRecordingConfigurationTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationTypeDef",
+_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
     },
 )
-_OptionalRecordingConfigurationTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationTypeDef",
+_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
-        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
-        "tags": Dict[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
+        "renditionConfiguration": RenditionConfigurationTypeDef,
+        "tags": Mapping[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class RecordingConfigurationTypeDef(
-    _RequiredRecordingConfigurationTypeDef, _OptionalRecordingConfigurationTypeDef
+class CreateRecordingConfigurationRequestRequestTypeDef(
+    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
+    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
@@ -1084,15 +1036,14 @@
         "endTime": datetime,
         "ingestConfiguration": IngestConfigurationTypeDef,
         "recordingConfiguration": RecordingConfigurationTypeDef,
         "startTime": datetime,
         "streamId": str,
         "truncatedEvents": List[StreamEventTypeDef],
     },
-    total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs/type_defs.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ivs.type_defs import AudioConfigurationTypeDef
 
-    data: AudioConfigurationTypeDef = ...
+    data: AudioConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
     RenditionConfigurationRenditionSelectionType,
@@ -49,14 +49,15 @@
     "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
@@ -93,14 +94,15 @@
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
@@ -108,19 +110,17 @@
     "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
-    "RenditionConfigurationUnionTypeDef",
-    "ThumbnailConfigurationUnionTypeDef",
-    "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
+    "CreateRecordingConfigurationRequestRequestTypeDef",
     "ListRecordingConfigurationsResponseTypeDef",
     "CreateRecordingConfigurationResponseTypeDef",
     "GetRecordingConfigurationResponseTypeDef",
     "StreamSessionTypeDef",
     "GetStreamSessionResponseTypeDef",
 )
 
@@ -128,25 +128,23 @@
     "AudioConfigurationTypeDef",
     {
         "channels": int,
         "codec": str,
         "sampleRate": int,
         "targetBitrate": int,
     },
-    total=False,
 )
 
 BatchErrorTypeDef = TypedDict(
     "BatchErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
-    total=False,
 )
 
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -163,15 +161,14 @@
         "name": str,
         "playbackUrl": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -192,39 +189,26 @@
     "StreamKeyTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
-    total=False,
 )
 
-_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+BatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationErrorTypeDef",
     {
         "channelArn": str,
-        "viewerId": str,
-    },
-)
-_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
-    {
         "code": str,
         "message": str,
+        "viewerId": str,
     },
-    total=False,
 )
 
-class BatchStartViewerSessionRevocationErrorTypeDef(
-    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
-    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
-):
-    pass
-
 _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
     "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
     },
 )
@@ -251,15 +235,14 @@
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
         "insecureIngest": bool,
@@ -336,14 +319,21 @@
 DeleteStreamKeyRequestRequestTypeDef = TypedDict(
     "DeleteStreamKeyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
         "bucketName": str,
     },
 )
 
@@ -365,15 +355,14 @@
     "PlaybackKeyPairTypeDef",
     {
         "arn": str,
         "fingerprint": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 GetRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecordingConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
@@ -400,15 +389,14 @@
         "health": StreamHealthType,
         "playbackUrl": str,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 _RequiredGetStreamSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetStreamSessionRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -455,15 +443,14 @@
         "codec": str,
         "encoder": str,
         "targetBitrate": int,
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -495,15 +482,14 @@
 PlaybackKeyPairSummaryTypeDef = TypedDict(
     "PlaybackKeyPairSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
@@ -534,15 +520,14 @@
 StreamKeySummaryTypeDef = TypedDict(
     "StreamKeySummaryTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListStreamSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamSessionsRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -566,15 +551,14 @@
     "StreamSessionSummaryTypeDef",
     {
         "endTime": datetime,
         "hasErrorEvent": bool,
         "startTime": datetime,
         "streamId": str,
     },
-    total=False,
 )
 
 StreamFiltersTypeDef = TypedDict(
     "StreamFiltersTypeDef",
     {
         "health": StreamHealthType,
     },
@@ -587,15 +571,14 @@
         "channelArn": str,
         "health": StreamHealthType,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
@@ -611,26 +594,24 @@
 
 RenditionConfigurationOutputTypeDef = TypedDict(
     "RenditionConfigurationOutputTypeDef",
     {
         "renditionSelection": RenditionConfigurationRenditionSelectionType,
         "renditions": List[RenditionConfigurationRenditionType],
     },
-    total=False,
 )
 
 ThumbnailConfigurationOutputTypeDef = TypedDict(
     "ThumbnailConfigurationOutputTypeDef",
     {
         "recordingMode": RecordingModeType,
         "resolution": ThumbnailConfigurationResolutionType,
         "storage": List[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
-    total=False,
 )
 
 _RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
@@ -660,15 +641,14 @@
 StreamEventTypeDef = TypedDict(
     "StreamEventTypeDef",
     {
         "eventTime": datetime,
         "name": str,
         "type": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -802,14 +782,21 @@
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "s3": S3DestinationConfigurationOutputTypeDef,
+    },
+)
+
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
@@ -840,15 +827,14 @@
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
-    total=False,
 )
 
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "filterByName": str,
         "filterByRecordingConfigurationArn": str,
@@ -944,88 +930,60 @@
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RenditionConfigurationUnionTypeDef = Union[
-    RenditionConfigurationTypeDef, RenditionConfigurationOutputTypeDef
-]
-ThumbnailConfigurationUnionTypeDef = Union[
-    ThumbnailConfigurationTypeDef, ThumbnailConfigurationOutputTypeDef
-]
-_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
+RecordingConfigurationSummaryTypeDef = TypedDict(
+    "RecordingConfigurationSummaryTypeDef",
     {
+        "arn": str,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
-        "recordingReconnectWindowSeconds": int,
-        "renditionConfiguration": RenditionConfigurationTypeDef,
-        "tags": Mapping[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
+        "state": RecordingConfigurationStateType,
+        "tags": Dict[str, str],
     },
-    total=False,
 )
 
-class CreateRecordingConfigurationRequestRequestTypeDef(
-    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
-    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationSummaryTypeDef",
+RecordingConfigurationTypeDef = TypedDict(
+    "RecordingConfigurationTypeDef",
     {
         "arn": str,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationSummaryTypeDef",
-    {
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
+        "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-class RecordingConfigurationSummaryTypeDef(
-    _RequiredRecordingConfigurationSummaryTypeDef, _OptionalRecordingConfigurationSummaryTypeDef
-):
-    pass
-
-_RequiredRecordingConfigurationTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationTypeDef",
+_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
     },
 )
-_OptionalRecordingConfigurationTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationTypeDef",
+_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
-        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
-        "tags": Dict[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
+        "renditionConfiguration": RenditionConfigurationTypeDef,
+        "tags": Mapping[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
-class RecordingConfigurationTypeDef(
-    _RequiredRecordingConfigurationTypeDef, _OptionalRecordingConfigurationTypeDef
+class CreateRecordingConfigurationRequestRequestTypeDef(
+    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
+    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
@@ -1057,15 +1015,14 @@
         "endTime": datetime,
         "ingestConfiguration": IngestConfigurationTypeDef,
         "recordingConfiguration": RecordingConfigurationTypeDef,
         "startTime": datetime,
         "streamId": str,
         "truncatedEvents": List[StreamEventTypeDef],
     },
-    total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs.egg-info/PKG-INFO` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.28.16
-Summary: Type annotations for boto3.IVS 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.4
+Summary: Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ivs type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 ivs type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -337,20 +337,20 @@
 )
 
 
 def check_value(value: ChannelLatencyModeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_ivs.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
@@ -364,14 +364,15 @@
     RenditionConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
@@ -408,14 +409,15 @@
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
@@ -423,28 +425,26 @@
     ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
-    RenditionConfigurationUnionTypeDef,
-    ThumbnailConfigurationUnionTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
     RecordingConfigurationSummaryTypeDef,
     RecordingConfigurationTypeDef,
+    CreateRecordingConfigurationRequestRequestTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     GetRecordingConfigurationResponseTypeDef,
     StreamSessionTypeDef,
     GetStreamSessionResponseTypeDef,
 )
 
 
-def get_value() -> AudioConfigurationTypeDef:
+def get_structure() -> AudioConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ivs-1.28.16/mypy_boto3_ivs.egg-info/SOURCES.txt` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.16/setup.py` & `mypy-boto3-ivs-1.28.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs",
-    version="1.28.16",
+    version="1.28.4",
     packages=["mypy_boto3_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IVS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -33,15 +33,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 ivs type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 ivs type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ivs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

