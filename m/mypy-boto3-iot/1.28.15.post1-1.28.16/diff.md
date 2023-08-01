# Comparing `tmp/mypy-boto3-iot-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iot-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:19 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-1.28.16.tar", last modified: Tue Aug  1 11:36:59 2023, max compression
```

## Comparing `mypy-boto3-iot-1.28.15.post1.tar` & `mypy-boto3-iot-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.933182 mypy-boto3-iot-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    55458 2023-07-29 10:03:19.925182 mypy-boto3-iot-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    53981 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.921182 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   183696 2023-07-29 09:47:30.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   183380 2023-07-29 09:47:29.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25037 2023-07-29 09:47:31.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-29 09:47:31.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    68966 2023-07-29 09:47:30.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    68905 2023-07-29 09:47:30.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   270219 2023-07-29 09:47:42.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   269870 2023-07-29 09:47:36.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.925182 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    55458 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:19.933182 mypy-boto3-iot-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.776866 mypy-boto3-iot-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:09.000000 mypy-boto3-iot-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    56098 2023-08-01 11:36:59.776866 mypy-boto3-iot-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54630 2023-08-01 11:20:09.000000 mypy-boto3-iot-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.768866 mypy-boto3-iot-1.28.16/mypy_boto3_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-08-01 11:20:09.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-08-01 11:20:09.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:20:09.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181808 2023-08-01 11:20:13.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181492 2023-08-01 11:20:10.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25037 2023-08-01 11:20:14.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-08-01 11:20:14.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    68895 2023-08-01 11:20:14.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68834 2023-08-01 11:20:13.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:09.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   272423 2023-08-01 11:20:23.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   272075 2023-08-01 11:20:18.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:09.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.776866 mypy-boto3-iot-1.28.16/mypy_boto3_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    56098 2023-08-01 11:36:59.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:36:59.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:59.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:59.000000 mypy-boto3-iot-1.28.16/mypy_boto3_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:59.776866 mypy-boto3-iot-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:20:09.000000 mypy-boto3-iot-1.28.16/setup.py
```

### Comparing `mypy-boto3-iot-1.28.15.post1/LICENSE` & `mypy-boto3-iot-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15.post1/PKG-INFO` & `mypy-boto3-iot-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoT 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iot type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot)](https://pepy.tech/project/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
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
@@ -636,20 +636,20 @@
 )
 
 
 def check_value(value: AbortActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot.type_defs import (
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
@@ -709,31 +709,32 @@
     MachineLearningDetectionConfigTypeDef,
     StatisticalThresholdTypeDef,
     MetricValueTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
     BillingGroupPropertiesTypeDef,
+    BlobTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
     CodeSigningCertificateChainTypeDef,
     CodeSigningSignatureOutputTypeDef,
-    CodeSigningSignatureTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
+    TimestampTypeDef,
     TagTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
     TlsConfigTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
     MaintenanceWindowTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
@@ -869,35 +870,30 @@
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
-    ListAuditMitigationActionsTasksRequestRequestTypeDef,
-    ListAuditTasksRequestRequestTypeDef,
     ListAuthorizersRequestRequestTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
     ListCACertificatesRequestRequestTypeDef,
     ListCertificatesByCARequestRequestTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListCustomMetricsRequestRequestTypeDef,
-    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
-    ListDetectMitigationActionsTasksRequestRequestTypeDef,
     ListDimensionsRequestRequestTypeDef,
     ListDomainConfigurationsRequestRequestTypeDef,
     ListFleetMetricsRequestRequestTypeDef,
     ListIndicesRequestRequestTypeDef,
     ListJobExecutionsForJobRequestRequestTypeDef,
     ListJobExecutionsForThingRequestRequestTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListManagedJobTemplatesRequestRequestTypeDef,
     ManagedJobTemplateSummaryTypeDef,
-    ListMetricValuesRequestRequestTypeDef,
     ListMitigationActionsRequestRequestTypeDef,
     MitigationActionIdentifierTypeDef,
     ListOTAUpdatesRequestRequestTypeDef,
     OTAUpdateSummaryTypeDef,
     ListOutgoingCertificatesRequestRequestTypeDef,
     OutgoingCertificateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
@@ -937,23 +933,21 @@
     ListThingsInThingGroupRequestRequestTypeDef,
     ListThingsRequestRequestTypeDef,
     ThingAttributeTypeDef,
     ListTopicRuleDestinationsRequestRequestTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
-    ListViolationEventsRequestRequestTypeDef,
     LocationTimestampTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
-    MqttContextTypeDef,
     UserPropertyTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
     RegisterThingRequestRequestTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
@@ -961,15 +955,14 @@
     RemoveThingFromThingGroupRequestRequestTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
     SigningProfileParameterTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
     ThingConnectivityTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
@@ -988,14 +981,15 @@
     UpdateScheduledAuditRequestRequestTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
     AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
+    AggregationTypeUnionTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
     AssetPropertyValueTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
     CancelJobResponseTypeDef,
@@ -1077,46 +1071,56 @@
     UpdateDynamicThingGroupResponseTypeDef,
     UpdateMitigationActionResponseTypeDef,
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ThingGroupPropertiesOutputTypeDef,
+    AttributePayloadUnionTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
     DescribeAccountAuditConfigurationResponseTypeDef,
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
-    TestAuthorizationRequestRequestTypeDef,
+    AuthInfoUnionTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
     BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
+    CodeSigningSignatureTypeDef,
+    MqttContextTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
     CertificateDescriptionTypeDef,
     ListCertificatesByCAResponseTypeDef,
     ListCertificatesResponseTypeDef,
     CustomCodeSigningOutputTypeDef,
-    CustomCodeSigningTypeDef,
     DescribeEventConfigurationsResponseTypeDef,
     UpdateEventConfigurationsRequestRequestTypeDef,
+    ListAuditMitigationActionsTasksRequestRequestTypeDef,
+    ListAuditTasksRequestRequestTypeDef,
+    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
+    ListDetectMitigationActionsTasksRequestRequestTypeDef,
+    ListMetricValuesRequestRequestTypeDef,
+    ListViolationEventsRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
@@ -1137,16 +1141,18 @@
     RegisterCACertificateRequestRequestTypeDef,
     UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     ListDomainConfigurationsResponseTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     ExponentialRolloutRateTypeDef,
     ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
     StreamFileTypeDef,
@@ -1248,56 +1254,66 @@
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
     MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
     MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
     ResourceIdentifierTypeDef,
-    StartDetectMitigationActionsTaskRequestRequestTypeDef,
-    TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
     TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
+    AbortConfigUnionTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
     PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
+    TestAuthorizationRequestRequestTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     BehaviorOutputTypeDef,
     BehaviorTypeDef,
+    CustomCodeSigningTypeDef,
+    TestInvokeAuthorizerRequestRequestTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
+    StartDetectMitigationActionsTaskRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
+    SchedulingConfigUnionTypeDef,
     ListThingTypesResponseTypeDef,
     StartSigningJobParameterTypeDef,
     JobExecutionsRolloutConfigTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
     CreateStreamRequestRequestTypeDef,
     StreamInfoTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
     HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     ListJobExecutionsForJobResponseTypeDef,
     ListJobExecutionsForThingResponseTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
     CreateMitigationActionRequestRequestTypeDef,
+    MitigationActionParamsUnionTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
     RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
@@ -1317,17 +1333,15 @@
     AuthResultTypeDef,
     IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     ActiveViolationTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     ViolationEventTypeDef,
-    CreateSecurityProfileRequestRequestTypeDef,
-    UpdateSecurityProfileRequestRequestTypeDef,
-    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
+    BehaviorUnionTypeDef,
     CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
     CreateJobRequestRequestTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     JobTypeDef,
     UpdateJobRequestRequestTypeDef,
@@ -1338,33 +1352,37 @@
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
     TestAuthorizationResponseTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
+    CreateSecurityProfileRequestRequestTypeDef,
+    UpdateSecurityProfileRequestRequestTypeDef,
+    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     DescribeJobResponseTypeDef,
     DescribeDetectMitigationActionsTaskResponseTypeDef,
     ListDetectMitigationActionsTasksResponseTypeDef,
     DescribeAuditFindingResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     TopicRuleTypeDef,
     TopicRulePayloadTypeDef,
     OTAUpdateInfoTypeDef,
-    CreateOTAUpdateRequestRequestTypeDef,
+    OTAUpdateFileUnionTypeDef,
     GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
     GetOTAUpdateResponseTypeDef,
+    CreateOTAUpdateRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaTypeDef:
+def get_value() -> AbortCriteriaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-1.28.15.post1/README.md` & `mypy-boto3-iot-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot)](https://pepy.tech/project/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
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
@@ -604,20 +604,20 @@
 )
 
 
 def check_value(value: AbortActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot.type_defs import (
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
@@ -677,31 +677,32 @@
     MachineLearningDetectionConfigTypeDef,
     StatisticalThresholdTypeDef,
     MetricValueTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
     BillingGroupPropertiesTypeDef,
+    BlobTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
     CodeSigningCertificateChainTypeDef,
     CodeSigningSignatureOutputTypeDef,
-    CodeSigningSignatureTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
+    TimestampTypeDef,
     TagTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
     TlsConfigTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
     MaintenanceWindowTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
@@ -837,35 +838,30 @@
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
-    ListAuditMitigationActionsTasksRequestRequestTypeDef,
-    ListAuditTasksRequestRequestTypeDef,
     ListAuthorizersRequestRequestTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
     ListCACertificatesRequestRequestTypeDef,
     ListCertificatesByCARequestRequestTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListCustomMetricsRequestRequestTypeDef,
-    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
-    ListDetectMitigationActionsTasksRequestRequestTypeDef,
     ListDimensionsRequestRequestTypeDef,
     ListDomainConfigurationsRequestRequestTypeDef,
     ListFleetMetricsRequestRequestTypeDef,
     ListIndicesRequestRequestTypeDef,
     ListJobExecutionsForJobRequestRequestTypeDef,
     ListJobExecutionsForThingRequestRequestTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListManagedJobTemplatesRequestRequestTypeDef,
     ManagedJobTemplateSummaryTypeDef,
-    ListMetricValuesRequestRequestTypeDef,
     ListMitigationActionsRequestRequestTypeDef,
     MitigationActionIdentifierTypeDef,
     ListOTAUpdatesRequestRequestTypeDef,
     OTAUpdateSummaryTypeDef,
     ListOutgoingCertificatesRequestRequestTypeDef,
     OutgoingCertificateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
@@ -905,23 +901,21 @@
     ListThingsInThingGroupRequestRequestTypeDef,
     ListThingsRequestRequestTypeDef,
     ThingAttributeTypeDef,
     ListTopicRuleDestinationsRequestRequestTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
-    ListViolationEventsRequestRequestTypeDef,
     LocationTimestampTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
-    MqttContextTypeDef,
     UserPropertyTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
     RegisterThingRequestRequestTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
@@ -929,15 +923,14 @@
     RemoveThingFromThingGroupRequestRequestTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
     SigningProfileParameterTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
     ThingConnectivityTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
@@ -956,14 +949,15 @@
     UpdateScheduledAuditRequestRequestTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
     AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
+    AggregationTypeUnionTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
     AssetPropertyValueTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
     CancelJobResponseTypeDef,
@@ -1045,46 +1039,56 @@
     UpdateDynamicThingGroupResponseTypeDef,
     UpdateMitigationActionResponseTypeDef,
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ThingGroupPropertiesOutputTypeDef,
+    AttributePayloadUnionTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
     DescribeAccountAuditConfigurationResponseTypeDef,
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
-    TestAuthorizationRequestRequestTypeDef,
+    AuthInfoUnionTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
     BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
+    CodeSigningSignatureTypeDef,
+    MqttContextTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
     CertificateDescriptionTypeDef,
     ListCertificatesByCAResponseTypeDef,
     ListCertificatesResponseTypeDef,
     CustomCodeSigningOutputTypeDef,
-    CustomCodeSigningTypeDef,
     DescribeEventConfigurationsResponseTypeDef,
     UpdateEventConfigurationsRequestRequestTypeDef,
+    ListAuditMitigationActionsTasksRequestRequestTypeDef,
+    ListAuditTasksRequestRequestTypeDef,
+    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
+    ListDetectMitigationActionsTasksRequestRequestTypeDef,
+    ListMetricValuesRequestRequestTypeDef,
+    ListViolationEventsRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
@@ -1105,16 +1109,18 @@
     RegisterCACertificateRequestRequestTypeDef,
     UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     ListDomainConfigurationsResponseTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     ExponentialRolloutRateTypeDef,
     ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
     StreamFileTypeDef,
@@ -1216,56 +1222,66 @@
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
     MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
     MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
     ResourceIdentifierTypeDef,
-    StartDetectMitigationActionsTaskRequestRequestTypeDef,
-    TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
     TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
+    AbortConfigUnionTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
     PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
+    TestAuthorizationRequestRequestTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     BehaviorOutputTypeDef,
     BehaviorTypeDef,
+    CustomCodeSigningTypeDef,
+    TestInvokeAuthorizerRequestRequestTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
+    StartDetectMitigationActionsTaskRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
+    SchedulingConfigUnionTypeDef,
     ListThingTypesResponseTypeDef,
     StartSigningJobParameterTypeDef,
     JobExecutionsRolloutConfigTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
     CreateStreamRequestRequestTypeDef,
     StreamInfoTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
     HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     ListJobExecutionsForJobResponseTypeDef,
     ListJobExecutionsForThingResponseTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
     CreateMitigationActionRequestRequestTypeDef,
+    MitigationActionParamsUnionTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
     RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
@@ -1285,17 +1301,15 @@
     AuthResultTypeDef,
     IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     ActiveViolationTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     ViolationEventTypeDef,
-    CreateSecurityProfileRequestRequestTypeDef,
-    UpdateSecurityProfileRequestRequestTypeDef,
-    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
+    BehaviorUnionTypeDef,
     CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
     CreateJobRequestRequestTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     JobTypeDef,
     UpdateJobRequestRequestTypeDef,
@@ -1306,33 +1320,37 @@
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
     TestAuthorizationResponseTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
+    CreateSecurityProfileRequestRequestTypeDef,
+    UpdateSecurityProfileRequestRequestTypeDef,
+    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     DescribeJobResponseTypeDef,
     DescribeDetectMitigationActionsTaskResponseTypeDef,
     ListDetectMitigationActionsTasksResponseTypeDef,
     DescribeAuditFindingResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     TopicRuleTypeDef,
     TopicRulePayloadTypeDef,
     OTAUpdateInfoTypeDef,
-    CreateOTAUpdateRequestRequestTypeDef,
+    OTAUpdateFileUnionTypeDef,
     GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
     GetOTAUpdateResponseTypeDef,
+    CreateOTAUpdateRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaTypeDef:
+def get_value() -> AbortCriteriaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__init__.py` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__init__.pyi` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__main__.py` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoT 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
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

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/client.py` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iot.client import IoTClient
 
     session = Session()
     client: IoTClient = session.client("iot")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuditFrequencyType,
     AuditMitigationActionsExecutionStatusType,
     AuditMitigationActionsTaskStatusType,
@@ -112,35 +111,29 @@
     ListThingTypesPaginator,
     ListTopicRuleDestinationsPaginator,
     ListTopicRulesPaginator,
     ListV2LoggingLevelsPaginator,
     ListViolationEventsPaginator,
 )
 from .type_defs import (
-    AbortConfigOutputTypeDef,
-    AbortConfigTypeDef,
-    AggregationTypeOutputTypeDef,
-    AggregationTypeTypeDef,
+    AbortConfigUnionTypeDef,
+    AggregationTypeUnionTypeDef,
     AlertTargetTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
-    AttributePayloadOutputTypeDef,
-    AttributePayloadTypeDef,
+    AttributePayloadUnionTypeDef,
     AuditCheckConfigurationTypeDef,
-    AuditMitigationActionsTaskTargetOutputTypeDef,
-    AuditMitigationActionsTaskTargetTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     AuditNotificationTargetTypeDef,
-    AuthInfoOutputTypeDef,
-    AuthInfoTypeDef,
+    AuthInfoUnionTypeDef,
     AuthorizerConfigTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
-    BehaviorOutputTypeDef,
-    BehaviorTypeDef,
+    BehaviorUnionTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketsAggregationTypeTypeDef,
     CancelJobResponseTypeDef,
     ConfigurationTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrResponseTypeDef,
@@ -198,16 +191,15 @@
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeThingGroupResponseTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
-    DetectMitigationActionsTaskTargetOutputTypeDef,
-    DetectMitigationActionsTaskTargetTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     GetBucketsAggregationResponseTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     GetJobDocumentResponseTypeDef,
@@ -221,16 +213,15 @@
     GetPolicyVersionResponseTypeDef,
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     GetTopicRuleResponseTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     HttpContextTypeDef,
-    JobExecutionsRetryConfigOutputTypeDef,
-    JobExecutionsRetryConfigTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     JobExecutionsRolloutConfigTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     ListAuditSuppressionsResponseTypeDef,
@@ -287,48 +278,42 @@
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
     MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
-    MitigationActionParamsOutputTypeDef,
-    MitigationActionParamsTypeDef,
+    MitigationActionParamsUnionTypeDef,
     MqttContextTypeDef,
-    OTAUpdateFileOutputTypeDef,
-    OTAUpdateFileTypeDef,
+    OTAUpdateFileUnionTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
-    SchedulingConfigOutputTypeDef,
-    SchedulingConfigTypeDef,
+    SchedulingConfigUnionTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
     TagTypeDef,
     TestAuthorizationResponseTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
-    ThingGroupIndexingConfigurationOutputTypeDef,
-    ThingGroupIndexingConfigurationTypeDef,
-    ThingGroupPropertiesOutputTypeDef,
-    ThingGroupPropertiesTypeDef,
-    ThingIndexingConfigurationOutputTypeDef,
-    ThingIndexingConfigurationTypeDef,
-    ThingTypePropertiesOutputTypeDef,
-    ThingTypePropertiesTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     TimeoutConfigTypeDef,
+    TimestampTypeDef,
     TlsConfigTypeDef,
     TlsContextTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRulePayloadTypeDef,
     TransferCertificateResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
     UpdateBillingGroupResponseTypeDef,
@@ -340,16 +325,15 @@
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     VersionUpdateByJobsConfigTypeDef,
-    ViolationEventOccurrenceRangeOutputTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -601,15 +585,15 @@
 
     def create_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
         clientRequestToken: str,
-        expirationDate: Union[datetime, str] = ...,
+        expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
         description: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_audit_suppression)
@@ -713,17 +697,15 @@
         """
 
     def create_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
         queryString: str,
-        thingGroupProperties: Union[
-            ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
-        ] = ...,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
         indexName: str = ...,
         queryVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
@@ -732,15 +714,15 @@
         """
 
     def create_fleet_metric(
         self,
         *,
         metricName: str,
         queryString: str,
-        aggregationType: Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef],
+        aggregationType: AggregationTypeUnionTypeDef,
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -759,24 +741,22 @@
         targets: Sequence[str],
         documentSource: str = ...,
         document: str = ...,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         targetSelection: TargetSelectionType = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
-        jobExecutionsRetryConfig: Union[
-            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
-        ] = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
         documentParameters: Mapping[str, str] = ...,
-        schedulingConfig: Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef] = ...,
+        schedulingConfig: SchedulingConfigUnionTypeDef = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_job)
@@ -788,20 +768,18 @@
         jobTemplateId: str,
         description: str,
         jobArn: str = ...,
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: Union[
-            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
-        ] = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
@@ -820,15 +798,15 @@
         """
 
     def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
-        actionParams: Union[MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef],
+        actionParams: MitigationActionParamsUnionTypeDef,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
@@ -836,15 +814,15 @@
         """
 
     def create_ota_update(
         self,
         *,
         otaUpdateId: str,
         targets: Sequence[str],
-        files: Sequence[Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]],
+        files: Sequence[OTAUpdateFileUnionTypeDef],
         roleArn: str,
         description: str = ...,
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
@@ -983,15 +961,15 @@
         """
 
     def create_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]] = ...,
+        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
@@ -1017,48 +995,44 @@
         """
 
     def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef] = ...,
