# Comparing `tmp/mypy-boto3-sesv2-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-sesv2-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sesv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:12 2023, max compression
+gzip compressed data, was "mypy-boto3-sesv2-1.28.16.tar", last modified: Tue Aug  1 11:37:51 2023, max compression
```

## Comparing `mypy-boto3-sesv2-1.28.15.post1.tar` & `mypy-boto3-sesv2-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21187 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57068 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56975 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-29 09:59:34.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70597 2023-07-29 09:59:40.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70527 2023-07-29 09:59:34.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21187 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.804729 mypy-boto3-sesv2-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:05.000000 mypy-boto3-sesv2-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-08-01 11:37:51.804729 mypy-boto3-sesv2-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19863 2023-08-01 11:33:05.000000 mypy-boto3-sesv2-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.796729 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 11:33:05.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-01 11:33:05.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 11:33:05.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56729 2023-08-01 11:33:06.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56636 2023-08-01 11:33:06.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-08-01 11:33:06.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-08-01 11:33:06.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:05.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71021 2023-08-01 11:33:12.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70951 2023-08-01 11:33:11.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:05.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.804729 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-08-01 11:37:51.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-01 11:37:51.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:51.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:37:51.000000 mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:51.804729 mypy-boto3-sesv2-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:33:05.000000 mypy-boto3-sesv2-1.28.16/setup.py
```

### Comparing `mypy-boto3-sesv2-1.28.15.post1/LICENSE` & `mypy-boto3-sesv2-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.15.post1/PKG-INFO` & `mypy-boto3-sesv2-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SESV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sesv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sesv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
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
@@ -320,40 +320,40 @@
 )
 
 
 def check_value(value: BehaviorOnMxFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sesv2.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sesv2.type_defs import (
     ReviewDetailsTypeDef,
-    BatchGetMetricDataQueryTypeDef,
+    TimestampTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
     ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
     TopicPreferenceTypeDef,
     DeliveryOptionsTypeDef,
-    ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
@@ -378,15 +378,14 @@
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
-    RawMessageTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
@@ -400,15 +399,14 @@
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
-    GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
     GuardianAttributesTypeDef,
@@ -417,22 +415,20 @@
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
-    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    ListSuppressedDestinationsRequestRequestTypeDef,
     SuppressedDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountDetailsRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
@@ -452,27 +448,32 @@
     SendCustomVerificationEmailRequestRequestTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
-    BatchGetMetricDataRequestRequestTypeDef,
+    BatchGetMetricDataQueryTypeDef,
+    GetDomainStatisticsReportRequestRequestTypeDef,
+    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ListSuppressedDestinationsRequestRequestTypeDef,
+    ReputationOptionsTypeDef,
     BatchGetMetricDataResponseTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateImportJobResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetEmailIdentityPoliciesResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
@@ -499,32 +500,35 @@
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     ListEmailTemplatesResponseTypeDef,
+    SuppressionOptionsUnionTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
+    BatchGetMetricDataRequestRequestTypeDef,
+    ReputationOptionsUnionTypeDef,
     MessageTypeDef,
     EventDestinationTypeDef,
     EventDestinationDefinitionTypeDef,
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
-    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     GetConfigurationSetResponseTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
     CreateImportJobRequestRequestTypeDef,
@@ -533,22 +537,23 @@
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
+    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     ListImportJobsResponseTypeDef,
     SendBulkEmailRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ReviewDetailsTypeDef:
+def get_value() -> ReviewDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sesv2-1.28.15.post1/README.md` & `mypy-boto3-sesv2-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
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
@@ -288,40 +288,40 @@
 )
 
 
 def check_value(value: BehaviorOnMxFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sesv2.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sesv2.type_defs import (
     ReviewDetailsTypeDef,
-    BatchGetMetricDataQueryTypeDef,
+    TimestampTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
     ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
     TopicPreferenceTypeDef,
     DeliveryOptionsTypeDef,
-    ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
@@ -346,15 +346,14 @@
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
-    RawMessageTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
@@ -368,15 +367,14 @@
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
-    GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
     GuardianAttributesTypeDef,
@@ -385,22 +383,20 @@
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
-    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    ListSuppressedDestinationsRequestRequestTypeDef,
     SuppressedDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountDetailsRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
@@ -420,27 +416,32 @@
     SendCustomVerificationEmailRequestRequestTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
-    BatchGetMetricDataRequestRequestTypeDef,
+    BatchGetMetricDataQueryTypeDef,
+    GetDomainStatisticsReportRequestRequestTypeDef,
+    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ListSuppressedDestinationsRequestRequestTypeDef,
+    ReputationOptionsTypeDef,
     BatchGetMetricDataResponseTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateImportJobResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetEmailIdentityPoliciesResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
@@ -467,32 +468,35 @@
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     ListEmailTemplatesResponseTypeDef,
+    SuppressionOptionsUnionTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
+    BatchGetMetricDataRequestRequestTypeDef,
+    ReputationOptionsUnionTypeDef,
     MessageTypeDef,
     EventDestinationTypeDef,
     EventDestinationDefinitionTypeDef,
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
-    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     GetConfigurationSetResponseTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
     CreateImportJobRequestRequestTypeDef,
@@ -501,22 +505,23 @@
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
+    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     ListImportJobsResponseTypeDef,
     SendBulkEmailRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ReviewDetailsTypeDef:
+def get_value() -> ReviewDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/__main__.py` & `mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SESV2 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.SESV2 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\nOther"
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

### Comparing `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/client.py` & `mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_sesv2.client import SESV2Client
 
     session = Session()
     client: SESV2Client = session.client("sesv2")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BehaviorOnMxFailureType,
     ContactLanguageType,
     DkimSigningAttributesOriginType,
@@ -36,16 +35,15 @@
     BulkEmailEntryTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
-    DomainDeliverabilityTrackingOptionOutputTypeDef,
-    DomainDeliverabilityTrackingOptionTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
@@ -79,24 +77,23 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    ReputationOptionsOutputTypeDef,
-    ReputationOptionsTypeDef,
+    ReputationOptionsUnionTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
-    SuppressionOptionsOutputTypeDef,
-    SuppressionOptionsTypeDef,
+    SuppressionOptionsUnionTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
+    TimestampTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
 )
 
@@ -173,18 +170,18 @@
 
     def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef] = ...,
+        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef] = ...,
+        SuppressionOptions: SuppressionOptionsUnionTypeDef = ...,
         VdmOptions: VdmOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_configuration_set)
