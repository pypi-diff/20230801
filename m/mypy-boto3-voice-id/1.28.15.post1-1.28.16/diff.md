# Comparing `tmp/mypy-boto3-voice-id-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-voice-id-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-voice-id-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:23 2023, max compression
+gzip compressed data, was "mypy-boto3-voice-id-1.28.16.tar", last modified: Tue Aug  1 11:38:02 2023, max compression
```

## Comparing `mypy-boto3-voice-id-1.28.15.post1.tar` & `mypy-boto3-voice-id-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.673449 mypy-boto3-voice-id-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-07-29 10:04:23.669449 mypy-boto3-voice-id-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16038 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.661449 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23305 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23263 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33375 2023-07-29 10:01:08.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33338 2023-07-29 10:01:08.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.669449 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:23.673449 mypy-boto3-voice-id-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:02.892683 mypy-boto3-voice-id-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:45.000000 mypy-boto3-voice-id-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-08-01 11:38:02.892683 mypy-boto3-voice-id-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-08-01 11:34:45.000000 mypy-boto3-voice-id-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:02.888683 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-01 11:34:45.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-01 11:34:45.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-01 11:34:45.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23168 2023-08-01 11:34:46.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23126 2023-08-01 11:34:46.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-08-01 11:34:46.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-08-01 11:34:46.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-08-01 11:34:46.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-08-01 11:34:46.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:45.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33646 2023-08-01 11:34:47.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33609 2023-08-01 11:34:46.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:45.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:02.892683 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-08-01 11:38:02.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:38:02.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:02.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:02.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:02.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:38:02.000000 mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:02.892683 mypy-boto3-voice-id-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-01 11:34:45.000000 mypy-boto3-voice-id-1.28.16/setup.py
```

### Comparing `mypy-boto3-voice-id-1.28.15.post1/LICENSE` & `mypy-boto3-voice-id-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15.post1/PKG-INFO` & `mypy-boto3-voice-id-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.VoiceID 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 voice-id type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 voice-id type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-voice-id)](https://pepy.tech/project/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
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
@@ -342,20 +342,20 @@
 )
 
 
 def check_value(value: AuthenticationDecisionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_voice_id.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
     ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
@@ -430,33 +430,35 @@
     ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
     ListWatchlistsResponseTypeDef,
+    RegistrationConfigUnionTypeDef,
     StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
+    EnrollmentConfigUnionTypeDef,
     StartSpeakerEnrollmentJobRequestRequestTypeDef,
     FraudDetectionResultTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     DescribeFraudsterRegistrationJobResponseTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     EvaluateSessionResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateFraudsterRequestRequestTypeDef:
+def get_value() -> AssociateFraudsterRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-voice-id-1.28.15.post1/README.md` & `mypy-boto3-voice-id-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-voice-id)](https://pepy.tech/project/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
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
@@ -310,20 +310,20 @@
 )
 
 
 def check_value(value: AuthenticationDecisionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_voice_id.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
     ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
@@ -398,33 +398,35 @@
     ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
     ListWatchlistsResponseTypeDef,
+    RegistrationConfigUnionTypeDef,
     StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
+    EnrollmentConfigUnionTypeDef,
     StartSpeakerEnrollmentJobRequestRequestTypeDef,
     FraudDetectionResultTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     DescribeFraudsterRegistrationJobResponseTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     EvaluateSessionResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateFraudsterRequestRequestTypeDef:
+def get_value() -> AssociateFraudsterRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__init__.py` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__init__.pyi` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__main__.py` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VoiceID 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.VoiceID 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
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

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/client.py` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_voice_id.client import VoiceIDClient
 
     session = Session()
     client: VoiceIDClient = session.client("voice-id")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FraudsterRegistrationJobStatusType, SpeakerEnrollmentJobStatusType
 from .paginator import (
     ListDomainsPaginator,
     ListFraudsterRegistrationJobsPaginator,
@@ -35,29 +35,27 @@
     DescribeFraudsterRegistrationJobResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnrollmentConfigOutputTypeDef,
-    EnrollmentConfigTypeDef,
+    EnrollmentConfigUnionTypeDef,
     EvaluateSessionResponseTypeDef,
     InputDataConfigTypeDef,
     ListDomainsResponseTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListFraudstersResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     ListSpeakersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     OutputDataConfigTypeDef,
-    RegistrationConfigOutputTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigUnionTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     TagTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
 )
@@ -376,15 +374,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef] = ...
+        RegistrationConfig: RegistrationConfigUnionTypeDef = ...
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/client/#start_fraudster_registration_job)
         """
@@ -393,15 +391,15 @@
         self,
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
-        EnrollmentConfig: Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef] = ...,
+        EnrollmentConfig: EnrollmentConfigUnionTypeDef = ...,
         JobName: str = ...
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/client/#start_speaker_enrollment_job)
```

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/client.pyi` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_voice_id.client import VoiceIDClient
 
     session = Session()
     client: VoiceIDClient = session.client("voice-id")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FraudsterRegistrationJobStatusType, SpeakerEnrollmentJobStatusType
 from .paginator import (
     ListDomainsPaginator,
     ListFraudsterRegistrationJobsPaginator,
@@ -35,29 +35,27 @@
     DescribeFraudsterRegistrationJobResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnrollmentConfigOutputTypeDef,
-    EnrollmentConfigTypeDef,
+    EnrollmentConfigUnionTypeDef,
     EvaluateSessionResponseTypeDef,
     InputDataConfigTypeDef,
     ListDomainsResponseTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListFraudstersResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     ListSpeakersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     OutputDataConfigTypeDef,
-    RegistrationConfigOutputTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigUnionTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     TagTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
 )
@@ -345,15 +343,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef] = ...
+        RegistrationConfig: RegistrationConfigUnionTypeDef = ...
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/client/#start_fraudster_registration_job)
         """