+        attributePayload: AttributePayloadUnionTypeDef = ...,
         billingGroupName: str = ...
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing)
         """
 
     def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
-        thingGroupProperties: Union[
-            ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
-        ] = ...,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_group)
         """
 
     def create_thing_type(
         self,
         *,
         thingTypeName: str,
-        thingTypeProperties: Union[
-            ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
-        ] = ...,
+        thingTypeProperties: ThingTypePropertiesUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_type)
@@ -1986,16 +1960,16 @@
         self,
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...
     ) -> ListAuditFindingsResponseTypeDef:
         """
         Lists the findings (results) of a Device Defender audit or of the audits
         performed during a specified time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_findings)
@@ -2017,16 +1991,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_mitigation_actions_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#list_audit_mitigation_actions_executions)
         """
 
     def list_audit_mitigation_actions_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListAuditMitigationActionsTasksResponseTypeDef:
         """
@@ -2051,16 +2025,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_suppressions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#list_audit_suppressions)
         """
 
     def list_audit_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListAuditTasksResponseTypeDef:
         """
         Lists the Device Defender audits that have been performed during a given time
@@ -2147,32 +2121,32 @@
 
     def list_detect_mitigation_actions_executions(
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListDetectMitigationActionsExecutionsResponseTypeDef:
         """
         Lists mitigation actions executions for a Device Defender ML Detect Security
         Profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#list_detect_mitigation_actions_executions)
         """
 
     def list_detect_mitigation_actions_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListDetectMitigationActionsTasksResponseTypeDef:
         """
         List of Device Defender ML Detect mitigation actions tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_tasks)
@@ -2291,16 +2265,16 @@
         """
 
     def list_metric_values(
         self,
         *,
         thingName: str,
         metricName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListMetricValuesResponseTypeDef:
         """
         Lists the values reported for an IoT Device Defender metric (device-side metric,
@@ -2690,16 +2664,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_v2_logging_levels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#list_v2_logging_levels)
         """
 
     def list_violation_events(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -2897,39 +2871,33 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#set_v2_logging_options)
         """
 
     def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: Union[
-            AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
-        ],
+        target: AuditMitigationActionsTaskTargetUnionTypeDef,
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
         clientRequestToken: str
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#start_audit_mitigation_actions_task)
         """
 
     def start_detect_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: Union[
-            DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
-        ],
+        target: DetectMitigationActionsTaskTargetUnionTypeDef,
         actions: Sequence[str],
         clientRequestToken: str,
-        violationEventOccurrenceRange: Union[
-            ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
-        ] = ...,
+        violationEventOccurrenceRange: ViolationEventOccurrenceRangeUnionTypeDef = ...,
         includeOnlyActiveViolations: bool = ...,
         includeSuppressedAlerts: bool = ...
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
@@ -2971,15 +2939,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#tag_resource)
         """
 
     def test_authorization(
         self,
         *,
-        authInfos: Sequence[Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]],
+        authInfos: Sequence[AuthInfoUnionTypeDef],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
         policyNamesToSkip: Sequence[str] = ...
     ) -> TestAuthorizationResponseTypeDef:
         """
@@ -3043,15 +3011,15 @@
         """
 
     def update_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
-        expirationDate: Union[datetime, str] = ...,
+        expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
         description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_audit_suppression)
@@ -3151,15 +3119,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_domain_configuration)
         """
 
     def update_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: Union[ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef],
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
         queryVersion: str = ...
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
@@ -3180,15 +3148,15 @@
 
     def update_fleet_metric(
         self,
         *,
         metricName: str,
         indexName: str,
         queryString: str = ...,
-        aggregationType: Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef] = ...,
+        aggregationType: AggregationTypeUnionTypeDef = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
         expectedVersion: int = ...
     ) -> EmptyResponseMetadataTypeDef:
@@ -3198,20 +3166,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_fleet_metric)
         """
 
     def update_indexing_configuration(
         self,
         *,
-        thingIndexingConfiguration: Union[
-            ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
-        ] = ...,
-        thingGroupIndexingConfiguration: Union[
-            ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
-        ] = ...
+        thingIndexingConfiguration: ThingIndexingConfigurationUnionTypeDef = ...,
+        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_indexing_configuration)
         """
@@ -3219,36 +3183,32 @@
     def update_job(
         self,
         *,
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: Union[
-            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
-        ] = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_job)
         """
 
     def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: Union[
-            MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
-        ] = ...
+        actionParams: MitigationActionParamsUnionTypeDef = ...
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_mitigation_action)
         """
@@ -3345,15 +3305,15 @@
         """
 
     def update_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]] = ...,
