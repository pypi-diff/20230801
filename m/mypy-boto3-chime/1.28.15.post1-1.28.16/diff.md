# Comparing `tmp/mypy-boto3-chime-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-chime-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:38 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-1.28.16.tar", last modified: Tue Aug  1 11:36:18 2023, max compression
```

## Comparing `mypy-boto3-chime-1.28.15.post1.tar` & `mypy-boto3-chime-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.097036 mypy-boto3-chime-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32823 2023-07-29 10:02:38.097036 mypy-boto3-chime-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31338 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.077036 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   121941 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   121741 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   146654 2023-07-29 09:39:25.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   146493 2023-07-29 09:39:22.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.097036 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32823 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:38.097036 mypy-boto3-chime-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:39:17.000000 mypy-boto3-chime-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.824939 mypy-boto3-chime-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:50.000000 mypy-boto3-chime-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33026 2023-08-01 11:36:18.812939 mypy-boto3-chime-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31550 2023-08-01 11:11:50.000000 mypy-boto3-chime-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.812939 mypy-boto3-chime-1.28.16/mypy_boto3_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-01 11:11:50.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-01 11:11:50.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 11:11:50.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121423 2023-08-01 11:11:52.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121223 2023-08-01 11:11:52.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-08-01 11:11:53.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-08-01 11:11:53.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-01 11:11:52.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-08-01 11:11:52.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:50.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   147455 2023-08-01 11:11:57.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147294 2023-08-01 11:11:55.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:50.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.812939 mypy-boto3-chime-1.28.16/mypy_boto3_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33026 2023-08-01 11:36:18.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 11:36:18.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:18.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:36:18.000000 mypy-boto3-chime-1.28.16/mypy_boto3_chime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:18.824939 mypy-boto3-chime-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:11:50.000000 mypy-boto3-chime-1.28.16/setup.py
```

### Comparing `mypy-boto3-chime-1.28.15.post1/LICENSE` & `mypy-boto3-chime-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15.post1/PKG-INFO` & `mypy-boto3-chime-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Chime 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 chime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime)](https://pepy.tech/project/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
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
@@ -361,20 +361,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_chime.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_chime.type_defs import (
     AccountSettingsTypeDef,
     SigninDelegateGroupTypeDef,
     AddressTypeDef,
     AlexaForBusinessMetadataTypeDef,
@@ -523,15 +523,15 @@
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     ListMeetingTagsRequestRequestTypeDef,
     ListMeetingsRequestRequestTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
@@ -714,23 +714,25 @@
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     InviteUsersResponseTypeDef,
     ListAccountsRequestListAccountsPaginateTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
+    TerminationUnionTypeDef,
     RetentionSettingsTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     UserSettingsTypeDef,
     CreateAccountResponseTypeDef,
@@ -774,28 +776,30 @@
     UpdateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
     ListMeetingsResponseTypeDef,
     CreateRoomMembershipResponseTypeDef,
     ListRoomMembershipsResponseTypeDef,
     UpdateRoomMembershipResponseTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
+    OriginationUnionTypeDef,
     PutVoiceConnectorOriginationRequestRequestTypeDef,
     CreateProxySessionResponseTypeDef,
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
@@ -805,25 +809,27 @@
     PutRetentionSettingsRequestRequestTypeDef,
     PutRetentionSettingsResponseTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
+    StreamingConfigurationUnionTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-1.28.15.post1/README.md` & `mypy-boto3-chime-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime)](https://pepy.tech/project/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
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
@@ -329,20 +329,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_chime.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_chime.type_defs import (
     AccountSettingsTypeDef,
     SigninDelegateGroupTypeDef,
     AddressTypeDef,
     AlexaForBusinessMetadataTypeDef,
@@ -491,15 +491,15 @@
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     ListMeetingTagsRequestRequestTypeDef,
     ListMeetingsRequestRequestTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
@@ -682,23 +682,25 @@
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     InviteUsersResponseTypeDef,
     ListAccountsRequestListAccountsPaginateTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
+    TerminationUnionTypeDef,
     RetentionSettingsTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     UserSettingsTypeDef,
     CreateAccountResponseTypeDef,
@@ -742,28 +744,30 @@
     UpdateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
     ListMeetingsResponseTypeDef,
     CreateRoomMembershipResponseTypeDef,
     ListRoomMembershipsResponseTypeDef,
     UpdateRoomMembershipResponseTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
+    OriginationUnionTypeDef,
     PutVoiceConnectorOriginationRequestRequestTypeDef,
     CreateProxySessionResponseTypeDef,
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
@@ -773,25 +777,27 @@
     PutRetentionSettingsRequestRequestTypeDef,
     PutRetentionSettingsResponseTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
+    StreamingConfigurationUnionTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__init__.py` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__init__.pyi` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__main__.py` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Chime 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.Chime 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
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

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/client.py` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_chime.client import ChimeClient
 
     session = Session()
     client: ChimeClient = session.client("chime")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CapabilityType,
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
@@ -53,16 +52,15 @@
     BatchCreateRoomMembershipResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
     BatchUnsuspendUserResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     BatchUpdateUserResponseTypeDef,
     BusinessCallingSettingsTypeDef,
-    ChimeSdkMeetingConfigurationOutputTypeDef,
-    ChimeSdkMeetingConfigurationTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateAccountResponseTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeResponseTypeDef,
     CreateBotResponseTypeDef,
@@ -92,16 +90,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmergencyCallingConfigurationOutputTypeDef,
-    EmergencyCallingConfigurationTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetAccountResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
     GetAttendeeResponseTypeDef,
@@ -162,16 +159,15 @@
     ListUsersResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     LoggingConfigurationTypeDef,
     MeetingNotificationConfigurationTypeDef,
     MembershipItemTypeDef,
-    OriginationOutputTypeDef,
-    OriginationTypeDef,
+    OriginationUnionTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     PutRetentionSettingsResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
@@ -186,19 +182,18 @@
     RetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     SigninDelegateGroupTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
-    StreamingConfigurationOutputTypeDef,
-    StreamingConfigurationTypeDef,
+    StreamingConfigurationUnionTypeDef,
     TagTypeDef,
-    TerminationOutputTypeDef,
-    TerminationTypeDef,
+    TerminationUnionTypeDef,
+    TimestampTypeDef,
     TranscriptionConfigurationTypeDef,
     UpdateAccountResponseTypeDef,
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
@@ -546,17 +541,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: Union[
-            ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
-        ] = ...
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#create_media_capture_pipeline)
         """
@@ -1592,16 +1585,16 @@
         """
 
     def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         SortOrder: SortOrderType = ...,
-        NotBefore: Union[datetime, str] = ...,
-        NotAfter: Union[datetime, str] = ...,
+        NotBefore: TimestampTypeDef = ...,
+        NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChimeBearer: str = ...
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
@@ -1906,17 +1899,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_sip_media_application_logging_configuration)
         """
 
     def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: Union[
-            EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
-        ]
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Puts emergency calling configuration details to the specified Amazon Chime Voice
         Connector, such as emergency phone numbers and calling countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_emergency_calling_configuration)
@@ -1929,18 +1920,15 @@
         Adds a logging configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_logging_configuration)
         """
 
     def put_voice_connector_origination(
-        self,
-        *,
-        VoiceConnectorId: str,
-        Origination: Union[OriginationTypeDef, OriginationOutputTypeDef]
+        self, *, VoiceConnectorId: str, Origination: OriginationUnionTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Adds origination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_origination)
         """
@@ -1959,33 +1947,25 @@
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_proxy)
         """
 
     def put_voice_connector_streaming_configuration(
-        self,
-        *,
-        VoiceConnectorId: str,
-        StreamingConfiguration: Union[
-            StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
-        ]
+        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Adds a streaming configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_streaming_configuration)
         """
 
     def put_voice_connector_termination(
-        self,
-        *,
-        VoiceConnectorId: str,
-        Termination: Union[TerminationTypeDef, TerminationOutputTypeDef]
+        self, *, VoiceConnectorId: str, Termination: TerminationUnionTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Adds termination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_termination)
         """
```

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/client.pyi` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_chime.client import ChimeClient
 
     session = Session()
     client: ChimeClient = session.client("chime")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CapabilityType,
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
@@ -53,16 +52,15 @@
     BatchCreateRoomMembershipResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
     BatchUnsuspendUserResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     BatchUpdateUserResponseTypeDef,
     BusinessCallingSettingsTypeDef,
-    ChimeSdkMeetingConfigurationOutputTypeDef,
-    ChimeSdkMeetingConfigurationTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateAccountResponseTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeResponseTypeDef,
     CreateBotResponseTypeDef,
@@ -92,16 +90,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmergencyCallingConfigurationOutputTypeDef,
-    EmergencyCallingConfigurationTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetAccountResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
     GetAttendeeResponseTypeDef,
@@ -162,16 +159,15 @@
     ListUsersResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     LoggingConfigurationTypeDef,
     MeetingNotificationConfigurationTypeDef,
     MembershipItemTypeDef,
-    OriginationOutputTypeDef,
-    OriginationTypeDef,
+    OriginationUnionTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     PutRetentionSettingsResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
@@ -186,19 +182,18 @@
     RetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     SigninDelegateGroupTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
-    StreamingConfigurationOutputTypeDef,
-    StreamingConfigurationTypeDef,
+    StreamingConfigurationUnionTypeDef,
     TagTypeDef,
-    TerminationOutputTypeDef,
-    TerminationTypeDef,
+    TerminationUnionTypeDef,
+    TimestampTypeDef,
     TranscriptionConfigurationTypeDef,
     UpdateAccountResponseTypeDef,
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
@@ -517,17 +512,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: Union[
-            ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
-        ] = ...
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#create_media_capture_pipeline)
         """
@@ -1464,16 +1457,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_channel_memberships_for_app_instance_user)
         """
     def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         SortOrder: SortOrderType = ...,
-        NotBefore: Union[datetime, str] = ...,
-        NotAfter: Union[datetime, str] = ...,
+        NotBefore: TimestampTypeDef = ...,
+        NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChimeBearer: str = ...
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
@@ -1752,17 +1745,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_sip_media_application_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_sip_media_application_logging_configuration)
         """
     def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: Union[
-            EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
-        ]
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Puts emergency calling configuration details to the specified Amazon Chime Voice
         Connector, such as emergency phone numbers and calling countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_emergency_calling_configuration)
@@ -1773,18 +1764,15 @@
         """
         Adds a logging configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_logging_configuration)
         """
     def put_voice_connector_origination(
-        self,
-        *,
-        VoiceConnectorId: str,
-        Origination: Union[OriginationTypeDef, OriginationOutputTypeDef]
+        self, *, VoiceConnectorId: str, Origination: OriginationUnionTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Adds origination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_origination)
         """
