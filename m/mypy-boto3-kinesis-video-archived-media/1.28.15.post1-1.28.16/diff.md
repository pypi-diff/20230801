# Comparing `tmp/mypy-boto3-kinesis-video-archived-media-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-kinesis-video-archived-media-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-video-archived-media-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:27 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-video-archived-media-1.28.16.tar", last modified: Tue Aug  1 11:37:06 2023, max compression
```

## Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1.tar` & `mypy-boto3-kinesis-video-archived-media-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:27.153218 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-29 10:03:27.153218 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:27.153218 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-29 09:48:50.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-29 09:48:50.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-29 09:48:50.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:27.153218 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 10:03:26.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:27.153218 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-29 09:48:49.000000 mypy-boto3-kinesis-video-archived-media-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-08-01 11:21:37.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-08-01 11:21:37.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/setup.py
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/LICENSE` & `mypy-boto3-kinesis-video-archived-media-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/PKG-INFO` & `mypy-boto3-kinesis-video-archived-media-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-archived-media
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesis-video-archived-media type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesis-video-archived-media type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-archived-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoArchivedMedia 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[boto3.KinesisVideoArchivedMedia 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [mypy-boto3-kinesis-video-archived-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/).
 
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
@@ -331,53 +331,55 @@
 )
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesis_video_archived_media.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_kinesis_video_archived_media.type_defs import (
-    ClipTimestampRangeTypeDef,
-    DASHTimestampRangeTypeDef,
-    TimestampRangeTypeDef,
+    TimestampTypeDef,
     FragmentTypeDef,
     ResponseMetadataTypeDef,
     PaginatorConfigTypeDef,
-    GetImagesInputRequestTypeDef,
     ImageTypeDef,
     GetMediaForFragmentListInputRequestTypeDef,
+    ClipTimestampRangeTypeDef,
+    DASHTimestampRangeTypeDef,
+    GetImagesInputRequestTypeDef,
     HLSTimestampRangeTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
+    TimestampRangeTypeDef,
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
     GetMediaForFragmentListOutputTypeDef,
     ListFragmentsOutputTypeDef,
     GetImagesInputGetImagesPaginateTypeDef,
     GetImagesOutputTypeDef,
+    ClipFragmentSelectorTypeDef,
+    DASHFragmentSelectorTypeDef,
     HLSFragmentSelectorTypeDef,
+    FragmentSelectorTypeDef,
     GetClipInputRequestTypeDef,
     GetDASHStreamingSessionURLInputRequestTypeDef,
+    GetHLSStreamingSessionURLInputRequestTypeDef,
     ListFragmentsInputListFragmentsPaginateTypeDef,
     ListFragmentsInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
 )
 
 
-def get_structure() -> ClipTimestampRangeTypeDef:
+def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/README.md` & `mypy-boto3-kinesis-video-archived-media-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-archived-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoArchivedMedia 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[boto3.KinesisVideoArchivedMedia 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [mypy-boto3-kinesis-video-archived-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/).
 
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
@@ -299,53 +299,55 @@
 )
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesis_video_archived_media.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_kinesis_video_archived_media.type_defs import (
-    ClipTimestampRangeTypeDef,
-    DASHTimestampRangeTypeDef,
-    TimestampRangeTypeDef,
+    TimestampTypeDef,
     FragmentTypeDef,
     ResponseMetadataTypeDef,
     PaginatorConfigTypeDef,
-    GetImagesInputRequestTypeDef,
     ImageTypeDef,
     GetMediaForFragmentListInputRequestTypeDef,
+    ClipTimestampRangeTypeDef,
+    DASHTimestampRangeTypeDef,
+    GetImagesInputRequestTypeDef,
     HLSTimestampRangeTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
+    TimestampRangeTypeDef,
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
     GetMediaForFragmentListOutputTypeDef,
     ListFragmentsOutputTypeDef,
     GetImagesInputGetImagesPaginateTypeDef,
     GetImagesOutputTypeDef,
+    ClipFragmentSelectorTypeDef,
+    DASHFragmentSelectorTypeDef,
     HLSFragmentSelectorTypeDef,
+    FragmentSelectorTypeDef,
     GetClipInputRequestTypeDef,
     GetDASHStreamingSessionURLInputRequestTypeDef,
+    GetHLSStreamingSessionURLInputRequestTypeDef,
     ListFragmentsInputListFragmentsPaginateTypeDef,
     ListFragmentsInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
 )
 
 
-def get_structure() -> ClipTimestampRangeTypeDef:
+def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/__init__.py` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/__init__.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/__main__.py` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia\nOther"
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

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/client.py` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_kinesis_video_archived_media.client import KinesisVideoArchivedMediaClient
 
     session = Session()
     client: KinesisVideoArchivedMediaClient = session.client("kinesis-video-archived-media")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ContainerFormatType,
     DASHDisplayFragmentNumberType,
     DASHDisplayFragmentTimestampType,
