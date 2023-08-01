# Comparing `tmp/mypy-boto3-pinpoint-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-pinpoint-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:53 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-1.28.16.tar", last modified: Tue Aug  1 11:37:33 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-1.28.15.post1.tar` & `mypy-boto3-pinpoint-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:53.357338 mypy-boto3-pinpoint-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-07-29 10:03:53.357338 mypy-boto3-pinpoint-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28667 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:53.353338 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79811 2023-07-29 09:53:09.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79683 2023-07-29 09:53:09.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-29 09:53:09.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-29 09:53:09.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   170188 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   169965 2023-07-29 09:53:15.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:53.357338 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:53.357338 mypy-boto3-pinpoint-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:33.900787 mypy-boto3-pinpoint-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:11.000000 mypy-boto3-pinpoint-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-08-01 11:37:33.900787 mypy-boto3-pinpoint-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-08-01 11:26:11.000000 mypy-boto3-pinpoint-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:33.888787 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 11:26:11.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 11:26:11.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:26:11.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79723 2023-08-01 11:26:12.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79595 2023-08-01 11:26:11.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-08-01 11:26:12.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-08-01 11:26:12.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:11.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   170364 2023-08-01 11:26:19.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170141 2023-08-01 11:26:14.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:11.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:33.900787 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:33.900787 mypy-boto3-pinpoint-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:26:11.000000 mypy-boto3-pinpoint-1.28.16/setup.py
```

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/LICENSE` & `mypy-boto3-pinpoint-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/PKG-INFO` & `mypy-boto3-pinpoint-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Pinpoint 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pinpoint type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pinpoint type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: ActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pinpoint.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint.type_defs import (
     ADMChannelRequestTypeDef,
     ADMChannelResponseTypeDef,
     ADMMessageTypeDef,
     APNSChannelRequestTypeDef,
@@ -352,14 +352,15 @@
     QuietTimeTypeDef,
     AttributeDimensionOutputTypeDef,
     AttributeDimensionTypeDef,
     AttributesResourceTypeDef,
     BaiduChannelRequestTypeDef,
     BaiduChannelResponseTypeDef,
     BaiduMessageTypeDef,
+    BlobTypeDef,
     CampaignCustomMessageTypeDef,
     CampaignEmailMessageTypeDef,
     CampaignStateTypeDef,
     CustomDeliveryConfigurationOutputTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
@@ -411,15 +412,14 @@
     VoiceChannelResponseTypeDef,
     DeleteVoiceTemplateRequestRequestTypeDef,
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
-    RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointUserOutputTypeDef,
@@ -434,20 +434,19 @@
     GPSCoordinatesTypeDef,
     GetAdmChannelRequestRequestTypeDef,
     GetApnsChannelRequestRequestTypeDef,
     GetApnsSandboxChannelRequestRequestTypeDef,
     GetApnsVoipChannelRequestRequestTypeDef,
     GetApnsVoipSandboxChannelRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
-    GetApplicationDateRangeKpiRequestRequestTypeDef,
+    TimestampTypeDef,
     GetApplicationSettingsRequestRequestTypeDef,
     GetAppsRequestRequestTypeDef,
     GetBaiduChannelRequestRequestTypeDef,
     GetCampaignActivitiesRequestRequestTypeDef,
-    GetCampaignDateRangeKpiRequestRequestTypeDef,
     GetCampaignRequestRequestTypeDef,
     GetCampaignVersionRequestRequestTypeDef,
     GetCampaignVersionsRequestRequestTypeDef,
     GetCampaignsRequestRequestTypeDef,
     GetChannelsRequestRequestTypeDef,
     GetEmailChannelRequestRequestTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
@@ -456,15 +455,14 @@
     GetExportJobRequestRequestTypeDef,
     GetExportJobsRequestRequestTypeDef,
     GetGcmChannelRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetImportJobsRequestRequestTypeDef,
     GetInAppMessagesRequestRequestTypeDef,
     GetInAppTemplateRequestRequestTypeDef,
-    GetJourneyDateRangeKpiRequestRequestTypeDef,
     GetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     JourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsRequestRequestTypeDef,
     JourneyExecutionMetricsResponseTypeDef,
     GetJourneyRequestRequestTypeDef,
     GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
     JourneyRunExecutionActivityMetricsResponseTypeDef,
@@ -492,15 +490,14 @@
     OverrideButtonConfigurationTypeDef,
     InAppMessageHeaderConfigTypeDef,
     JourneyChannelSettingsTypeDef,
     JourneyPushMessageTypeDef,
     JourneyScheduleOutputTypeDef,
     JourneyRunResponseTypeDef,
     JourneySMSMessageTypeDef,
-    JourneyScheduleTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagsModelOutputTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
     MessageTypeDef,
@@ -535,14 +532,15 @@
     UpdateApnsVoipChannelRequestRequestTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
     ApplicationSettingsJourneyLimitsTypeDef,
     JourneyLimitsTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
+    RawEmailTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysOutputTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppResponseTypeDef,
     DeleteAdmChannelResponseTypeDef,
@@ -631,14 +629,18 @@
     EventDimensionsTypeDef,
     SegmentDemographicsTypeDef,
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
     GPSPointDimensionTypeDef,
+    GetApplicationDateRangeKpiRequestRequestTypeDef,
+    GetCampaignDateRangeKpiRequestRequestTypeDef,
+    GetJourneyDateRangeKpiRequestRequestTypeDef,
+    JourneyScheduleTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyRunExecutionActivityMetricsResponseTypeDef,
     GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
@@ -659,14 +661,15 @@
     SegmentBehaviorsTypeDef,
     RemoveAttributesRequestRequestTypeDef,
     ResultRowTypeDef,
     UpdateSmsChannelRequestRequestTypeDef,
     SendOTPMessageRequestRequestTypeDef,
     SimpleEmailTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagsModelUnionTypeDef,
     UpdateTemplateActiveVersionRequestRequestTypeDef,
     TemplateConfigurationTypeDef,
     TemplatesResponseTypeDef,
     TemplateVersionsResponseTypeDef,
     UpdateRecommenderConfigurationRequestRequestTypeDef,
     UpdateVoiceChannelRequestRequestTypeDef,
     VerifyOTPMessageResponseTypeDef,
@@ -808,15 +811,15 @@
     UpdateJourneyStateResponseTypeDef,
     CreateJourneyRequestRequestTypeDef,
     UpdateJourneyRequestRequestTypeDef,
     ListJourneysResponseTypeDef,
 )
 
 
-def get_structure() -> ADMChannelRequestTypeDef:
+def get_value() -> ADMChannelRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/README.md` & `mypy-boto3-pinpoint-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
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
@@ -282,20 +282,20 @@
 )
 
 
 def check_value(value: ActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pinpoint.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint.type_defs import (
     ADMChannelRequestTypeDef,
     ADMChannelResponseTypeDef,
     ADMMessageTypeDef,
     APNSChannelRequestTypeDef,
@@ -320,14 +320,15 @@
     QuietTimeTypeDef,
     AttributeDimensionOutputTypeDef,
     AttributeDimensionTypeDef,
     AttributesResourceTypeDef,
     BaiduChannelRequestTypeDef,
     BaiduChannelResponseTypeDef,
     BaiduMessageTypeDef,
+    BlobTypeDef,
     CampaignCustomMessageTypeDef,
     CampaignEmailMessageTypeDef,
     CampaignStateTypeDef,
     CustomDeliveryConfigurationOutputTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
@@ -379,15 +380,14 @@
     VoiceChannelResponseTypeDef,
     DeleteVoiceTemplateRequestRequestTypeDef,
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
-    RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointUserOutputTypeDef,
@@ -402,20 +402,19 @@
     GPSCoordinatesTypeDef,
     GetAdmChannelRequestRequestTypeDef,
     GetApnsChannelRequestRequestTypeDef,
     GetApnsSandboxChannelRequestRequestTypeDef,
     GetApnsVoipChannelRequestRequestTypeDef,
     GetApnsVoipSandboxChannelRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
-    GetApplicationDateRangeKpiRequestRequestTypeDef,
+    TimestampTypeDef,
     GetApplicationSettingsRequestRequestTypeDef,
     GetAppsRequestRequestTypeDef,
     GetBaiduChannelRequestRequestTypeDef,
     GetCampaignActivitiesRequestRequestTypeDef,
-    GetCampaignDateRangeKpiRequestRequestTypeDef,
     GetCampaignRequestRequestTypeDef,
     GetCampaignVersionRequestRequestTypeDef,
     GetCampaignVersionsRequestRequestTypeDef,
     GetCampaignsRequestRequestTypeDef,
     GetChannelsRequestRequestTypeDef,
     GetEmailChannelRequestRequestTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
@@ -424,15 +423,14 @@
     GetExportJobRequestRequestTypeDef,
     GetExportJobsRequestRequestTypeDef,
     GetGcmChannelRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetImportJobsRequestRequestTypeDef,
     GetInAppMessagesRequestRequestTypeDef,
     GetInAppTemplateRequestRequestTypeDef,
-    GetJourneyDateRangeKpiRequestRequestTypeDef,
     GetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     JourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsRequestRequestTypeDef,
     JourneyExecutionMetricsResponseTypeDef,
     GetJourneyRequestRequestTypeDef,
     GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
     JourneyRunExecutionActivityMetricsResponseTypeDef,
@@ -460,15 +458,14 @@
     OverrideButtonConfigurationTypeDef,
     InAppMessageHeaderConfigTypeDef,
     JourneyChannelSettingsTypeDef,
     JourneyPushMessageTypeDef,
     JourneyScheduleOutputTypeDef,
     JourneyRunResponseTypeDef,
     JourneySMSMessageTypeDef,
-    JourneyScheduleTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagsModelOutputTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
     MessageTypeDef,
@@ -503,14 +500,15 @@
     UpdateApnsVoipChannelRequestRequestTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
     ApplicationSettingsJourneyLimitsTypeDef,
     JourneyLimitsTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
+    RawEmailTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysOutputTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppResponseTypeDef,
     DeleteAdmChannelResponseTypeDef,
@@ -599,14 +597,18 @@
     EventDimensionsTypeDef,
     SegmentDemographicsTypeDef,
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
     GPSPointDimensionTypeDef,
+    GetApplicationDateRangeKpiRequestRequestTypeDef,
+    GetCampaignDateRangeKpiRequestRequestTypeDef,
+    GetJourneyDateRangeKpiRequestRequestTypeDef,
+    JourneyScheduleTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyRunExecutionActivityMetricsResponseTypeDef,
     GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
@@ -627,14 +629,15 @@
     SegmentBehaviorsTypeDef,
     RemoveAttributesRequestRequestTypeDef,
     ResultRowTypeDef,
     UpdateSmsChannelRequestRequestTypeDef,
     SendOTPMessageRequestRequestTypeDef,
     SimpleEmailTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagsModelUnionTypeDef,
     UpdateTemplateActiveVersionRequestRequestTypeDef,
     TemplateConfigurationTypeDef,
     TemplatesResponseTypeDef,
     TemplateVersionsResponseTypeDef,
     UpdateRecommenderConfigurationRequestRequestTypeDef,
     UpdateVoiceChannelRequestRequestTypeDef,
     VerifyOTPMessageResponseTypeDef,
@@ -776,15 +779,15 @@
     UpdateJourneyStateResponseTypeDef,
     CreateJourneyRequestRequestTypeDef,
     UpdateJourneyRequestRequestTypeDef,
     ListJourneysResponseTypeDef,
 )
 
 
-def get_structure() -> ADMChannelRequestTypeDef:
+def get_value() -> ADMChannelRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/__main__.py` & `mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pinpoint 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Pinpoint 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\nOther"
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

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/client.py` & `mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_pinpoint.client import PinpointClient
 
     session = Session()
     client: PinpointClient = session.client("pinpoint")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     ADMChannelRequestTypeDef,
     APNSChannelRequestTypeDef,
     APNSSandboxChannelRequestTypeDef,
@@ -136,17 +135,17 @@
     SendMessagesResponseTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SendOTPMessageResponseTypeDef,
     SendUsersMessageRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     SMSChannelRequestTypeDef,
     SMSTemplateRequestTypeDef,
-    TagsModelOutputTypeDef,
-    TagsModelTypeDef,
+    TagsModelUnionTypeDef,
     TemplateActiveVersionRequestTypeDef,
+    TimestampTypeDef,
     UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelResponseTypeDef,
     UpdateApplicationSettingsResponseTypeDef,
     UpdateAttributesRequestTypeDef,
@@ -656,18 +655,18 @@
         """
 
     def get_application_date_range_kpi(
         self,
         *,
         ApplicationId: str,
         KpiName: str,
-        EndTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: Union[datetime, str] = ...
+        StartTime: TimestampTypeDef = ...
     ) -> GetApplicationDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_application_date_range_kpi)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_application_date_range_kpi)
@@ -722,18 +721,18 @@
 
     def get_campaign_date_range_kpi(
         self,
         *,
         ApplicationId: str,
         CampaignId: str,
         KpiName: str,
-        EndTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: Union[datetime, str] = ...
+        StartTime: TimestampTypeDef = ...
     ) -> GetCampaignDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to a
         campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_date_range_kpi)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_campaign_date_range_kpi)
@@ -899,18 +898,18 @@
 
     def get_journey_date_range_kpi(
         self,
         *,
         ApplicationId: str,
         JourneyId: str,
         KpiName: str,
-        EndTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: Union[datetime, str] = ...
+        StartTime: TimestampTypeDef = ...
     ) -> GetJourneyDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard engagement metric that
         applies to a journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_date_range_kpi)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_date_range_kpi)
@@ -1261,15 +1260,15 @@
         Creates and sends a message to a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_users_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_users_messages)
         """
 
     def tag_resource(
-        self, *, ResourceArn: str, TagsModel: Union[TagsModelTypeDef, TagsModelOutputTypeDef]
+        self, *, ResourceArn: str, TagsModel: TagsModelUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds one or more tags (keys and values) to an application, campaign, message
         template, or segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#tag_resource)
```

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/client.pyi` & `mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_pinpoint.client import PinpointClient
 
     session = Session()
     client: PinpointClient = session.client("pinpoint")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     ADMChannelRequestTypeDef,
     APNSChannelRequestTypeDef,
     APNSSandboxChannelRequestTypeDef,
