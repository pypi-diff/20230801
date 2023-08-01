# Comparing `tmp/mypy-boto3-medialive-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-medialive-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medialive-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:38 2023, max compression
+gzip compressed data, was "mypy-boto3-medialive-1.28.16.tar", last modified: Tue Aug  1 11:37:19 2023, max compression
```

## Comparing `mypy-boto3-medialive-1.28.15.post1.tar` & `mypy-boto3-medialive-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:38.613275 mypy-boto3-medialive-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-07-29 10:03:38.609275 mypy-boto3-medialive-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37373 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:38.605275 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53424 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53334 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39584 2023-07-29 09:51:05.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   173017 2023-07-29 09:51:09.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   172840 2023-07-29 09:51:07.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:38.609275 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:38.613275 mypy-boto3-medialive-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:51:00.000000 mypy-boto3-medialive-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    38965 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37473 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52988 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39584 2023-08-01 11:24:00.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   173232 2023-08-01 11:24:07.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173055 2023-08-01 11:24:02.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38965 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/setup.py
```

### Comparing `mypy-boto3-medialive-1.28.15.post1/LICENSE` & `mypy-boto3-medialive-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/PKG-INFO` & `mypy-boto3-medialive-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaLive 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 medialive type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 medialive type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
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
@@ -665,20 +665,20 @@
 )
 
 
 def check_value(value: AacCodingModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_medialive.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_medialive.type_defs import (
     AacSettingsTypeDef,
     Ac3SettingsTypeDef,
     AcceptInputDeviceTransferRequestRequestTypeDef,
     AccountConfigurationTypeDef,
@@ -989,15 +989,15 @@
     DescribeMultiplexResponseTypeDef,
     MultiplexTypeDef,
     StartMultiplexResponseTypeDef,
     StopMultiplexResponseTypeDef,
     ListMultiplexesResponseTypeDef,
     MultiplexProgramSettingsTypeDef,
     AudioWatermarkSettingsTypeDef,
-    UpdateChannelClassRequestRequestTypeDef,
+    OutputDestinationUnionTypeDef,
     Scte35DescriptorSettingsTypeDef,
     DescribeThumbnailsResponseTypeDef,
     VideoSelectorTypeDef,
     CaptionDescriptionOutputTypeDef,
     CaptionDescriptionTypeDef,
     HlsGroupSettingsOutputTypeDef,
     HlsGroupSettingsTypeDef,
@@ -1021,14 +1021,15 @@
     CreateMultiplexProgramRequestRequestTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     MultiplexProgramTypeDef,
     UpdateMultiplexProgramRequestRequestTypeDef,
     AudioDescriptionOutputTypeDef,
     AudioDescriptionTypeDef,
+    UpdateChannelClassRequestRequestTypeDef,
     Scte35DescriptorTypeDef,
     OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
     InputSettingsOutputTypeDef,
     InputSettingsTypeDef,
     VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
@@ -1039,14 +1040,15 @@
     Scte35TimeSignalScheduleActionSettingsTypeDef,
     InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     OutputTypeDef,
     ScheduleActionSettingsOutputTypeDef,
     ScheduleActionSettingsTypeDef,
     ChannelSummaryTypeDef,
+    InputAttachmentUnionTypeDef,
     OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
     ScheduleActionOutputTypeDef,
     ScheduleActionTypeDef,
     ListChannelsResponseTypeDef,
     EncoderSettingsOutputTypeDef,
     EncoderSettingsTypeDef,
@@ -1056,24 +1058,25 @@
     BatchScheduleActionCreateRequestTypeDef,
     ChannelTypeDef,
     DeleteChannelResponseTypeDef,
     DescribeChannelResponseTypeDef,
     StartChannelResponseTypeDef,
     StopChannelResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
+    EncoderSettingsUnionTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchUpdateScheduleResponseTypeDef,
     BatchUpdateScheduleRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_value() -> AacSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medialive-1.28.15.post1/README.md` & `mypy-boto3-medialive-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
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
@@ -633,20 +633,20 @@
 )
 
 
 def check_value(value: AacCodingModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_medialive.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_medialive.type_defs import (
     AacSettingsTypeDef,
     Ac3SettingsTypeDef,
     AcceptInputDeviceTransferRequestRequestTypeDef,
     AccountConfigurationTypeDef,
@@ -957,15 +957,15 @@
     DescribeMultiplexResponseTypeDef,
     MultiplexTypeDef,
     StartMultiplexResponseTypeDef,
     StopMultiplexResponseTypeDef,
     ListMultiplexesResponseTypeDef,
     MultiplexProgramSettingsTypeDef,
     AudioWatermarkSettingsTypeDef,
-    UpdateChannelClassRequestRequestTypeDef,
+    OutputDestinationUnionTypeDef,
     Scte35DescriptorSettingsTypeDef,
     DescribeThumbnailsResponseTypeDef,
     VideoSelectorTypeDef,
     CaptionDescriptionOutputTypeDef,
     CaptionDescriptionTypeDef,
     HlsGroupSettingsOutputTypeDef,
     HlsGroupSettingsTypeDef,
@@ -989,14 +989,15 @@
     CreateMultiplexProgramRequestRequestTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     MultiplexProgramTypeDef,
     UpdateMultiplexProgramRequestRequestTypeDef,
     AudioDescriptionOutputTypeDef,
     AudioDescriptionTypeDef,
+    UpdateChannelClassRequestRequestTypeDef,
     Scte35DescriptorTypeDef,
     OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
     InputSettingsOutputTypeDef,
     InputSettingsTypeDef,
     VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
@@ -1007,14 +1008,15 @@
     Scte35TimeSignalScheduleActionSettingsTypeDef,
     InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     OutputTypeDef,
     ScheduleActionSettingsOutputTypeDef,
     ScheduleActionSettingsTypeDef,
     ChannelSummaryTypeDef,
+    InputAttachmentUnionTypeDef,
     OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
     ScheduleActionOutputTypeDef,
     ScheduleActionTypeDef,
     ListChannelsResponseTypeDef,
     EncoderSettingsOutputTypeDef,
     EncoderSettingsTypeDef,
@@ -1024,24 +1026,25 @@
     BatchScheduleActionCreateRequestTypeDef,
     ChannelTypeDef,
     DeleteChannelResponseTypeDef,
     DescribeChannelResponseTypeDef,
     StartChannelResponseTypeDef,
     StopChannelResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
+    EncoderSettingsUnionTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchUpdateScheduleResponseTypeDef,
     BatchUpdateScheduleRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_value() -> AacSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__init__.py` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__init__.pyi` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__main__.py` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaLive 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MediaLive 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\nOther"
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

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/client.py` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_medialive.client import MediaLiveClient
 
     session = Session()
     client: MediaLiveClient = session.client("medialive")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ChannelClassType, InputTypeType, LogLevelType, RebootInputDeviceForceType
 from .paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
@@ -59,18 +59,16 @@
     DescribeMultiplexProgramResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
     DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EncoderSettingsOutputTypeDef,
-    EncoderSettingsTypeDef,
-    InputAttachmentOutputTypeDef,
-    InputAttachmentTypeDef,
+    EncoderSettingsUnionTypeDef,
+    InputAttachmentUnionTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
     InputVpcRequestTypeDef,
@@ -86,16 +84,15 @@
     ListReservationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
-    OutputDestinationOutputTypeDef,
-    OutputDestinationTypeDef,
+    OutputDestinationUnionTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     StartChannelResponseTypeDef,
     StartMultiplexResponseTypeDef,
     StopChannelResponseTypeDef,
     StopMultiplexResponseTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
@@ -264,21 +261,17 @@
         """
 
     def create_channel(
         self,
         *,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
         ChannelClass: ChannelClassType = ...,
-        Destinations: Sequence[
-            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
-        ] = ...,
-        EncoderSettings: Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef] = ...,
-        InputAttachments: Sequence[
-            Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
-        ] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
+        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
@@ -812,21 +805,17 @@
         """
 
     def update_channel(
         self,
         *,
         ChannelId: str,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
-        Destinations: Sequence[
-            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
-        ] = ...,
-        EncoderSettings: Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef] = ...,
-        InputAttachments: Sequence[
-            Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
-        ] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
+        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
         RoleArn: str = ...
     ) -> UpdateChannelResponseTypeDef:
         """
@@ -837,17 +826,15 @@
         """
 
     def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[
-            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
-        ] = ...
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel_class)
         """
```

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/client.pyi` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_medialive.client import MediaLiveClient
 
     session = Session()
     client: MediaLiveClient = session.client("medialive")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ChannelClassType, InputTypeType, LogLevelType, RebootInputDeviceForceType
 from .paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
@@ -59,18 +59,16 @@
     DescribeMultiplexProgramResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
     DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EncoderSettingsOutputTypeDef,
-    EncoderSettingsTypeDef,
-    InputAttachmentOutputTypeDef,
-    InputAttachmentTypeDef,
+    EncoderSettingsUnionTypeDef,
+    InputAttachmentUnionTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
     InputVpcRequestTypeDef,
@@ -86,16 +84,15 @@
     ListReservationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
-    OutputDestinationOutputTypeDef,
-    OutputDestinationTypeDef,
+    OutputDestinationUnionTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     StartChannelResponseTypeDef,
     StartMultiplexResponseTypeDef,
     StopChannelResponseTypeDef,
     StopMultiplexResponseTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
@@ -250,21 +247,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#close)
         """
     def create_channel(
         self,
         *,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
         ChannelClass: ChannelClassType = ...,
-        Destinations: Sequence[
-            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
-        ] = ...,
-        EncoderSettings: Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef] = ...,
-        InputAttachments: Sequence[
-            Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
-        ] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
+        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
@@ -750,21 +743,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_account_configuration)
         """
     def update_channel(
         self,
         *,
         ChannelId: str,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
-        Destinations: Sequence[
-            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
-        ] = ...,
-        EncoderSettings: Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef] = ...,
-        InputAttachments: Sequence[
-            Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
-        ] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
+        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
         RoleArn: str = ...
     ) -> UpdateChannelResponseTypeDef:
         """