+        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...
@@ -3381,30 +3341,30 @@
         """
 
     def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef] = ...,
+        attributePayload: AttributePayloadUnionTypeDef = ...,
         expectedVersion: int = ...,
         removeThingType: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_thing)
         """
 
     def update_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: Union[ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef],
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
         expectedVersion: int = ...
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_thing_group)
@@ -3432,15 +3392,15 @@
         Updates a topic rule destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_topic_rule_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_topic_rule_destination)
         """
 
     def validate_security_profile_behaviors(
-        self, *, behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]]
+        self, *, behaviors: Sequence[BehaviorUnionTypeDef]
     ) -> ValidateSecurityProfileBehaviorsResponseTypeDef:
         """
         Validates a Device Defender security profile behaviors specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.validate_security_profile_behaviors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#validate_security_profile_behaviors)
         """
```

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/client.pyi` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iot.client import IoTClient
 
     session = Session()
     client: IoTClient = session.client("iot")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuditFrequencyType,
     AuditMitigationActionsExecutionStatusType,
     AuditMitigationActionsTaskStatusType,
@@ -112,35 +111,29 @@
     ListThingTypesPaginator,
     ListTopicRuleDestinationsPaginator,
     ListTopicRulesPaginator,
     ListV2LoggingLevelsPaginator,
     ListViolationEventsPaginator,
 )
 from .type_defs import (
-    AbortConfigOutputTypeDef,
-    AbortConfigTypeDef,
-    AggregationTypeOutputTypeDef,
-    AggregationTypeTypeDef,
+    AbortConfigUnionTypeDef,
+    AggregationTypeUnionTypeDef,
     AlertTargetTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
-    AttributePayloadOutputTypeDef,
-    AttributePayloadTypeDef,
+    AttributePayloadUnionTypeDef,
     AuditCheckConfigurationTypeDef,
-    AuditMitigationActionsTaskTargetOutputTypeDef,
-    AuditMitigationActionsTaskTargetTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     AuditNotificationTargetTypeDef,
-    AuthInfoOutputTypeDef,
-    AuthInfoTypeDef,
+    AuthInfoUnionTypeDef,
     AuthorizerConfigTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
-    BehaviorOutputTypeDef,
-    BehaviorTypeDef,
+    BehaviorUnionTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketsAggregationTypeTypeDef,
     CancelJobResponseTypeDef,
     ConfigurationTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrResponseTypeDef,
@@ -198,16 +191,15 @@
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeThingGroupResponseTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
-    DetectMitigationActionsTaskTargetOutputTypeDef,
-    DetectMitigationActionsTaskTargetTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     GetBucketsAggregationResponseTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     GetJobDocumentResponseTypeDef,
@@ -221,16 +213,15 @@
     GetPolicyVersionResponseTypeDef,
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     GetTopicRuleResponseTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     HttpContextTypeDef,
-    JobExecutionsRetryConfigOutputTypeDef,
-    JobExecutionsRetryConfigTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     JobExecutionsRolloutConfigTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     ListAuditSuppressionsResponseTypeDef,
@@ -287,48 +278,42 @@
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
     MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
-    MitigationActionParamsOutputTypeDef,
-    MitigationActionParamsTypeDef,
+    MitigationActionParamsUnionTypeDef,
     MqttContextTypeDef,
-    OTAUpdateFileOutputTypeDef,
-    OTAUpdateFileTypeDef,
+    OTAUpdateFileUnionTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
-    SchedulingConfigOutputTypeDef,
-    SchedulingConfigTypeDef,
+    SchedulingConfigUnionTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
     TagTypeDef,
     TestAuthorizationResponseTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
-    ThingGroupIndexingConfigurationOutputTypeDef,
-    ThingGroupIndexingConfigurationTypeDef,
-    ThingGroupPropertiesOutputTypeDef,
-    ThingGroupPropertiesTypeDef,
-    ThingIndexingConfigurationOutputTypeDef,
-    ThingIndexingConfigurationTypeDef,
-    ThingTypePropertiesOutputTypeDef,
-    ThingTypePropertiesTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     TimeoutConfigTypeDef,
+    TimestampTypeDef,
     TlsConfigTypeDef,
     TlsContextTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRulePayloadTypeDef,
     TransferCertificateResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
     UpdateBillingGroupResponseTypeDef,
@@ -340,16 +325,15 @@
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     VersionUpdateByJobsConfigTypeDef,
-    ViolationEventOccurrenceRangeOutputTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -578,15 +562,15 @@
         """
     def create_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
         clientRequestToken: str,
-        expirationDate: Union[datetime, str] = ...,
+        expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
         description: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_audit_suppression)
@@ -683,17 +667,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_domain_configuration)
         """
     def create_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
         queryString: str,
-        thingGroupProperties: Union[
-            ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
-        ] = ...,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
         indexName: str = ...,
         queryVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
@@ -701,15 +683,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_dynamic_thing_group)
         """
     def create_fleet_metric(
         self,
         *,
         metricName: str,
         queryString: str,
-        aggregationType: Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef],
+        aggregationType: AggregationTypeUnionTypeDef,
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -727,24 +709,22 @@
         targets: Sequence[str],
         documentSource: str = ...,
         document: str = ...,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         targetSelection: TargetSelectionType = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
-        jobExecutionsRetryConfig: Union[
-            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
-        ] = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
         documentParameters: Mapping[str, str] = ...,
-        schedulingConfig: Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef] = ...,
+        schedulingConfig: SchedulingConfigUnionTypeDef = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_job)
@@ -755,20 +735,18 @@
         jobTemplateId: str,
         description: str,
         jobArn: str = ...,
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: Union[
-            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
-        ] = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
@@ -785,30 +763,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_keys_and_certificate)
         """
     def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
-        actionParams: Union[MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef],
+        actionParams: MitigationActionParamsUnionTypeDef,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_mitigation_action)
         """
     def create_ota_update(
         self,
         *,
         otaUpdateId: str,
         targets: Sequence[str],
-        files: Sequence[Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]],
+        files: Sequence[OTAUpdateFileUnionTypeDef],
         roleArn: str,
         description: str = ...,
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
@@ -937,15 +915,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_scheduled_audit)
         """
     def create_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]] = ...,
+        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
@@ -969,46 +947,42 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_stream)
         """
     def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef] = ...,
+        attributePayload: AttributePayloadUnionTypeDef = ...,
         billingGroupName: str = ...
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing)
         """
     def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
-        thingGroupProperties: Union[
-            ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
-        ] = ...,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_group)
         """
     def create_thing_type(
         self,
         *,
         thingTypeName: str,
-        thingTypeProperties: Union[
-            ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
-        ] = ...,
+        thingTypeProperties: ThingTypePropertiesUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_type)
@@ -1838,16 +1812,16 @@
         self,
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...
     ) -> ListAuditFindingsResponseTypeDef:
         """
         Lists the findings (results) of a Device Defender audit or of the audits
         performed during a specified time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_findings)
@@ -1867,16 +1841,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_mitigation_actions_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#list_audit_mitigation_actions_executions)
         """
     def list_audit_mitigation_actions_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListAuditMitigationActionsTasksResponseTypeDef:
         """
@@ -1899,16 +1873,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_suppressions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#list_audit_suppressions)
         """
     def list_audit_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListAuditTasksResponseTypeDef:
         """
         Lists the Device Defender audits that have been performed during a given time
@@ -1988,31 +1962,31 @@
         """
     def list_detect_mitigation_actions_executions(
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListDetectMitigationActionsExecutionsResponseTypeDef:
         """
         Lists mitigation actions executions for a Device Defender ML Detect Security
         Profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#list_detect_mitigation_actions_executions)
         """
     def list_detect_mitigation_actions_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListDetectMitigationActionsTasksResponseTypeDef:
         """
         List of Device Defender ML Detect mitigation actions tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_tasks)
@@ -2121,16 +2095,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#list_managed_job_templates)
         """
     def list_metric_values(
         self,
         *,
         thingName: str,
         metricName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListMetricValuesResponseTypeDef:
         """
         Lists the values reported for an IoT Device Defender metric (device-side metric,
@@ -2486,16 +2460,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_v2_logging_levels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#list_v2_logging_levels)
         """
     def list_violation_events(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -2677,38 +2651,32 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.set_v2_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#set_v2_logging_options)
         """
     def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: Union[
-            AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
-        ],
+        target: AuditMitigationActionsTaskTargetUnionTypeDef,
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
         clientRequestToken: str
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#start_audit_mitigation_actions_task)
         """
     def start_detect_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: Union[
-            DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
-        ],
+        target: DetectMitigationActionsTaskTargetUnionTypeDef,
         actions: Sequence[str],
         clientRequestToken: str,
-        violationEventOccurrenceRange: Union[
-            ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
-        ] = ...,
+        violationEventOccurrenceRange: ViolationEventOccurrenceRangeUnionTypeDef = ...,
         includeOnlyActiveViolations: bool = ...,
         includeSuppressedAlerts: bool = ...
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
@@ -2745,15 +2713,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#tag_resource)
         """
     def test_authorization(
         self,
         *,
-        authInfos: Sequence[Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]],
+        authInfos: Sequence[AuthInfoUnionTypeDef],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
         policyNamesToSkip: Sequence[str] = ...
     ) -> TestAuthorizationResponseTypeDef:
         """
@@ -2812,15 +2780,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_account_audit_configuration)
         """
     def update_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
-        expirationDate: Union[datetime, str] = ...,
+        expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
         description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_audit_suppression)
@@ -2912,15 +2880,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_domain_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_domain_configuration)
         """
     def update_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: Union[ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef],
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
         queryVersion: str = ...
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
@@ -2939,15 +2907,15 @@
         """
     def update_fleet_metric(
         self,
         *,
         metricName: str,
         indexName: str,
         queryString: str = ...,
-        aggregationType: Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef] = ...,
+        aggregationType: AggregationTypeUnionTypeDef = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
         expectedVersion: int = ...
     ) -> EmptyResponseMetadataTypeDef:
@@ -2956,55 +2924,47 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_fleet_metric)
         """
     def update_indexing_configuration(
         self,
         *,
-        thingIndexingConfiguration: Union[
-            ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
-        ] = ...,
-        thingGroupIndexingConfiguration: Union[
-            ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
-        ] = ...
+        thingIndexingConfiguration: ThingIndexingConfigurationUnionTypeDef = ...,
+        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_indexing_configuration)
         """
     def update_job(
         self,
         *,
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: Union[
-            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
-        ] = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_job)
         """
     def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: Union[
-            MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
-        ] = ...
+        actionParams: MitigationActionParamsUnionTypeDef = ...
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_mitigation_action)
         """
@@ -3094,15 +3054,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_scheduled_audit)
         """
     def update_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]] = ...,
+        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...
@@ -3128,29 +3088,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_stream)
         """
     def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef] = ...,
+        attributePayload: AttributePayloadUnionTypeDef = ...,
         expectedVersion: int = ...,
         removeThingType: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_thing)
         """
     def update_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: Union[ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef],
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
         expectedVersion: int = ...
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_thing_group)
@@ -3175,15 +3135,15 @@
         """
         Updates a topic rule destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_topic_rule_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_topic_rule_destination)
         """
     def validate_security_profile_behaviors(
-        self, *, behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]]
+        self, *, behaviors: Sequence[BehaviorUnionTypeDef]
     ) -> ValidateSecurityProfileBehaviorsResponseTypeDef:
         """
         Validates a Device Defender security profile behaviors specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.validate_security_profile_behaviors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#validate_security_profile_behaviors)
         """
```

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/literals.py` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/literals.pyi` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/paginator.py` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,15 @@
     list_things_in_thing_group_paginator: ListThingsInThingGroupPaginator = client.get_paginator("list_things_in_thing_group")
     list_topic_rule_destinations_paginator: ListTopicRuleDestinationsPaginator = client.get_paginator("list_topic_rule_destinations")
     list_topic_rules_paginator: ListTopicRulesPaginator = client.get_paginator("list_topic_rules")
     list_v2_logging_levels_paginator: ListV2LoggingLevelsPaginator = client.get_paginator("list_v2_logging_levels")
     list_violation_events_paginator: ListViolationEventsPaginator = client.get_paginator("list_violation_events")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AuditMitigationActionsExecutionStatusType,
     AuditMitigationActionsTaskStatusType,
     AuditTaskStatusType,
@@ -218,14 +217,15 @@
     ListThingTypesResponseTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     PaginatorConfigTypeDef,
     ResourceIdentifierTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetBehaviorModelTrainingSummariesPaginator",
     "ListActiveViolationsPaginator",
     "ListAttachedPoliciesPaginator",
     "ListAuditFindingsPaginator",
@@ -357,16 +357,16 @@
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditfindingspaginator)
         """
@@ -397,16 +397,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditmitigationactionstaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks.paginate)
@@ -439,16 +439,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listaudittaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listaudittaskspaginator)
@@ -565,16 +565,16 @@
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionsexecutionspaginator)
         """
 
@@ -584,16 +584,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionstaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionstaskspaginator)
         """
 
@@ -757,16 +757,16 @@
     """
 
     def paginate(
         self,
         *,
         thingName: str,
         metricName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMetricValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMetricValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmetricvaluespaginator)
@@ -1307,16 +1307,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listviolationeventspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListViolationEventsResponseTypeDef]:
```

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/paginator.pyi` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,15 @@
     list_things_in_thing_group_paginator: ListThingsInThingGroupPaginator = client.get_paginator("list_things_in_thing_group")
     list_topic_rule_destinations_paginator: ListTopicRuleDestinationsPaginator = client.get_paginator("list_topic_rule_destinations")
     list_topic_rules_paginator: ListTopicRulesPaginator = client.get_paginator("list_topic_rules")
     list_v2_logging_levels_paginator: ListV2LoggingLevelsPaginator = client.get_paginator("list_v2_logging_levels")
     list_violation_events_paginator: ListViolationEventsPaginator = client.get_paginator("list_violation_events")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AuditMitigationActionsExecutionStatusType,
     AuditMitigationActionsTaskStatusType,
     AuditTaskStatusType,
