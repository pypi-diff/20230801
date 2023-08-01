# Comparing `tmp/mypy-boto3-kinesisvideo-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-kinesisvideo-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:29 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.16.tar", last modified: Tue Aug  1 11:37:09 2023, max compression
```

## Comparing `mypy-boto3-kinesisvideo-1.28.15.post1.tar` & `mypy-boto3-kinesisvideo-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:29.917229 mypy-boto3-kinesisvideo-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-29 10:03:29.917229 mypy-boto3-kinesisvideo-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15701 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:29.913229 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25063 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29470 2023-07-29 09:49:00.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-07-29 09:49:00.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:29.917229 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:29.917229 mypy-boto3-kinesisvideo-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24947 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-08-01 11:21:50.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/setup.py
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/LICENSE` & `mypy-boto3-kinesisvideo-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/PKG-INFO` & `mypy-boto3-kinesisvideo-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisVideo 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesisvideo type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesisvideo type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisvideo)](https://pepy.tech/project/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
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
@@ -344,20 +344,20 @@
 )
 
 
 def check_value(value: APINameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesisvideo.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
     SingleMasterConfigurationTypeDef,
     ChannelNameConditionTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
@@ -423,27 +423,28 @@
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     ListEdgeAgentConfigurationsEdgeConfigTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationTypeDef:
+def get_value() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/README.md` & `mypy-boto3-kinesisvideo-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisvideo)](https://pepy.tech/project/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
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
@@ -312,20 +312,20 @@
 )
 
 
 def check_value(value: APINameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesisvideo.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
     SingleMasterConfigurationTypeDef,
     ChannelNameConditionTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
@@ -391,27 +391,28 @@
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     ListEdgeAgentConfigurationsEdgeConfigTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationTypeDef:
+def get_value() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__init__.py` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__init__.pyi` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__main__.py` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideo 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.KinesisVideo 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
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

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/client.py` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_kinesisvideo.client import KinesisVideoClient
 
     session = Session()
     client: KinesisVideoClient = session.client("kinesisvideo")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
     ListEdgeAgentConfigurationsPaginator,
@@ -35,16 +35,15 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationOutputTypeDef,
-    ImageGenerationConfigurationTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
@@ -423,17 +422,15 @@
         """
 
     def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: Union[
-            ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
-        ] = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/client.pyi` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_kinesisvideo.client import KinesisVideoClient
 
     session = Session()
     client: KinesisVideoClient = session.client("kinesisvideo")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
     ListEdgeAgentConfigurationsPaginator,
@@ -35,16 +35,15 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationOutputTypeDef,
-    ImageGenerationConfigurationTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
@@ -390,17 +389,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_data_retention)
         """
     def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: Union[
-            ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
-        ] = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/literals.py` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/literals.pyi` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/paginator.py` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/paginator.pyi` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/type_defs.py` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
-    data: SingleMasterConfigurationTypeDef = {...}
+    data: SingleMasterConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
@@ -110,14 +110,15 @@
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
+    "ImageGenerationConfigurationUnionTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
@@ -1006,14 +1007,17 @@
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
         "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImageGenerationConfigurationUnionTypeDef = Union[
+    ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
+]
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
     },
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/type_defs.pyi` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
-    data: SingleMasterConfigurationTypeDef = {...}
+    data: SingleMasterConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
@@ -109,14 +109,15 @@
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
+    "ImageGenerationConfigurationUnionTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
@@ -969,14 +970,17 @@
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
         "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImageGenerationConfigurationUnionTypeDef = Union[
+    ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
+]
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
     },
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/PKG-INFO` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisVideo 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesisvideo type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesisvideo type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisvideo)](https://pepy.tech/project/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
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
@@ -344,20 +344,20 @@
 )
 
 
 def check_value(value: APINameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesisvideo.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
     SingleMasterConfigurationTypeDef,
     ChannelNameConditionTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
@@ -423,27 +423,28 @@
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     ListEdgeAgentConfigurationsEdgeConfigTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationTypeDef:
+def get_value() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt` & `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15.post1/setup.py` & `mypy-boto3-kinesisvideo-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisvideo",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.KinesisVideo 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 kinesisvideo type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 kinesisvideo type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_kinesisvideo": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