@@ -774,17 +763,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel)
         """
     def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[
-            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
-        ] = ...
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel_class)
         """
```

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/literals.py` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/literals.pyi` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/paginator.py` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/paginator.pyi` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/type_defs.py` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_medialive.type_defs import AacSettingsTypeDef
 
-    data: AacSettingsTypeDef = {...}
+    data: AacSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -602,15 +602,15 @@
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
     "MultiplexProgramSettingsTypeDef",
     "AudioWatermarkSettingsTypeDef",
-    "UpdateChannelClassRequestRequestTypeDef",
+    "OutputDestinationUnionTypeDef",
     "Scte35DescriptorSettingsTypeDef",
     "DescribeThumbnailsResponseTypeDef",
     "VideoSelectorTypeDef",
     "CaptionDescriptionOutputTypeDef",
     "CaptionDescriptionTypeDef",
     "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
@@ -634,14 +634,15 @@
     "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
     "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
+    "UpdateChannelClassRequestRequestTypeDef",
     "Scte35DescriptorTypeDef",
     "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
     "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
     "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
@@ -652,14 +653,15 @@
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
     "ScheduleActionSettingsOutputTypeDef",
     "ScheduleActionSettingsTypeDef",
     "ChannelSummaryTypeDef",
+    "InputAttachmentUnionTypeDef",
     "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
     "ScheduleActionOutputTypeDef",
     "ScheduleActionTypeDef",
     "ListChannelsResponseTypeDef",
     "EncoderSettingsOutputTypeDef",
     "EncoderSettingsTypeDef",