@@ -552,15 +549,15 @@
         Retrieve all the deliverability data for a specific campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_deliverability_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#get_domain_deliverability_campaign)
         """
 
     def get_domain_statistics_report(
-        self, *, Domain: str, StartDate: Union[datetime, str], EndDate: Union[datetime, str]
+        self, *, Domain: str, StartDate: TimestampTypeDef, EndDate: TimestampTypeDef
     ) -> GetDomainStatisticsReportResponseTypeDef:
         """
         Retrieve inbox placement and engagement rates for the domains that you use to
         send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_statistics_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#get_domain_statistics_report)
@@ -683,16 +680,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_deliverability_test_reports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#list_deliverability_test_reports)
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
@@ -752,16 +749,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#list_recommendations)
         """
 
     def list_suppressed_destinations(
         self,
         *,
         Reasons: Sequence[SuppressionListReasonType] = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: int = ...
     ) -> ListSuppressedDestinationsResponseTypeDef:
         """
         Retrieves a list of email addresses that are on the suppression list for your
         account.
 
@@ -930,20 +927,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_warmup_attributes)
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
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/client.pyi` & `mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_sesv2.client import SESV2Client
 
     session = Session()
     client: SESV2Client = session.client("sesv2")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BehaviorOnMxFailureType,
     ContactLanguageType,
     DkimSigningAttributesOriginType,
@@ -36,16 +35,15 @@
     BulkEmailEntryTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
-    DomainDeliverabilityTrackingOptionOutputTypeDef,
-    DomainDeliverabilityTrackingOptionTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
@@ -79,24 +77,23 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    ReputationOptionsOutputTypeDef,
-    ReputationOptionsTypeDef,
+    ReputationOptionsUnionTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
-    SuppressionOptionsOutputTypeDef,
-    SuppressionOptionsTypeDef,
+    SuppressionOptionsUnionTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
+    TimestampTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
 )
 
