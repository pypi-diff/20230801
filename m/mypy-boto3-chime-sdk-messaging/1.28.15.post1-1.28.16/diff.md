# Comparing `tmp/mypy-boto3-chime-sdk-messaging-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-chime-sdk-messaging-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:40 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.28.16.tar", last modified: Tue Aug  1 11:36:21 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1.tar` & `mypy-boto3-chime-sdk-messaging-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:40.285045 mypy-boto3-chime-sdk-messaging-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:31.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-07-29 10:02:40.273045 mypy-boto3-chime-sdk-messaging-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16833 2023-07-29 09:39:31.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:40.269045 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-29 09:39:31.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-29 09:39:31.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-29 09:39:31.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38288 2023-07-29 09:39:32.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38231 2023-07-29 09:39:32.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-29 09:39:32.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-29 09:39:32.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:31.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47836 2023-07-29 09:39:34.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47779 2023-07-29 09:39:34.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:31.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:40.273045 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:40.285045 mypy-boto3-chime-sdk-messaging-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-29 09:39:31.000000 mypy-boto3-chime-sdk-messaging-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:21.728934 mypy-boto3-chime-sdk-messaging-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:12:04.000000 mypy-boto3-chime-sdk-messaging-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-08-01 11:36:21.724934 mypy-boto3-chime-sdk-messaging-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16893 2023-08-01 11:12:04.000000 mypy-boto3-chime-sdk-messaging-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:21.724934 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-01 11:12:04.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 11:12:04.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 11:12:04.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38170 2023-08-01 11:12:05.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38113 2023-08-01 11:12:04.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-08-01 11:12:05.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-08-01 11:12:05.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:12:04.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47985 2023-08-01 11:12:07.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47928 2023-08-01 11:12:06.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:12:04.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:21.724934 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-08-01 11:36:21.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-01 11:36:21.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:21.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:21.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:21.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 11:36:21.000000 mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:21.728934 mypy-boto3-chime-sdk-messaging-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-01 11:12:04.000000 mypy-boto3-chime-sdk-messaging-1.28.16/setup.py
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/LICENSE` & `mypy-boto3-chime-sdk-messaging-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime-sdk-messaging type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 chime-sdk-messaging type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-messaging)](https://pepy.tech/project/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
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
@@ -304,20 +304,20 @@
 )
 
 
 def check_value(value: AllowNotificationsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_chime_sdk_messaging.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
@@ -359,15 +359,15 @@
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
     StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
@@ -401,28 +401,29 @@
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
     PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     ProcessorConfigurationTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSubChannelsResponseTypeDef,
     SearchChannelsRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
@@ -432,28 +433,29 @@
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
     PutChannelMembershipPreferencesRequestRequestTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
 )
 
 
-def get_structure() -> AppInstanceUserMembershipSummaryTypeDef:
+def get_value() -> AppInstanceUserMembershipSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/README.md` & `mypy-boto3-chime-sdk-messaging-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-messaging)](https://pepy.tech/project/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
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
@@ -272,20 +272,20 @@
 )
 
 
 def check_value(value: AllowNotificationsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_chime_sdk_messaging.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
@@ -327,15 +327,15 @@
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
     StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
@@ -369,28 +369,29 @@
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
     PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     ProcessorConfigurationTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSubChannelsResponseTypeDef,
     SearchChannelsRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
@@ -400,28 +401,29 @@
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
     PutChannelMembershipPreferencesRequestRequestTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
 )
 
 
-def get_structure() -> AppInstanceUserMembershipSummaryTypeDef:
+def get_value() -> AppInstanceUserMembershipSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/__main__.py` & `mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMessaging 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMessaging 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging\nOther"
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

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/client.py` & `mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_chime_sdk_messaging.client import ChimeSDKMessagingClient
 
     session = Session()
     client: ChimeSDKMessagingClient = session.client("chime-sdk-messaging")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
     ChannelMessageTypeType,
@@ -58,28 +57,28 @@
     ListChannelMessagesResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListSubChannelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MessageAttributeValueOutputTypeDef,
-    MessageAttributeValueTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ProcessorTypeDef,
     PushNotificationConfigurationTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
     SearchFieldTypeDef,
     SendChannelMessageResponseTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
     TargetTypeDef,
+    TimestampTypeDef,
     UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 __all__ = ("ChimeSDKMessagingClient",)
@@ -520,16 +519,16 @@
 
     def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         SortOrder: SortOrderType = ...,
-        NotBefore: Union[datetime, str] = ...,
-        NotAfter: Union[datetime, str] = ...,
+        NotBefore: TimestampTypeDef = ...,
+        NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SubChannelId: str = ...
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
@@ -681,17 +680,15 @@
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
-        MessageAttributes: Mapping[
-            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
-        ] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
         SubChannelId: str = ...,
         ContentType: str = ...,
         Target: Sequence[TargetTypeDef] = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/client.pyi` & `mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_chime_sdk_messaging.client import ChimeSDKMessagingClient
 
     session = Session()
     client: ChimeSDKMessagingClient = session.client("chime-sdk-messaging")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
     ChannelMessageTypeType,
@@ -58,28 +57,28 @@
     ListChannelMessagesResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListSubChannelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MessageAttributeValueOutputTypeDef,
-    MessageAttributeValueTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ProcessorTypeDef,
     PushNotificationConfigurationTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
     SearchFieldTypeDef,
     SendChannelMessageResponseTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
     TargetTypeDef,
+    TimestampTypeDef,
     UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 __all__ = ("ChimeSDKMessagingClient",)