@@ -669,14 +671,15 @@
     "BatchScheduleActionCreateRequestTypeDef",
     "ChannelTypeDef",
     "DeleteChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "StartChannelResponseTypeDef",
     "StopChannelResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "EncoderSettingsUnionTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchUpdateScheduleResponseTypeDef",
     "BatchUpdateScheduleRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
@@ -4906,37 +4909,15 @@
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NielsenWatermarksSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateChannelClassRequestRequestTypeDef",
-    {
-        "ChannelClass": ChannelClassType,
-        "ChannelId": str,
-    },
-)
-_OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateChannelClassRequestRequestTypeDef",
-    {
-        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
-    },
-    total=False,
-)
-
-
-class UpdateChannelClassRequestRequestTypeDef(
-    _RequiredUpdateChannelClassRequestRequestTypeDef,
-    _OptionalUpdateChannelClassRequestRequestTypeDef,
-):
-    pass
-
-
+OutputDestinationUnionTypeDef = Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 
@@ -5522,14 +5503,37 @@
 )
 
 
 class AudioDescriptionTypeDef(_RequiredAudioDescriptionTypeDef, _OptionalAudioDescriptionTypeDef):
     pass
 
 
+_RequiredUpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateChannelClassRequestRequestTypeDef",
+    {
+        "ChannelClass": ChannelClassType,
+        "ChannelId": str,
+    },
+)
+_OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateChannelClassRequestRequestTypeDef",
+    {
+        "Destinations": Sequence[OutputDestinationUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateChannelClassRequestRequestTypeDef(
+    _RequiredUpdateChannelClassRequestRequestTypeDef,
+    _OptionalUpdateChannelClassRequestRequestTypeDef,
+):
+    pass
+
+
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
 
@@ -5797,14 +5801,15 @@
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
+InputAttachmentUnionTypeDef = Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
 _RequiredOutputGroupOutputTypeDef = TypedDict(
     "_RequiredOutputGroupOutputTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
         "Outputs": List[OutputTypeDef],
     },
 )
@@ -6088,43 +6093,44 @@
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
+        "Destinations": Sequence[OutputDestinationUnionTypeDef],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]],
+        "InputAttachments": Sequence[InputAttachmentUnionTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceCreateSettingsTypeDef,
         "Name": str,
         "RequestId": str,
         "Reserved": str,
         "RoleArn": str,
         "Tags": Mapping[str, str],
         "Vpc": VpcOutputSettingsTypeDef,
     },
     total=False,
 )
 