@@ -38,14 +37,15 @@
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
     GetImagesOutputTypeDef,
     GetMediaForFragmentListOutputTypeDef,
     HLSFragmentSelectorTypeDef,
     ListFragmentsOutputTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -176,16 +176,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/client/#get_hls_streaming_session_url)
         """
 
     def get_images(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
-        StartTimestamp: Union[datetime, str],
-        EndTimestamp: Union[datetime, str],
+        StartTimestamp: TimestampTypeDef,
+        EndTimestamp: TimestampTypeDef,
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/client.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_kinesis_video_archived_media.client import KinesisVideoArchivedMediaClient
 
     session = Session()
     client: KinesisVideoArchivedMediaClient = session.client("kinesis-video-archived-media")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ContainerFormatType,
     DASHDisplayFragmentNumberType,
     DASHDisplayFragmentTimestampType,
@@ -38,14 +37,15 @@
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
     GetImagesOutputTypeDef,
     GetMediaForFragmentListOutputTypeDef,
     HLSFragmentSelectorTypeDef,
     ListFragmentsOutputTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -165,16 +165,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_hls_streaming_session_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/client/#get_hls_streaming_session_url)
         """
     def get_images(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
-        StartTimestamp: Union[datetime, str],
-        EndTimestamp: Union[datetime, str],
+        StartTimestamp: TimestampTypeDef,
+        EndTimestamp: TimestampTypeDef,
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/literals.py` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/literals.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/paginator.py` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -18,73 +18,68 @@
     client: KinesisVideoArchivedMediaClient = session.client("kinesis-video-archived-media")
 
     get_images_paginator: GetImagesPaginator = client.get_paginator("get_images")
     list_fragments_paginator: ListFragmentsPaginator = client.get_paginator("list_fragments")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Mapping, TypeVar, Union
+from typing import Generic, Iterator, Mapping, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import FormatType, ImageSelectorTypeType
 from .type_defs import (
     FragmentSelectorTypeDef,
     GetImagesOutputTypeDef,
     ListFragmentsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GetImagesPaginator", "ListFragmentsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
     """
 
     def paginate(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
-        StartTimestamp: Union[datetime, str],
-        EndTimestamp: Union[datetime, str],
+        StartTimestamp: TimestampTypeDef,
+        EndTimestamp: TimestampTypeDef,
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
-
 class ListFragmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#listfragmentspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/paginator.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/paginator.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,68 +18,73 @@
     client: KinesisVideoArchivedMediaClient = session.client("kinesis-video-archived-media")
 
     get_images_paginator: GetImagesPaginator = client.get_paginator("get_images")
     list_fragments_paginator: ListFragmentsPaginator = client.get_paginator("list_fragments")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Mapping, TypeVar, Union
+from typing import Generic, Iterator, Mapping, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import FormatType, ImageSelectorTypeType
 from .type_defs import (
     FragmentSelectorTypeDef,
     GetImagesOutputTypeDef,
     ListFragmentsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("GetImagesPaginator", "ListFragmentsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
     """
 
     def paginate(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
-        StartTimestamp: Union[datetime, str],
-        EndTimestamp: Union[datetime, str],
+        StartTimestamp: TimestampTypeDef,
+        EndTimestamp: TimestampTypeDef,
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
+
 class ListFragmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#listfragmentspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/type_defs.py` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for kinesis-video-archived-media service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kinesis_video_archived_media.type_defs import ClipTimestampRangeTypeDef
+    from mypy_boto3_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
-    data: ClipTimestampRangeTypeDef = {...}
+    data: TimestampTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,67 +41,44 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ClipTimestampRangeTypeDef",
-    "DASHTimestampRangeTypeDef",
-    "TimestampRangeTypeDef",
+    "TimestampTypeDef",
     "FragmentTypeDef",
     "ResponseMetadataTypeDef",
     "PaginatorConfigTypeDef",
-    "GetImagesInputRequestTypeDef",
     "ImageTypeDef",
     "GetMediaForFragmentListInputRequestTypeDef",
+    "ClipTimestampRangeTypeDef",
+    "DASHTimestampRangeTypeDef",
+    "GetImagesInputRequestTypeDef",
     "HLSTimestampRangeTypeDef",
-    "ClipFragmentSelectorTypeDef",
-    "DASHFragmentSelectorTypeDef",
-    "FragmentSelectorTypeDef",
+    "TimestampRangeTypeDef",
     "GetClipOutputTypeDef",
     "GetDASHStreamingSessionURLOutputTypeDef",
     "GetHLSStreamingSessionURLOutputTypeDef",
     "GetMediaForFragmentListOutputTypeDef",
     "ListFragmentsOutputTypeDef",
     "GetImagesInputGetImagesPaginateTypeDef",
     "GetImagesOutputTypeDef",
+    "ClipFragmentSelectorTypeDef",
+    "DASHFragmentSelectorTypeDef",
     "HLSFragmentSelectorTypeDef",
+    "FragmentSelectorTypeDef",
     "GetClipInputRequestTypeDef",
     "GetDASHStreamingSessionURLInputRequestTypeDef",
+    "GetHLSStreamingSessionURLInputRequestTypeDef",
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     "ListFragmentsInputRequestTypeDef",
-    "GetHLSStreamingSessionURLInputRequestTypeDef",
-)
-
-ClipTimestampRangeTypeDef = TypedDict(
-    "ClipTimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-)
-
-DASHTimestampRangeTypeDef = TypedDict(
-    "DASHTimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
 )
 
+TimestampTypeDef = Union[datetime, str]
 FragmentTypeDef = TypedDict(
     "FragmentTypeDef",
     {
         "FragmentNumber": str,
         "FragmentSizeInBytes": int,
         "ProducerTimestamp": datetime,
         "ServerTimestamp": datetime,
@@ -127,45 +104,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredGetImagesInputRequestTypeDef = TypedDict(
-    "_RequiredGetImagesInputRequestTypeDef",
-    {
-        "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-        "SamplingInterval": int,
-        "Format": FormatType,
-    },
-)
-_OptionalGetImagesInputRequestTypeDef = TypedDict(
-    "_OptionalGetImagesInputRequestTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetImagesInputRequestTypeDef(
-    _RequiredGetImagesInputRequestTypeDef, _OptionalGetImagesInputRequestTypeDef
-):
-    pass
-
-
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "TimeStamp": datetime,
         "Error": ImageErrorType,
         "ImageContent": str,
     },
@@ -191,45 +137,76 @@
 class GetMediaForFragmentListInputRequestTypeDef(
     _RequiredGetMediaForFragmentListInputRequestTypeDef,
     _OptionalGetMediaForFragmentListInputRequestTypeDef,
 ):
     pass
 
 
-HLSTimestampRangeTypeDef = TypedDict(
-    "HLSTimestampRangeTypeDef",
+ClipTimestampRangeTypeDef = TypedDict(
+    "ClipTimestampRangeTypeDef",
     {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+)
+
+DASHTimestampRangeTypeDef = TypedDict(
+    "DASHTimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-ClipFragmentSelectorTypeDef = TypedDict(
-    "ClipFragmentSelectorTypeDef",
+_RequiredGetImagesInputRequestTypeDef = TypedDict(
+    "_RequiredGetImagesInputRequestTypeDef",
     {
-        "FragmentSelectorType": ClipFragmentSelectorTypeType,
-        "TimestampRange": ClipTimestampRangeTypeDef,
+        "ImageSelectorType": ImageSelectorTypeType,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+        "SamplingInterval": int,
+        "Format": FormatType,
+    },
+)
+_OptionalGetImagesInputRequestTypeDef = TypedDict(
+    "_OptionalGetImagesInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+        "MaxResults": int,
+        "NextToken": str,
     },
+    total=False,
 )
 
-DASHFragmentSelectorTypeDef = TypedDict(
-    "DASHFragmentSelectorTypeDef",
+
+class GetImagesInputRequestTypeDef(
+    _RequiredGetImagesInputRequestTypeDef, _OptionalGetImagesInputRequestTypeDef
+):
+    pass
+
+
+HLSTimestampRangeTypeDef = TypedDict(
+    "HLSTimestampRangeTypeDef",
     {
-        "FragmentSelectorType": DASHFragmentSelectorTypeType,
-        "TimestampRange": DASHTimestampRangeTypeDef,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-FragmentSelectorTypeDef = TypedDict(
-    "FragmentSelectorTypeDef",
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
     {
-        "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeTypeDef,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
 )
 
 GetClipOutputTypeDef = TypedDict(
     "GetClipOutputTypeDef",
     {
         "ContentType": str,
@@ -272,16 +249,16 @@
     },
 )
 
 _RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
     "_RequiredGetImagesInputGetImagesPaginateTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
     "_OptionalGetImagesInputGetImagesPaginateTypeDef",
     {
@@ -307,23 +284,48 @@
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ClipFragmentSelectorTypeDef = TypedDict(
+    "ClipFragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": ClipFragmentSelectorTypeType,
+        "TimestampRange": ClipTimestampRangeTypeDef,
+    },
+)
+
+DASHFragmentSelectorTypeDef = TypedDict(
+    "DASHFragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": DASHFragmentSelectorTypeType,
+        "TimestampRange": DASHTimestampRangeTypeDef,
+    },
+    total=False,
+)
+
 HLSFragmentSelectorTypeDef = TypedDict(
     "HLSFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": HLSFragmentSelectorTypeType,
         "TimestampRange": HLSTimestampRangeTypeDef,
     },
     total=False,
 )
 
+FragmentSelectorTypeDef = TypedDict(
+    "FragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeTypeDef,
+    },
+)
+
 _RequiredGetClipInputRequestTypeDef = TypedDict(
     "_RequiredGetClipInputRequestTypeDef",
     {
         "ClipFragmentSelector": ClipFragmentSelectorTypeDef,
     },
 )
 _OptionalGetClipInputRequestTypeDef = TypedDict(
@@ -353,14 +355,30 @@
         "DASHFragmentSelector": DASHFragmentSelectorTypeDef,
         "Expires": int,
         "MaxManifestFragmentResults": int,
     },
     total=False,
 )
 
+GetHLSStreamingSessionURLInputRequestTypeDef = TypedDict(
+    "GetHLSStreamingSessionURLInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "PlaybackMode": HLSPlaybackModeType,
+        "HLSFragmentSelector": HLSFragmentSelectorTypeDef,
+        "ContainerFormat": ContainerFormatType,
+        "DiscontinuityMode": HLSDiscontinuityModeType,
+        "DisplayFragmentTimestamp": HLSDisplayFragmentTimestampType,
+        "Expires": int,
+        "MaxMediaPlaylistFragmentResults": int,
+    },
+    total=False,
+)
+
 ListFragmentsInputListFragmentsPaginateTypeDef = TypedDict(
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "FragmentSelector": FragmentSelectorTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -375,23 +393,7 @@
         "StreamARN": str,
         "MaxResults": int,
         "NextToken": str,
         "FragmentSelector": FragmentSelectorTypeDef,
     },
     total=False,
 )
-
-GetHLSStreamingSessionURLInputRequestTypeDef = TypedDict(
-    "GetHLSStreamingSessionURLInputRequestTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "PlaybackMode": HLSPlaybackModeType,
-        "HLSFragmentSelector": HLSFragmentSelectorTypeDef,
-        "ContainerFormat": ContainerFormatType,
-        "DiscontinuityMode": HLSDiscontinuityModeType,
-        "DisplayFragmentTimestamp": HLSDisplayFragmentTimestampType,
-        "Expires": int,
-        "MaxMediaPlaylistFragmentResults": int,
-    },
-    total=False,
-)
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media/type_defs.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for kinesis-video-archived-media service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kinesis_video_archived_media.type_defs import ClipTimestampRangeTypeDef
+    from mypy_boto3_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
-    data: ClipTimestampRangeTypeDef = {...}
+    data: TimestampTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -40,67 +40,44 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ClipTimestampRangeTypeDef",
-    "DASHTimestampRangeTypeDef",
-    "TimestampRangeTypeDef",
+    "TimestampTypeDef",
     "FragmentTypeDef",
     "ResponseMetadataTypeDef",
     "PaginatorConfigTypeDef",
-    "GetImagesInputRequestTypeDef",
     "ImageTypeDef",
     "GetMediaForFragmentListInputRequestTypeDef",
+    "ClipTimestampRangeTypeDef",
+    "DASHTimestampRangeTypeDef",
+    "GetImagesInputRequestTypeDef",
     "HLSTimestampRangeTypeDef",
-    "ClipFragmentSelectorTypeDef",
-    "DASHFragmentSelectorTypeDef",
-    "FragmentSelectorTypeDef",
+    "TimestampRangeTypeDef",
     "GetClipOutputTypeDef",
     "GetDASHStreamingSessionURLOutputTypeDef",
     "GetHLSStreamingSessionURLOutputTypeDef",
     "GetMediaForFragmentListOutputTypeDef",
     "ListFragmentsOutputTypeDef",
     "GetImagesInputGetImagesPaginateTypeDef",
     "GetImagesOutputTypeDef",
+    "ClipFragmentSelectorTypeDef",
+    "DASHFragmentSelectorTypeDef",
     "HLSFragmentSelectorTypeDef",
+    "FragmentSelectorTypeDef",
     "GetClipInputRequestTypeDef",
     "GetDASHStreamingSessionURLInputRequestTypeDef",
+    "GetHLSStreamingSessionURLInputRequestTypeDef",
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     "ListFragmentsInputRequestTypeDef",
-    "GetHLSStreamingSessionURLInputRequestTypeDef",
-)
-
-ClipTimestampRangeTypeDef = TypedDict(
-    "ClipTimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-)
-
-DASHTimestampRangeTypeDef = TypedDict(
-    "DASHTimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
 )
 
+TimestampTypeDef = Union[datetime, str]
 FragmentTypeDef = TypedDict(
     "FragmentTypeDef",
     {
         "FragmentNumber": str,
         "FragmentSizeInBytes": int,
         "ProducerTimestamp": datetime,
         "ServerTimestamp": datetime,
@@ -126,43 +103,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredGetImagesInputRequestTypeDef = TypedDict(
-    "_RequiredGetImagesInputRequestTypeDef",
-    {
-        "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-        "SamplingInterval": int,
-        "Format": FormatType,
-    },
-)
-_OptionalGetImagesInputRequestTypeDef = TypedDict(
-    "_OptionalGetImagesInputRequestTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetImagesInputRequestTypeDef(
-    _RequiredGetImagesInputRequestTypeDef, _OptionalGetImagesInputRequestTypeDef
-):
-    pass
-
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "TimeStamp": datetime,
         "Error": ImageErrorType,
         "ImageContent": str,
     },
@@ -186,45 +134,74 @@
 
 class GetMediaForFragmentListInputRequestTypeDef(
     _RequiredGetMediaForFragmentListInputRequestTypeDef,
     _OptionalGetMediaForFragmentListInputRequestTypeDef,
 ):
     pass
 
-HLSTimestampRangeTypeDef = TypedDict(
-    "HLSTimestampRangeTypeDef",
+ClipTimestampRangeTypeDef = TypedDict(
+    "ClipTimestampRangeTypeDef",
     {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+)
+
+DASHTimestampRangeTypeDef = TypedDict(
+    "DASHTimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-ClipFragmentSelectorTypeDef = TypedDict(
-    "ClipFragmentSelectorTypeDef",
+_RequiredGetImagesInputRequestTypeDef = TypedDict(
+    "_RequiredGetImagesInputRequestTypeDef",
     {
-        "FragmentSelectorType": ClipFragmentSelectorTypeType,
-        "TimestampRange": ClipTimestampRangeTypeDef,
+        "ImageSelectorType": ImageSelectorTypeType,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+        "SamplingInterval": int,
+        "Format": FormatType,
+    },
+)
+_OptionalGetImagesInputRequestTypeDef = TypedDict(
+    "_OptionalGetImagesInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+        "MaxResults": int,
+        "NextToken": str,
     },
+    total=False,
 )
 
-DASHFragmentSelectorTypeDef = TypedDict(
-    "DASHFragmentSelectorTypeDef",
+class GetImagesInputRequestTypeDef(
+    _RequiredGetImagesInputRequestTypeDef, _OptionalGetImagesInputRequestTypeDef
+):
+    pass
+
+HLSTimestampRangeTypeDef = TypedDict(
+    "HLSTimestampRangeTypeDef",
     {
-        "FragmentSelectorType": DASHFragmentSelectorTypeType,
-        "TimestampRange": DASHTimestampRangeTypeDef,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-FragmentSelectorTypeDef = TypedDict(
-    "FragmentSelectorTypeDef",
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
     {
-        "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeTypeDef,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
 )
 
 GetClipOutputTypeDef = TypedDict(
     "GetClipOutputTypeDef",
     {
         "ContentType": str,
@@ -267,16 +244,16 @@
     },
 )
 
 _RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
     "_RequiredGetImagesInputGetImagesPaginateTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
     "_OptionalGetImagesInputGetImagesPaginateTypeDef",
     {
@@ -300,23 +277,48 @@
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ClipFragmentSelectorTypeDef = TypedDict(
+    "ClipFragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": ClipFragmentSelectorTypeType,
+        "TimestampRange": ClipTimestampRangeTypeDef,
+    },
+)
+
+DASHFragmentSelectorTypeDef = TypedDict(
+    "DASHFragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": DASHFragmentSelectorTypeType,
+        "TimestampRange": DASHTimestampRangeTypeDef,
+    },
+    total=False,
+)
+
 HLSFragmentSelectorTypeDef = TypedDict(
     "HLSFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": HLSFragmentSelectorTypeType,
         "TimestampRange": HLSTimestampRangeTypeDef,
     },
     total=False,
 )
 
+FragmentSelectorTypeDef = TypedDict(
+    "FragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeTypeDef,
+    },
+)
+
 _RequiredGetClipInputRequestTypeDef = TypedDict(
     "_RequiredGetClipInputRequestTypeDef",
     {
         "ClipFragmentSelector": ClipFragmentSelectorTypeDef,
     },
 )
 _OptionalGetClipInputRequestTypeDef = TypedDict(
@@ -344,14 +346,30 @@
         "DASHFragmentSelector": DASHFragmentSelectorTypeDef,
         "Expires": int,
         "MaxManifestFragmentResults": int,
     },
     total=False,
 )
 
+GetHLSStreamingSessionURLInputRequestTypeDef = TypedDict(
+    "GetHLSStreamingSessionURLInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "PlaybackMode": HLSPlaybackModeType,
+        "HLSFragmentSelector": HLSFragmentSelectorTypeDef,
+        "ContainerFormat": ContainerFormatType,
+        "DiscontinuityMode": HLSDiscontinuityModeType,
+        "DisplayFragmentTimestamp": HLSDisplayFragmentTimestampType,
+        "Expires": int,
+        "MaxMediaPlaylistFragmentResults": int,
+    },
+    total=False,
+)
+
 ListFragmentsInputListFragmentsPaginateTypeDef = TypedDict(
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "FragmentSelector": FragmentSelectorTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -366,23 +384,7 @@
         "StreamARN": str,
         "MaxResults": int,
         "NextToken": str,
         "FragmentSelector": FragmentSelectorTypeDef,
     },
     total=False,
 )
-
-GetHLSStreamingSessionURLInputRequestTypeDef = TypedDict(
-    "GetHLSStreamingSessionURLInputRequestTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "PlaybackMode": HLSPlaybackModeType,
-        "HLSFragmentSelector": HLSFragmentSelectorTypeDef,
-        "ContainerFormat": ContainerFormatType,
-        "DiscontinuityMode": HLSDiscontinuityModeType,
-        "DisplayFragmentTimestamp": HLSDisplayFragmentTimestampType,
-        "Expires": int,
-        "MaxMediaPlaylistFragmentResults": int,
-    },
-    total=False,
-)
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-archived-media
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesis-video-archived-media type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kinesis-video-archived-media type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-archived-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoArchivedMedia 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[boto3.KinesisVideoArchivedMedia 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [mypy-boto3-kinesis-video-archived-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/).
 
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
@@ -331,53 +331,55 @@
 )
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kinesis_video_archived_media.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from mypy_boto3_kinesis_video_archived_media.type_defs import (
-    ClipTimestampRangeTypeDef,
-    DASHTimestampRangeTypeDef,
-    TimestampRangeTypeDef,
+    TimestampTypeDef,
     FragmentTypeDef,
     ResponseMetadataTypeDef,
     PaginatorConfigTypeDef,
-    GetImagesInputRequestTypeDef,
     ImageTypeDef,
     GetMediaForFragmentListInputRequestTypeDef,
+    ClipTimestampRangeTypeDef,
+    DASHTimestampRangeTypeDef,
+    GetImagesInputRequestTypeDef,
     HLSTimestampRangeTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
+    TimestampRangeTypeDef,
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
     GetMediaForFragmentListOutputTypeDef,
     ListFragmentsOutputTypeDef,
     GetImagesInputGetImagesPaginateTypeDef,
     GetImagesOutputTypeDef,
+    ClipFragmentSelectorTypeDef,
+    DASHFragmentSelectorTypeDef,
     HLSFragmentSelectorTypeDef,
+    FragmentSelectorTypeDef,
     GetClipInputRequestTypeDef,
     GetDASHStreamingSessionURLInputRequestTypeDef,
+    GetHLSStreamingSessionURLInputRequestTypeDef,
     ListFragmentsInputListFragmentsPaginateTypeDef,
     ListFragmentsInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
 )
 
 
-def get_structure() -> ClipTimestampRangeTypeDef:
+def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.15.post1/setup.py` & `mypy-boto3-kinesis-video-archived-media-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis-video-archived-media",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_kinesis_video_archived_media"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -35,15 +35,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords=(
-        "boto3 kinesis-video-archived-media type-annotations boto3-stubs mypy typeshed autocomplete"
+        "boto3 kinesis-video-archived-media type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_kinesis_video_archived_media": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
```