@@ -218,14 +217,15 @@
     ListThingTypesResponseTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     PaginatorConfigTypeDef,
     ResourceIdentifierTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetBehaviorModelTrainingSummariesPaginator",
     "ListActiveViolationsPaginator",
     "ListAttachedPoliciesPaginator",
     "ListAuditFindingsPaginator",
@@ -351,16 +351,16 @@
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditfindingspaginator)
         """
@@ -389,16 +389,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditmitigationactionstaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks.paginate)
@@ -429,16 +429,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listaudittaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listaudittaskspaginator)
@@ -548,16 +548,16 @@
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionsexecutionspaginator)
         """
 
@@ -566,16 +566,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionstaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionstaskspaginator)
         """
 
@@ -729,16 +729,16 @@
     """
 
     def paginate(
         self,
         *,
         thingName: str,
         metricName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMetricValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMetricValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmetricvaluespaginator)
@@ -1246,16 +1246,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listviolationeventspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListViolationEventsResponseTypeDef]:
```

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/type_defs.py` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iot.type_defs import AbortCriteriaTypeDef
 
-    data: AbortCriteriaTypeDef = {...}
+    data: AbortCriteriaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -153,31 +153,32 @@
     "MachineLearningDetectionConfigTypeDef",
     "StatisticalThresholdTypeDef",
     "MetricValueTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
     "BillingGroupPropertiesTypeDef",
+    "BlobTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
     "CertificateValidityTypeDef",
     "CACertificateTypeDef",
     "CancelAuditMitigationActionsTaskRequestRequestTypeDef",
     "CancelAuditTaskRequestRequestTypeDef",
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
     "CodeSigningCertificateChainTypeDef",
     "CodeSigningSignatureOutputTypeDef",
-    "CodeSigningSignatureTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "TagTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "PresignedUrlConfigTypeDef",
     "TimeoutConfigTypeDef",
     "MaintenanceWindowTypeDef",
     "CreateKeysAndCertificateRequestRequestTypeDef",
@@ -313,35 +314,30 @@
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
     "ScheduledJobRolloutTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
     "ListAttachedPoliciesRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListAuditMitigationActionsTasksRequestRequestTypeDef",
-    "ListAuditTasksRequestRequestTypeDef",
     "ListAuthorizersRequestRequestTypeDef",
     "ListBillingGroupsRequestRequestTypeDef",
     "ListCACertificatesRequestRequestTypeDef",
     "ListCertificatesByCARequestRequestTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListCustomMetricsRequestRequestTypeDef",
-    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListDetectMitigationActionsTasksRequestRequestTypeDef",
     "ListDimensionsRequestRequestTypeDef",
     "ListDomainConfigurationsRequestRequestTypeDef",
     "ListFleetMetricsRequestRequestTypeDef",
     "ListIndicesRequestRequestTypeDef",
     "ListJobExecutionsForJobRequestRequestTypeDef",
     "ListJobExecutionsForThingRequestRequestTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListManagedJobTemplatesRequestRequestTypeDef",
     "ManagedJobTemplateSummaryTypeDef",
-    "ListMetricValuesRequestRequestTypeDef",
     "ListMitigationActionsRequestRequestTypeDef",
     "MitigationActionIdentifierTypeDef",
     "ListOTAUpdatesRequestRequestTypeDef",
     "OTAUpdateSummaryTypeDef",
     "ListOutgoingCertificatesRequestRequestTypeDef",
     "OutgoingCertificateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
@@ -381,23 +377,21 @@
     "ListThingsInThingGroupRequestRequestTypeDef",
     "ListThingsRequestRequestTypeDef",
     "ThingAttributeTypeDef",
     "ListTopicRuleDestinationsRequestRequestTypeDef",
     "ListTopicRulesRequestRequestTypeDef",
     "TopicRuleListItemTypeDef",
     "ListV2LoggingLevelsRequestRequestTypeDef",
-    "ListViolationEventsRequestRequestTypeDef",
     "LocationTimestampTypeDef",
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
-    "MqttContextTypeDef",
     "UserPropertyTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
     "RegisterThingRequestRequestTypeDef",
     "RejectCertificateTransferRequestRequestTypeDef",
@@ -405,15 +399,14 @@
     "RemoveThingFromThingGroupRequestRequestTypeDef",
     "SearchIndexRequestRequestTypeDef",
     "ThingGroupDocumentTypeDef",
     "SetDefaultAuthorizerRequestRequestTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetV2LoggingOptionsRequestRequestTypeDef",
     "SigningProfileParameterTypeDef",
-    "ViolationEventOccurrenceRangeTypeDef",
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     "StartThingRegistrationTaskRequestRequestTypeDef",
     "StopThingRegistrationTaskRequestRequestTypeDef",
     "TlsContextTypeDef",
     "ThingConnectivityTypeDef",
     "TimestreamDimensionTypeDef",
     "TimestreamTimestampTypeDef",
@@ -432,14 +425,15 @@
     "UpdateScheduledAuditRequestRequestTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
     "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
+    "AggregationTypeUnionTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
     "AssetPropertyValueTypeDef",
     "AssociateTargetsWithJobResponseTypeDef",
     "CancelJobResponseTypeDef",
@@ -521,46 +515,56 @@
     "UpdateDynamicThingGroupResponseTypeDef",
     "UpdateMitigationActionResponseTypeDef",
     "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditResponseTypeDef",
     "UpdateStreamResponseTypeDef",
     "UpdateThingGroupResponseTypeDef",
     "ThingGroupPropertiesOutputTypeDef",
+    "AttributePayloadUnionTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
+    "AuditMitigationActionsTaskTargetUnionTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     "DescribeAccountAuditConfigurationResponseTypeDef",
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
-    "TestAuthorizationRequestRequestTypeDef",
+    "AuthInfoUnionTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
     "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
+    "CodeSigningSignatureTypeDef",
+    "MqttContextTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
     "CertificateDescriptionTypeDef",
     "ListCertificatesByCAResponseTypeDef",
     "ListCertificatesResponseTypeDef",
     "CustomCodeSigningOutputTypeDef",
-    "CustomCodeSigningTypeDef",
     "DescribeEventConfigurationsResponseTypeDef",
     "UpdateEventConfigurationsRequestRequestTypeDef",
+    "ListAuditMitigationActionsTasksRequestRequestTypeDef",
+    "ListAuditTasksRequestRequestTypeDef",
+    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
+    "ListDetectMitigationActionsTasksRequestRequestTypeDef",
+    "ListMetricValuesRequestRequestTypeDef",
+    "ListViolationEventsRequestRequestTypeDef",
+    "ViolationEventOccurrenceRangeTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
@@ -581,16 +585,18 @@
     "RegisterCACertificateRequestRequestTypeDef",
     "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
+    "ThingTypePropertiesUnionTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
+    "DetectMitigationActionsTaskTargetUnionTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
     "ExponentialRolloutRateTypeDef",
     "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
     "StreamFileTypeDef",
@@ -692,56 +698,66 @@
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
     "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
     "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
     "ResourceIdentifierTypeDef",
-    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
-    "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
     "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
+    "AbortConfigUnionTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
     "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
+    "ThingGroupPropertiesUnionTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
+    "TestAuthorizationRequestRequestTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
     "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
+    "CustomCodeSigningTypeDef",
+    "TestInvokeAuthorizerRequestRequestTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
+    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
+    "ViolationEventOccurrenceRangeUnionTypeDef",
+    "SchedulingConfigUnionTypeDef",
     "ListThingTypesResponseTypeDef",
     "StartSigningJobParameterTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
+    "ThingGroupIndexingConfigurationUnionTypeDef",
     "CreateStreamRequestRequestTypeDef",
     "StreamInfoTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
     "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
+    "ThingIndexingConfigurationUnionTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "ListJobExecutionsForJobResponseTypeDef",
     "ListJobExecutionsForThingResponseTypeDef",
+    "JobExecutionsRetryConfigUnionTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
     "CreateMitigationActionRequestRequestTypeDef",
+    "MitigationActionParamsUnionTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
     "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
@@ -761,17 +777,15 @@
     "AuthResultTypeDef",
     "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "ActiveViolationTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
     "UpdateSecurityProfileResponseTypeDef",
     "ViolationEventTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    "BehaviorUnionTypeDef",
     "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
     "CreateJobRequestRequestTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "JobTypeDef",
     "UpdateJobRequestRequestTypeDef",
@@ -782,29 +796,33 @@
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     "TestAuthorizationResponseTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListActiveViolationsResponseTypeDef",
     "ListViolationEventsResponseTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "OTAUpdateFileOutputTypeDef",
     "OTAUpdateFileTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     "ListDetectMitigationActionsTasksResponseTypeDef",
     "DescribeAuditFindingResponseTypeDef",
     "ListAuditFindingsResponseTypeDef",
     "TopicRuleTypeDef",
     "TopicRulePayloadTypeDef",
     "OTAUpdateInfoTypeDef",
-    "CreateOTAUpdateRequestRequestTypeDef",
+    "OTAUpdateFileUnionTypeDef",
     "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
     "GetOTAUpdateResponseTypeDef",
+    "CreateOTAUpdateRequestRequestTypeDef",
 )
 
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
@@ -1687,14 +1705,15 @@
     "BillingGroupPropertiesTypeDef",
     {
         "billingGroupDescription": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "keyValue": str,
         "count": int,
     },
     total=False,
@@ -1841,22 +1860,14 @@
     "CodeSigningSignatureOutputTypeDef",
     {
         "inlineDocument": bytes,
     },
     total=False,
 )
 