@@ -136,17 +135,17 @@
     SendMessagesResponseTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SendOTPMessageResponseTypeDef,
     SendUsersMessageRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     SMSChannelRequestTypeDef,
     SMSTemplateRequestTypeDef,
-    TagsModelOutputTypeDef,
-    TagsModelTypeDef,
+    TagsModelUnionTypeDef,
     TemplateActiveVersionRequestTypeDef,
+    TimestampTypeDef,
     UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelResponseTypeDef,
     UpdateApplicationSettingsResponseTypeDef,
     UpdateAttributesRequestTypeDef,
@@ -608,18 +607,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_app)
         """
     def get_application_date_range_kpi(
         self,
         *,
         ApplicationId: str,
         KpiName: str,
-        EndTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: Union[datetime, str] = ...
+        StartTime: TimestampTypeDef = ...
     ) -> GetApplicationDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_application_date_range_kpi)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_application_date_range_kpi)
@@ -668,18 +667,18 @@
         """
     def get_campaign_date_range_kpi(
         self,
         *,
         ApplicationId: str,
         CampaignId: str,
         KpiName: str,
-        EndTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: Union[datetime, str] = ...
+        StartTime: TimestampTypeDef = ...
     ) -> GetCampaignDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to a
         campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_date_range_kpi)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_campaign_date_range_kpi)