+EncoderSettingsUnionTypeDef = Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef]
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
+        "Destinations": Sequence[OutputDestinationUnionTypeDef],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]],
+        "InputAttachments": Sequence[InputAttachmentUnionTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceUpdateSettingsTypeDef,
         "Name": str,
         "RoleArn": str,
     },
     total=False,
```

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/type_defs.pyi` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_medialive.type_defs import AacSettingsTypeDef
 
-    data: AacSettingsTypeDef = {...}
+    data: AacSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -601,15 +601,15 @@
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
     "MultiplexProgramSettingsTypeDef",
     "AudioWatermarkSettingsTypeDef",
-    "UpdateChannelClassRequestRequestTypeDef",
+    "OutputDestinationUnionTypeDef",
     "Scte35DescriptorSettingsTypeDef",
     "DescribeThumbnailsResponseTypeDef",
     "VideoSelectorTypeDef",
     "CaptionDescriptionOutputTypeDef",
     "CaptionDescriptionTypeDef",
     "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
@@ -633,14 +633,15 @@
     "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
     "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
+    "UpdateChannelClassRequestRequestTypeDef",
     "Scte35DescriptorTypeDef",
     "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
     "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
     "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
@@ -651,14 +652,15 @@
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
     "ScheduleActionSettingsOutputTypeDef",
     "ScheduleActionSettingsTypeDef",
     "ChannelSummaryTypeDef",
+    "InputAttachmentUnionTypeDef",
     "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
     "ScheduleActionOutputTypeDef",
     "ScheduleActionTypeDef",
     "ListChannelsResponseTypeDef",
     "EncoderSettingsOutputTypeDef",
     "EncoderSettingsTypeDef",
@@ -668,14 +670,15 @@
     "BatchScheduleActionCreateRequestTypeDef",
     "ChannelTypeDef",
     "DeleteChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "StartChannelResponseTypeDef",
     "StopChannelResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "EncoderSettingsUnionTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchUpdateScheduleResponseTypeDef",
     "BatchUpdateScheduleRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
@@ -4781,35 +4784,15 @@
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NielsenWatermarksSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateChannelClassRequestRequestTypeDef",
-    {
-        "ChannelClass": ChannelClassType,
-        "ChannelId": str,
-    },
-)
-_OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateChannelClassRequestRequestTypeDef",
-    {
-        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
-    },
-    total=False,
-)
-
-class UpdateChannelClassRequestRequestTypeDef(
-    _RequiredUpdateChannelClassRequestRequestTypeDef,
-    _OptionalUpdateChannelClassRequestRequestTypeDef,
-):
-    pass
-
+OutputDestinationUnionTypeDef = Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 
@@ -5363,14 +5346,35 @@
     },
     total=False,
 )
 
 class AudioDescriptionTypeDef(_RequiredAudioDescriptionTypeDef, _OptionalAudioDescriptionTypeDef):
     pass
 