@@ -361,15 +359,15 @@
         self,
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
-        EnrollmentConfig: Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef] = ...,
+        EnrollmentConfig: EnrollmentConfigUnionTypeDef = ...,
         JobName: str = ...
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/client/#start_speaker_enrollment_job)
```

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/literals.py` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/literals.pyi` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/paginator.py` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/paginator.pyi` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/type_defs.py` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_voice_id.type_defs import AssociateFraudsterRequestRequestTypeDef
 
-    data: AssociateFraudsterRequestRequestTypeDef = {...}
+    data: AssociateFraudsterRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AuthenticationDecisionType,
     DomainStatusType,
     DuplicateRegistrationActionType,
     ExistingEnrollmentActionType,
     FraudDetectionActionType,
@@ -112,20 +112,22 @@
     "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
+    "RegistrationConfigUnionTypeDef",
     "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
+    "EnrollmentConfigUnionTypeDef",
     "StartSpeakerEnrollmentJobRequestRequestTypeDef",
     "FraudDetectionResultTypeDef",
     "ListFraudsterRegistrationJobsResponseTypeDef",
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     "StartFraudsterRegistrationJobResponseTypeDef",
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
@@ -1094,14 +1096,15 @@
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RegistrationConfigUnionTypeDef = Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef]
 _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
     {
         "DataAccessRoleArn": str,
         "DomainId": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
@@ -1173,14 +1176,15 @@
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
     },
     total=False,
 )
 
+EnrollmentConfigUnionTypeDef = Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef]
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
         "DataAccessRoleArn": str,
         "DomainId": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/type_defs.pyi` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_voice_id.type_defs import AssociateFraudsterRequestRequestTypeDef
 
-    data: AssociateFraudsterRequestRequestTypeDef = {...}
+    data: AssociateFraudsterRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AuthenticationDecisionType,
     DomainStatusType,
     DuplicateRegistrationActionType,
     ExistingEnrollmentActionType,
     FraudDetectionActionType,
@@ -111,20 +111,22 @@
     "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
+    "RegistrationConfigUnionTypeDef",
     "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
+    "EnrollmentConfigUnionTypeDef",
     "StartSpeakerEnrollmentJobRequestRequestTypeDef",
     "FraudDetectionResultTypeDef",
     "ListFraudsterRegistrationJobsResponseTypeDef",
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     "StartFraudsterRegistrationJobResponseTypeDef",
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
@@ -1061,14 +1063,15 @@
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RegistrationConfigUnionTypeDef = Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef]
 _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
     {
         "DataAccessRoleArn": str,
         "DomainId": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
@@ -1138,14 +1141,15 @@
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
     },
     total=False,
 )
 
+EnrollmentConfigUnionTypeDef = Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef]
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
         "DataAccessRoleArn": str,
         "DomainId": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/PKG-INFO` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.VoiceID 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 voice-id type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 voice-id type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-voice-id)](https://pepy.tech/project/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
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
@@ -342,20 +342,20 @@
 )
 
 
 def check_value(value: AuthenticationDecisionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_voice_id.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
     ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
@@ -430,33 +430,35 @@
     ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
     ListWatchlistsResponseTypeDef,
+    RegistrationConfigUnionTypeDef,
     StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
+    EnrollmentConfigUnionTypeDef,
     StartSpeakerEnrollmentJobRequestRequestTypeDef,
     FraudDetectionResultTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     DescribeFraudsterRegistrationJobResponseTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     EvaluateSessionResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateFraudsterRequestRequestTypeDef:
+def get_value() -> AssociateFraudsterRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/SOURCES.txt` & `mypy-boto3-voice-id-1.28.16/mypy_boto3_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15.post1/setup.py` & `mypy-boto3-voice-id-1.28.16/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-voice-id",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.VoiceID 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 voice-id type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 voice-id type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_voice_id": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