@@ -828,18 +827,18 @@
         """
     def get_journey_date_range_kpi(
         self,
         *,
         ApplicationId: str,
         JourneyId: str,
         KpiName: str,
-        EndTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: Union[datetime, str] = ...
+        StartTime: TimestampTypeDef = ...
     ) -> GetJourneyDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard engagement metric that
         applies to a journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_date_range_kpi)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_date_range_kpi)
@@ -1159,15 +1158,15 @@
         """
         Creates and sends a message to a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_users_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_users_messages)
         """
     def tag_resource(
-        self, *, ResourceArn: str, TagsModel: Union[TagsModelTypeDef, TagsModelOutputTypeDef]
+        self, *, ResourceArn: str, TagsModel: TagsModelUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds one or more tags (keys and values) to an application, campaign, message
         template, or segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#tag_resource)
```

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/literals.py` & `mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/literals.pyi` & `mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/type_defs.py` & `mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pinpoint.type_defs import ADMChannelRequestTypeDef
 
-    data: ADMChannelRequestTypeDef = {...}
+    data: ADMChannelRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -80,14 +80,15 @@
     "QuietTimeTypeDef",
     "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
+    "BlobTypeDef",
     "CampaignCustomMessageTypeDef",
     "CampaignEmailMessageTypeDef",
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationOutputTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
@@ -139,15 +140,14 @@
     "VoiceChannelResponseTypeDef",
     "DeleteVoiceTemplateRequestRequestTypeDef",
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
-    "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointUserOutputTypeDef",
@@ -162,20 +162,19 @@
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
     "GetApnsChannelRequestRequestTypeDef",
     "GetApnsSandboxChannelRequestRequestTypeDef",
     "GetApnsVoipChannelRequestRequestTypeDef",
     "GetApnsVoipSandboxChannelRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
-    "GetApplicationDateRangeKpiRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetApplicationSettingsRequestRequestTypeDef",
     "GetAppsRequestRequestTypeDef",
     "GetBaiduChannelRequestRequestTypeDef",
     "GetCampaignActivitiesRequestRequestTypeDef",
-    "GetCampaignDateRangeKpiRequestRequestTypeDef",
     "GetCampaignRequestRequestTypeDef",
     "GetCampaignVersionRequestRequestTypeDef",
     "GetCampaignVersionsRequestRequestTypeDef",
     "GetCampaignsRequestRequestTypeDef",
     "GetChannelsRequestRequestTypeDef",
     "GetEmailChannelRequestRequestTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
@@ -184,15 +183,14 @@
     "GetExportJobRequestRequestTypeDef",
     "GetExportJobsRequestRequestTypeDef",
     "GetGcmChannelRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
     "GetImportJobsRequestRequestTypeDef",
     "GetInAppMessagesRequestRequestTypeDef",
     "GetInAppTemplateRequestRequestTypeDef",
-    "GetJourneyDateRangeKpiRequestRequestTypeDef",
     "GetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     "JourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsRequestRequestTypeDef",
     "JourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRequestRequestTypeDef",
     "GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef",
     "JourneyRunExecutionActivityMetricsResponseTypeDef",
@@ -220,15 +218,14 @@
     "OverrideButtonConfigurationTypeDef",
     "InAppMessageHeaderConfigTypeDef",
     "JourneyChannelSettingsTypeDef",
     "JourneyPushMessageTypeDef",
     "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
     "JourneySMSMessageTypeDef",
-    "JourneyScheduleTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagsModelOutputTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "MessageTypeDef",
@@ -263,14 +260,15 @@
     "UpdateApnsVoipChannelRequestRequestTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
     "ApplicationSettingsJourneyLimitsTypeDef",
     "JourneyLimitsTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
+    "RawEmailTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "DeleteAdmChannelResponseTypeDef",
@@ -359,14 +357,18 @@
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
     "GPSPointDimensionTypeDef",
+    "GetApplicationDateRangeKpiRequestRequestTypeDef",
+    "GetCampaignDateRangeKpiRequestRequestTypeDef",
+    "GetJourneyDateRangeKpiRequestRequestTypeDef",
+    "JourneyScheduleTypeDef",
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     "GetSmsTemplateResponseTypeDef",
     "GetVoiceTemplateResponseTypeDef",
     "ImportJobResponseTypeDef",
@@ -387,14 +389,15 @@
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagsModelUnionTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
@@ -1120,14 +1123,15 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CampaignCustomMessageTypeDef = TypedDict(
     "CampaignCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
@@ -1988,22 +1992,14 @@
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
 )
 
-RawEmailTypeDef = TypedDict(
-    "RawEmailTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 _RequiredEmailTemplateResponseTypeDef = TypedDict(
     "_RequiredEmailTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2282,40 +2278,15 @@
 GetAppRequestRequestTypeDef = TypedDict(
     "GetAppRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-_RequiredGetApplicationDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_RequiredGetApplicationDateRangeKpiRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "KpiName": str,
-    },
-)
-_OptionalGetApplicationDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_OptionalGetApplicationDateRangeKpiRequestRequestTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": str,
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GetApplicationDateRangeKpiRequestRequestTypeDef(
-    _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
-    _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 GetApplicationSettingsRequestRequestTypeDef = TypedDict(
     "GetApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2355,41 +2326,14 @@
 class GetCampaignActivitiesRequestRequestTypeDef(
     _RequiredGetCampaignActivitiesRequestRequestTypeDef,
     _OptionalGetCampaignActivitiesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "CampaignId": str,
-        "KpiName": str,
-    },
-)
-_OptionalGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_OptionalGetCampaignDateRangeKpiRequestRequestTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": str,
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GetCampaignDateRangeKpiRequestRequestTypeDef(
-    _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
-    _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
-):
-    pass
-
-
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
     },
 )
@@ -2591,41 +2535,14 @@
 
 class GetInAppTemplateRequestRequestTypeDef(
     _RequiredGetInAppTemplateRequestRequestTypeDef, _OptionalGetInAppTemplateRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "JourneyId": str,
-        "KpiName": str,
-    },
-)
-_OptionalGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_OptionalGetJourneyDateRangeKpiRequestRequestTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": str,
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GetJourneyDateRangeKpiRequestRequestTypeDef(
-    _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
-    _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
     },
@@ -3183,24 +3100,14 @@
         "SenderId": str,
         "EntityId": str,
         "TemplateId": str,
     },
     total=False,
 )
 
-JourneyScheduleTypeDef = TypedDict(
-    "JourneyScheduleTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
-        "Timezone": str,
-    },
-    total=False,
-)
-
 JourneyStateRequestTypeDef = TypedDict(
     "JourneyStateRequestTypeDef",
     {
         "State": StateType,
     },
     total=False,
 )
@@ -3732,14 +3639,22 @@
     "UpdateBaiduChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
+RawEmailTypeDef = TypedDict(
+    "RawEmailTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+    total=False,
+)
+
 ChannelsResponseTypeDef = TypedDict(
     "ChannelsResponseTypeDef",
     {
         "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
@@ -4744,14 +4659,104 @@
 
 class GPSPointDimensionTypeDef(
     _RequiredGPSPointDimensionTypeDef, _OptionalGPSPointDimensionTypeDef
 ):
     pass
 
 
+_RequiredGetApplicationDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_RequiredGetApplicationDateRangeKpiRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "KpiName": str,
+    },
+)
+_OptionalGetApplicationDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_OptionalGetApplicationDateRangeKpiRequestRequestTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": str,
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GetApplicationDateRangeKpiRequestRequestTypeDef(
+    _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
+    _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "CampaignId": str,
+        "KpiName": str,
+    },
+)
+_OptionalGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_OptionalGetCampaignDateRangeKpiRequestRequestTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": str,
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GetCampaignDateRangeKpiRequestRequestTypeDef(
+    _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
+    _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyId": str,
+        "KpiName": str,
+    },
+)
+_OptionalGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_OptionalGetJourneyDateRangeKpiRequestRequestTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": str,
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GetJourneyDateRangeKpiRequestRequestTypeDef(
+    _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
+    _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
+):
+    pass
+
+
+JourneyScheduleTypeDef = TypedDict(
+    "JourneyScheduleTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
+        "Timezone": str,
+    },
+    total=False,
+)
+
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5040,14 +5045,15 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagsModel": TagsModelTypeDef,
     },
 )
 
+TagsModelUnionTypeDef = Union[TagsModelTypeDef, TagsModelOutputTypeDef]
 UpdateTemplateActiveVersionRequestRequestTypeDef = TypedDict(
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
```

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/type_defs.pyi` & `mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pinpoint.type_defs import ADMChannelRequestTypeDef
 
-    data: ADMChannelRequestTypeDef = {...}
+    data: ADMChannelRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -79,14 +79,15 @@
     "QuietTimeTypeDef",
     "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
+    "BlobTypeDef",
     "CampaignCustomMessageTypeDef",
     "CampaignEmailMessageTypeDef",
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationOutputTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
@@ -138,15 +139,14 @@
     "VoiceChannelResponseTypeDef",
     "DeleteVoiceTemplateRequestRequestTypeDef",
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
-    "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointUserOutputTypeDef",
@@ -161,20 +161,19 @@
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
     "GetApnsChannelRequestRequestTypeDef",
     "GetApnsSandboxChannelRequestRequestTypeDef",
     "GetApnsVoipChannelRequestRequestTypeDef",
     "GetApnsVoipSandboxChannelRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
-    "GetApplicationDateRangeKpiRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetApplicationSettingsRequestRequestTypeDef",
     "GetAppsRequestRequestTypeDef",
     "GetBaiduChannelRequestRequestTypeDef",
     "GetCampaignActivitiesRequestRequestTypeDef",
-    "GetCampaignDateRangeKpiRequestRequestTypeDef",
     "GetCampaignRequestRequestTypeDef",
     "GetCampaignVersionRequestRequestTypeDef",
     "GetCampaignVersionsRequestRequestTypeDef",
     "GetCampaignsRequestRequestTypeDef",
     "GetChannelsRequestRequestTypeDef",
     "GetEmailChannelRequestRequestTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
@@ -183,15 +182,14 @@
     "GetExportJobRequestRequestTypeDef",
     "GetExportJobsRequestRequestTypeDef",
     "GetGcmChannelRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
     "GetImportJobsRequestRequestTypeDef",
     "GetInAppMessagesRequestRequestTypeDef",
     "GetInAppTemplateRequestRequestTypeDef",
-    "GetJourneyDateRangeKpiRequestRequestTypeDef",
     "GetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     "JourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsRequestRequestTypeDef",
     "JourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRequestRequestTypeDef",
     "GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef",
     "JourneyRunExecutionActivityMetricsResponseTypeDef",
@@ -219,15 +217,14 @@
     "OverrideButtonConfigurationTypeDef",
     "InAppMessageHeaderConfigTypeDef",
     "JourneyChannelSettingsTypeDef",
     "JourneyPushMessageTypeDef",
     "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
     "JourneySMSMessageTypeDef",
-    "JourneyScheduleTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagsModelOutputTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "MessageTypeDef",
@@ -262,14 +259,15 @@
     "UpdateApnsVoipChannelRequestRequestTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
     "ApplicationSettingsJourneyLimitsTypeDef",
     "JourneyLimitsTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
+    "RawEmailTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "DeleteAdmChannelResponseTypeDef",
@@ -358,14 +356,18 @@
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
     "GPSPointDimensionTypeDef",
+    "GetApplicationDateRangeKpiRequestRequestTypeDef",
+    "GetCampaignDateRangeKpiRequestRequestTypeDef",
+    "GetJourneyDateRangeKpiRequestRequestTypeDef",
+    "JourneyScheduleTypeDef",
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     "GetSmsTemplateResponseTypeDef",
     "GetVoiceTemplateResponseTypeDef",
     "ImportJobResponseTypeDef",
@@ -386,14 +388,15 @@
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagsModelUnionTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
@@ -1091,14 +1094,15 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CampaignCustomMessageTypeDef = TypedDict(
     "CampaignCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
@@ -1921,22 +1925,14 @@
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
 )
 
-RawEmailTypeDef = TypedDict(
-    "RawEmailTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 _RequiredEmailTemplateResponseTypeDef = TypedDict(
     "_RequiredEmailTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2203,38 +2199,15 @@
 GetAppRequestRequestTypeDef = TypedDict(
     "GetAppRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-_RequiredGetApplicationDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_RequiredGetApplicationDateRangeKpiRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "KpiName": str,
-    },
-)
-_OptionalGetApplicationDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_OptionalGetApplicationDateRangeKpiRequestRequestTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": str,
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GetApplicationDateRangeKpiRequestRequestTypeDef(
-    _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
-    _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 GetApplicationSettingsRequestRequestTypeDef = TypedDict(
     "GetApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2272,39 +2245,14 @@
 
 class GetCampaignActivitiesRequestRequestTypeDef(
     _RequiredGetCampaignActivitiesRequestRequestTypeDef,
     _OptionalGetCampaignActivitiesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "CampaignId": str,
-        "KpiName": str,
-    },
-)
-_OptionalGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_OptionalGetCampaignDateRangeKpiRequestRequestTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": str,
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GetCampaignDateRangeKpiRequestRequestTypeDef(
-    _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
-    _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
-):
-    pass
-
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
     },
 )
@@ -2494,39 +2442,14 @@
 )
 
 class GetInAppTemplateRequestRequestTypeDef(
     _RequiredGetInAppTemplateRequestRequestTypeDef, _OptionalGetInAppTemplateRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "JourneyId": str,
-        "KpiName": str,
-    },
-)
-_OptionalGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
-    "_OptionalGetJourneyDateRangeKpiRequestRequestTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": str,
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GetJourneyDateRangeKpiRequestRequestTypeDef(
-    _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
-    _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
-):
-    pass
-
 _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
     },
@@ -3052,24 +2975,14 @@
         "SenderId": str,
         "EntityId": str,
         "TemplateId": str,
     },
     total=False,
 )
 
-JourneyScheduleTypeDef = TypedDict(
-    "JourneyScheduleTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
-        "Timezone": str,
-    },
-    total=False,
-)
-
 JourneyStateRequestTypeDef = TypedDict(
     "JourneyStateRequestTypeDef",
     {
         "State": StateType,
     },
     total=False,
 )
@@ -3581,14 +3494,22 @@
     "UpdateBaiduChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
+RawEmailTypeDef = TypedDict(
+    "RawEmailTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+    total=False,
+)
+
 ChannelsResponseTypeDef = TypedDict(
     "ChannelsResponseTypeDef",
     {
         "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
@@ -4575,14 +4496,98 @@
 )
 
 class GPSPointDimensionTypeDef(
     _RequiredGPSPointDimensionTypeDef, _OptionalGPSPointDimensionTypeDef
 ):
     pass
 
+_RequiredGetApplicationDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_RequiredGetApplicationDateRangeKpiRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "KpiName": str,
+    },
+)
+_OptionalGetApplicationDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_OptionalGetApplicationDateRangeKpiRequestRequestTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": str,
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class GetApplicationDateRangeKpiRequestRequestTypeDef(
+    _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
+    _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
+):
+    pass
+
+_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "CampaignId": str,
+        "KpiName": str,
+    },
+)
+_OptionalGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_OptionalGetCampaignDateRangeKpiRequestRequestTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": str,
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class GetCampaignDateRangeKpiRequestRequestTypeDef(
+    _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
+    _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
+):
+    pass
+
+_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyId": str,
+        "KpiName": str,
+    },
+)
+_OptionalGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
+    "_OptionalGetJourneyDateRangeKpiRequestRequestTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": str,
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class GetJourneyDateRangeKpiRequestRequestTypeDef(
+    _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
+    _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
+):
+    pass
+
+JourneyScheduleTypeDef = TypedDict(
+    "JourneyScheduleTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
+        "Timezone": str,
+    },
+    total=False,
+)
+
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4865,14 +4870,15 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagsModel": TagsModelTypeDef,
     },
 )
 
+TagsModelUnionTypeDef = Union[TagsModelTypeDef, TagsModelOutputTypeDef]
 UpdateTemplateActiveVersionRequestRequestTypeDef = TypedDict(
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
```

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Pinpoint 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pinpoint type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pinpoint type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: ActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pinpoint.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint.type_defs import (
     ADMChannelRequestTypeDef,
     ADMChannelResponseTypeDef,
     ADMMessageTypeDef,
     APNSChannelRequestTypeDef,
@@ -352,14 +352,15 @@
     QuietTimeTypeDef,
     AttributeDimensionOutputTypeDef,
     AttributeDimensionTypeDef,
     AttributesResourceTypeDef,
     BaiduChannelRequestTypeDef,
     BaiduChannelResponseTypeDef,
     BaiduMessageTypeDef,
+    BlobTypeDef,
     CampaignCustomMessageTypeDef,
     CampaignEmailMessageTypeDef,
     CampaignStateTypeDef,
     CustomDeliveryConfigurationOutputTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
@@ -411,15 +412,14 @@
     VoiceChannelResponseTypeDef,
     DeleteVoiceTemplateRequestRequestTypeDef,
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
-    RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointUserOutputTypeDef,
@@ -434,20 +434,19 @@
     GPSCoordinatesTypeDef,
     GetAdmChannelRequestRequestTypeDef,
     GetApnsChannelRequestRequestTypeDef,
     GetApnsSandboxChannelRequestRequestTypeDef,
     GetApnsVoipChannelRequestRequestTypeDef,
     GetApnsVoipSandboxChannelRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
-    GetApplicationDateRangeKpiRequestRequestTypeDef,
+    TimestampTypeDef,
     GetApplicationSettingsRequestRequestTypeDef,
     GetAppsRequestRequestTypeDef,
     GetBaiduChannelRequestRequestTypeDef,
     GetCampaignActivitiesRequestRequestTypeDef,
-    GetCampaignDateRangeKpiRequestRequestTypeDef,
     GetCampaignRequestRequestTypeDef,
     GetCampaignVersionRequestRequestTypeDef,
     GetCampaignVersionsRequestRequestTypeDef,
     GetCampaignsRequestRequestTypeDef,
     GetChannelsRequestRequestTypeDef,
     GetEmailChannelRequestRequestTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
@@ -456,15 +455,14 @@
     GetExportJobRequestRequestTypeDef,
     GetExportJobsRequestRequestTypeDef,
     GetGcmChannelRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetImportJobsRequestRequestTypeDef,
     GetInAppMessagesRequestRequestTypeDef,
     GetInAppTemplateRequestRequestTypeDef,
-    GetJourneyDateRangeKpiRequestRequestTypeDef,
     GetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     JourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsRequestRequestTypeDef,
     JourneyExecutionMetricsResponseTypeDef,
     GetJourneyRequestRequestTypeDef,
     GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
     JourneyRunExecutionActivityMetricsResponseTypeDef,
@@ -492,15 +490,14 @@
     OverrideButtonConfigurationTypeDef,
     InAppMessageHeaderConfigTypeDef,
     JourneyChannelSettingsTypeDef,
     JourneyPushMessageTypeDef,
     JourneyScheduleOutputTypeDef,
     JourneyRunResponseTypeDef,
     JourneySMSMessageTypeDef,
-    JourneyScheduleTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagsModelOutputTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
     MessageTypeDef,
@@ -535,14 +532,15 @@
     UpdateApnsVoipChannelRequestRequestTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
     ApplicationSettingsJourneyLimitsTypeDef,
     JourneyLimitsTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
+    RawEmailTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysOutputTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppResponseTypeDef,
     DeleteAdmChannelResponseTypeDef,
@@ -631,14 +629,18 @@
     EventDimensionsTypeDef,
     SegmentDemographicsTypeDef,
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
     GPSPointDimensionTypeDef,
+    GetApplicationDateRangeKpiRequestRequestTypeDef,
+    GetCampaignDateRangeKpiRequestRequestTypeDef,
+    GetJourneyDateRangeKpiRequestRequestTypeDef,
+    JourneyScheduleTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyRunExecutionActivityMetricsResponseTypeDef,
     GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
@@ -659,14 +661,15 @@
     SegmentBehaviorsTypeDef,
     RemoveAttributesRequestRequestTypeDef,
     ResultRowTypeDef,
     UpdateSmsChannelRequestRequestTypeDef,
     SendOTPMessageRequestRequestTypeDef,
     SimpleEmailTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagsModelUnionTypeDef,
     UpdateTemplateActiveVersionRequestRequestTypeDef,
     TemplateConfigurationTypeDef,
     TemplatesResponseTypeDef,
     TemplateVersionsResponseTypeDef,
     UpdateRecommenderConfigurationRequestRequestTypeDef,
     UpdateVoiceChannelRequestRequestTypeDef,
     VerifyOTPMessageResponseTypeDef,
@@ -808,15 +811,15 @@
     UpdateJourneyStateResponseTypeDef,
     CreateJourneyRequestRequestTypeDef,
     UpdateJourneyRequestRequestTypeDef,
     ListJourneysResponseTypeDef,
 )
 
 
-def get_structure() -> ADMChannelRequestTypeDef:
+def get_value() -> ADMChannelRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-1.28.16/mypy_boto3_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15.post1/setup.py` & `mypy-boto3-pinpoint-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Pinpoint 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 pinpoint type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 pinpoint type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_pinpoint": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