-CodeSigningSignatureTypeDef = TypedDict(
-    "CodeSigningSignatureTypeDef",
-    {
-        "inlineDocument": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1864,14 +1875,15 @@
 ConfirmTopicRuleDestinationRequestRequestTypeDef = TypedDict(
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     {
         "confirmationToken": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -3451,66 +3463,14 @@
 class ListAuditMitigationActionsExecutionsRequestRequestTypeDef(
     _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef,
     _OptionalListAuditMitigationActionsExecutionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "auditTaskId": str,
-        "findingId": str,
-        "taskStatus": AuditMitigationActionsTaskStatusType,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListAuditMitigationActionsTasksRequestRequestTypeDef(
-    _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
-    _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListAuditTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListAuditTasksRequestRequestTypeDef",
-    {
-        "taskType": AuditTaskTypeType,
-        "taskStatus": AuditTaskStatusType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListAuditTasksRequestRequestTypeDef(
-    _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
-):
-    pass
-
-
 ListAuthorizersRequestRequestTypeDef = TypedDict(
     "ListAuthorizersRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "status": AuthorizerStatusType,
@@ -3578,52 +3538,14 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
-    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "violationId": str,
-        "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListDetectMitigationActionsTasksRequestRequestTypeDef(
-    _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
-    _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
-):
-    pass
-
-
 ListDimensionsRequestRequestTypeDef = TypedDict(
     "ListDimensionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -3748,41 +3670,14 @@
         "description": str,
         "environments": List[str],
         "templateVersion": str,
     },
     total=False,
 )
 
-_RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
-    "_RequiredListMetricValuesRequestRequestTypeDef",
-    {
-        "thingName": str,
-        "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListMetricValuesRequestRequestTypeDef = TypedDict(
-    "_OptionalListMetricValuesRequestRequestTypeDef",
-    {
-        "dimensionName": str,
-        "dimensionValueOperator": DimensionValueOperatorType,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListMetricValuesRequestRequestTypeDef(
-    _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
-):
-    pass
-
-
 ListMitigationActionsRequestRequestTypeDef = TypedDict(
     "ListMitigationActionsRequestRequestTypeDef",
     {
         "actionType": MitigationActionTypeType,
         "maxResults": int,
         "nextToken": str,
     },
@@ -4457,43 +4352,14 @@
         "targetType": LogTargetTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListViolationEventsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListViolationEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListViolationEventsRequestRequestTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListViolationEventsRequestRequestTypeDef(
-    _RequiredListViolationEventsRequestRequestTypeDef,
-    _OptionalListViolationEventsRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredLocationTimestampTypeDef = TypedDict(
     "_RequiredLocationTimestampTypeDef",
     {
         "value": str,
     },
 )
 _OptionalLocationTimestampTypeDef = TypedDict(
@@ -4575,24 +4441,14 @@
 UpdateDeviceCertificateParamsTypeDef = TypedDict(
     "UpdateDeviceCertificateParamsTypeDef",
     {
         "action": Literal["DEACTIVATE"],
     },
 )
 
-MqttContextTypeDef = TypedDict(
-    "MqttContextTypeDef",
-    {
-        "username": str,
-        "password": Union[str, bytes, IO[Any], StreamingBody],
-        "clientId": str,
-    },
-    total=False,
-)
-
 UserPropertyTypeDef = TypedDict(
     "UserPropertyTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -4807,22 +4663,14 @@
         "certificateArn": str,
         "platform": str,
         "certificatePathOnDevice": str,
     },
     total=False,
 )
 
-ViolationEventOccurrenceRangeTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-
 StartOnDemandAuditTaskRequestRequestTypeDef = TypedDict(
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     {
         "targetCheckNames": Sequence[str],
     },
 )
 
@@ -5145,14 +4993,15 @@
     {
         "timestamp": datetime,
         "value": MetricValueOutputTypeDef,
     },
     total=False,
 )
 
+AggregationTypeUnionTypeDef = Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef]
 _RequiredUpdateFleetMetricRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "indexName": str,
     },
 )
@@ -6069,14 +5918,15 @@
     {
         "thingGroupDescription": str,
         "attributePayload": AttributePayloadOutputTypeDef,
     },
     total=False,
 )
 
+AttributePayloadUnionTypeDef = Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef]
 _RequiredCreateThingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalCreateThingRequestRequestTypeDef = TypedDict(
@@ -6143,14 +5993,17 @@
     {
         "tasks": List[AuditMitigationActionsTaskMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AuditMitigationActionsTaskTargetUnionTypeDef = Union[
+    AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
+]
 StartAuditMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
         "target": AuditMitigationActionsTaskTargetTypeDef,
         "auditCheckToActionsMapping": Mapping[str, Sequence[str]],
         "clientRequestToken": str,
@@ -6186,39 +6039,15 @@
     {
         "tasks": List[AuditTaskMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_RequiredTestAuthorizationRequestRequestTypeDef",
-    {
-        "authInfos": Sequence[Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]],
-    },
-)
-_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_OptionalTestAuthorizationRequestRequestTypeDef",
-    {
-        "principal": str,
-        "cognitoIdentityPoolId": str,
-        "clientId": str,
-        "policyNamesToAdd": Sequence[str],
-        "policyNamesToSkip": Sequence[str],
-    },
-    total=False,
-)
-
-
-class TestAuthorizationRequestRequestTypeDef(
-    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
-):
-    pass
-
-
+AuthInfoUnionTypeDef = Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]
 DescribeAuthorizerResponseTypeDef = TypedDict(
     "DescribeAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6344,14 +6173,32 @@
 class UpdateBillingGroupRequestRequestTypeDef(
     _RequiredUpdateBillingGroupRequestRequestTypeDef,
     _OptionalUpdateBillingGroupRequestRequestTypeDef,
 ):
     pass
 
 
+CodeSigningSignatureTypeDef = TypedDict(
+    "CodeSigningSignatureTypeDef",
+    {
+        "inlineDocument": BlobTypeDef,
+    },
+    total=False,
+)
+
+MqttContextTypeDef = TypedDict(
+    "MqttContextTypeDef",
+    {
+        "username": str,
+        "password": BlobTypeDef,
+        "clientId": str,
+    },
+    total=False,
+)
+
 GetBucketsAggregationResponseTypeDef = TypedDict(
     "GetBucketsAggregationResponseTypeDef",
     {
         "totalCount": int,
         "buckets": List[BucketTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6439,25 +6286,14 @@
         "certificateChain": CodeSigningCertificateChainTypeDef,
         "hashAlgorithm": str,
         "signatureAlgorithm": str,
     },
     total=False,
 )
 
-CustomCodeSigningTypeDef = TypedDict(
-    "CustomCodeSigningTypeDef",
-    {
-        "signature": CodeSigningSignatureTypeDef,
-        "certificateChain": CodeSigningCertificateChainTypeDef,
-        "hashAlgorithm": str,
-        "signatureAlgorithm": str,
-    },
-    total=False,
-)
-
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
         "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6468,14 +6304,168 @@
     "UpdateEventConfigurationsRequestRequestTypeDef",
     {
         "eventConfigurations": Mapping[EventTypeType, ConfigurationTypeDef],
     },
     total=False,
 )
 
+_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "auditTaskId": str,
+        "findingId": str,
+        "taskStatus": AuditMitigationActionsTaskStatusType,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListAuditMitigationActionsTasksRequestRequestTypeDef(
+    _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
+    _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListAuditTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListAuditTasksRequestRequestTypeDef",
+    {
+        "taskType": AuditTaskTypeType,
+        "taskStatus": AuditTaskStatusType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListAuditTasksRequestRequestTypeDef(
+    _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
+):
+    pass
+
+
+ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
+    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "violationId": str,
+        "thingName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListDetectMitigationActionsTasksRequestRequestTypeDef(
+    _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
+    _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
+    "_RequiredListMetricValuesRequestRequestTypeDef",
+    {
+        "thingName": str,
+        "metricName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListMetricValuesRequestRequestTypeDef = TypedDict(
+    "_OptionalListMetricValuesRequestRequestTypeDef",
+    {
+        "dimensionName": str,
+        "dimensionValueOperator": DimensionValueOperatorType,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListMetricValuesRequestRequestTypeDef(
+    _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListViolationEventsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListViolationEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListViolationEventsRequestRequestTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListViolationEventsRequestRequestTypeDef(
+    _RequiredListViolationEventsRequestRequestTypeDef,
+    _OptionalListViolationEventsRequestRequestTypeDef,
+):
+    pass
+
+
+ViolationEventOccurrenceRangeTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
         "authorizerFunctionArn": str,
     },
 )
@@ -7003,14 +6993,17 @@
         "thingTypeArn": str,
         "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
+ThingTypePropertiesUnionTypeDef = Union[
+    ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
+]
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
@@ -7020,14 +7013,17 @@
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DetectMitigationActionsTaskTargetUnionTypeDef = Union[
+    DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
+]
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7200,16 +7196,16 @@
 ):
     pass
 
 
 _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
     "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
     "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
     {
         "auditTaskId": str,
         "findingId": str,
@@ -7226,16 +7222,16 @@
 ):
     pass
 
 
 _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
     "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
     "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
     {
         "taskType": AuditTaskTypeType,
         "taskStatus": AuditTaskStatusType,
@@ -7323,26 +7319,26 @@
 
 ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
     "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
     {
         "taskId": str,
         "violationId": str,
         "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
     "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
     "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -7469,16 +7465,16 @@
 )
 
 _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
     "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
     {
         "thingName": str,
         "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
     "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
     {
         "dimensionName": str,
         "dimensionValueOperator": DimensionValueOperatorType,
@@ -7994,16 +7990,16 @@
     },
     total=False,
 )
 
 _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
     "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
     "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
     {
         "thingName": str,
         "securityProfileName": str,
@@ -8477,67 +8473,14 @@
         "roleAliasArn": str,
         "issuerCertificateIdentifier": IssuerCertificateIdentifierTypeDef,
         "deviceCertificateArn": str,
     },
     total=False,
 )
 
-_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "actions": Sequence[str],
-        "clientRequestToken": str,
-    },
-)
-_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
-        "includeOnlyActiveViolations": bool,
-        "includeSuppressedAlerts": bool,
-    },
-    total=False,
-)
-
-
-class StartDetectMitigationActionsTaskRequestRequestTypeDef(
-    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
-    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
-    "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
-    {
-        "authorizerName": str,
-    },
-)
-_OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
-    "_OptionalTestInvokeAuthorizerRequestRequestTypeDef",
-    {
-        "token": str,
-        "tokenSignature": str,
-        "httpContext": HttpContextTypeDef,
-        "mqttContext": MqttContextTypeDef,
-        "tlsContext": TlsContextTypeDef,
-    },
-    total=False,
-)
-
-
-class TestInvokeAuthorizerRequestRequestTypeDef(
-    _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
-    _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
-):
-    pass
-
-
 ThingDocumentTypeDef = TypedDict(
     "ThingDocumentTypeDef",
     {
         "thingName": str,
         "thingId": str,
         "thingTypeName": str,
         "thingGroupNames": List[str],
@@ -8637,14 +8580,15 @@
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AbortConfigUnionTypeDef = Union[AbortConfigTypeDef, AbortConfigOutputTypeDef]
 ListMetricValuesResponseTypeDef = TypedDict(
     "ListMetricValuesResponseTypeDef",
     {
         "metricDatumList": List[MetricDatumTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8753,14 +8697,17 @@
 
 class CreateThingGroupRequestRequestTypeDef(
     _RequiredCreateThingGroupRequestRequestTypeDef, _OptionalCreateThingGroupRequestRequestTypeDef
 ):
     pass
 
 
+ThingGroupPropertiesUnionTypeDef = Union[
+    ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
+]
 _RequiredUpdateDynamicThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDynamicThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
         "thingGroupProperties": ThingGroupPropertiesTypeDef,
     },
 )
@@ -8801,14 +8748,39 @@
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_RequiredTestAuthorizationRequestRequestTypeDef",
+    {
+        "authInfos": Sequence[AuthInfoUnionTypeDef],
+    },
+)
+_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_OptionalTestAuthorizationRequestRequestTypeDef",
+    {
+        "principal": str,
+        "cognitoIdentityPoolId": str,
+        "clientId": str,
+        "policyNamesToAdd": Sequence[str],
+        "policyNamesToSkip": Sequence[str],
+    },
+    total=False,
+)
+
+
+class TestAuthorizationRequestRequestTypeDef(
+    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
+):
+    pass
+
+
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
@@ -8854,14 +8826,51 @@
 )
 
 
 class BehaviorTypeDef(_RequiredBehaviorTypeDef, _OptionalBehaviorTypeDef):
     pass
 
 
+CustomCodeSigningTypeDef = TypedDict(
+    "CustomCodeSigningTypeDef",
+    {
+        "signature": CodeSigningSignatureTypeDef,
+        "certificateChain": CodeSigningCertificateChainTypeDef,
+        "hashAlgorithm": str,
+        "signatureAlgorithm": str,
+    },
+    total=False,
+)
+
+_RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
+    "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
+    {
+        "authorizerName": str,
+    },
+)
+_OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
+    "_OptionalTestInvokeAuthorizerRequestRequestTypeDef",
+    {
+        "token": str,
+        "tokenSignature": str,
+        "httpContext": HttpContextTypeDef,
+        "mqttContext": MqttContextTypeDef,
+        "tlsContext": TlsContextTypeDef,
+    },
+    total=False,
+)
+
+
+class TestInvokeAuthorizerRequestRequestTypeDef(
+    _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
+    _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredGetBucketsAggregationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketsAggregationRequestRequestTypeDef",
     {
         "queryString": str,
         "aggregationField": str,
         "bucketsAggregationType": BucketsAggregationTypeTypeDef,
     },
@@ -8896,14 +8905,45 @@
     "DescribeCertificateResponseTypeDef",
     {
         "certificateDescription": CertificateDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "actions": Sequence[str],
+        "clientRequestToken": str,
+    },
+)
+_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "includeOnlyActiveViolations": bool,
+        "includeSuppressedAlerts": bool,
+    },
+    total=False,
+)
+
+
+class StartDetectMitigationActionsTaskRequestRequestTypeDef(
+    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
+    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
+):
+    pass
+
+
+ViolationEventOccurrenceRangeUnionTypeDef = Union[
+    ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
+]
+SchedulingConfigUnionTypeDef = Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef]
 ListThingTypesResponseTypeDef = TypedDict(
     "ListThingTypesResponseTypeDef",
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8924,14 +8964,17 @@
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+ThingGroupIndexingConfigurationUnionTypeDef = Union[
+    ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
+]
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -9054,14 +9097,17 @@
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ThingIndexingConfigurationUnionTypeDef = Union[
+    ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
+]
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
     },
     total=False,