@@ -1801,32 +1789,24 @@
         Puts the specified proxy configuration to the specified Amazon Chime Voice
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_proxy)
         """
     def put_voice_connector_streaming_configuration(
-        self,
-        *,
-        VoiceConnectorId: str,
-        StreamingConfiguration: Union[
-            StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
-        ]
+        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Adds a streaming configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_streaming_configuration)
         """
     def put_voice_connector_termination(
-        self,
-        *,
-        VoiceConnectorId: str,
-        Termination: Union[TerminationTypeDef, TerminationOutputTypeDef]
+        self, *, VoiceConnectorId: str, Termination: TerminationUnionTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Adds termination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_termination)
         """
```

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/literals.py` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/literals.pyi` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/paginator.py` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/paginator.pyi` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/type_defs.py` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_chime.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -220,15 +220,15 @@
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
-    "ListChannelMessagesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "ListMeetingTagsRequestRequestTypeDef",
     "ListMeetingsRequestRequestTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
@@ -411,23 +411,25 @@
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "InviteUsersResponseTypeDef",
     "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
+    "ListChannelMessagesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "TerminationUnionTypeDef",
     "RetentionSettingsTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
     "UserSettingsTypeDef",
     "CreateAccountResponseTypeDef",
@@ -471,28 +473,30 @@
     "UpdateSipRuleResponseTypeDef",
     "CreateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "EmergencyCallingConfigurationUnionTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
     "ListMeetingsResponseTypeDef",
     "CreateRoomMembershipResponseTypeDef",
     "ListRoomMembershipsResponseTypeDef",
     "UpdateRoomMembershipResponseTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
     "PutVoiceConnectorOriginationResponseTypeDef",
+    "OriginationUnionTypeDef",
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
@@ -502,17 +506,19 @@
     "PutRetentionSettingsRequestRequestTypeDef",
     "PutRetentionSettingsResponseTypeDef",
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    "StreamingConfigurationUnionTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
     "MediaCapturePipelineTypeDef",
+    "ChimeSdkMeetingConfigurationUnionTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
@@ -2342,41 +2348,15 @@
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_RequiredListChannelMessagesRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-    },
-)
-_OptionalListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_OptionalListChannelMessagesRequestRequestTypeDef",
-    {
-        "SortOrder": SortOrderType,
-        "NotBefore": Union[datetime, str],
-        "NotAfter": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "ChimeBearer": str,
-    },
-    total=False,
-)
-
-
-class ListChannelMessagesRequestRequestTypeDef(
-    _RequiredListChannelMessagesRequestRequestTypeDef,
-    _OptionalListChannelMessagesRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListChannelModeratorsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelModeratorsRequestRequestTypeDef",
     {
         "ChannelArn": str,
     },
 )
 _OptionalListChannelModeratorsRequestRequestTypeDef = TypedDict(
@@ -4651,14 +4631,41 @@
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
 
+_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_RequiredListChannelMessagesRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+    },
+)
+_OptionalListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_OptionalListChannelMessagesRequestRequestTypeDef",
+    {
+        "SortOrder": SortOrderType,
+        "NotBefore": TimestampTypeDef,
+        "NotAfter": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "ChimeBearer": str,
+    },
+    total=False,
+)
+
+
+class ListChannelMessagesRequestRequestTypeDef(
+    _RequiredListChannelMessagesRequestRequestTypeDef,
+    _OptionalListChannelMessagesRequestRequestTypeDef,
+):
+    pass
+
+
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4761,14 +4768,15 @@
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Termination": TerminationTypeDef,
     },
 )
 
+TerminationUnionTypeDef = Union[TerminationTypeDef, TerminationOutputTypeDef]
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
@@ -5236,14 +5244,17 @@
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EmergencyCallingConfigurationUnionTypeDef = Union[
+    EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
+]
 PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
     },
 )
@@ -5353,14 +5364,15 @@
     "PutVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OriginationUnionTypeDef = Union[OriginationTypeDef, OriginationOutputTypeDef]
 PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
     },
 )
@@ -5495,14 +5507,17 @@
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
     },
 )
 
+StreamingConfigurationUnionTypeDef = Union[
+    StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
+]
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "UserSettings": UserSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5528,14 +5543,17 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+ChimeSdkMeetingConfigurationUnionTypeDef = Union[
+    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+]
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
```

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/type_defs.pyi` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_chime.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -219,15 +219,15 @@
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
-    "ListChannelMessagesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "ListMeetingTagsRequestRequestTypeDef",
     "ListMeetingsRequestRequestTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
@@ -410,23 +410,25 @@
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "InviteUsersResponseTypeDef",
     "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
+    "ListChannelMessagesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "TerminationUnionTypeDef",
     "RetentionSettingsTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
     "UserSettingsTypeDef",
     "CreateAccountResponseTypeDef",
@@ -470,28 +472,30 @@
     "UpdateSipRuleResponseTypeDef",
     "CreateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "EmergencyCallingConfigurationUnionTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
     "ListMeetingsResponseTypeDef",
     "CreateRoomMembershipResponseTypeDef",
     "ListRoomMembershipsResponseTypeDef",
     "UpdateRoomMembershipResponseTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
     "PutVoiceConnectorOriginationResponseTypeDef",
+    "OriginationUnionTypeDef",
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
@@ -501,17 +505,19 @@
     "PutRetentionSettingsRequestRequestTypeDef",
     "PutRetentionSettingsResponseTypeDef",
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    "StreamingConfigurationUnionTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
     "MediaCapturePipelineTypeDef",
+    "ChimeSdkMeetingConfigurationUnionTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
@@ -2269,39 +2275,15 @@
 
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_RequiredListChannelMessagesRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-    },
-)
-_OptionalListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_OptionalListChannelMessagesRequestRequestTypeDef",
-    {
-        "SortOrder": SortOrderType,
-        "NotBefore": Union[datetime, str],
-        "NotAfter": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "ChimeBearer": str,
-    },
-    total=False,
-)
-
-class ListChannelMessagesRequestRequestTypeDef(
-    _RequiredListChannelMessagesRequestRequestTypeDef,
-    _OptionalListChannelMessagesRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListChannelModeratorsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelModeratorsRequestRequestTypeDef",
     {
         "ChannelArn": str,
     },
 )
 _OptionalListChannelModeratorsRequestRequestTypeDef = TypedDict(
@@ -4498,14 +4480,39 @@
 
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
+_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_RequiredListChannelMessagesRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+    },
+)
+_OptionalListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_OptionalListChannelMessagesRequestRequestTypeDef",
+    {
+        "SortOrder": SortOrderType,
+        "NotBefore": TimestampTypeDef,
+        "NotAfter": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "ChimeBearer": str,
+    },
+    total=False,
+)
+
+class ListChannelMessagesRequestRequestTypeDef(
+    _RequiredListChannelMessagesRequestRequestTypeDef,
+    _OptionalListChannelMessagesRequestRequestTypeDef,
+):
+    pass
+
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4608,14 +4615,15 @@
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Termination": TerminationTypeDef,
     },
 )
 
+TerminationUnionTypeDef = Union[TerminationTypeDef, TerminationOutputTypeDef]
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
@@ -5077,14 +5085,17 @@
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EmergencyCallingConfigurationUnionTypeDef = Union[
+    EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
+]
 PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
     },
 )
@@ -5194,14 +5205,15 @@
     "PutVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OriginationUnionTypeDef = Union[OriginationTypeDef, OriginationOutputTypeDef]
 PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
     },
 )
@@ -5336,14 +5348,17 @@
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
     },
 )
 
+StreamingConfigurationUnionTypeDef = Union[
+    StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
+]
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "UserSettings": UserSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5369,14 +5384,17 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+ChimeSdkMeetingConfigurationUnionTypeDef = Union[
+    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+]
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
```

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/PKG-INFO` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Chime 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 chime type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime)](https://pepy.tech/project/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
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
@@ -361,20 +361,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_chime.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_chime.type_defs import (
     AccountSettingsTypeDef,
     SigninDelegateGroupTypeDef,
     AddressTypeDef,
     AlexaForBusinessMetadataTypeDef,
@@ -523,15 +523,15 @@
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     ListMeetingTagsRequestRequestTypeDef,
     ListMeetingsRequestRequestTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
@@ -714,23 +714,25 @@
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     InviteUsersResponseTypeDef,
     ListAccountsRequestListAccountsPaginateTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
+    TerminationUnionTypeDef,
     RetentionSettingsTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     UserSettingsTypeDef,
     CreateAccountResponseTypeDef,
@@ -774,28 +776,30 @@
     UpdateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
     ListMeetingsResponseTypeDef,
     CreateRoomMembershipResponseTypeDef,
     ListRoomMembershipsResponseTypeDef,
     UpdateRoomMembershipResponseTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
+    OriginationUnionTypeDef,
     PutVoiceConnectorOriginationRequestRequestTypeDef,
     CreateProxySessionResponseTypeDef,
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
@@ -805,25 +809,27 @@
     PutRetentionSettingsRequestRequestTypeDef,
     PutRetentionSettingsResponseTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
+    StreamingConfigurationUnionTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/SOURCES.txt` & `mypy-boto3-chime-1.28.16/mypy_boto3_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15.post1/setup.py` & `mypy-boto3-chime-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Chime 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 chime type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 chime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_chime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