+_RequiredUpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateChannelClassRequestRequestTypeDef",
+    {
+        "ChannelClass": ChannelClassType,
+        "ChannelId": str,
+    },
+)
+_OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateChannelClassRequestRequestTypeDef",
+    {
+        "Destinations": Sequence[OutputDestinationUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateChannelClassRequestRequestTypeDef(
+    _RequiredUpdateChannelClassRequestRequestTypeDef,
+    _OptionalUpdateChannelClassRequestRequestTypeDef,
+):
+    pass
+
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
 
@@ -5632,14 +5636,15 @@
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
+InputAttachmentUnionTypeDef = Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
 _RequiredOutputGroupOutputTypeDef = TypedDict(
     "_RequiredOutputGroupOutputTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
         "Outputs": List[OutputTypeDef],
     },
 )
@@ -5915,43 +5920,44 @@
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
+        "Destinations": Sequence[OutputDestinationUnionTypeDef],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]],
+        "InputAttachments": Sequence[InputAttachmentUnionTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceCreateSettingsTypeDef,
         "Name": str,
         "RequestId": str,
         "Reserved": str,
         "RoleArn": str,
         "Tags": Mapping[str, str],
         "Vpc": VpcOutputSettingsTypeDef,
     },
     total=False,
 )
 
+EncoderSettingsUnionTypeDef = Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef]
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
+        "Destinations": Sequence[OutputDestinationUnionTypeDef],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]],
+        "InputAttachments": Sequence[InputAttachmentUnionTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceUpdateSettingsTypeDef,
         "Name": str,
         "RoleArn": str,
     },
     total=False,
```

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/waiter.py` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/waiter.pyi` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/PKG-INFO` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaLive 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 medialive type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 medialive type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
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
@@ -665,20 +665,20 @@
 )
 
 
 def check_value(value: AacCodingModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_medialive.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_medialive.type_defs import (
     AacSettingsTypeDef,
     Ac3SettingsTypeDef,
     AcceptInputDeviceTransferRequestRequestTypeDef,
     AccountConfigurationTypeDef,
@@ -989,15 +989,15 @@
     DescribeMultiplexResponseTypeDef,
     MultiplexTypeDef,
     StartMultiplexResponseTypeDef,
     StopMultiplexResponseTypeDef,
     ListMultiplexesResponseTypeDef,
     MultiplexProgramSettingsTypeDef,
     AudioWatermarkSettingsTypeDef,
-    UpdateChannelClassRequestRequestTypeDef,
+    OutputDestinationUnionTypeDef,
     Scte35DescriptorSettingsTypeDef,
     DescribeThumbnailsResponseTypeDef,
     VideoSelectorTypeDef,
     CaptionDescriptionOutputTypeDef,
     CaptionDescriptionTypeDef,
     HlsGroupSettingsOutputTypeDef,
     HlsGroupSettingsTypeDef,
@@ -1021,14 +1021,15 @@
     CreateMultiplexProgramRequestRequestTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     MultiplexProgramTypeDef,
     UpdateMultiplexProgramRequestRequestTypeDef,
     AudioDescriptionOutputTypeDef,
     AudioDescriptionTypeDef,
+    UpdateChannelClassRequestRequestTypeDef,
     Scte35DescriptorTypeDef,
     OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
     InputSettingsOutputTypeDef,
     InputSettingsTypeDef,
     VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
@@ -1039,14 +1040,15 @@
     Scte35TimeSignalScheduleActionSettingsTypeDef,
     InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     OutputTypeDef,
     ScheduleActionSettingsOutputTypeDef,
     ScheduleActionSettingsTypeDef,
     ChannelSummaryTypeDef,
+    InputAttachmentUnionTypeDef,
     OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
     ScheduleActionOutputTypeDef,
     ScheduleActionTypeDef,
     ListChannelsResponseTypeDef,
     EncoderSettingsOutputTypeDef,
     EncoderSettingsTypeDef,
@@ -1056,24 +1058,25 @@
     BatchScheduleActionCreateRequestTypeDef,
     ChannelTypeDef,
     DeleteChannelResponseTypeDef,
     DescribeChannelResponseTypeDef,
     StartChannelResponseTypeDef,
     StopChannelResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
+    EncoderSettingsUnionTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchUpdateScheduleResponseTypeDef,
     BatchUpdateScheduleRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_value() -> AacSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/SOURCES.txt` & `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15.post1/setup.py` & `mypy-boto3-medialive-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medialive",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.MediaLive 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 medialive type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 medialive type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_medialive": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

