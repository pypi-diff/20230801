# Comparing `tmp/mypy-boto3-pinpoint-email-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-pinpoint-email-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-email-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:52 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-email-1.28.16.tar", last modified: Tue Aug  1 11:37:33 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-email-1.28.15.post1.tar` & `mypy-boto3-pinpoint-email-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33224 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33170 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36158 2023-07-29 09:53:19.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-07-29 09:53:19.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:33.448789 mypy-boto3-pinpoint-email-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-08-01 11:37:33.448789 mypy-boto3-pinpoint-email-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:33.432789 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32960 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32906 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-08-01 11:26:21.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-08-01 11:26:21.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36461 2023-08-01 11:26:22.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36427 2023-08-01 11:26:21.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:33.448789 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:37:33.000000 mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:33.448789 mypy-boto3-pinpoint-email-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-01 11:26:20.000000 mypy-boto3-pinpoint-email-1.28.16/setup.py
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/LICENSE` & `mypy-boto3-pinpoint-email-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/PKG-INFO` & `mypy-boto3-pinpoint-email-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PinpointEmail 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pinpoint-email type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pinpoint-email type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-email)](https://pepy.tech/project/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
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
@@ -343,28 +343,28 @@
 )
 
 
 def check_value(value: BehaviorOnMxFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pinpoint_email.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_email.type_defs import (
     BlacklistEntryTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
-    ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     ResponseMetadataTypeDef,
     DkimAttributesTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
@@ -374,15 +374,15 @@
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
     DestinationTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
-    RawMessageTypeDef,
+    TimestampTypeDef,
     TemplateTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
@@ -390,22 +390,20 @@
     ReputationOptionsOutputTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
-    GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     IdentityInfoTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
-    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MessageTagTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
@@ -413,21 +411,21 @@
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateConfigurationSetRequestRequestTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
@@ -436,14 +434,17 @@
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
+    GetDomainStatisticsReportRequestRequestTypeDef,
+    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ReputationOptionsTypeDef,
     GetAccountResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
@@ -451,26 +452,29 @@
     GetEmailIdentityResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     MessageTypeDef,
     EventDestinationTypeDef,
     EventDestinationDefinitionTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
-    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
+    CreateConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsUnionTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     EmailContentTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
+    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BlacklistEntryTypeDef:
+def get_value() -> BlacklistEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/README.md` & `mypy-boto3-pinpoint-email-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-email)](https://pepy.tech/project/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
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
@@ -311,28 +311,28 @@
 )
 
 
 def check_value(value: BehaviorOnMxFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pinpoint_email.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_email.type_defs import (
     BlacklistEntryTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
-    ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     ResponseMetadataTypeDef,
     DkimAttributesTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
@@ -342,15 +342,15 @@
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
     DestinationTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
-    RawMessageTypeDef,
+    TimestampTypeDef,
     TemplateTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
@@ -358,22 +358,20 @@
     ReputationOptionsOutputTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
-    GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     IdentityInfoTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
-    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MessageTagTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
@@ -381,21 +379,21 @@
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateConfigurationSetRequestRequestTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
@@ -404,14 +402,17 @@
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
+    GetDomainStatisticsReportRequestRequestTypeDef,
+    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ReputationOptionsTypeDef,
     GetAccountResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
@@ -419,26 +420,29 @@
     GetEmailIdentityResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     MessageTypeDef,
     EventDestinationTypeDef,
     EventDestinationDefinitionTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
-    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
+    CreateConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsUnionTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     EmailContentTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
+    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BlacklistEntryTypeDef:
+def get_value() -> BlacklistEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__init__.py` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__init__.pyi` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__main__.py` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PinpointEmail 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.PinpointEmail 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail\nOther"
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

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/client.py` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_pinpoint_email.client import PinpointEmailClient
 
     session = Session()
     client: PinpointEmailClient = session.client("pinpoint-email")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BehaviorOnMxFailureType, TlsPolicyType
 from .paginator import (
     GetDedicatedIpsPaginator,
     ListConfigurationSetsPaginator,
@@ -28,16 +27,15 @@
     ListEmailIdentitiesPaginator,
 )
 from .type_defs import (
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
-    DomainDeliverabilityTrackingOptionOutputTypeDef,
-    DomainDeliverabilityTrackingOptionTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     EmailContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
@@ -50,19 +48,19 @@
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
-    ReputationOptionsOutputTypeDef,
-    ReputationOptionsTypeDef,
+    ReputationOptionsUnionTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TrackingOptionsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -128,15 +126,15 @@
 
     def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef] = ...,
+        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set)
@@ -332,15 +330,15 @@
         Retrieve all the deliverability data for a specific campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_domain_deliverability_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#get_domain_deliverability_campaign)
         """
 
     def get_domain_statistics_report(
-        self, *, Domain: str, StartDate: Union[datetime, str], EndDate: Union[datetime, str]
+        self, *, Domain: str, StartDate: TimestampTypeDef, EndDate: TimestampTypeDef
     ) -> GetDomainStatisticsReportResponseTypeDef:
         """
         Retrieve inbox placement and engagement rates for the domains that you use to
         send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_domain_statistics_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#get_domain_statistics_report)
@@ -388,16 +386,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_deliverability_test_reports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#list_deliverability_test_reports)
         """
 
     def list_domain_deliverability_campaigns(
         self,
         *,
-        StartDate: Union[datetime, str],
-        EndDate: Union[datetime, str],
+        StartDate: TimestampTypeDef,
+        EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
         PageSize: int = ...
     ) -> ListDomainDeliverabilityCampaignsResponseTypeDef:
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time range.
@@ -511,20 +509,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#put_dedicated_ip_warmup_attributes)
         """
 
     def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[
-            Union[
-                DomainDeliverabilityTrackingOptionTypeDef,
-                DomainDeliverabilityTrackingOptionOutputTypeDef,
-            ]
-        ] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard for your Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/client.pyi` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_pinpoint_email.client import PinpointEmailClient
 
     session = Session()
     client: PinpointEmailClient = session.client("pinpoint-email")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BehaviorOnMxFailureType, TlsPolicyType
 from .paginator import (
     GetDedicatedIpsPaginator,
     ListConfigurationSetsPaginator,
@@ -28,16 +27,15 @@
     ListEmailIdentitiesPaginator,
 )
 from .type_defs import (
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
-    DomainDeliverabilityTrackingOptionOutputTypeDef,
-    DomainDeliverabilityTrackingOptionTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     EmailContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
@@ -50,19 +48,19 @@
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
-    ReputationOptionsOutputTypeDef,
-    ReputationOptionsTypeDef,
+    ReputationOptionsUnionTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TrackingOptionsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -121,15 +119,15 @@
         """
     def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef] = ...,
+        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set)
@@ -306,15 +304,15 @@
         """
         Retrieve all the deliverability data for a specific campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_domain_deliverability_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#get_domain_deliverability_campaign)
         """
     def get_domain_statistics_report(
-        self, *, Domain: str, StartDate: Union[datetime, str], EndDate: Union[datetime, str]
+        self, *, Domain: str, StartDate: TimestampTypeDef, EndDate: TimestampTypeDef
     ) -> GetDomainStatisticsReportResponseTypeDef:
         """
         Retrieve inbox placement and engagement rates for the domains that you use to
         send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_domain_statistics_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#get_domain_statistics_report)
@@ -357,16 +355,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_deliverability_test_reports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#list_deliverability_test_reports)
         """
     def list_domain_deliverability_campaigns(
         self,
         *,
-        StartDate: Union[datetime, str],
-        EndDate: Union[datetime, str],
+        StartDate: TimestampTypeDef,
+        EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
         PageSize: int = ...
     ) -> ListDomainDeliverabilityCampaignsResponseTypeDef:
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time range.
@@ -469,20 +467,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_dedicated_ip_warmup_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#put_dedicated_ip_warmup_attributes)
         """
     def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[
-            Union[
-                DomainDeliverabilityTrackingOptionTypeDef,
-                DomainDeliverabilityTrackingOptionOutputTypeDef,
-            ]
-        ] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard for your Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/literals.py` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/literals.pyi` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/paginator.py` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/paginator.pyi` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/type_defs.py` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pinpoint_email.type_defs import BlacklistEntryTypeDef
 
-    data: BlacklistEntryTypeDef = {...}
+    data: BlacklistEntryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -34,18 +34,18 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BlacklistEntryTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
-    "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "ResponseMetadataTypeDef",
     "DkimAttributesTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
@@ -55,15 +55,15 @@
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DestinationTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
     "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
-    "RawMessageTypeDef",
+    "TimestampTypeDef",
     "TemplateTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
@@ -71,22 +71,20 @@
     "ReputationOptionsOutputTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
-    "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "IdentityInfoTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
-    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MessageTagTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
@@ -94,21 +92,21 @@
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateConfigurationSetRequestRequestTypeDef",
     "CreateDeliverabilityTestReportResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
     "ListDedicatedIpPoolsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SendEmailResponseTypeDef",
     "CreateEmailIdentityResponseTypeDef",
@@ -117,14 +115,17 @@
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ReputationOptionsTypeDef",
     "GetAccountResponseTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
@@ -132,34 +133,38 @@
     "GetEmailIdentityResponseTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "MessageTypeDef",
     "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "DomainDeliverabilityTrackingOptionUnionTypeDef",
+    "CreateConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsUnionTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "EmailContentTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
         "RblName": str,
         "ListingTime": datetime,
         "Description": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredContentTypeDef = TypedDict(
     "_RequiredContentTypeDef",
     {
         "Data": str,
     },
 )
 _OptionalContentTypeDef = TypedDict(
@@ -189,23 +194,14 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
-ReputationOptionsTypeDef = TypedDict(
-    "ReputationOptionsTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": Union[datetime, str],
-    },
-    total=False,
-)
-
 SendingOptionsTypeDef = TypedDict(
     "SendingOptionsTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
@@ -377,21 +373,15 @@
     {
         "Global": bool,
         "TrackedIsps": Sequence[str],
     },
     total=False,
 )
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateArn": str,
         "TemplateData": str,
     },
     total=False,