@@ -166,18 +163,18 @@
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
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef] = ...,
+        SuppressionOptions: SuppressionOptionsUnionTypeDef = ...,
         VdmOptions: VdmOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_configuration_set)
@@ -510,15 +507,15 @@
         """
         Retrieve all the deliverability data for a specific campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_deliverability_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#get_domain_deliverability_campaign)
         """
     def get_domain_statistics_report(
-        self, *, Domain: str, StartDate: Union[datetime, str], EndDate: Union[datetime, str]
+        self, *, Domain: str, StartDate: TimestampTypeDef, EndDate: TimestampTypeDef
     ) -> GetDomainStatisticsReportResponseTypeDef:
         """
         Retrieve inbox placement and engagement rates for the domains that you use to
         send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_statistics_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#get_domain_statistics_report)
@@ -629,16 +626,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_deliverability_test_reports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#list_deliverability_test_reports)
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
@@ -693,16 +690,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#list_recommendations)
         """
     def list_suppressed_destinations(
         self,
         *,
         Reasons: Sequence[SuppressionListReasonType] = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: int = ...
     ) -> ListSuppressedDestinationsResponseTypeDef:
         """
         Retrieves a list of email addresses that are on the suppression list for your
         account.
 
@@ -855,20 +852,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_warmup_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_warmup_attributes)
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
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/literals.py` & `mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/literals.pyi` & `mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/type_defs.py` & `mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sesv2.type_defs import ReviewDetailsTypeDef
 
-    data: ReviewDetailsTypeDef = {...}
+    data: ReviewDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -61,30 +61,30 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ReviewDetailsTypeDef",
-    "BatchGetMetricDataQueryTypeDef",
+    "TimestampTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
     "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
     "TopicPreferenceTypeDef",
     "DeliveryOptionsTypeDef",
-    "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
@@ -109,15 +109,14 @@
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
     "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
-    "RawMessageTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
@@ -131,15 +130,14 @@
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
-    "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
     "GuardianAttributesTypeDef",
@@ -148,22 +146,20 @@
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
-    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListEmailTemplatesRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
-    "ListSuppressedDestinationsRequestRequestTypeDef",
     "SuppressedDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountDetailsRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
@@ -183,27 +179,32 @@
     "SendCustomVerificationEmailRequestRequestTypeDef",
     "SuppressedDestinationAttributesTypeDef",
     "TestRenderEmailTemplateRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "UpdateEmailIdentityPolicyRequestRequestTypeDef",
     "AccountDetailsTypeDef",
-    "BatchGetMetricDataRequestRequestTypeDef",
+    "BatchGetMetricDataQueryTypeDef",
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ListSuppressedDestinationsRequestRequestTypeDef",
+    "ReputationOptionsTypeDef",
     "BatchGetMetricDataResponseTypeDef",
     "CreateDeliverabilityTestReportResponseTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetEmailIdentityPoliciesResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
     "ListDedicatedIpPoolsResponseTypeDef",
     "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     "SendCustomVerificationEmailResponseTypeDef",
     "SendEmailResponseTypeDef",
     "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
@@ -230,32 +231,35 @@
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "ListEmailTemplatesResponseTypeDef",
+    "SuppressionOptionsUnionTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
+    "BatchGetMetricDataRequestRequestTypeDef",
+    "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
     "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "DomainDeliverabilityTrackingOptionUnionTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
@@ -264,14 +268,15 @@
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "ListImportJobsResponseTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -279,39 +284,15 @@
     {
         "Status": ReviewStatusType,
         "CaseId": str,
     },
     total=False,
 )
 
-_RequiredBatchGetMetricDataQueryTypeDef = TypedDict(
-    "_RequiredBatchGetMetricDataQueryTypeDef",
-    {
-        "Id": str,
-        "Namespace": Literal["VDM"],
-        "Metric": MetricType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-    },
-)
-_OptionalBatchGetMetricDataQueryTypeDef = TypedDict(
-    "_OptionalBatchGetMetricDataQueryTypeDef",
-    {
-        "Dimensions": Mapping[MetricDimensionNameType, str],
-    },
-    total=False,
-)
-
-
-class BatchGetMetricDataQueryTypeDef(
-    _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 MetricDataErrorTypeDef = TypedDict(
     "MetricDataErrorTypeDef",
     {
         "Id": str,
         "Code": QueryErrorCodeType,
         "Message": str,
     },
@@ -345,14 +326,15 @@
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
@@ -445,23 +427,14 @@
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
@@ -774,21 +747,14 @@
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
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
@@ -950,23 +916,14 @@
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
 GetEmailIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -1091,39 +1048,14 @@
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
@@ -1189,26 +1121,14 @@
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Impact": RecommendationImpactType,
     },
     total=False,
 )
 
-ListSuppressedDestinationsRequestRequestTypeDef = TypedDict(
-    "ListSuppressedDestinationsRequestRequestTypeDef",
-    {
-        "Reasons": Sequence[SuppressionListReasonType],
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
 SuppressedDestinationSummaryTypeDef = TypedDict(
     "SuppressedDestinationSummaryTypeDef",
     {
         "EmailAddress": str,
         "Reason": SuppressionListReasonType,
         "LastUpdateTime": datetime,
     },
@@ -1588,19 +1508,92 @@
         "UseCaseDescription": str,
         "AdditionalContactEmailAddresses": List[str],
         "ReviewDetails": ReviewDetailsTypeDef,
     },
     total=False,
 )
 
-BatchGetMetricDataRequestRequestTypeDef = TypedDict(
-    "BatchGetMetricDataRequestRequestTypeDef",
+_RequiredBatchGetMetricDataQueryTypeDef = TypedDict(
+    "_RequiredBatchGetMetricDataQueryTypeDef",
     {
-        "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
+        "Id": str,
+        "Namespace": Literal["VDM"],
+        "Metric": MetricType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+    },
+)
+_OptionalBatchGetMetricDataQueryTypeDef = TypedDict(
+    "_OptionalBatchGetMetricDataQueryTypeDef",
+    {
+        "Dimensions": Mapping[MetricDimensionNameType, str],
+    },
+    total=False,
+)
+
+
+class BatchGetMetricDataQueryTypeDef(
+    _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
+):
+    pass
+
+
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
     },
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
+ListSuppressedDestinationsRequestRequestTypeDef = TypedDict(
+    "ListSuppressedDestinationsRequestRequestTypeDef",
+    {
+        "Reasons": Sequence[SuppressionListReasonType],
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": int,
+    },
+    total=False,
+)
+
+ReputationOptionsTypeDef = TypedDict(
+    "ReputationOptionsTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": TimestampTypeDef,
+    },
+    total=False,
 )
 
 BatchGetMetricDataResponseTypeDef = TypedDict(
     "BatchGetMetricDataResponseTypeDef",
     {
         "Results": List[MetricDataResultTypeDef],
         "Errors": List[MetricDataErrorTypeDef],
@@ -1701,14 +1694,21 @@
     "GetBlacklistReportsResponseTypeDef",
     {
         "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
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
@@ -2097,29 +2097,30 @@
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
 
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SuppressionOptionsUnionTypeDef = Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef]
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -2242,14 +2243,22 @@
 
 class SuppressedDestinationTypeDef(
     _RequiredSuppressedDestinationTypeDef, _OptionalSuppressedDestinationTypeDef
 ):
     pass
 
 
+BatchGetMetricDataRequestRequestTypeDef = TypedDict(
+    "BatchGetMetricDataRequestRequestTypeDef",
+    {
+        "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
+    },
+)
+
+ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -2317,41 +2326,17 @@
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
         "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-    },
-)
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "SubscribedDomains": Sequence[
-            Union[
-                DomainDeliverabilityTrackingOptionTypeDef,
-                DomainDeliverabilityTrackingOptionOutputTypeDef,
-            ]
-        ],
-    },
-    total=False,
-)
-
-
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-):
-    pass
-
-
+DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
+    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
+]
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
@@ -2567,14 +2552,36 @@
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
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/type_defs.pyi` & `mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sesv2.type_defs import ReviewDetailsTypeDef
 
-    data: ReviewDetailsTypeDef = {...}
+    data: ReviewDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -60,30 +60,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ReviewDetailsTypeDef",
-    "BatchGetMetricDataQueryTypeDef",
+    "TimestampTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
     "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
     "TopicPreferenceTypeDef",
     "DeliveryOptionsTypeDef",
-    "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
@@ -108,15 +108,14 @@
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
     "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
-    "RawMessageTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
@@ -130,15 +129,14 @@
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
-    "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
     "GuardianAttributesTypeDef",
@@ -147,22 +145,20 @@
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
-    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListEmailTemplatesRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
-    "ListSuppressedDestinationsRequestRequestTypeDef",
     "SuppressedDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountDetailsRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
@@ -182,27 +178,32 @@
     "SendCustomVerificationEmailRequestRequestTypeDef",
     "SuppressedDestinationAttributesTypeDef",
     "TestRenderEmailTemplateRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "UpdateEmailIdentityPolicyRequestRequestTypeDef",
     "AccountDetailsTypeDef",
-    "BatchGetMetricDataRequestRequestTypeDef",
+    "BatchGetMetricDataQueryTypeDef",
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ListSuppressedDestinationsRequestRequestTypeDef",
+    "ReputationOptionsTypeDef",
     "BatchGetMetricDataResponseTypeDef",
     "CreateDeliverabilityTestReportResponseTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetEmailIdentityPoliciesResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
     "ListDedicatedIpPoolsResponseTypeDef",
     "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     "SendCustomVerificationEmailResponseTypeDef",
     "SendEmailResponseTypeDef",
     "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
@@ -229,32 +230,35 @@
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "ListEmailTemplatesResponseTypeDef",
+    "SuppressionOptionsUnionTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
+    "BatchGetMetricDataRequestRequestTypeDef",
+    "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
     "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "DomainDeliverabilityTrackingOptionUnionTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
@@ -263,14 +267,15 @@
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "ListImportJobsResponseTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -278,37 +283,15 @@
     {
         "Status": ReviewStatusType,
         "CaseId": str,
     },
     total=False,
 )
 
-_RequiredBatchGetMetricDataQueryTypeDef = TypedDict(
-    "_RequiredBatchGetMetricDataQueryTypeDef",
-    {
-        "Id": str,
-        "Namespace": Literal["VDM"],
-        "Metric": MetricType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-    },
-)
-_OptionalBatchGetMetricDataQueryTypeDef = TypedDict(
-    "_OptionalBatchGetMetricDataQueryTypeDef",
-    {
-        "Dimensions": Mapping[MetricDimensionNameType, str],
-    },
-    total=False,
-)
-
-class BatchGetMetricDataQueryTypeDef(
-    _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 MetricDataErrorTypeDef = TypedDict(
     "MetricDataErrorTypeDef",
     {
         "Id": str,
         "Code": QueryErrorCodeType,
         "Message": str,
     },
@@ -342,14 +325,15 @@
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
@@ -440,23 +424,14 @@
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
@@ -765,21 +740,14 @@
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
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
@@ -941,23 +909,14 @@
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
 GetEmailIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -1082,37 +1041,14 @@
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
@@ -1176,26 +1112,14 @@
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Impact": RecommendationImpactType,
     },
     total=False,
 )
 
-ListSuppressedDestinationsRequestRequestTypeDef = TypedDict(
-    "ListSuppressedDestinationsRequestRequestTypeDef",
-    {
-        "Reasons": Sequence[SuppressionListReasonType],
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
 SuppressedDestinationSummaryTypeDef = TypedDict(
     "SuppressedDestinationSummaryTypeDef",
     {
         "EmailAddress": str,
         "Reason": SuppressionListReasonType,
         "LastUpdateTime": datetime,
     },
@@ -1553,19 +1477,88 @@
         "UseCaseDescription": str,
         "AdditionalContactEmailAddresses": List[str],
         "ReviewDetails": ReviewDetailsTypeDef,
     },
     total=False,
 )
 
-BatchGetMetricDataRequestRequestTypeDef = TypedDict(
-    "BatchGetMetricDataRequestRequestTypeDef",
+_RequiredBatchGetMetricDataQueryTypeDef = TypedDict(
+    "_RequiredBatchGetMetricDataQueryTypeDef",
     {
-        "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
+        "Id": str,
+        "Namespace": Literal["VDM"],
+        "Metric": MetricType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+    },
+)
+_OptionalBatchGetMetricDataQueryTypeDef = TypedDict(
+    "_OptionalBatchGetMetricDataQueryTypeDef",
+    {
+        "Dimensions": Mapping[MetricDimensionNameType, str],
     },
+    total=False,
+)
+
+class BatchGetMetricDataQueryTypeDef(
+    _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
+):
+    pass
+
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
+ListSuppressedDestinationsRequestRequestTypeDef = TypedDict(
+    "ListSuppressedDestinationsRequestRequestTypeDef",
+    {
+        "Reasons": Sequence[SuppressionListReasonType],
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": int,
+    },
+    total=False,
+)
+
+ReputationOptionsTypeDef = TypedDict(
+    "ReputationOptionsTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": TimestampTypeDef,
+    },
+    total=False,
 )
 
 BatchGetMetricDataResponseTypeDef = TypedDict(
     "BatchGetMetricDataResponseTypeDef",
     {
         "Results": List[MetricDataResultTypeDef],
         "Errors": List[MetricDataErrorTypeDef],
@@ -1666,14 +1659,21 @@
     "GetBlacklistReportsResponseTypeDef",
     {
         "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
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
@@ -2048,29 +2048,30 @@
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
 
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SuppressionOptionsUnionTypeDef = Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef]
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -2189,14 +2190,22 @@
 )
 
 class SuppressedDestinationTypeDef(
     _RequiredSuppressedDestinationTypeDef, _OptionalSuppressedDestinationTypeDef
 ):
     pass
 
+BatchGetMetricDataRequestRequestTypeDef = TypedDict(
+    "BatchGetMetricDataRequestRequestTypeDef",
+    {
+        "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
+    },
+)
+
+ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -2262,39 +2271,17 @@
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
         "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-    },
-)
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "SubscribedDomains": Sequence[
-            Union[
-                DomainDeliverabilityTrackingOptionTypeDef,
-                DomainDeliverabilityTrackingOptionOutputTypeDef,
-            ]
-        ],
-    },
-    total=False,
-)
-
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-):
-    pass
-
+DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
+    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
+]
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
@@ -2502,14 +2489,34 @@
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
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/PKG-INFO` & `mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SESV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sesv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sesv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
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
@@ -320,40 +320,40 @@
 )
 
 
 def check_value(value: BehaviorOnMxFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sesv2.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sesv2.type_defs import (
     ReviewDetailsTypeDef,
-    BatchGetMetricDataQueryTypeDef,
+    TimestampTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
     ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
     TopicPreferenceTypeDef,
     DeliveryOptionsTypeDef,
-    ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
@@ -378,15 +378,14 @@
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
-    RawMessageTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
@@ -400,15 +399,14 @@
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
-    GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
     GuardianAttributesTypeDef,
@@ -417,22 +415,20 @@
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
-    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    ListSuppressedDestinationsRequestRequestTypeDef,
     SuppressedDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountDetailsRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
@@ -452,27 +448,32 @@
     SendCustomVerificationEmailRequestRequestTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
-    BatchGetMetricDataRequestRequestTypeDef,
+    BatchGetMetricDataQueryTypeDef,
+    GetDomainStatisticsReportRequestRequestTypeDef,
+    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ListSuppressedDestinationsRequestRequestTypeDef,
+    ReputationOptionsTypeDef,
     BatchGetMetricDataResponseTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateImportJobResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetEmailIdentityPoliciesResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
@@ -499,32 +500,35 @@
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     ListEmailTemplatesResponseTypeDef,
+    SuppressionOptionsUnionTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
+    BatchGetMetricDataRequestRequestTypeDef,
+    ReputationOptionsUnionTypeDef,
     MessageTypeDef,
     EventDestinationTypeDef,
     EventDestinationDefinitionTypeDef,
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
-    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     GetConfigurationSetResponseTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
     CreateImportJobRequestRequestTypeDef,
@@ -533,22 +537,23 @@
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
+    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     ListImportJobsResponseTypeDef,
     SendBulkEmailRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ReviewDetailsTypeDef:
+def get_value() -> ReviewDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/SOURCES.txt` & `mypy-boto3-sesv2-1.28.16/mypy_boto3_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.15.post1/setup.py` & `mypy-boto3-sesv2-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sesv2",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SESV2 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 sesv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 sesv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sesv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

