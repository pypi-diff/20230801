# Comparing `tmp/mypy-boto3-iotevents-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iotevents-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotevents-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:21 2023, max compression
+gzip compressed data, was "mypy-boto3-iotevents-1.28.16.tar", last modified: Tue Aug  1 11:37:01 2023, max compression
```

## Comparing `mypy-boto3-iotevents-1.28.15.post1.tar` & `mypy-boto3-iotevents-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.209187 mypy-boto3-iotevents-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-29 10:03:21.209187 mypy-boto3-iotevents-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.201187 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19455 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42731 2023-07-29 09:47:55.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42652 2023-07-29 09:47:55.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.209187 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:21.209187 mypy-boto3-iotevents-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:01.232863 mypy-boto3-iotevents-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:37.000000 mypy-boto3-iotevents-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-08-01 11:37:01.228863 mypy-boto3-iotevents-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-08-01 11:20:37.000000 mypy-boto3-iotevents-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:01.212863 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 11:20:37.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-01 11:20:37.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:20:37.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-08-01 11:20:39.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18827 2023-08-01 11:20:37.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-08-01 11:20:39.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-08-01 11:20:39.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:37.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43411 2023-08-01 11:20:40.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43332 2023-08-01 11:20:40.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:37.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:01.228863 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-08-01 11:37:00.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 11:37:01.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:00.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:00.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:00.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:37:00.000000 mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:01.232863 mypy-boto3-iotevents-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:20:36.000000 mypy-boto3-iotevents-1.28.16/setup.py
```

### Comparing `mypy-boto3-iotevents-1.28.15.post1/LICENSE` & `mypy-boto3-iotevents-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15.post1/PKG-INFO` & `mypy-boto3-iotevents-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTEvents 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotevents type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotevents type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents)](https://pepy.tech/project/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
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
@@ -295,20 +295,20 @@
 )
 
 
 def check_value(value: AlarmModelVersionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotevents.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotevents.type_defs import (
     AcknowledgeFlowTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
@@ -385,16 +385,18 @@
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
     IotSiteWiseActionTypeDef,
     InputTypeDef,
     CreateInputRequestRequestTypeDef,
+    InputDefinitionUnionTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    LoggingOptionsUnionTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
     EmailRecipientsOutputTypeDef,
     EmailRecipientsTypeDef,
     SMSConfigurationOutputTypeDef,
     SMSConfigurationTypeDef,
@@ -414,32 +416,35 @@
     NotificationActionTypeDef,
     OnEnterLifecycleOutputTypeDef,
     OnExitLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
     OnInputLifecycleOutputTypeDef,
     OnInputLifecycleTypeDef,
+    AlarmEventActionsUnionTypeDef,
     AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
     StateOutputTypeDef,
     StateTypeDef,
     DescribeAlarmModelResponseTypeDef,
+    AlarmNotificationUnionTypeDef,
     CreateAlarmModelRequestRequestTypeDef,
     UpdateAlarmModelRequestRequestTypeDef,
     DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
     DetectorModelTypeDef,
     CreateDetectorModelRequestRequestTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowTypeDef:
+def get_value() -> AcknowledgeFlowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotevents-1.28.15.post1/README.md` & `mypy-boto3-iotevents-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents)](https://pepy.tech/project/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
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
@@ -263,20 +263,20 @@
 )
 
 
 def check_value(value: AlarmModelVersionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotevents.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotevents.type_defs import (
     AcknowledgeFlowTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
@@ -353,16 +353,18 @@
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
     IotSiteWiseActionTypeDef,
     InputTypeDef,
     CreateInputRequestRequestTypeDef,
+    InputDefinitionUnionTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    LoggingOptionsUnionTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
     EmailRecipientsOutputTypeDef,
     EmailRecipientsTypeDef,
     SMSConfigurationOutputTypeDef,
     SMSConfigurationTypeDef,
@@ -382,32 +384,35 @@
     NotificationActionTypeDef,
     OnEnterLifecycleOutputTypeDef,
     OnExitLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
     OnInputLifecycleOutputTypeDef,
     OnInputLifecycleTypeDef,
+    AlarmEventActionsUnionTypeDef,
     AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
     StateOutputTypeDef,
     StateTypeDef,
     DescribeAlarmModelResponseTypeDef,
+    AlarmNotificationUnionTypeDef,
     CreateAlarmModelRequestRequestTypeDef,
     UpdateAlarmModelRequestRequestTypeDef,
     DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
     DetectorModelTypeDef,
     CreateDetectorModelRequestRequestTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowTypeDef:
+def get_value() -> AcknowledgeFlowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/__main__.py` & `mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTEvents 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTEvents 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/client.py` & `mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,50 +9,45 @@
     from boto3.session import Session
     from mypy_boto3_iotevents.client import IoTEventsClient
 
     session = Session()
     client: IoTEventsClient = session.client("iotevents")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EvaluationMethodType
 from .type_defs import (
     AlarmCapabilitiesTypeDef,
-    AlarmEventActionsOutputTypeDef,
-    AlarmEventActionsTypeDef,
-    AlarmNotificationOutputTypeDef,
-    AlarmNotificationTypeDef,
+    AlarmEventActionsUnionTypeDef,
+    AlarmNotificationUnionTypeDef,
     AlarmRuleTypeDef,
     CreateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     DescribeAlarmModelResponseTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    DetectorModelDefinitionOutputTypeDef,
-    DetectorModelDefinitionTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
-    InputDefinitionOutputTypeDef,
-    InputDefinitionTypeDef,
+    InputDefinitionUnionTypeDef,
     InputIdentifierTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     ListInputRoutingsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggingOptionsOutputTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsUnionTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     TagTypeDef,
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
 
@@ -119,32 +114,30 @@
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
-        alarmNotification: Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef] = ...,
-        alarmEventActions: Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef] = ...,
+        alarmNotification: AlarmNotificationUnionTypeDef = ...,
+        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#create_alarm_model)
         """
 
     def create_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: Union[
-            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
-        ],
+        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> CreateDetectorModelResponseTypeDef:
         """
@@ -154,15 +147,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#create_detector_model)
         """
 
     def create_input(
         self,
         *,
         inputName: str,
-        inputDefinition: Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef],
+        inputDefinition: InputDefinitionUnionTypeDef,
         inputDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
@@ -332,29 +325,25 @@
         Lists the tags (metadata) you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#list_tags_for_resource)
         """
 
     def put_logging_options(
-        self, *, loggingOptions: Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
+        self, *, loggingOptions: LoggingOptionsUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets or updates the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.put_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#put_logging_options)
         """
 
     def start_detector_model_analysis(
-        self,
-        *,
-        detectorModelDefinition: Union[
-            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
-        ]
+        self, *, detectorModelDefinition: DetectorModelDefinitionUnionTypeDef
     ) -> StartDetectorModelAnalysisResponseTypeDef:
         """
         Performs an analysis of your detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.start_detector_model_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#start_detector_model_analysis)
         """
@@ -379,32 +368,30 @@
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
-        alarmNotification: Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef] = ...,
-        alarmEventActions: Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef] = ...,
+        alarmNotification: AlarmNotificationUnionTypeDef = ...,
+        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_alarm_model)
         """
 
     def update_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: Union[
-            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
-        ],
+        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
@@ -412,15 +399,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_detector_model)
         """
 
     def update_input(
         self,
         *,
         inputName: str,
-        inputDefinition: Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef],
+        inputDefinition: InputDefinitionUnionTypeDef,
         inputDescription: str = ...
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_input)
```

### Comparing `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/client.pyi` & `mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,50 +9,45 @@
     from boto3.session import Session
     from mypy_boto3_iotevents.client import IoTEventsClient
 
     session = Session()
     client: IoTEventsClient = session.client("iotevents")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EvaluationMethodType
 from .type_defs import (
     AlarmCapabilitiesTypeDef,
-    AlarmEventActionsOutputTypeDef,
-    AlarmEventActionsTypeDef,
-    AlarmNotificationOutputTypeDef,
-    AlarmNotificationTypeDef,
+    AlarmEventActionsUnionTypeDef,
+    AlarmNotificationUnionTypeDef,
     AlarmRuleTypeDef,
     CreateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     DescribeAlarmModelResponseTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    DetectorModelDefinitionOutputTypeDef,
-    DetectorModelDefinitionTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
-    InputDefinitionOutputTypeDef,
-    InputDefinitionTypeDef,
+    InputDefinitionUnionTypeDef,
     InputIdentifierTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     ListInputRoutingsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggingOptionsOutputTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsUnionTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     TagTypeDef,
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
 
@@ -113,31 +108,29 @@
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
-        alarmNotification: Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef] = ...,
-        alarmEventActions: Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef] = ...,
+        alarmNotification: AlarmNotificationUnionTypeDef = ...,
+        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#create_alarm_model)
         """
     def create_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: Union[
-            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
-        ],
+        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> CreateDetectorModelResponseTypeDef:
         """
@@ -146,15 +139,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_detector_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#create_detector_model)
         """
     def create_input(
         self,
         *,
         inputName: str,
-        inputDefinition: Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef],
+        inputDefinition: InputDefinitionUnionTypeDef,
         inputDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
@@ -306,28 +299,24 @@
         """
         Lists the tags (metadata) you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#list_tags_for_resource)
         """
     def put_logging_options(
-        self, *, loggingOptions: Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
+        self, *, loggingOptions: LoggingOptionsUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets or updates the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.put_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#put_logging_options)
         """
     def start_detector_model_analysis(
-        self,
-        *,
-        detectorModelDefinition: Union[
-            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
-        ]
+        self, *, detectorModelDefinition: DetectorModelDefinitionUnionTypeDef
     ) -> StartDetectorModelAnalysisResponseTypeDef:
         """
         Performs an analysis of your detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.start_detector_model_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#start_detector_model_analysis)
         """
@@ -349,46 +338,44 @@
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
-        alarmNotification: Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef] = ...,
-        alarmEventActions: Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef] = ...,
+        alarmNotification: AlarmNotificationUnionTypeDef = ...,
+        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_alarm_model)
         """
     def update_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: Union[
-            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
-        ],
+        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_detector_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_detector_model)
         """
     def update_input(
         self,
         *,
         inputName: str,
-        inputDefinition: Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef],
+        inputDefinition: InputDefinitionUnionTypeDef,
         inputDescription: str = ...
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_input)
```

### Comparing `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/literals.py` & `mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/literals.pyi` & `mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/type_defs.py` & `mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotevents.type_defs import AcknowledgeFlowTypeDef
 
-    data: AcknowledgeFlowTypeDef = {...}
+    data: AcknowledgeFlowTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AlarmModelVersionStatusType,
     AnalysisResultLevelType,
     AnalysisStatusType,
     ComparisonOperatorType,
     DetectorModelVersionStatusType,
@@ -111,16 +111,18 @@
     "IotSiteWiseInputIdentifierTypeDef",
     "ListInputRoutingsResponseTypeDef",
     "RecipientDetailTypeDef",
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     "IotSiteWiseActionTypeDef",
     "InputTypeDef",
     "CreateInputRequestRequestTypeDef",
+    "InputDefinitionUnionTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
+    "LoggingOptionsUnionTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "NotificationTargetActionsTypeDef",
     "InputIdentifierTypeDef",
     "EmailRecipientsOutputTypeDef",
     "EmailRecipientsTypeDef",
     "SMSConfigurationOutputTypeDef",
     "SMSConfigurationTypeDef",
@@ -140,25 +142,28 @@
     "NotificationActionTypeDef",
     "OnEnterLifecycleOutputTypeDef",
     "OnExitLifecycleOutputTypeDef",
     "OnEnterLifecycleTypeDef",
     "OnExitLifecycleTypeDef",
     "OnInputLifecycleOutputTypeDef",
     "OnInputLifecycleTypeDef",
+    "AlarmEventActionsUnionTypeDef",
     "AlarmNotificationOutputTypeDef",
     "AlarmNotificationTypeDef",
     "StateOutputTypeDef",
     "StateTypeDef",
     "DescribeAlarmModelResponseTypeDef",
+    "AlarmNotificationUnionTypeDef",
     "CreateAlarmModelRequestRequestTypeDef",
     "UpdateAlarmModelRequestRequestTypeDef",
     "DetectorModelDefinitionOutputTypeDef",
     "DetectorModelDefinitionTypeDef",
     "DetectorModelTypeDef",
     "CreateDetectorModelRequestRequestTypeDef",
+    "DetectorModelDefinitionUnionTypeDef",
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     "UpdateDetectorModelRequestRequestTypeDef",
     "DescribeDetectorModelResponseTypeDef",
 )
 
 AcknowledgeFlowTypeDef = TypedDict(
     "AcknowledgeFlowTypeDef",
@@ -1143,14 +1148,15 @@
 
 class CreateInputRequestRequestTypeDef(
     _RequiredCreateInputRequestRequestTypeDef, _OptionalCreateInputRequestRequestTypeDef
 ):
     pass
 
 
+InputDefinitionUnionTypeDef = Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef]
 _RequiredUpdateInputRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1173,14 +1179,15 @@
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingOptionsUnionTypeDef = Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
@@ -1559,14 +1566,15 @@
     {
         "events": Sequence[EventTypeDef],
         "transitionEvents": Sequence[TransitionEventTypeDef],
     },
     total=False,
 )
 
+AlarmEventActionsUnionTypeDef = Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef]
 AlarmNotificationOutputTypeDef = TypedDict(
     "AlarmNotificationOutputTypeDef",
     {
         "notificationActions": List[NotificationActionOutputTypeDef],
     },
     total=False,
 )
@@ -1639,14 +1647,15 @@
         "alarmNotification": AlarmNotificationOutputTypeDef,
         "alarmEventActions": AlarmEventActionsOutputTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AlarmNotificationUnionTypeDef = Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef]
 _RequiredCreateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1747,14 +1756,17 @@
 class CreateDetectorModelRequestRequestTypeDef(
     _RequiredCreateDetectorModelRequestRequestTypeDef,
     _OptionalCreateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
 
+DetectorModelDefinitionUnionTypeDef = Union[
+    DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+]
 StartDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     {
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/type_defs.pyi` & `mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotevents.type_defs import AcknowledgeFlowTypeDef
 
-    data: AcknowledgeFlowTypeDef = {...}
+    data: AcknowledgeFlowTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AlarmModelVersionStatusType,
     AnalysisResultLevelType,
     AnalysisStatusType,
     ComparisonOperatorType,
     DetectorModelVersionStatusType,
@@ -110,16 +110,18 @@
     "IotSiteWiseInputIdentifierTypeDef",
     "ListInputRoutingsResponseTypeDef",
     "RecipientDetailTypeDef",
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     "IotSiteWiseActionTypeDef",
     "InputTypeDef",
     "CreateInputRequestRequestTypeDef",
+    "InputDefinitionUnionTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
+    "LoggingOptionsUnionTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "NotificationTargetActionsTypeDef",
     "InputIdentifierTypeDef",
     "EmailRecipientsOutputTypeDef",
     "EmailRecipientsTypeDef",
     "SMSConfigurationOutputTypeDef",
     "SMSConfigurationTypeDef",
@@ -139,25 +141,28 @@
     "NotificationActionTypeDef",
     "OnEnterLifecycleOutputTypeDef",
     "OnExitLifecycleOutputTypeDef",
     "OnEnterLifecycleTypeDef",
     "OnExitLifecycleTypeDef",
     "OnInputLifecycleOutputTypeDef",
     "OnInputLifecycleTypeDef",
+    "AlarmEventActionsUnionTypeDef",
     "AlarmNotificationOutputTypeDef",
     "AlarmNotificationTypeDef",
     "StateOutputTypeDef",
     "StateTypeDef",
     "DescribeAlarmModelResponseTypeDef",
+    "AlarmNotificationUnionTypeDef",
     "CreateAlarmModelRequestRequestTypeDef",
     "UpdateAlarmModelRequestRequestTypeDef",
     "DetectorModelDefinitionOutputTypeDef",
     "DetectorModelDefinitionTypeDef",
     "DetectorModelTypeDef",
     "CreateDetectorModelRequestRequestTypeDef",
+    "DetectorModelDefinitionUnionTypeDef",
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     "UpdateDetectorModelRequestRequestTypeDef",
     "DescribeDetectorModelResponseTypeDef",
 )
 
 AcknowledgeFlowTypeDef = TypedDict(
     "AcknowledgeFlowTypeDef",
@@ -1100,14 +1105,15 @@
 )
 
 class CreateInputRequestRequestTypeDef(
     _RequiredCreateInputRequestRequestTypeDef, _OptionalCreateInputRequestRequestTypeDef
 ):
     pass
 
+InputDefinitionUnionTypeDef = Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef]
 _RequiredUpdateInputRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1128,14 +1134,15 @@
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingOptionsUnionTypeDef = Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
@@ -1492,14 +1499,15 @@
     {
         "events": Sequence[EventTypeDef],
         "transitionEvents": Sequence[TransitionEventTypeDef],
     },
     total=False,
 )
 
+AlarmEventActionsUnionTypeDef = Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef]
 AlarmNotificationOutputTypeDef = TypedDict(
     "AlarmNotificationOutputTypeDef",
     {
         "notificationActions": List[NotificationActionOutputTypeDef],
     },
     total=False,
 )
@@ -1568,14 +1576,15 @@
         "alarmNotification": AlarmNotificationOutputTypeDef,
         "alarmEventActions": AlarmEventActionsOutputTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AlarmNotificationUnionTypeDef = Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef]
 _RequiredCreateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1670,14 +1679,17 @@
 
 class CreateDetectorModelRequestRequestTypeDef(
     _RequiredCreateDetectorModelRequestRequestTypeDef,
     _OptionalCreateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
+DetectorModelDefinitionUnionTypeDef = Union[
+    DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+]
 StartDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     {
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/PKG-INFO` & `mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTEvents 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotevents type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotevents type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents)](https://pepy.tech/project/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
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
@@ -295,20 +295,20 @@
 )
 
 
 def check_value(value: AlarmModelVersionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotevents.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotevents.type_defs import (
     AcknowledgeFlowTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
@@ -385,16 +385,18 @@
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
     IotSiteWiseActionTypeDef,
     InputTypeDef,
     CreateInputRequestRequestTypeDef,
+    InputDefinitionUnionTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    LoggingOptionsUnionTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
     EmailRecipientsOutputTypeDef,
     EmailRecipientsTypeDef,
     SMSConfigurationOutputTypeDef,
     SMSConfigurationTypeDef,
@@ -414,32 +416,35 @@
     NotificationActionTypeDef,
     OnEnterLifecycleOutputTypeDef,
     OnExitLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
     OnInputLifecycleOutputTypeDef,
     OnInputLifecycleTypeDef,
+    AlarmEventActionsUnionTypeDef,
     AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
     StateOutputTypeDef,
     StateTypeDef,
     DescribeAlarmModelResponseTypeDef,
+    AlarmNotificationUnionTypeDef,
     CreateAlarmModelRequestRequestTypeDef,
     UpdateAlarmModelRequestRequestTypeDef,
     DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
     DetectorModelTypeDef,
     CreateDetectorModelRequestRequestTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowTypeDef:
+def get_value() -> AcknowledgeFlowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/SOURCES.txt` & `mypy-boto3-iotevents-1.28.16/mypy_boto3_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15.post1/setup.py` & `mypy-boto3-iotevents-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotevents",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.IoTEvents 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 iotevents type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iotevents type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iotevents": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