@@ -509,23 +499,14 @@
 GetDomainDeliverabilityCampaignRequestRequestTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     {
         "CampaignId": str,
     },
 )
 
-GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
-    "GetDomainStatisticsReportRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-    },
-)
-
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -571,39 +552,14 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "SubscribedDomain": str,
-    },
-)
-_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
-
-class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
-    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-):
-    pass
-
-
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -816,14 +772,21 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
@@ -891,40 +854,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConfigurationSetRequestRequestTypeDef",
-    {
-        "ConfigurationSetName": str,
-    },
-)
-_OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConfigurationSetRequestRequestTypeDef",
-    {
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
-        "SendingOptions": SendingOptionsTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateConfigurationSetRequestRequestTypeDef(
-    _RequiredCreateConfigurationSetRequestRequestTypeDef,
-    _OptionalCreateConfigurationSetRequestRequestTypeDef,
-):
-    pass
-
-
 CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
     "CreateDeliverabilityTestReportResponseTypeDef",
     {
         "ReportId": str,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1055,20 +992,63 @@
     total=False,
 )
 
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": Union[datetime, str],
+        "SubscriptionStartDate": TimestampTypeDef,
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
+GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+    },
+)
+
+_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "SubscribedDomain": str,
+    },
+)
+_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": int,
+    },
+    total=False,
+)
+
+
+class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
+    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+):
+    pass
+
+
+ReputationOptionsTypeDef = TypedDict(
+    "ReputationOptionsTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
@@ -1224,41 +1204,44 @@
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
         "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
+    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
+]
+_RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConfigurationSetRequestRequestTypeDef",
     {
-        "DashboardEnabled": bool,
+        "ConfigurationSetName": str,
     },
 )
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+_OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConfigurationSetRequestRequestTypeDef",
     {
-        "SubscribedDomains": Sequence[
-            Union[
-                DomainDeliverabilityTrackingOptionTypeDef,
-                DomainDeliverabilityTrackingOptionOutputTypeDef,
-            ]
-        ],
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsTypeDef,
+        "SendingOptions": SendingOptionsTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+class CreateConfigurationSetRequestRequestTypeDef(
+    _RequiredCreateConfigurationSetRequestRequestTypeDef,
+    _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
 
+ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
@@ -1299,14 +1282,36 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
+_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "DashboardEnabled": bool,
+    },
+)
+_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
+    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/type_defs.pyi` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pinpoint_email.type_defs import BlacklistEntryTypeDef
 
-    data: BlacklistEntryTypeDef = {...}
+    data: BlacklistEntryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -33,18 +33,18 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BlacklistEntryTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
-    "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "ResponseMetadataTypeDef",
     "DkimAttributesTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
@@ -54,15 +54,15 @@
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DestinationTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
     "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
-    "RawMessageTypeDef",
+    "TimestampTypeDef",
     "TemplateTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
@@ -70,22 +70,20 @@
     "ReputationOptionsOutputTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
-    "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "IdentityInfoTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
-    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MessageTagTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
@@ -93,21 +91,21 @@
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateConfigurationSetRequestRequestTypeDef",
     "CreateDeliverabilityTestReportResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
     "ListDedicatedIpPoolsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SendEmailResponseTypeDef",
     "CreateEmailIdentityResponseTypeDef",
@@ -116,14 +114,17 @@
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ReputationOptionsTypeDef",
     "GetAccountResponseTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
@@ -131,34 +132,38 @@
     "GetEmailIdentityResponseTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "MessageTypeDef",
     "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "DomainDeliverabilityTrackingOptionUnionTypeDef",
+    "CreateConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsUnionTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "EmailContentTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
         "RblName": str,
         "ListingTime": datetime,
         "Description": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredContentTypeDef = TypedDict(
     "_RequiredContentTypeDef",
     {
         "Data": str,
     },
 )
 _OptionalContentTypeDef = TypedDict(
@@ -186,23 +191,14 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
-ReputationOptionsTypeDef = TypedDict(
-    "ReputationOptionsTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": Union[datetime, str],
-    },
-    total=False,
-)
-
 SendingOptionsTypeDef = TypedDict(
     "SendingOptionsTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
@@ -372,21 +368,15 @@
     {
         "Global": bool,
         "TrackedIsps": Sequence[str],
     },
     total=False,
 )
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateArn": str,
         "TemplateData": str,
     },
     total=False,
@@ -504,23 +494,14 @@
 GetDomainDeliverabilityCampaignRequestRequestTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     {
         "CampaignId": str,
     },
 )
 
-GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
-    "GetDomainStatisticsReportRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-    },
-)
-
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -566,37 +547,14 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "SubscribedDomain": str,
-    },
-)
-_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
-class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
-    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-):
-    pass
-
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -795,14 +753,21 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
@@ -866,38 +831,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConfigurationSetRequestRequestTypeDef",
-    {
-        "ConfigurationSetName": str,
-    },
-)
-_OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConfigurationSetRequestRequestTypeDef",
-    {
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
-        "SendingOptions": SendingOptionsTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateConfigurationSetRequestRequestTypeDef(
-    _RequiredCreateConfigurationSetRequestRequestTypeDef,
-    _OptionalCreateConfigurationSetRequestRequestTypeDef,
-):
-    pass
-
 CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
     "CreateDeliverabilityTestReportResponseTypeDef",
     {
         "ReportId": str,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1028,20 +969,61 @@
     total=False,
 )
 
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": Union[datetime, str],
+        "SubscriptionStartDate": TimestampTypeDef,
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
+GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+    },
+)
+
+_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "SubscribedDomain": str,
+    },
+)
+_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": int,
+    },
+    total=False,
+)
+
+class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
+    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+):
+    pass
+
+ReputationOptionsTypeDef = TypedDict(
+    "ReputationOptionsTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
@@ -1195,39 +1177,42 @@
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
         "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
+    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
+]
+_RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConfigurationSetRequestRequestTypeDef",
     {
-        "DashboardEnabled": bool,
+        "ConfigurationSetName": str,
     },
 )
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+_OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConfigurationSetRequestRequestTypeDef",
     {
-        "SubscribedDomains": Sequence[
-            Union[
-                DomainDeliverabilityTrackingOptionTypeDef,
-                DomainDeliverabilityTrackingOptionOutputTypeDef,
-            ]
-        ],
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsTypeDef,
+        "SendingOptions": SendingOptionsTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+class CreateConfigurationSetRequestRequestTypeDef(
+    _RequiredCreateConfigurationSetRequestRequestTypeDef,
+    _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
+ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
@@ -1268,14 +1253,34 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
+_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "DashboardEnabled": bool,
+    },
+)
+_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef],
+    },
+    total=False,
+)
+
+class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
+    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PinpointEmail 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pinpoint-email type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pinpoint-email type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-email)](https://pepy.tech/project/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
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
@@ -343,28 +343,28 @@
 )
 
 
 def check_value(value: BehaviorOnMxFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pinpoint_email.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_email.type_defs import (
     BlacklistEntryTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
-    ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     ResponseMetadataTypeDef,
     DkimAttributesTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
@@ -374,15 +374,15 @@
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
     DestinationTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
-    RawMessageTypeDef,
+    TimestampTypeDef,
     TemplateTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
@@ -390,22 +390,20 @@
     ReputationOptionsOutputTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
-    GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     IdentityInfoTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
-    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MessageTagTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
@@ -413,21 +411,21 @@
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateConfigurationSetRequestRequestTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
@@ -436,14 +434,17 @@
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
+    GetDomainStatisticsReportRequestRequestTypeDef,
+    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ReputationOptionsTypeDef,
     GetAccountResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
@@ -451,26 +452,29 @@
     GetEmailIdentityResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     MessageTypeDef,
     EventDestinationTypeDef,
     EventDestinationDefinitionTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
-    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
+    CreateConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsUnionTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     EmailContentTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
+    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BlacklistEntryTypeDef:
+def get_value() -> BlacklistEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-email-1.28.16/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15.post1/setup.py` & `mypy-boto3-pinpoint-email-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint-email",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_pinpoint_email"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.PinpointEmail 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 pinpoint-email type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 pinpoint-email type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_pinpoint_email": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

