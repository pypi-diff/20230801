# Comparing `tmp/mypy-boto3-kinesis-video-signaling-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-kinesis-video-signaling-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-video-signaling-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:27 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-video-signaling-1.28.16.tar", last modified: Tue Aug  1 11:37:07 2023, max compression
```

## Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1.tar` & `mypy-boto3-kinesis-video-signaling-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:27.361219 mypy-boto3-kinesis-video-signaling-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-07-29 10:03:27.361219 mypy-boto3-kinesis-video-signaling-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:27.349219 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:27.357219 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-07-29 10:03:27.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-29 10:03:27.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:27.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:27.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:27.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 10:03:27.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:27.361219 mypy-boto3-kinesis-video-signaling-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-29 09:48:51.000000 mypy-boto3-kinesis-video-signaling-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:07.164851 mypy-boto3-kinesis-video-signaling-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12901 2023-08-01 11:37:07.156851 mypy-boto3-kinesis-video-signaling-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:07.156851 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:07.156851 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12901 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:07.164851 mypy-boto3-kinesis-video-signaling-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-01 11:21:38.000000 mypy-boto3-kinesis-video-signaling-1.28.16/setup.py
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/LICENSE` & `mypy-boto3-kinesis-video-signaling-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/PKG-INFO` & `mypy-boto3-kinesis-video-signaling-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-signaling
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisVideoSignalingChannels 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisVideoSignalingChannels 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesis-video-signaling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesis-video-signaling type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-signaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-signaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-signaling)](https://pepy.tech/project/mypy-boto3-kinesis-video-signaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoSignalingChannels 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
+[boto3.KinesisVideoSignalingChannels 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
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
 [mypy-boto3-kinesis-video-signaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/).
 
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
@@ -289,33 +289,33 @@
 )
 
 
 def check_value(value: ServiceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesis_video_signaling.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesis_video_signaling.type_defs import (
     GetIceServerConfigRequestRequestTypeDef,
     IceServerTypeDef,
     ResponseMetadataTypeDef,
     SendAlexaOfferToMasterRequestRequestTypeDef,
     GetIceServerConfigResponseTypeDef,
     SendAlexaOfferToMasterResponseTypeDef,
 )
 
 
-def get_structure() -> GetIceServerConfigRequestRequestTypeDef:
+def get_value() -> GetIceServerConfigRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/README.md` & `mypy-boto3-kinesis-video-signaling-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-signaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-signaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-signaling)](https://pepy.tech/project/mypy-boto3-kinesis-video-signaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoSignalingChannels 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
+[boto3.KinesisVideoSignalingChannels 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
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
 [mypy-boto3-kinesis-video-signaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/).
 
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
@@ -257,33 +257,33 @@
 )
 
 
 def check_value(value: ServiceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesis_video_signaling.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesis_video_signaling.type_defs import (
     GetIceServerConfigRequestRequestTypeDef,
     IceServerTypeDef,
     ResponseMetadataTypeDef,
     SendAlexaOfferToMasterRequestRequestTypeDef,
     GetIceServerConfigResponseTypeDef,
     SendAlexaOfferToMasterResponseTypeDef,
 )
 
 
-def get_structure() -> GetIceServerConfigRequestRequestTypeDef:
+def get_value() -> GetIceServerConfigRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/__init__.py` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/__init__.pyi` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/__main__.py` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideoSignalingChannels 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.KinesisVideoSignalingChannels 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels\nOther"
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

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/client.py` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/client.pyi` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/literals.py` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/literals.pyi` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/type_defs.py` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesis_video_signaling.type_defs import GetIceServerConfigRequestRequestTypeDef
 
-    data: GetIceServerConfigRequestRequestTypeDef = {...}
+    data: GetIceServerConfigRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
     from typing import Literal
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling/type_defs.pyi` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kinesis_video_signaling.type_defs import GetIceServerConfigRequestRequestTypeDef
 
-    data: GetIceServerConfigRequestRequestTypeDef = {...}
+    data: GetIceServerConfigRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
     from typing import Literal
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling.egg-info/PKG-INFO` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-signaling
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisVideoSignalingChannels 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisVideoSignalingChannels 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesis-video-signaling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesis-video-signaling type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-signaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-signaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-signaling)](https://pepy.tech/project/mypy-boto3-kinesis-video-signaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoSignalingChannels 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
+[boto3.KinesisVideoSignalingChannels 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
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
 [mypy-boto3-kinesis-video-signaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/).
 
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
@@ -289,33 +289,33 @@
 )
 
 
 def check_value(value: ServiceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesis_video_signaling.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kinesis_video_signaling.type_defs import (
     GetIceServerConfigRequestRequestTypeDef,
     IceServerTypeDef,
     ResponseMetadataTypeDef,
     SendAlexaOfferToMasterRequestRequestTypeDef,
     GetIceServerConfigResponseTypeDef,
     SendAlexaOfferToMasterResponseTypeDef,
 )
 
 
-def get_structure() -> GetIceServerConfigRequestRequestTypeDef:
+def get_value() -> GetIceServerConfigRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/mypy_boto3_kinesis_video_signaling.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-video-signaling-1.28.16/mypy_boto3_kinesis_video_signaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.15.post1/setup.py` & `mypy-boto3-kinesis-video-signaling-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis-video-signaling",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_kinesis_video_signaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideoSignalingChannels 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.KinesisVideoSignalingChannels 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,17 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords=(
-        "boto3 kinesis-video-signaling type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="boto3 kinesis-video-signaling type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_kinesis_video_signaling": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/"
```