@@ -9089,14 +9135,17 @@
     {
         "executionSummaries": List[JobExecutionSummaryForThingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+JobExecutionsRetryConfigUnionTypeDef = Union[
+    JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+]
 ListSecurityProfilesForTargetResponseTypeDef = TypedDict(
     "ListSecurityProfilesForTargetResponseTypeDef",
     {
         "securityProfileTargetMappings": List[SecurityProfileTargetMappingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -9157,14 +9206,17 @@
 class CreateMitigationActionRequestRequestTypeDef(
     _RequiredCreateMitigationActionRequestRequestTypeDef,
     _OptionalCreateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
 
+MitigationActionParamsUnionTypeDef = Union[
+    MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
+]
 _RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMitigationActionRequestRequestTypeDef",
     {
         "actionName": str,
     },
 )
 _OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
@@ -9257,15 +9309,15 @@
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "clientRequestToken": str,
     },
 )
 _OptionalCreateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAuditSuppressionRequestRequestTypeDef",
     {
-        "expirationDate": Union[datetime, str],
+        "expirationDate": TimestampTypeDef,
         "suppressIndefinitely": bool,
         "description": str,
     },
     total=False,
 )
 
 
@@ -9306,32 +9358,32 @@
 
 ListAuditFindingsRequestListAuditFindingsPaginateTypeDef = TypedDict(
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "listSuppressedFindings": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditFindingsRequestRequestTypeDef = TypedDict(
     "ListAuditFindingsRequestRequestTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "maxResults": int,
         "nextToken": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "listSuppressedFindings": bool,
     },
     total=False,
 )
 
 ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef = TypedDict(
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
@@ -9382,15 +9434,15 @@
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 _OptionalUpdateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAuditSuppressionRequestRequestTypeDef",
     {
-        "expirationDate": Union[datetime, str],
+        "expirationDate": TimestampTypeDef,
         "suppressIndefinitely": bool,
         "description": str,
     },
     total=False,
 )
 
 
@@ -9535,78 +9587,15 @@
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "violationEventTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateSecurityProfileRequestRequestTypeDef(
-    _RequiredCreateSecurityProfileRequestRequestTypeDef,
-    _OptionalCreateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "deleteBehaviors": bool,
-        "deleteAlertTargets": bool,
-        "deleteAdditionalMetricsToRetain": bool,
-        "expectedVersion": int,
-    },
-    total=False,
-)
-
-
-class UpdateSecurityProfileRequestRequestTypeDef(
-    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
-    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-
-ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
-    {
-        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
-    },
-)
-
+BehaviorUnionTypeDef = Union[BehaviorTypeDef, BehaviorOutputTypeDef]
 CodeSigningOutputTypeDef = TypedDict(
     "CodeSigningOutputTypeDef",
     {
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningOutputTypeDef,
     },
@@ -9927,14 +9916,78 @@
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSecurityProfileRequestRequestTypeDef(
+    _RequiredCreateSecurityProfileRequestRequestTypeDef,
+    _OptionalCreateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "deleteBehaviors": bool,
+        "deleteAlertTargets": bool,
+        "deleteAdditionalMetricsToRetain": bool,
+        "expectedVersion": int,
+    },
+    total=False,
+)
+
+
+class UpdateSecurityProfileRequestRequestTypeDef(
+    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
+    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+
+ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    {
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+    },
+)
+
 OTAUpdateFileOutputTypeDef = TypedDict(
     "OTAUpdateFileOutputTypeDef",
     {
         "fileName": str,
         "fileType": int,
         "fileVersion": str,
         "fileLocation": FileLocationTypeDef,
@@ -10057,46 +10110,15 @@
         "awsIotJobArn": str,
         "errorInfo": ErrorInfoTypeDef,
         "additionalParameters": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
-    {
-        "otaUpdateId": str,
-        "targets": Sequence[str],
-        "files": Sequence[Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]],
-        "roleArn": str,
-    },
-)
-_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
-    {
-        "description": str,
-        "protocols": Sequence[ProtocolType],
-        "targetSelection": TargetSelectionType,
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
-        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
-        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
-        "additionalParameters": Mapping[str, str],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateOTAUpdateRequestRequestTypeDef(
-    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
-):
-    pass
-
-
+OTAUpdateFileUnionTypeDef = Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]
 GetTopicRuleResponseTypeDef = TypedDict(
     "GetTopicRuleResponseTypeDef",
     {
         "ruleArn": str,
         "rule": TopicRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -10135,7 +10157,38 @@
 GetOTAUpdateResponseTypeDef = TypedDict(
     "GetOTAUpdateResponseTypeDef",
     {
         "otaUpdateInfo": OTAUpdateInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
+    {
+        "otaUpdateId": str,
+        "targets": Sequence[str],
+        "files": Sequence[OTAUpdateFileUnionTypeDef],
+        "roleArn": str,
+    },
+)
+_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
+    {
+        "description": str,
+        "protocols": Sequence[ProtocolType],
+        "targetSelection": TargetSelectionType,
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
+        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
+        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
+        "additionalParameters": Mapping[str, str],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateOTAUpdateRequestRequestTypeDef(
+    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/type_defs.pyi` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iot.type_defs import AbortCriteriaTypeDef
 
-    data: AbortCriteriaTypeDef = {...}
+    data: AbortCriteriaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -152,31 +152,32 @@
     "MachineLearningDetectionConfigTypeDef",
     "StatisticalThresholdTypeDef",
     "MetricValueTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
     "BillingGroupPropertiesTypeDef",
+    "BlobTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
     "CertificateValidityTypeDef",
     "CACertificateTypeDef",
     "CancelAuditMitigationActionsTaskRequestRequestTypeDef",
     "CancelAuditTaskRequestRequestTypeDef",
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
     "CodeSigningCertificateChainTypeDef",
     "CodeSigningSignatureOutputTypeDef",
-    "CodeSigningSignatureTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "TagTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "PresignedUrlConfigTypeDef",
     "TimeoutConfigTypeDef",
     "MaintenanceWindowTypeDef",
     "CreateKeysAndCertificateRequestRequestTypeDef",
@@ -312,35 +313,30 @@
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
     "ScheduledJobRolloutTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
     "ListAttachedPoliciesRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListAuditMitigationActionsTasksRequestRequestTypeDef",
-    "ListAuditTasksRequestRequestTypeDef",
     "ListAuthorizersRequestRequestTypeDef",
     "ListBillingGroupsRequestRequestTypeDef",
     "ListCACertificatesRequestRequestTypeDef",
     "ListCertificatesByCARequestRequestTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListCustomMetricsRequestRequestTypeDef",
-    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListDetectMitigationActionsTasksRequestRequestTypeDef",
     "ListDimensionsRequestRequestTypeDef",
     "ListDomainConfigurationsRequestRequestTypeDef",
     "ListFleetMetricsRequestRequestTypeDef",
     "ListIndicesRequestRequestTypeDef",
     "ListJobExecutionsForJobRequestRequestTypeDef",
     "ListJobExecutionsForThingRequestRequestTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListManagedJobTemplatesRequestRequestTypeDef",
     "ManagedJobTemplateSummaryTypeDef",
-    "ListMetricValuesRequestRequestTypeDef",
     "ListMitigationActionsRequestRequestTypeDef",
     "MitigationActionIdentifierTypeDef",
     "ListOTAUpdatesRequestRequestTypeDef",
     "OTAUpdateSummaryTypeDef",
     "ListOutgoingCertificatesRequestRequestTypeDef",
     "OutgoingCertificateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
@@ -380,23 +376,21 @@
     "ListThingsInThingGroupRequestRequestTypeDef",
     "ListThingsRequestRequestTypeDef",
     "ThingAttributeTypeDef",
     "ListTopicRuleDestinationsRequestRequestTypeDef",
     "ListTopicRulesRequestRequestTypeDef",
     "TopicRuleListItemTypeDef",
     "ListV2LoggingLevelsRequestRequestTypeDef",
-    "ListViolationEventsRequestRequestTypeDef",
     "LocationTimestampTypeDef",
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
-    "MqttContextTypeDef",
     "UserPropertyTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
     "RegisterThingRequestRequestTypeDef",
     "RejectCertificateTransferRequestRequestTypeDef",
@@ -404,15 +398,14 @@
     "RemoveThingFromThingGroupRequestRequestTypeDef",
     "SearchIndexRequestRequestTypeDef",
     "ThingGroupDocumentTypeDef",
     "SetDefaultAuthorizerRequestRequestTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetV2LoggingOptionsRequestRequestTypeDef",
     "SigningProfileParameterTypeDef",
-    "ViolationEventOccurrenceRangeTypeDef",
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     "StartThingRegistrationTaskRequestRequestTypeDef",
     "StopThingRegistrationTaskRequestRequestTypeDef",
     "TlsContextTypeDef",
     "ThingConnectivityTypeDef",
     "TimestreamDimensionTypeDef",
     "TimestreamTimestampTypeDef",
@@ -431,14 +424,15 @@
     "UpdateScheduledAuditRequestRequestTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
     "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
+    "AggregationTypeUnionTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
     "AssetPropertyValueTypeDef",
     "AssociateTargetsWithJobResponseTypeDef",
     "CancelJobResponseTypeDef",
@@ -520,46 +514,56 @@
     "UpdateDynamicThingGroupResponseTypeDef",
     "UpdateMitigationActionResponseTypeDef",
     "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditResponseTypeDef",
     "UpdateStreamResponseTypeDef",
     "UpdateThingGroupResponseTypeDef",
     "ThingGroupPropertiesOutputTypeDef",
+    "AttributePayloadUnionTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
+    "AuditMitigationActionsTaskTargetUnionTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     "DescribeAccountAuditConfigurationResponseTypeDef",
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
-    "TestAuthorizationRequestRequestTypeDef",
+    "AuthInfoUnionTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
     "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
+    "CodeSigningSignatureTypeDef",
+    "MqttContextTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
     "CertificateDescriptionTypeDef",
     "ListCertificatesByCAResponseTypeDef",
     "ListCertificatesResponseTypeDef",
     "CustomCodeSigningOutputTypeDef",
-    "CustomCodeSigningTypeDef",
     "DescribeEventConfigurationsResponseTypeDef",
     "UpdateEventConfigurationsRequestRequestTypeDef",
+    "ListAuditMitigationActionsTasksRequestRequestTypeDef",
+    "ListAuditTasksRequestRequestTypeDef",
+    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
+    "ListDetectMitigationActionsTasksRequestRequestTypeDef",
+    "ListMetricValuesRequestRequestTypeDef",
+    "ListViolationEventsRequestRequestTypeDef",
+    "ViolationEventOccurrenceRangeTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
@@ -580,16 +584,18 @@
     "RegisterCACertificateRequestRequestTypeDef",
     "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
+    "ThingTypePropertiesUnionTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
+    "DetectMitigationActionsTaskTargetUnionTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
     "ExponentialRolloutRateTypeDef",
     "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
     "StreamFileTypeDef",
@@ -691,56 +697,66 @@
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
     "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
     "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
     "ResourceIdentifierTypeDef",
-    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
-    "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
     "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
+    "AbortConfigUnionTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
     "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
+    "ThingGroupPropertiesUnionTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
+    "TestAuthorizationRequestRequestTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
     "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
+    "CustomCodeSigningTypeDef",
+    "TestInvokeAuthorizerRequestRequestTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
+    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
+    "ViolationEventOccurrenceRangeUnionTypeDef",
+    "SchedulingConfigUnionTypeDef",
     "ListThingTypesResponseTypeDef",
     "StartSigningJobParameterTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
+    "ThingGroupIndexingConfigurationUnionTypeDef",
     "CreateStreamRequestRequestTypeDef",
     "StreamInfoTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
     "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
+    "ThingIndexingConfigurationUnionTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "ListJobExecutionsForJobResponseTypeDef",
     "ListJobExecutionsForThingResponseTypeDef",
+    "JobExecutionsRetryConfigUnionTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
     "CreateMitigationActionRequestRequestTypeDef",
+    "MitigationActionParamsUnionTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
     "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
@@ -760,17 +776,15 @@
     "AuthResultTypeDef",
     "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "ActiveViolationTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
     "UpdateSecurityProfileResponseTypeDef",
     "ViolationEventTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    "BehaviorUnionTypeDef",
     "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
     "CreateJobRequestRequestTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "JobTypeDef",
     "UpdateJobRequestRequestTypeDef",
@@ -781,29 +795,33 @@
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     "TestAuthorizationResponseTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListActiveViolationsResponseTypeDef",
     "ListViolationEventsResponseTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "OTAUpdateFileOutputTypeDef",
     "OTAUpdateFileTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     "ListDetectMitigationActionsTasksResponseTypeDef",
     "DescribeAuditFindingResponseTypeDef",
     "ListAuditFindingsResponseTypeDef",
     "TopicRuleTypeDef",
     "TopicRulePayloadTypeDef",
     "OTAUpdateInfoTypeDef",
-    "CreateOTAUpdateRequestRequestTypeDef",
+    "OTAUpdateFileUnionTypeDef",
     "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
     "GetOTAUpdateResponseTypeDef",
+    "CreateOTAUpdateRequestRequestTypeDef",
 )
 
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
@@ -1642,14 +1660,15 @@
     "BillingGroupPropertiesTypeDef",
     {
         "billingGroupDescription": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "keyValue": str,
         "count": int,
     },
     total=False,
@@ -1792,22 +1811,14 @@
     "CodeSigningSignatureOutputTypeDef",
     {
         "inlineDocument": bytes,
     },
     total=False,
 )
 
-CodeSigningSignatureTypeDef = TypedDict(
-    "CodeSigningSignatureTypeDef",
-    {
-        "inlineDocument": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1815,14 +1826,15 @@
 ConfirmTopicRuleDestinationRequestRequestTypeDef = TypedDict(
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     {
         "confirmationToken": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -3348,62 +3360,14 @@
 
 class ListAuditMitigationActionsExecutionsRequestRequestTypeDef(
     _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef,
     _OptionalListAuditMitigationActionsExecutionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "auditTaskId": str,
-        "findingId": str,
-        "taskStatus": AuditMitigationActionsTaskStatusType,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListAuditMitigationActionsTasksRequestRequestTypeDef(
-    _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
-    _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListAuditTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListAuditTasksRequestRequestTypeDef",
-    {
-        "taskType": AuditTaskTypeType,
-        "taskStatus": AuditTaskStatusType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListAuditTasksRequestRequestTypeDef(
-    _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
-):
-    pass
-
 ListAuthorizersRequestRequestTypeDef = TypedDict(
     "ListAuthorizersRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "status": AuthorizerStatusType,
@@ -3469,50 +3433,14 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
-    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "violationId": str,
-        "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListDetectMitigationActionsTasksRequestRequestTypeDef(
-    _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
-    _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
-):
-    pass
-
 ListDimensionsRequestRequestTypeDef = TypedDict(
     "ListDimensionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -3633,39 +3561,14 @@
         "description": str,
         "environments": List[str],
         "templateVersion": str,
     },
     total=False,
 )
 
-_RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
-    "_RequiredListMetricValuesRequestRequestTypeDef",
-    {
-        "thingName": str,
-        "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListMetricValuesRequestRequestTypeDef = TypedDict(
-    "_OptionalListMetricValuesRequestRequestTypeDef",
-    {
-        "dimensionName": str,
-        "dimensionValueOperator": DimensionValueOperatorType,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListMetricValuesRequestRequestTypeDef(
-    _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
-):
-    pass
-
 ListMitigationActionsRequestRequestTypeDef = TypedDict(
     "ListMitigationActionsRequestRequestTypeDef",
     {
         "actionType": MitigationActionTypeType,
         "maxResults": int,
         "nextToken": str,
     },
@@ -4310,41 +4213,14 @@
         "targetType": LogTargetTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListViolationEventsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListViolationEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListViolationEventsRequestRequestTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListViolationEventsRequestRequestTypeDef(
-    _RequiredListViolationEventsRequestRequestTypeDef,
-    _OptionalListViolationEventsRequestRequestTypeDef,
-):
-    pass
-
 _RequiredLocationTimestampTypeDef = TypedDict(
     "_RequiredLocationTimestampTypeDef",
     {
         "value": str,
     },
 )
 _OptionalLocationTimestampTypeDef = TypedDict(
@@ -4420,24 +4296,14 @@
 UpdateDeviceCertificateParamsTypeDef = TypedDict(
     "UpdateDeviceCertificateParamsTypeDef",
     {
         "action": Literal["DEACTIVATE"],
     },
 )
 
-MqttContextTypeDef = TypedDict(
-    "MqttContextTypeDef",
-    {
-        "username": str,
-        "password": Union[str, bytes, IO[Any], StreamingBody],
-        "clientId": str,
-    },
-    total=False,
-)
-
 UserPropertyTypeDef = TypedDict(
     "UserPropertyTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -4640,22 +4506,14 @@
         "certificateArn": str,
         "platform": str,
         "certificatePathOnDevice": str,
     },
     total=False,
 )
 
-ViolationEventOccurrenceRangeTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-
 StartOnDemandAuditTaskRequestRequestTypeDef = TypedDict(
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     {
         "targetCheckNames": Sequence[str],
     },
 )
 
@@ -4964,14 +4822,15 @@
     {
         "timestamp": datetime,
         "value": MetricValueOutputTypeDef,
     },
     total=False,
 )
 
+AggregationTypeUnionTypeDef = Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef]
 _RequiredUpdateFleetMetricRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "indexName": str,
     },
 )
@@ -5884,14 +5743,15 @@
     {
         "thingGroupDescription": str,
         "attributePayload": AttributePayloadOutputTypeDef,
     },
     total=False,
 )
 
+AttributePayloadUnionTypeDef = Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef]
 _RequiredCreateThingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalCreateThingRequestRequestTypeDef = TypedDict(
@@ -5954,14 +5814,17 @@
     {
         "tasks": List[AuditMitigationActionsTaskMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AuditMitigationActionsTaskTargetUnionTypeDef = Union[
+    AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
+]
 StartAuditMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
         "target": AuditMitigationActionsTaskTargetTypeDef,
         "auditCheckToActionsMapping": Mapping[str, Sequence[str]],
         "clientRequestToken": str,
@@ -5997,37 +5860,15 @@
     {
         "tasks": List[AuditTaskMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_RequiredTestAuthorizationRequestRequestTypeDef",
-    {
-        "authInfos": Sequence[Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]],
-    },
-)
-_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_OptionalTestAuthorizationRequestRequestTypeDef",
-    {
-        "principal": str,
-        "cognitoIdentityPoolId": str,
-        "clientId": str,
-        "policyNamesToAdd": Sequence[str],
-        "policyNamesToSkip": Sequence[str],
-    },
-    total=False,
-)
-
-class TestAuthorizationRequestRequestTypeDef(
-    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
-):
-    pass
-
+AuthInfoUnionTypeDef = Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]
 DescribeAuthorizerResponseTypeDef = TypedDict(
     "DescribeAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6149,14 +5990,32 @@
 
 class UpdateBillingGroupRequestRequestTypeDef(
     _RequiredUpdateBillingGroupRequestRequestTypeDef,
     _OptionalUpdateBillingGroupRequestRequestTypeDef,
 ):
     pass
 
+CodeSigningSignatureTypeDef = TypedDict(
+    "CodeSigningSignatureTypeDef",
+    {
+        "inlineDocument": BlobTypeDef,
+    },
+    total=False,
+)
+
+MqttContextTypeDef = TypedDict(
+    "MqttContextTypeDef",
+    {
+        "username": str,
+        "password": BlobTypeDef,
+        "clientId": str,
+    },
+    total=False,
+)
+
 GetBucketsAggregationResponseTypeDef = TypedDict(
     "GetBucketsAggregationResponseTypeDef",
     {
         "totalCount": int,
         "buckets": List[BucketTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6244,25 +6103,14 @@
         "certificateChain": CodeSigningCertificateChainTypeDef,
         "hashAlgorithm": str,
         "signatureAlgorithm": str,
     },
     total=False,
 )
 
-CustomCodeSigningTypeDef = TypedDict(
-    "CustomCodeSigningTypeDef",
-    {
-        "signature": CodeSigningSignatureTypeDef,
-        "certificateChain": CodeSigningCertificateChainTypeDef,
-        "hashAlgorithm": str,
-        "signatureAlgorithm": str,
-    },
-    total=False,
-)
-
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
         "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6273,14 +6121,158 @@
     "UpdateEventConfigurationsRequestRequestTypeDef",
     {
         "eventConfigurations": Mapping[EventTypeType, ConfigurationTypeDef],
     },
     total=False,
 )
 
+_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "auditTaskId": str,
+        "findingId": str,
+        "taskStatus": AuditMitigationActionsTaskStatusType,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListAuditMitigationActionsTasksRequestRequestTypeDef(
+    _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
+    _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListAuditTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListAuditTasksRequestRequestTypeDef",
+    {
+        "taskType": AuditTaskTypeType,
+        "taskStatus": AuditTaskStatusType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListAuditTasksRequestRequestTypeDef(
+    _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
+):
+    pass
+
+ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
+    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "violationId": str,
+        "thingName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListDetectMitigationActionsTasksRequestRequestTypeDef(
+    _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
+    _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
+    "_RequiredListMetricValuesRequestRequestTypeDef",
+    {
+        "thingName": str,
+        "metricName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListMetricValuesRequestRequestTypeDef = TypedDict(
+    "_OptionalListMetricValuesRequestRequestTypeDef",
+    {
+        "dimensionName": str,
+        "dimensionValueOperator": DimensionValueOperatorType,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListMetricValuesRequestRequestTypeDef(
+    _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
+):
+    pass
+
+_RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListViolationEventsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListViolationEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListViolationEventsRequestRequestTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListViolationEventsRequestRequestTypeDef(
+    _RequiredListViolationEventsRequestRequestTypeDef,
+    _OptionalListViolationEventsRequestRequestTypeDef,
+):
+    pass
+
+ViolationEventOccurrenceRangeTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
         "authorizerFunctionArn": str,
     },
 )
@@ -6778,14 +6770,17 @@
         "thingTypeArn": str,
         "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
+ThingTypePropertiesUnionTypeDef = Union[
+    ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
+]
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
@@ -6795,14 +6790,17 @@
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DetectMitigationActionsTaskTargetUnionTypeDef = Union[
+    DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
+]
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6967,16 +6965,16 @@
     _OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
 ):
     pass
 
 _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
     "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
     "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
     {
         "auditTaskId": str,
         "findingId": str,
@@ -6991,16 +6989,16 @@
     _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
 ):
     pass
 
 _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
     "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
     "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
     {
         "taskType": AuditTaskTypeType,
         "taskStatus": AuditTaskStatusType,
@@ -7084,26 +7082,26 @@
 
 ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
     "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
     {
         "taskId": str,
         "violationId": str,
         "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
     "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
     "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -7224,16 +7222,16 @@
 )
 
 _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
     "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
     {
         "thingName": str,
         "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
     "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
     {
         "dimensionName": str,
         "dimensionValueOperator": DimensionValueOperatorType,
@@ -7717,16 +7715,16 @@
     },
     total=False,
 )
 
 _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
     "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
     },
 )
 _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
     "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
     {
         "thingName": str,
         "securityProfileName": str,
@@ -8192,63 +8190,14 @@
         "roleAliasArn": str,
         "issuerCertificateIdentifier": IssuerCertificateIdentifierTypeDef,
         "deviceCertificateArn": str,
     },
     total=False,
 )
 
-_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "actions": Sequence[str],
-        "clientRequestToken": str,
-    },
-)
-_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
-        "includeOnlyActiveViolations": bool,
-        "includeSuppressedAlerts": bool,
-    },
-    total=False,
-)
-
-class StartDetectMitigationActionsTaskRequestRequestTypeDef(
-    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
-    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
-):
-    pass
-
-_RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
-    "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
-    {
-        "authorizerName": str,
-    },
-)
-_OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
-    "_OptionalTestInvokeAuthorizerRequestRequestTypeDef",
-    {
-        "token": str,
-        "tokenSignature": str,
-        "httpContext": HttpContextTypeDef,
-        "mqttContext": MqttContextTypeDef,
-        "tlsContext": TlsContextTypeDef,
-    },
-    total=False,
-)
-
-class TestInvokeAuthorizerRequestRequestTypeDef(
-    _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
-    _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
-):
-    pass
-
 ThingDocumentTypeDef = TypedDict(
     "ThingDocumentTypeDef",
     {
         "thingName": str,
         "thingId": str,
         "thingTypeName": str,
         "thingGroupNames": List[str],
@@ -8344,14 +8293,15 @@
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AbortConfigUnionTypeDef = Union[AbortConfigTypeDef, AbortConfigOutputTypeDef]
 ListMetricValuesResponseTypeDef = TypedDict(
     "ListMetricValuesResponseTypeDef",
     {
         "metricDatumList": List[MetricDatumTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8452,14 +8402,17 @@
 )
 
 class CreateThingGroupRequestRequestTypeDef(
     _RequiredCreateThingGroupRequestRequestTypeDef, _OptionalCreateThingGroupRequestRequestTypeDef
 ):
     pass
 
+ThingGroupPropertiesUnionTypeDef = Union[
+    ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
+]
 _RequiredUpdateDynamicThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDynamicThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
         "thingGroupProperties": ThingGroupPropertiesTypeDef,
     },
 )
@@ -8496,14 +8449,37 @@
 )
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
+_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_RequiredTestAuthorizationRequestRequestTypeDef",
+    {
+        "authInfos": Sequence[AuthInfoUnionTypeDef],
+    },
+)
+_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_OptionalTestAuthorizationRequestRequestTypeDef",
+    {
+        "principal": str,
+        "cognitoIdentityPoolId": str,
+        "clientId": str,
+        "policyNamesToAdd": Sequence[str],
+        "policyNamesToSkip": Sequence[str],
+    },
+    total=False,
+)
+
+class TestAuthorizationRequestRequestTypeDef(
+    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
+):
+    pass
+
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
@@ -8545,14 +8521,49 @@
     },
     total=False,
 )
 
 class BehaviorTypeDef(_RequiredBehaviorTypeDef, _OptionalBehaviorTypeDef):
     pass
 
+CustomCodeSigningTypeDef = TypedDict(
+    "CustomCodeSigningTypeDef",
+    {
+        "signature": CodeSigningSignatureTypeDef,
+        "certificateChain": CodeSigningCertificateChainTypeDef,
+        "hashAlgorithm": str,
+        "signatureAlgorithm": str,
+    },
+    total=False,
+)
+
+_RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
+    "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
+    {
+        "authorizerName": str,
+    },
+)
+_OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
+    "_OptionalTestInvokeAuthorizerRequestRequestTypeDef",
+    {
+        "token": str,
+        "tokenSignature": str,
+        "httpContext": HttpContextTypeDef,
+        "mqttContext": MqttContextTypeDef,
+        "tlsContext": TlsContextTypeDef,
+    },
+    total=False,
+)
+
+class TestInvokeAuthorizerRequestRequestTypeDef(
+    _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
+    _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
+):
+    pass
+
 _RequiredGetBucketsAggregationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketsAggregationRequestRequestTypeDef",
     {
         "queryString": str,
         "aggregationField": str,
         "bucketsAggregationType": BucketsAggregationTypeTypeDef,
     },
@@ -8585,14 +8596,43 @@
     "DescribeCertificateResponseTypeDef",
     {
         "certificateDescription": CertificateDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "actions": Sequence[str],
+        "clientRequestToken": str,
+    },
+)
+_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "includeOnlyActiveViolations": bool,
+        "includeSuppressedAlerts": bool,
+    },
+    total=False,
+)
+
+class StartDetectMitigationActionsTaskRequestRequestTypeDef(
+    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
+    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
+):
+    pass
+
+ViolationEventOccurrenceRangeUnionTypeDef = Union[
+    ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
+]
+SchedulingConfigUnionTypeDef = Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef]
 ListThingTypesResponseTypeDef = TypedDict(
     "ListThingTypesResponseTypeDef",
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8613,14 +8653,17 @@
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+ThingGroupIndexingConfigurationUnionTypeDef = Union[
+    ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
+]
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -8735,14 +8778,17 @@
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ThingIndexingConfigurationUnionTypeDef = Union[
+    ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
+]
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
     },
     total=False,
@@ -8770,14 +8816,17 @@
     {
         "executionSummaries": List[JobExecutionSummaryForThingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+JobExecutionsRetryConfigUnionTypeDef = Union[
+    JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+]
 ListSecurityProfilesForTargetResponseTypeDef = TypedDict(
     "ListSecurityProfilesForTargetResponseTypeDef",
     {
         "securityProfileTargetMappings": List[SecurityProfileTargetMappingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8836,14 +8885,17 @@
 
 class CreateMitigationActionRequestRequestTypeDef(
     _RequiredCreateMitigationActionRequestRequestTypeDef,
     _OptionalCreateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
+MitigationActionParamsUnionTypeDef = Union[
+    MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
+]
 _RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMitigationActionRequestRequestTypeDef",
     {
         "actionName": str,
     },
 )
 _OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
@@ -8928,15 +8980,15 @@
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "clientRequestToken": str,
     },
 )
 _OptionalCreateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAuditSuppressionRequestRequestTypeDef",
     {
-        "expirationDate": Union[datetime, str],
+        "expirationDate": TimestampTypeDef,
         "suppressIndefinitely": bool,
         "description": str,
     },
     total=False,
 )
 
 class CreateAuditSuppressionRequestRequestTypeDef(
@@ -8975,32 +9027,32 @@
 
 ListAuditFindingsRequestListAuditFindingsPaginateTypeDef = TypedDict(
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "listSuppressedFindings": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditFindingsRequestRequestTypeDef = TypedDict(
     "ListAuditFindingsRequestRequestTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "maxResults": int,
         "nextToken": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "listSuppressedFindings": bool,
     },
     total=False,
 )
 
 ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef = TypedDict(
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
@@ -9051,15 +9103,15 @@
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 _OptionalUpdateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAuditSuppressionRequestRequestTypeDef",
     {
-        "expirationDate": Union[datetime, str],
+        "expirationDate": TimestampTypeDef,
         "suppressIndefinitely": bool,
         "description": str,
     },
     total=False,
 )
 
 class UpdateAuditSuppressionRequestRequestTypeDef(
@@ -9202,74 +9254,15 @@
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "violationEventTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateSecurityProfileRequestRequestTypeDef(
-    _RequiredCreateSecurityProfileRequestRequestTypeDef,
-    _OptionalCreateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "deleteBehaviors": bool,
-        "deleteAlertTargets": bool,
-        "deleteAdditionalMetricsToRetain": bool,
-        "expectedVersion": int,
-    },
-    total=False,
-)
-
-class UpdateSecurityProfileRequestRequestTypeDef(
-    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
-    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
-    {
-        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
-    },
-)
-
+BehaviorUnionTypeDef = Union[BehaviorTypeDef, BehaviorOutputTypeDef]
 CodeSigningOutputTypeDef = TypedDict(
     "CodeSigningOutputTypeDef",
     {
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningOutputTypeDef,
     },
@@ -9584,14 +9577,74 @@
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateSecurityProfileRequestRequestTypeDef(
+    _RequiredCreateSecurityProfileRequestRequestTypeDef,
+    _OptionalCreateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "deleteBehaviors": bool,
+        "deleteAlertTargets": bool,
+        "deleteAdditionalMetricsToRetain": bool,
+        "expectedVersion": int,
+    },
+    total=False,
+)
+
+class UpdateSecurityProfileRequestRequestTypeDef(
+    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
+    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    {
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+    },
+)
+
 OTAUpdateFileOutputTypeDef = TypedDict(
     "OTAUpdateFileOutputTypeDef",
     {
         "fileName": str,
         "fileType": int,
         "fileVersion": str,
         "fileLocation": FileLocationTypeDef,
@@ -9712,44 +9765,15 @@
         "awsIotJobArn": str,
         "errorInfo": ErrorInfoTypeDef,
         "additionalParameters": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
-    {
-        "otaUpdateId": str,
-        "targets": Sequence[str],
-        "files": Sequence[Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]],
-        "roleArn": str,
-    },
-)
-_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
-    {
-        "description": str,
-        "protocols": Sequence[ProtocolType],
-        "targetSelection": TargetSelectionType,
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
-        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
-        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
-        "additionalParameters": Mapping[str, str],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateOTAUpdateRequestRequestTypeDef(
-    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
-):
-    pass
-
+OTAUpdateFileUnionTypeDef = Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]
 GetTopicRuleResponseTypeDef = TypedDict(
     "GetTopicRuleResponseTypeDef",
     {
         "ruleArn": str,
         "rule": TopicRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -9786,7 +9810,37 @@
 GetOTAUpdateResponseTypeDef = TypedDict(
     "GetOTAUpdateResponseTypeDef",
     {
         "otaUpdateInfo": OTAUpdateInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
+    {
+        "otaUpdateId": str,
+        "targets": Sequence[str],
+        "files": Sequence[OTAUpdateFileUnionTypeDef],
+        "roleArn": str,
+    },
+)
+_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
+    {
+        "description": str,
+        "protocols": Sequence[ProtocolType],
+        "targetSelection": TargetSelectionType,
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
+        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
+        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
+        "additionalParameters": Mapping[str, str],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateOTAUpdateRequestRequestTypeDef(
+    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/PKG-INFO` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoT 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iot type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot)](https://pepy.tech/project/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
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
@@ -636,20 +636,20 @@
 )
 
 
 def check_value(value: AbortActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot.type_defs import (
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
@@ -709,31 +709,32 @@
     MachineLearningDetectionConfigTypeDef,
     StatisticalThresholdTypeDef,
     MetricValueTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
     BillingGroupPropertiesTypeDef,
+    BlobTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
     CodeSigningCertificateChainTypeDef,
     CodeSigningSignatureOutputTypeDef,
-    CodeSigningSignatureTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
+    TimestampTypeDef,
     TagTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
     TlsConfigTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
     MaintenanceWindowTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
@@ -869,35 +870,30 @@
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
-    ListAuditMitigationActionsTasksRequestRequestTypeDef,
-    ListAuditTasksRequestRequestTypeDef,
     ListAuthorizersRequestRequestTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
     ListCACertificatesRequestRequestTypeDef,
     ListCertificatesByCARequestRequestTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListCustomMetricsRequestRequestTypeDef,
-    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
-    ListDetectMitigationActionsTasksRequestRequestTypeDef,
     ListDimensionsRequestRequestTypeDef,
     ListDomainConfigurationsRequestRequestTypeDef,
     ListFleetMetricsRequestRequestTypeDef,
     ListIndicesRequestRequestTypeDef,
     ListJobExecutionsForJobRequestRequestTypeDef,
     ListJobExecutionsForThingRequestRequestTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListManagedJobTemplatesRequestRequestTypeDef,
     ManagedJobTemplateSummaryTypeDef,
-    ListMetricValuesRequestRequestTypeDef,
     ListMitigationActionsRequestRequestTypeDef,
     MitigationActionIdentifierTypeDef,
     ListOTAUpdatesRequestRequestTypeDef,
     OTAUpdateSummaryTypeDef,
     ListOutgoingCertificatesRequestRequestTypeDef,
     OutgoingCertificateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
@@ -937,23 +933,21 @@
     ListThingsInThingGroupRequestRequestTypeDef,
     ListThingsRequestRequestTypeDef,
     ThingAttributeTypeDef,
     ListTopicRuleDestinationsRequestRequestTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
-    ListViolationEventsRequestRequestTypeDef,
     LocationTimestampTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
-    MqttContextTypeDef,
     UserPropertyTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
     RegisterThingRequestRequestTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
@@ -961,15 +955,14 @@
     RemoveThingFromThingGroupRequestRequestTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
     SigningProfileParameterTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
     ThingConnectivityTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
@@ -988,14 +981,15 @@
     UpdateScheduledAuditRequestRequestTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
     AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
+    AggregationTypeUnionTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
     AssetPropertyValueTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
     CancelJobResponseTypeDef,
@@ -1077,46 +1071,56 @@
     UpdateDynamicThingGroupResponseTypeDef,
     UpdateMitigationActionResponseTypeDef,
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ThingGroupPropertiesOutputTypeDef,
+    AttributePayloadUnionTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
     DescribeAccountAuditConfigurationResponseTypeDef,
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
-    TestAuthorizationRequestRequestTypeDef,
+    AuthInfoUnionTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
     BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
+    CodeSigningSignatureTypeDef,
+    MqttContextTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
     CertificateDescriptionTypeDef,
     ListCertificatesByCAResponseTypeDef,
     ListCertificatesResponseTypeDef,
     CustomCodeSigningOutputTypeDef,
-    CustomCodeSigningTypeDef,
     DescribeEventConfigurationsResponseTypeDef,
     UpdateEventConfigurationsRequestRequestTypeDef,
+    ListAuditMitigationActionsTasksRequestRequestTypeDef,
+    ListAuditTasksRequestRequestTypeDef,
+    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
+    ListDetectMitigationActionsTasksRequestRequestTypeDef,
+    ListMetricValuesRequestRequestTypeDef,
+    ListViolationEventsRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
@@ -1137,16 +1141,18 @@
     RegisterCACertificateRequestRequestTypeDef,
     UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     ListDomainConfigurationsResponseTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     ExponentialRolloutRateTypeDef,
     ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
     StreamFileTypeDef,
@@ -1248,56 +1254,66 @@
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
     MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
     MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
     ResourceIdentifierTypeDef,
-    StartDetectMitigationActionsTaskRequestRequestTypeDef,
-    TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
     TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
+    AbortConfigUnionTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
     PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
+    TestAuthorizationRequestRequestTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     BehaviorOutputTypeDef,
     BehaviorTypeDef,
+    CustomCodeSigningTypeDef,
+    TestInvokeAuthorizerRequestRequestTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
+    StartDetectMitigationActionsTaskRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
+    SchedulingConfigUnionTypeDef,
     ListThingTypesResponseTypeDef,
     StartSigningJobParameterTypeDef,
     JobExecutionsRolloutConfigTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
     CreateStreamRequestRequestTypeDef,
     StreamInfoTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
     HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     ListJobExecutionsForJobResponseTypeDef,
     ListJobExecutionsForThingResponseTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
     CreateMitigationActionRequestRequestTypeDef,
+    MitigationActionParamsUnionTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
     RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
@@ -1317,17 +1333,15 @@
     AuthResultTypeDef,
     IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     ActiveViolationTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     ViolationEventTypeDef,
-    CreateSecurityProfileRequestRequestTypeDef,
-    UpdateSecurityProfileRequestRequestTypeDef,
-    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
+    BehaviorUnionTypeDef,
     CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
     CreateJobRequestRequestTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     JobTypeDef,
     UpdateJobRequestRequestTypeDef,
@@ -1338,33 +1352,37 @@
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
     TestAuthorizationResponseTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
+    CreateSecurityProfileRequestRequestTypeDef,
+    UpdateSecurityProfileRequestRequestTypeDef,
+    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     DescribeJobResponseTypeDef,
     DescribeDetectMitigationActionsTaskResponseTypeDef,
     ListDetectMitigationActionsTasksResponseTypeDef,
     DescribeAuditFindingResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     TopicRuleTypeDef,
     TopicRulePayloadTypeDef,
     OTAUpdateInfoTypeDef,
-    CreateOTAUpdateRequestRequestTypeDef,
+    OTAUpdateFileUnionTypeDef,
     GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
     GetOTAUpdateResponseTypeDef,
+    CreateOTAUpdateRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaTypeDef:
+def get_value() -> AbortCriteriaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/SOURCES.txt` & `mypy-boto3-iot-1.28.16/mypy_boto3_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15.post1/setup.py` & `mypy-boto3-iot-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.IoT 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 iot type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iot type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iot": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