@@ -481,16 +480,16 @@
         """
     def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         SortOrder: SortOrderType = ...,
-        NotBefore: Union[datetime, str] = ...,
-        NotAfter: Union[datetime, str] = ...,
+        NotBefore: TimestampTypeDef = ...,
+        NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SubChannelId: str = ...
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
@@ -630,17 +629,15 @@
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
-        MessageAttributes: Mapping[
-            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
-        ] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
         SubChannelId: str = ...,
         ContentType: str = ...,
         Target: Sequence[TargetTypeDef] = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/literals.py` & `mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/literals.pyi` & `mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/type_defs.py` & `mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_chime_sdk_messaging.type_defs import AppInstanceUserMembershipSummaryTypeDef
 
-    data: AppInstanceUserMembershipSummaryTypeDef = {...}
+    data: AppInstanceUserMembershipSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -85,15 +85,15 @@
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     "StreamingConfigurationTypeDef",
     "LambdaConfigurationTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelFlowsRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
-    "ListChannelMessagesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -127,28 +127,29 @@
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
+    "MessageAttributeValueUnionTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
     "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
     "ProcessorConfigurationTypeDef",
+    "ListChannelMessagesRequestRequestTypeDef",
     "ListSubChannelsResponseTypeDef",
     "SearchChannelsRequestRequestTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
@@ -158,14 +159,15 @@
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "PutChannelMembershipPreferencesResponseTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
@@ -755,42 +757,15 @@
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_RequiredListChannelMessagesRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "ChimeBearer": str,
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
-        "SubChannelId": str,
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
         "ChimeBearer": str,
     },
 )
@@ -1291,14 +1266,17 @@
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MessageAttributeValueUnionTypeDef = Union[
+    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
+]
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
         "Content": str,
         "Metadata": str,
         "Type": ChannelMessageTypeType,
@@ -1334,48 +1312,14 @@
         "SubChannelId": str,
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[
-            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
-        ],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
-
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -1506,14 +1450,42 @@
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
     },
 )
 
+_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_RequiredListChannelMessagesRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "ChimeBearer": str,
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
+        "SubChannelId": str,
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
 ListSubChannelsResponseTypeDef = TypedDict(
     "ListSubChannelsResponseTypeDef",
     {
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1690,14 +1662,46 @@
 class ChannelFlowCallbackRequestRequestTypeDef(
     _RequiredChannelFlowCallbackRequestRequestTypeDef,
     _OptionalChannelFlowCallbackRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
+    },
+    total=False,
+)
+
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
+
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging/type_defs.pyi` & `mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_chime_sdk_messaging.type_defs import AppInstanceUserMembershipSummaryTypeDef
 
-    data: AppInstanceUserMembershipSummaryTypeDef = {...}
+    data: AppInstanceUserMembershipSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -84,15 +84,15 @@
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     "StreamingConfigurationTypeDef",
     "LambdaConfigurationTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelFlowsRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
-    "ListChannelMessagesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -126,28 +126,29 @@
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
+    "MessageAttributeValueUnionTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
     "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
     "ProcessorConfigurationTypeDef",
+    "ListChannelMessagesRequestRequestTypeDef",
     "ListSubChannelsResponseTypeDef",
     "SearchChannelsRequestRequestTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
@@ -157,14 +158,15 @@
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "PutChannelMembershipPreferencesResponseTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
@@ -730,40 +732,15 @@
 
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_RequiredListChannelMessagesRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "ChimeBearer": str,
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
-        "SubChannelId": str,
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
         "ChimeBearer": str,
     },
 )
@@ -1246,14 +1223,17 @@
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MessageAttributeValueUnionTypeDef = Union[
+    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
+]
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
         "Content": str,
         "Metadata": str,
         "Type": ChannelMessageTypeType,
@@ -1289,46 +1269,14 @@
         "SubChannelId": str,
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[
-            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
-        ],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -1455,14 +1403,40 @@
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
     },
 )
 
+_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_RequiredListChannelMessagesRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "ChimeBearer": str,
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
+        "SubChannelId": str,
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
 ListSubChannelsResponseTypeDef = TypedDict(
     "ListSubChannelsResponseTypeDef",
     {
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1635,14 +1609,44 @@
 
 class ChannelFlowCallbackRequestRequestTypeDef(
     _RequiredChannelFlowCallbackRequestRequestTypeDef,
     _OptionalChannelFlowCallbackRequestRequestTypeDef,
 ):
     pass
 
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
+    },
+    total=False,
+)
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime-sdk-messaging type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 chime-sdk-messaging type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-messaging)](https://pepy.tech/project/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
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
@@ -304,20 +304,20 @@
 )
 
 
 def check_value(value: AllowNotificationsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_chime_sdk_messaging.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
@@ -359,15 +359,15 @@
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
     StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
@@ -401,28 +401,29 @@
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
     PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     ProcessorConfigurationTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSubChannelsResponseTypeDef,
     SearchChannelsRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
@@ -432,28 +433,29 @@
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
     PutChannelMembershipPreferencesRequestRequestTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
 )
 
 
-def get_structure() -> AppInstanceUserMembershipSummaryTypeDef:
+def get_value() -> AppInstanceUserMembershipSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-messaging-1.28.16/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.15.post1/setup.py` & `mypy-boto3-chime-sdk-messaging-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-messaging",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_chime_sdk_messaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMessaging 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ChimeSDKMessaging 1.28.16 service generated with"
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
-    keywords="boto3 chime-sdk-messaging type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 chime-sdk-messaging type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_chime_sdk_messaging": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/"
```

