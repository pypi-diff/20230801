# Comparing `tmp/mypy-boto3-config-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-config-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-config-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:51 2023, max compression
+gzip compressed data, was "mypy-boto3-config-1.28.16.tar", last modified: Tue Aug  1 11:36:32 2023, max compression
```

## Comparing `mypy-boto3-config-1.28.15.post1.tar` & `mypy-boto3-config-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.617087 mypy-boto3-config-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37114 2023-07-29 10:02:51.609087 mypy-boto3-config-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35618 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.605087 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-29 09:41:21.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89729 2023-07-29 09:41:21.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    89599 2023-07-29 09:41:21.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-07-29 09:41:23.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-07-29 09:41:22.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42907 2023-07-29 09:41:22.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    42874 2023-07-29 09:41:22.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:21.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   135526 2023-07-29 09:41:27.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   135359 2023-07-29 09:41:25.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.609087 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37114 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:51.617087 mypy-boto3-config-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:32.100918 mypy-boto3-config-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:53.000000 mypy-boto3-config-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37449 2023-08-01 11:36:32.096918 mypy-boto3-config-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35962 2023-08-01 11:13:53.000000 mypy-boto3-config-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:32.092918 mypy-boto3-config-1.28.16/mypy_boto3_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-08-01 11:13:53.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-08-01 11:13:53.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-01 11:13:53.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88908 2023-08-01 11:13:54.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88778 2023-08-01 11:13:53.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-08-01 11:13:56.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-08-01 11:13:55.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42884 2023-08-01 11:13:55.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42851 2023-08-01 11:13:55.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:53.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   136671 2023-08-01 11:13:59.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136504 2023-08-01 11:13:57.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:53.000000 mypy-boto3-config-1.28.16/mypy_boto3_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:32.096918 mypy-boto3-config-1.28.16/mypy_boto3_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37449 2023-08-01 11:36:31.000000 mypy-boto3-config-1.28.16/mypy_boto3_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 11:36:31.000000 mypy-boto3-config-1.28.16/mypy_boto3_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:31.000000 mypy-boto3-config-1.28.16/mypy_boto3_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:31.000000 mypy-boto3-config-1.28.16/mypy_boto3_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:31.000000 mypy-boto3-config-1.28.16/mypy_boto3_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:36:31.000000 mypy-boto3-config-1.28.16/mypy_boto3_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:32.100918 mypy-boto3-config-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:13:53.000000 mypy-boto3-config-1.28.16/setup.py
```

### Comparing `mypy-boto3-config-1.28.15.post1/LICENSE` & `mypy-boto3-config-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15.post1/PKG-INFO` & `mypy-boto3-config-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ConfigService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 config type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 config type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
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
@@ -497,20 +497,20 @@
 )
 
 
 def check_value(value: AggregateConformancePackComplianceSummaryGroupKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_config.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_config.type_defs import (
     AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
@@ -587,19 +587,18 @@
     RemediationExceptionTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
     EvaluationContextTypeDef,
     EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
-    EvaluationTypeDef,
+    TimestampTypeDef,
     ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
     SsmControlsTypeDef,
-    ExternalEvaluationTypeDef,
     FieldInfoTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     GetComplianceDetailsByResourceRequestRequestTypeDef,
     GetComplianceSummaryByResourceTypeRequestRequestTypeDef,
@@ -608,15 +607,14 @@
     GetDiscoveredResourceCountsRequestRequestTypeDef,
     ResourceCountTypeDef,
     StatusDetailFiltersTypeDef,
     MemberAccountStatusTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
-    GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
     ResourceDetailsTypeDef,
     GetStoredQueryRequestRequestTypeDef,
     StoredQueryTypeDef,
     ResourceFiltersTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
@@ -635,22 +633,22 @@
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
     ResourceValueTypeDef,
     StaticValueOutputTypeDef,
     StaticValueTypeDef,
-    TimeWindowTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
@@ -692,15 +690,14 @@
     PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
     FailedDeleteRemediationExceptionsBatchTypeDef,
-    PutRemediationExceptionsRequestRequestTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
     DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
     DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
     DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
     DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
@@ -714,15 +711,14 @@
     DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
     DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
     GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
@@ -730,17 +726,21 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     EvaluationResultIdentifierTypeDef,
-    PutEvaluationsRequestRequestTypeDef,
+    EvaluationTypeDef,
+    ExternalEvaluationTypeDef,
+    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    GetResourceConfigHistoryRequestRequestTypeDef,
+    PutRemediationExceptionsRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ExecutionControlsTypeDef,
-    PutExternalEvaluationRequestRequestTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
@@ -755,25 +755,27 @@
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
     PutStoredQueryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    PutConfigurationAggregatorRequestRequestTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationConfigRuleTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     PutOrganizationConfigRuleRequestRequestTypeDef,
     RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
     RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
-    ResourceEvaluationFiltersTypeDef,
     SourceOutputTypeDef,
     SourceTypeDef,
+    PutConfigurationAggregatorRequestRequestTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
     GetComplianceSummaryByConfigRuleResponseTypeDef,
     AggregateComplianceByConfigRuleTypeDef,
     ComplianceByConfigRuleTypeDef,
@@ -788,47 +790,54 @@
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
+    EvaluationUnionTypeDef,
+    PutExternalEvaluationRequestRequestTypeDef,
+    ResourceEvaluationFiltersTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
     ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
-    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
-    ListResourceEvaluationsRequestRequestTypeDef,
     ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetComplianceSummaryByResourceTypeResponseTypeDef,
     DescribeAggregateComplianceByConfigRulesResponseTypeDef,
     DescribeComplianceByConfigRuleResponseTypeDef,
     DescribeComplianceByResourceResponseTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetConformancePackComplianceDetailsResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
     GetComplianceDetailsByResourceResponseTypeDef,
+    PutEvaluationsRequestRequestTypeDef,
+    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
+    ListResourceEvaluationsRequestRequestTypeDef,
     DescribeConfigurationRecordersResponseTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     PutConfigurationRecorderRequestRequestTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     FailedRemediationBatchTypeDef,
-    PutRemediationConfigurationsRequestRequestTypeDef,
+    RemediationConfigurationUnionTypeDef,
     DescribeConfigRulesResponseTypeDef,
+    ConfigRuleUnionTypeDef,
     PutConfigRuleRequestRequestTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
+    PutRemediationConfigurationsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountAggregationSourceOutputTypeDef:
+def get_value() -> AccountAggregationSourceOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-config-1.28.15.post1/README.md` & `mypy-boto3-config-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
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
@@ -465,20 +465,20 @@
 )
 
 
 def check_value(value: AggregateConformancePackComplianceSummaryGroupKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_config.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_config.type_defs import (
     AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
@@ -555,19 +555,18 @@
     RemediationExceptionTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
     EvaluationContextTypeDef,
     EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
-    EvaluationTypeDef,
+    TimestampTypeDef,
     ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
     SsmControlsTypeDef,
-    ExternalEvaluationTypeDef,
     FieldInfoTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     GetComplianceDetailsByResourceRequestRequestTypeDef,
     GetComplianceSummaryByResourceTypeRequestRequestTypeDef,
@@ -576,15 +575,14 @@
     GetDiscoveredResourceCountsRequestRequestTypeDef,
     ResourceCountTypeDef,
     StatusDetailFiltersTypeDef,
     MemberAccountStatusTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
-    GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
     ResourceDetailsTypeDef,
     GetStoredQueryRequestRequestTypeDef,
     StoredQueryTypeDef,
     ResourceFiltersTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
@@ -603,22 +601,22 @@
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
     ResourceValueTypeDef,
     StaticValueOutputTypeDef,
     StaticValueTypeDef,
-    TimeWindowTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
@@ -660,15 +658,14 @@
     PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
     FailedDeleteRemediationExceptionsBatchTypeDef,
-    PutRemediationExceptionsRequestRequestTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
     DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
     DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
     DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
     DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
@@ -682,15 +679,14 @@
     DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
     DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
     GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
@@ -698,17 +694,21 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     EvaluationResultIdentifierTypeDef,
-    PutEvaluationsRequestRequestTypeDef,
+    EvaluationTypeDef,
+    ExternalEvaluationTypeDef,
+    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    GetResourceConfigHistoryRequestRequestTypeDef,
+    PutRemediationExceptionsRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ExecutionControlsTypeDef,
-    PutExternalEvaluationRequestRequestTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
@@ -723,25 +723,27 @@
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
     PutStoredQueryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    PutConfigurationAggregatorRequestRequestTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationConfigRuleTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     PutOrganizationConfigRuleRequestRequestTypeDef,
     RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
     RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
-    ResourceEvaluationFiltersTypeDef,
     SourceOutputTypeDef,
     SourceTypeDef,
+    PutConfigurationAggregatorRequestRequestTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
     GetComplianceSummaryByConfigRuleResponseTypeDef,
     AggregateComplianceByConfigRuleTypeDef,
     ComplianceByConfigRuleTypeDef,
@@ -756,47 +758,54 @@
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
+    EvaluationUnionTypeDef,
+    PutExternalEvaluationRequestRequestTypeDef,
+    ResourceEvaluationFiltersTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
     ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
-    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
-    ListResourceEvaluationsRequestRequestTypeDef,
     ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetComplianceSummaryByResourceTypeResponseTypeDef,
     DescribeAggregateComplianceByConfigRulesResponseTypeDef,
     DescribeComplianceByConfigRuleResponseTypeDef,
     DescribeComplianceByResourceResponseTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetConformancePackComplianceDetailsResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
     GetComplianceDetailsByResourceResponseTypeDef,
+    PutEvaluationsRequestRequestTypeDef,
+    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
+    ListResourceEvaluationsRequestRequestTypeDef,
     DescribeConfigurationRecordersResponseTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     PutConfigurationRecorderRequestRequestTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     FailedRemediationBatchTypeDef,
-    PutRemediationConfigurationsRequestRequestTypeDef,
+    RemediationConfigurationUnionTypeDef,
     DescribeConfigRulesResponseTypeDef,
+    ConfigRuleUnionTypeDef,
     PutConfigRuleRequestRequestTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
+    PutRemediationConfigurationsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountAggregationSourceOutputTypeDef:
+def get_value() -> AccountAggregationSourceOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__init__.py` & `mypy-boto3-config-1.28.16/mypy_boto3_config/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__init__.pyi` & `mypy-boto3-config-1.28.16/mypy_boto3_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__main__.py` & `mypy-boto3-config-1.28.16/mypy_boto3_config/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConfigService 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ConfigService 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\nOther"
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

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/client.py` & `mypy-boto3-config-1.28.16/mypy_boto3_config/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_config.client import ConfigServiceClient
 
     session = Session()
     client: ConfigServiceClient = session.client("config")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregateConformancePackComplianceSummaryGroupKeyType,
     AggregatedSourceStatusTypeType,
     ChronologicalOrderType,
@@ -60,27 +59,24 @@
     ListDiscoveredResourcesPaginator,
     ListResourceEvaluationsPaginator,
     ListTagsForResourcePaginator,
     SelectAggregateResourceConfigPaginator,
     SelectResourceConfigPaginator,
 )
 from .type_defs import (
-    AccountAggregationSourceOutputTypeDef,
-    AccountAggregationSourceTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigResponseTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
-    ConfigRuleOutputTypeDef,
-    ConfigRuleTypeDef,
-    ConfigurationRecorderOutputTypeDef,
-    ConfigurationRecorderTypeDef,
+    ConfigRuleUnionTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     DeliverConfigSnapshotResponseTypeDef,
     DeliveryChannelTypeDef,
@@ -108,16 +104,15 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
-    EvaluationOutputTypeDef,
-    EvaluationTypeDef,
+    EvaluationUnionTypeDef,
     ExternalEvaluationTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
@@ -136,48 +131,45 @@
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesResponseTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OrganizationAggregationSourceOutputTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
-    OrganizationCustomRuleMetadataOutputTypeDef,
-    OrganizationCustomRuleMetadataTypeDef,
-    OrganizationManagedRuleMetadataOutputTypeDef,
-    OrganizationManagedRuleMetadataTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     PutConformancePackResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutStoredQueryResponseTypeDef,
-    RemediationConfigurationOutputTypeDef,
-    RemediationConfigurationTypeDef,
+    RemediationConfigurationUnionTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     ResourceCountFiltersTypeDef,
     ResourceDetailsTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     StartResourceEvaluationResponseTypeDef,
     StatusDetailFiltersTypeDef,
     StoredQueryTypeDef,
     TagTypeDef,
     TemplateSSMDocumentDetailsTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -1032,16 +1024,16 @@
         """
 
     def get_resource_config_history(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
-        laterTime: Union[datetime, str] = ...,
-        earlierTime: Union[datetime, str] = ...,
+        laterTime: TimestampTypeDef = ...,
+        earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
         limit: int = ...,
         nextToken: str = ...
     ) -> GetResourceConfigHistoryResponseTypeDef:
         """
         Returns a list of `ConfigurationItems` for the specified resource.
 
@@ -1166,53 +1158,42 @@
         account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_aggregation_authorization)
         """
 
     def put_config_rule(
-        self,
-        *,
-        ConfigRule: Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        self, *, ConfigRule: ConfigRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an Config rule to evaluate if your Amazon Web Services resources
         comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_config_rule)
         """
 
     def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
-        AccountAggregationSources: Sequence[
-            Union[AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef]
-        ] = ...,
-        OrganizationAggregationSource: Union[
-            OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
-        ] = ...,
+        AccountAggregationSources: Sequence[AccountAggregationSourceUnionTypeDef] = ...,
+        OrganizationAggregationSource: OrganizationAggregationSourceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_configuration_aggregator)
         """
 
     def put_configuration_recorder(
-        self,
-        *,
-        ConfigurationRecorder: Union[
-            ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
-        ]
+        self, *, ConfigurationRecorder: ConfigurationRecorderUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new configuration recorder to record configuration changes for
         specified resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_recorder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_configuration_recorder)
@@ -1247,15 +1228,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_delivery_channel)
         """
 
     def put_evaluations(
         self,
         *,
         ResultToken: str,
-        Evaluations: Sequence[Union[EvaluationTypeDef, EvaluationOutputTypeDef]] = ...,
+        Evaluations: Sequence[EvaluationUnionTypeDef] = ...,
         TestMode: bool = ...
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_evaluations)
@@ -1271,20 +1252,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_external_evaluation)
         """
 
     def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
-        OrganizationManagedRuleMetadata: Union[
-            OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
-        ] = ...,
-        OrganizationCustomRuleMetadata: Union[
-            OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
-        ] = ...,
+        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataUnionTypeDef = ...,
+        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataUnionTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired configurations.
 
@@ -1308,19 +1285,15 @@
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_organization_conformance_pack)
         """
 
     def put_remediation_configurations(
-        self,
-        *,
-        RemediationConfigurations: Sequence[
-            Union[RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef]
-        ]
+        self, *, RemediationConfigurations: Sequence[RemediationConfigurationUnionTypeDef]
     ) -> PutRemediationConfigurationsResponseTypeDef:
         """
         Adds or updates the remediation configuration with a specific Config rule with
         the selected target or action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_remediation_configurations)
@@ -1328,15 +1301,15 @@
 
     def put_remediation_exceptions(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],
         Message: str = ...,
-        ExpirationTime: Union[datetime, str] = ...
+        ExpirationTime: TimestampTypeDef = ...
     ) -> PutRemediationExceptionsResponseTypeDef:
         """
         A remediation exception is when a specified resource is no longer considered for
         auto-remediation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_remediation_exceptions)
```

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/client.pyi` & `mypy-boto3-config-1.28.16/mypy_boto3_config/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_config.client import ConfigServiceClient
 
     session = Session()
     client: ConfigServiceClient = session.client("config")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregateConformancePackComplianceSummaryGroupKeyType,
     AggregatedSourceStatusTypeType,
     ChronologicalOrderType,
@@ -60,27 +59,24 @@
     ListDiscoveredResourcesPaginator,
     ListResourceEvaluationsPaginator,
     ListTagsForResourcePaginator,
     SelectAggregateResourceConfigPaginator,
     SelectResourceConfigPaginator,
 )
 from .type_defs import (
-    AccountAggregationSourceOutputTypeDef,
-    AccountAggregationSourceTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigResponseTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
-    ConfigRuleOutputTypeDef,
-    ConfigRuleTypeDef,
-    ConfigurationRecorderOutputTypeDef,
-    ConfigurationRecorderTypeDef,
+    ConfigRuleUnionTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     DeliverConfigSnapshotResponseTypeDef,
     DeliveryChannelTypeDef,
@@ -108,16 +104,15 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
-    EvaluationOutputTypeDef,
-    EvaluationTypeDef,
+    EvaluationUnionTypeDef,
     ExternalEvaluationTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
@@ -136,48 +131,45 @@
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesResponseTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OrganizationAggregationSourceOutputTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
-    OrganizationCustomRuleMetadataOutputTypeDef,
-    OrganizationCustomRuleMetadataTypeDef,
-    OrganizationManagedRuleMetadataOutputTypeDef,
-    OrganizationManagedRuleMetadataTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     PutConformancePackResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutStoredQueryResponseTypeDef,
-    RemediationConfigurationOutputTypeDef,
-    RemediationConfigurationTypeDef,
+    RemediationConfigurationUnionTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     ResourceCountFiltersTypeDef,
     ResourceDetailsTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     StartResourceEvaluationResponseTypeDef,
     StatusDetailFiltersTypeDef,
     StoredQueryTypeDef,
     TagTypeDef,
     TemplateSSMDocumentDetailsTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -965,16 +957,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#get_organization_custom_rule_policy)
         """
     def get_resource_config_history(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
-        laterTime: Union[datetime, str] = ...,
-        earlierTime: Union[datetime, str] = ...,
+        laterTime: TimestampTypeDef = ...,
+        earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
         limit: int = ...,
         nextToken: str = ...
     ) -> GetResourceConfigHistoryResponseTypeDef:
         """
         Returns a list of `ConfigurationItems` for the specified resource.
 
@@ -1089,51 +1081,40 @@
         Authorizes the aggregator account and region to collect data from the source
         account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_aggregation_authorization)
         """
     def put_config_rule(
-        self,
-        *,
-        ConfigRule: Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        self, *, ConfigRule: ConfigRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an Config rule to evaluate if your Amazon Web Services resources
         comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_config_rule)
         """
     def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
-        AccountAggregationSources: Sequence[
-            Union[AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef]
-        ] = ...,
-        OrganizationAggregationSource: Union[
-            OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
-        ] = ...,
+        AccountAggregationSources: Sequence[AccountAggregationSourceUnionTypeDef] = ...,
+        OrganizationAggregationSource: OrganizationAggregationSourceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_configuration_aggregator)
         """
     def put_configuration_recorder(
-        self,
-        *,
-        ConfigurationRecorder: Union[
-            ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
-        ]
+        self, *, ConfigurationRecorder: ConfigurationRecorderUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new configuration recorder to record configuration changes for
         specified resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_recorder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_configuration_recorder)
@@ -1165,15 +1146,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_delivery_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_delivery_channel)
         """
     def put_evaluations(
         self,
         *,
         ResultToken: str,
-        Evaluations: Sequence[Union[EvaluationTypeDef, EvaluationOutputTypeDef]] = ...,
+        Evaluations: Sequence[EvaluationUnionTypeDef] = ...,
         TestMode: bool = ...
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_evaluations)
@@ -1187,20 +1168,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_external_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_external_evaluation)
         """
     def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
-        OrganizationManagedRuleMetadata: Union[
-            OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
-        ] = ...,
-        OrganizationCustomRuleMetadata: Union[
-            OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
-        ] = ...,
+        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataUnionTypeDef = ...,
+        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataUnionTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired configurations.
 
@@ -1222,34 +1199,30 @@
         Deploys conformance packs across member accounts in an Amazon Web Services
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_organization_conformance_pack)
         """
     def put_remediation_configurations(
-        self,
-        *,
-        RemediationConfigurations: Sequence[
-            Union[RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef]
-        ]
+        self, *, RemediationConfigurations: Sequence[RemediationConfigurationUnionTypeDef]
     ) -> PutRemediationConfigurationsResponseTypeDef:
         """
         Adds or updates the remediation configuration with a specific Config rule with
         the selected target or action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_remediation_configurations)
         """
     def put_remediation_exceptions(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],
         Message: str = ...,
-        ExpirationTime: Union[datetime, str] = ...
+        ExpirationTime: TimestampTypeDef = ...
     ) -> PutRemediationExceptionsResponseTypeDef:
         """
         A remediation exception is when a specified resource is no longer considered for
         auto-remediation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_remediation_exceptions)
```

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/literals.py` & `mypy-boto3-config-1.28.16/mypy_boto3_config/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/literals.pyi` & `mypy-boto3-config-1.28.16/mypy_boto3_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/paginator.py` & `mypy-boto3-config-1.28.16/mypy_boto3_config/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,15 @@
     list_discovered_resources_paginator: ListDiscoveredResourcesPaginator = client.get_paginator("list_discovered_resources")
     list_resource_evaluations_paginator: ListResourceEvaluationsPaginator = client.get_paginator("list_resource_evaluations")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     select_aggregate_resource_config_paginator: SelectAggregateResourceConfigPaginator = client.get_paginator("select_aggregate_resource_config")
     select_resource_config_paginator: SelectResourceConfigPaginator = client.get_paginator("select_resource_config")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AggregatedSourceStatusTypeType,
     ChronologicalOrderType,
     ComplianceTypeType,
@@ -127,14 +126,15 @@
     PaginatorConfigTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     StatusDetailFiltersTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeAggregateComplianceByConfigRulesPaginator",
     "DescribeAggregateComplianceByConformancePacksPaginator",
     "DescribeAggregationAuthorizationsPaginator",
     "DescribeComplianceByConfigRulePaginator",
@@ -626,16 +626,16 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
-        laterTime: Union[datetime, str] = ...,
-        earlierTime: Union[datetime, str] = ...,
+        laterTime: TimestampTypeDef = ...,
+        earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceConfigHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetResourceConfigHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getresourceconfighistorypaginator)
         """
```

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/paginator.pyi` & `mypy-boto3-config-1.28.16/mypy_boto3_config/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,15 @@
     list_discovered_resources_paginator: ListDiscoveredResourcesPaginator = client.get_paginator("list_discovered_resources")
     list_resource_evaluations_paginator: ListResourceEvaluationsPaginator = client.get_paginator("list_resource_evaluations")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     select_aggregate_resource_config_paginator: SelectAggregateResourceConfigPaginator = client.get_paginator("select_aggregate_resource_config")
     select_resource_config_paginator: SelectResourceConfigPaginator = client.get_paginator("select_resource_config")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AggregatedSourceStatusTypeType,
     ChronologicalOrderType,
     ComplianceTypeType,
@@ -127,14 +126,15 @@
     PaginatorConfigTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     StatusDetailFiltersTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeAggregateComplianceByConfigRulesPaginator",
     "DescribeAggregateComplianceByConformancePacksPaginator",
     "DescribeAggregationAuthorizationsPaginator",
     "DescribeComplianceByConfigRulePaginator",
@@ -599,16 +599,16 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
-        laterTime: Union[datetime, str] = ...,
-        earlierTime: Union[datetime, str] = ...,
+        laterTime: TimestampTypeDef = ...,
+        earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceConfigHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetResourceConfigHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getresourceconfighistorypaginator)
         """
```

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/type_defs.py` & `mypy-boto3-config-1.28.16/mypy_boto3_config/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_config.type_defs import AccountAggregationSourceOutputTypeDef
 
-    data: AccountAggregationSourceOutputTypeDef = {...}
+    data: AccountAggregationSourceOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,15 +52,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
@@ -135,19 +134,18 @@
     "RemediationExceptionTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
     "EvaluationContextTypeDef",
     "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
-    "EvaluationTypeDef",
+    "TimestampTypeDef",
     "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
     "SsmControlsTypeDef",
-    "ExternalEvaluationTypeDef",
     "FieldInfoTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
@@ -156,15 +154,14 @@
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     "ResourceCountTypeDef",
     "StatusDetailFiltersTypeDef",
     "MemberAccountStatusTypeDef",
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     "OrganizationConformancePackDetailedStatusTypeDef",
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
-    "GetResourceConfigHistoryRequestRequestTypeDef",
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     "ResourceDetailsTypeDef",
     "GetStoredQueryRequestRequestTypeDef",
     "StoredQueryTypeDef",
     "ResourceFiltersTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
@@ -183,22 +180,22 @@
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
     "ResourceValueTypeDef",
     "StaticValueOutputTypeDef",
     "StaticValueTypeDef",
-    "TimeWindowTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AccountAggregationSourceUnionTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigResponseTypeDef",
@@ -240,15 +237,14 @@
     "PutConformancePackRequestRequestTypeDef",
     "GetConformancePackComplianceDetailsRequestRequestTypeDef",
     "DescribeConformancePackComplianceResponseTypeDef",
     "DescribeConformancePackStatusResponseTypeDef",
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     "DescribeRemediationExceptionsRequestRequestTypeDef",
     "FailedDeleteRemediationExceptionsBatchTypeDef",
-    "PutRemediationExceptionsRequestRequestTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
     "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
     "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
     "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
     "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
@@ -262,15 +258,14 @@
     "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
     "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
     "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     "DescribeConfigRulesRequestRequestTypeDef",
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
@@ -278,17 +273,21 @@
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
     "PutEvaluationsResponseTypeDef",
     "EvaluationResultIdentifierTypeDef",
-    "PutEvaluationsRequestRequestTypeDef",
+    "EvaluationTypeDef",
+    "ExternalEvaluationTypeDef",
+    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    "GetResourceConfigHistoryRequestRequestTypeDef",
+    "PutRemediationExceptionsRequestRequestTypeDef",
+    "TimeWindowTypeDef",
     "ExecutionControlsTypeDef",
-    "PutExternalEvaluationRequestRequestTypeDef",
     "QueryInfoTypeDef",
     "GetAggregateDiscoveredResourceCountsRequestRequestTypeDef",
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     "GetDiscoveredResourceCountsResponseTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
@@ -303,25 +302,27 @@
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
     "PutStoredQueryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "PutConfigurationAggregatorRequestRequestTypeDef",
+    "OrganizationAggregationSourceUnionTypeDef",
     "OrganizationConfigRuleTypeDef",
+    "OrganizationCustomRuleMetadataUnionTypeDef",
+    "OrganizationManagedRuleMetadataUnionTypeDef",
     "PutOrganizationConfigRuleRequestRequestTypeDef",
     "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
     "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
-    "ResourceEvaluationFiltersTypeDef",
     "SourceOutputTypeDef",
     "SourceTypeDef",
+    "PutConfigurationAggregatorRequestRequestTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     "AggregateComplianceByConfigRuleTypeDef",
     "ComplianceByConfigRuleTypeDef",
@@ -336,43 +337,50 @@
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
     "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
+    "EvaluationUnionTypeDef",
+    "PutExternalEvaluationRequestRequestTypeDef",
+    "ResourceEvaluationFiltersTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
     "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
     "RemediationConfigurationOutputTypeDef",
     "RemediationConfigurationTypeDef",
-    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
-    "ListResourceEvaluationsRequestRequestTypeDef",
     "ConfigRuleOutputTypeDef",
     "ConfigRuleTypeDef",
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     "DescribeComplianceByConfigRuleResponseTypeDef",
     "DescribeComplianceByResourceResponseTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     "GetConformancePackComplianceDetailsResponseTypeDef",
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     "GetComplianceDetailsByResourceResponseTypeDef",
+    "PutEvaluationsRequestRequestTypeDef",
+    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+    "ListResourceEvaluationsRequestRequestTypeDef",
     "DescribeConfigurationRecordersResponseTypeDef",
+    "ConfigurationRecorderUnionTypeDef",
     "PutConfigurationRecorderRequestRequestTypeDef",
     "DescribeRemediationConfigurationsResponseTypeDef",
     "FailedRemediationBatchTypeDef",
-    "PutRemediationConfigurationsRequestRequestTypeDef",
+    "RemediationConfigurationUnionTypeDef",
     "DescribeConfigRulesResponseTypeDef",
+    "ConfigRuleUnionTypeDef",
     "PutConfigRuleRequestRequestTypeDef",
     "PutRemediationConfigurationsResponseTypeDef",
+    "PutRemediationConfigurationsRequestRequestTypeDef",
 )
 
 _RequiredAccountAggregationSourceOutputTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceOutputTypeDef",
     {
         "AccountIds": List[str],
     },
@@ -382,21 +390,19 @@
     {
         "AllAwsRegions": bool,
         "AwsRegions": List[str],
     },
     total=False,
 )
 
-
 class AccountAggregationSourceOutputTypeDef(
     _RequiredAccountAggregationSourceOutputTypeDef, _OptionalAccountAggregationSourceOutputTypeDef
 ):
     pass
 
-
 _RequiredAccountAggregationSourceTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 _OptionalAccountAggregationSourceTypeDef = TypedDict(
@@ -404,21 +410,19 @@
     {
         "AllAwsRegions": bool,
         "AwsRegions": Sequence[str],
     },
     total=False,
 )
 
-
 class AccountAggregationSourceTypeDef(
     _RequiredAccountAggregationSourceTypeDef, _OptionalAccountAggregationSourceTypeDef
 ):
     pass
 
-
 AggregateConformancePackComplianceTypeDef = TypedDict(
     "AggregateConformancePackComplianceTypeDef",
     {
         "ComplianceType": ConformancePackComplianceTypeType,
         "CompliantRuleCount": int,
         "NonCompliantRuleCount": int,
         "TotalRuleCount": int,
@@ -468,21 +472,19 @@
     "_OptionalAggregateResourceIdentifierTypeDef",
     {
         "ResourceName": str,
     },
     total=False,
 )
 
-
 class AggregateResourceIdentifierTypeDef(
     _RequiredAggregateResourceIdentifierTypeDef, _OptionalAggregateResourceIdentifierTypeDef
 ):
     pass
 
-
 AggregatedSourceStatusTypeDef = TypedDict(
     "AggregatedSourceStatusTypeDef",
     {
         "SourceId": str,
         "SourceType": AggregatedSourceTypeType,
         "AwsRegion": str,
         "LastUpdateStatus": AggregatedSourceStatusTypeType,
@@ -668,22 +670,20 @@
     {
         "AwsRegions": List[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
-
 class OrganizationAggregationSourceOutputTypeDef(
     _RequiredOrganizationAggregationSourceOutputTypeDef,
     _OptionalOrganizationAggregationSourceOutputTypeDef,
 ):
     pass
 
-
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "resourceName": str,
         "relationshipName": str,
@@ -758,21 +758,19 @@
     "_OptionalTemplateSSMDocumentDetailsTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
-
 class TemplateSSMDocumentDetailsTypeDef(
     _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
 ):
     pass
 
-
 ConformancePackEvaluationFiltersTypeDef = TypedDict(
     "ConformancePackEvaluationFiltersTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "ComplianceType": ConformancePackComplianceTypeType,
         "ResourceType": str,
         "ResourceIds": Sequence[str],
@@ -806,21 +804,19 @@
     {
         "ConformancePackStatusReason": str,
         "LastUpdateCompletedTime": datetime,
     },
     total=False,
 )
 
-
 class ConformancePackStatusDetailTypeDef(
     _RequiredConformancePackStatusDetailTypeDef, _OptionalConformancePackStatusDetailTypeDef
 ):
     pass
 
-
 _RequiredCustomPolicyDetailsTypeDef = TypedDict(
     "_RequiredCustomPolicyDetailsTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
 )
@@ -828,21 +824,19 @@
     "_OptionalCustomPolicyDetailsTypeDef",
     {
         "EnableDebugLogDelivery": bool,
     },
     total=False,
 )
 
-
 class CustomPolicyDetailsTypeDef(
     _RequiredCustomPolicyDetailsTypeDef, _OptionalCustomPolicyDetailsTypeDef
 ):
     pass
 
-
 DeleteAggregationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteAggregationAuthorizationRequestRequestTypeDef",
     {
         "AuthorizedAccountId": str,
         "AuthorizedAwsRegion": str,
     },
 )
@@ -921,22 +915,20 @@
     "_OptionalDeleteRemediationConfigurationRequestRequestTypeDef",
     {
         "ResourceType": str,
     },
     total=False,
 )
 
-
 class DeleteRemediationConfigurationRequestRequestTypeDef(
     _RequiredDeleteRemediationConfigurationRequestRequestTypeDef,
     _OptionalDeleteRemediationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 RemediationExceptionResourceKeyTypeDef = TypedDict(
     "RemediationExceptionResourceKeyTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
     },
     total=False,
@@ -1042,22 +1034,20 @@
         "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeConfigurationAggregatorsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -1139,21 +1129,19 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-
 class OrganizationConfigRuleStatusTypeDef(
     _RequiredOrganizationConfigRuleStatusTypeDef, _OptionalOrganizationConfigRuleStatusTypeDef
 ):
     pass
 
-
 DescribeOrganizationConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1183,22 +1171,20 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-
 class OrganizationConformancePackStatusTypeDef(
     _RequiredOrganizationConformancePackStatusTypeDef,
     _OptionalOrganizationConformancePackStatusTypeDef,
 ):
     pass
 
-
 DescribeOrganizationConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1243,21 +1229,19 @@
     {
         "Message": str,
         "ExpirationTime": datetime,
     },
     total=False,
 )
 
-
 class RemediationExceptionTypeDef(
     _RequiredRemediationExceptionTypeDef, _OptionalRemediationExceptionTypeDef
 ):
     pass
 
-
 DescribeRetentionConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -1292,19 +1276,17 @@
     "_OptionalEvaluationOutputTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
-
 class EvaluationOutputTypeDef(_RequiredEvaluationOutputTypeDef, _OptionalEvaluationOutputTypeDef):
     pass
 
-
 EvaluationResultQualifierTypeDef = TypedDict(
     "EvaluationResultQualifierTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceType": str,
         "ResourceId": str,
         "EvaluationMode": EvaluationModeType,
@@ -1322,41 +1304,18 @@
     "_OptionalEvaluationStatusTypeDef",
     {
         "FailureReason": str,
     },
     total=False,
 )
 
-
 class EvaluationStatusTypeDef(_RequiredEvaluationStatusTypeDef, _OptionalEvaluationStatusTypeDef):
     pass
 
-
-_RequiredEvaluationTypeDef = TypedDict(
-    "_RequiredEvaluationTypeDef",
-    {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": Union[datetime, str],
-    },
-)
-_OptionalEvaluationTypeDef = TypedDict(
-    "_OptionalEvaluationTypeDef",
-    {
-        "Annotation": str,
-    },
-    total=False,
-)
-
-
-class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ExclusionByResourceTypesOutputTypeDef = TypedDict(
     "ExclusionByResourceTypesOutputTypeDef",
     {
         "resourceTypes": List[ResourceTypeType],
     },
     total=False,
 )
@@ -1374,38 +1333,14 @@
     {
         "ConcurrentExecutionRatePercentage": int,
         "ErrorPercentage": int,
     },
     total=False,
 )
 
-_RequiredExternalEvaluationTypeDef = TypedDict(
-    "_RequiredExternalEvaluationTypeDef",
-    {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": Union[datetime, str],
-    },
-)
-_OptionalExternalEvaluationTypeDef = TypedDict(
-    "_OptionalExternalEvaluationTypeDef",
-    {
-        "Annotation": str,
-    },
-    total=False,
-)
-
-
-class ExternalEvaluationTypeDef(
-    _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
-):
-    pass
-
-
 FieldInfoTypeDef = TypedDict(
     "FieldInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -1425,22 +1360,20 @@
         "ComplianceType": ComplianceTypeType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceCountFiltersTypeDef = TypedDict(
     "ResourceCountFiltersTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "AccountId": str,
         "Region": str,
     },
@@ -1467,22 +1400,20 @@
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
-
 GetComplianceDetailsByResourceRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
@@ -1510,22 +1441,20 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
-
 GetCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetCustomRulePolicyRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
     total=False,
 )
@@ -1572,21 +1501,19 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-
 class MemberAccountStatusTypeDef(
     _RequiredMemberAccountStatusTypeDef, _OptionalMemberAccountStatusTypeDef
 ):
     pass
 
-
 OrganizationResourceDetailedStatusFiltersTypeDef = TypedDict(
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     {
         "AccountId": str,
         "Status": OrganizationResourceDetailedStatusType,
     },
     total=False,
@@ -1606,56 +1533,27 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-
 class OrganizationConformancePackDetailedStatusTypeDef(
     _RequiredOrganizationConformancePackDetailedStatusTypeDef,
     _OptionalOrganizationConformancePackDetailedStatusTypeDef,
 ):
     pass
 
-
 GetOrganizationCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 
-_RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestRequestTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "limit": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class GetResourceConfigHistoryRequestRequestTypeDef(
-    _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
-    _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
-):
-    pass
-
-
 GetResourceEvaluationSummaryRequestRequestTypeDef = TypedDict(
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     {
         "ResourceEvaluationId": str,
     },
 )
 
@@ -1671,19 +1569,17 @@
     "_OptionalResourceDetailsTypeDef",
     {
         "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
     },
     total=False,
 )
 
-
 class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
     pass
 
-
 GetStoredQueryRequestRequestTypeDef = TypedDict(
     "GetStoredQueryRequestRequestTypeDef",
     {
         "QueryName": str,
     },
 )
 
@@ -1700,19 +1596,17 @@
         "QueryArn": str,
         "Description": str,
         "Expression": str,
     },
     total=False,
 )
 
-
 class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
     pass
 
-
 ResourceFiltersTypeDef = TypedDict(
     "ResourceFiltersTypeDef",
     {
         "AccountId": str,
         "ResourceId": str,
         "ResourceName": str,
         "Region": str,
@@ -1734,22 +1628,20 @@
         "limit": int,
         "includeDeletedResources": bool,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "resourceName": str,
         "resourceDeletionTime": datetime,
@@ -1788,21 +1680,19 @@
     "_OptionalStoredQueryMetadataTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class StoredQueryMetadataTypeDef(
     _RequiredStoredQueryMetadataTypeDef, _OptionalStoredQueryMetadataTypeDef
 ):
     pass
 
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1810,22 +1700,20 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -1842,21 +1730,19 @@
     {
         "AwsRegions": Sequence[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
-
 class OrganizationAggregationSourceTypeDef(
     _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
 ):
     pass
 
-
 OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef = TypedDict(
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     {
         "Description": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeNoSNType],
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
@@ -1887,22 +1773,20 @@
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-
 class OrganizationCustomRuleMetadataOutputTypeDef(
     _RequiredOrganizationCustomRuleMetadataOutputTypeDef,
     _OptionalOrganizationCustomRuleMetadataOutputTypeDef,
 ):
     pass
 
-
 _RequiredOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
     "_RequiredOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
 _OptionalOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
@@ -1915,22 +1799,20 @@
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-
 class OrganizationManagedRuleMetadataOutputTypeDef(
     _RequiredOrganizationManagedRuleMetadataOutputTypeDef,
     _OptionalOrganizationManagedRuleMetadataOutputTypeDef,
 ):
     pass
 
-
 _RequiredOrganizationCustomPolicyRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomPolicyRuleMetadataTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
 )
@@ -1946,22 +1828,20 @@
         "TagKeyScope": str,
         "TagValueScope": str,
         "DebugLogDeliveryAccounts": Sequence[str],
     },
     total=False,
 )
 
-
 class OrganizationCustomPolicyRuleMetadataTypeDef(
     _RequiredOrganizationCustomPolicyRuleMetadataTypeDef,
     _OptionalOrganizationCustomPolicyRuleMetadataTypeDef,
 ):
     pass
 
-
 _RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomRuleMetadataTypeDef",
     {
         "LambdaFunctionArn": str,
         "OrganizationConfigRuleTriggerTypes": Sequence[OrganizationConfigRuleTriggerTypeType],
     },
 )
@@ -1975,21 +1855,19 @@
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-
 class OrganizationCustomRuleMetadataTypeDef(
     _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
 ):
     pass
 
-
 _RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationManagedRuleMetadataTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
 _OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
@@ -2002,21 +1880,19 @@
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-
 class OrganizationManagedRuleMetadataTypeDef(
     _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
 ):
     pass
 
-
 _RequiredPutResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceConfigRequestRequestTypeDef",
     {
         "ResourceType": str,
         "SchemaVersionId": str,
         "ResourceId": str,
         "Configuration": str,
@@ -2027,21 +1903,19 @@
     {
         "ResourceName": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class PutResourceConfigRequestRequestTypeDef(
     _RequiredPutResourceConfigRequestRequestTypeDef, _OptionalPutResourceConfigRequestRequestTypeDef
 ):
     pass
 
-
 PutRetentionConfigurationRequestRequestTypeDef = TypedDict(
     "PutRetentionConfigurationRequestRequestTypeDef",
     {
         "RetentionPeriodInDays": int,
     },
 )
 
@@ -2082,23 +1956,14 @@
 StaticValueTypeDef = TypedDict(
     "StaticValueTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-TimeWindowTypeDef = TypedDict(
-    "TimeWindowTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredSelectAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectAggregateResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
         "ConfigurationAggregatorName": str,
     },
 )
@@ -2108,22 +1973,20 @@
         "Limit": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SelectAggregateResourceConfigRequestRequestTypeDef(
     _RequiredSelectAggregateResourceConfigRequestRequestTypeDef,
     _OptionalSelectAggregateResourceConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSelectResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestRequestTypeDef = TypedDict(
@@ -2131,22 +1994,20 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SelectResourceConfigRequestRequestTypeDef(
     _RequiredSelectResourceConfigRequestRequestTypeDef,
     _OptionalSelectResourceConfigRequestRequestTypeDef,
 ):
     pass
 
-
 SourceDetailTypeDef = TypedDict(
     "SourceDetailTypeDef",
     {
         "EventSource": Literal["aws.config"],
         "MessageType": MessageTypeType,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
     },
@@ -2179,14 +2040,17 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AccountAggregationSourceUnionTypeDef = Union[
+    AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef
+]
 AggregateComplianceByConformancePackTypeDef = TypedDict(
     "AggregateComplianceByConformancePackTypeDef",
     {
         "ConformancePackName": str,
         "Compliance": AggregateConformancePackComplianceTypeDef,
         "AccountId": str,
         "AwsRegion": str,
@@ -2215,22 +2079,20 @@
         "Filters": AggregateConformancePackComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef(
     _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -2240,22 +2102,20 @@
         "GroupByKey": AggregateConformancePackComplianceSummaryGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
-
 BatchGetAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifiers": Sequence[AggregateResourceIdentifierTypeDef],
     },
 )
@@ -2411,22 +2271,20 @@
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeRemediationExecutionStatusRequestRequestTypeDef(
     _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef,
     _OptionalDescribeRemediationExecutionStatusRequestRequestTypeDef,
 ):
     pass
 
-
 StartRemediationExecutionRequestRequestTypeDef = TypedDict(
     "StartRemediationExecutionRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
     },
 )
@@ -2471,22 +2329,20 @@
         "Filters": ConfigRuleComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef(
     _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -2496,22 +2352,20 @@
         "GroupByKey": ConfigRuleComplianceSummaryGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeConfigRuleEvaluationStatusResponseTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     {
         "ConfigRulesEvaluationStatus": List[ConfigRuleEvaluationStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2600,22 +2454,20 @@
         "Filters": ConformancePackComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeConformancePackComplianceRequestRequestTypeDef(
     _RequiredDescribeConformancePackComplianceRequestRequestTypeDef,
     _OptionalDescribeConformancePackComplianceRequestRequestTypeDef,
 ):
     pass
 
-
 ListConformancePackComplianceScoresResponseTypeDef = TypedDict(
     "ListConformancePackComplianceScoresResponseTypeDef",
     {
         "NextToken": str,
         "ConformancePackComplianceScores": List[ConformancePackComplianceScoreTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2657,21 +2509,19 @@
         "DeliveryS3KeyPrefix": str,
         "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
         "ExcludedAccounts": List[str],
     },
     total=False,
 )
 
-
 class OrganizationConformancePackTypeDef(
     _RequiredOrganizationConformancePackTypeDef, _OptionalOrganizationConformancePackTypeDef
 ):
     pass
 
-
 _RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
     "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
@@ -2683,22 +2533,20 @@
         "DeliveryS3KeyPrefix": str,
         "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
         "ExcludedAccounts": Sequence[str],
     },
     total=False,
 )
 
-
 class PutOrganizationConformancePackRequestRequestTypeDef(
     _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
     _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredConformancePackDetailTypeDef = TypedDict(
     "_RequiredConformancePackDetailTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackArn": str,
         "ConformancePackId": str,
     },
@@ -2712,21 +2560,19 @@
         "LastUpdateRequestedTime": datetime,
         "CreatedBy": str,
         "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
-
 class ConformancePackDetailTypeDef(
     _RequiredConformancePackDetailTypeDef, _OptionalConformancePackDetailTypeDef
 ):
     pass
 
-
 _RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
     "_RequiredPutConformancePackRequestRequestTypeDef",
     {
         "ConformancePackName": str,
     },
 )
 _OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
@@ -2738,22 +2584,20 @@
         "DeliveryS3KeyPrefix": str,
         "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
         "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
-
 class PutConformancePackRequestRequestTypeDef(
     _RequiredPutConformancePackRequestRequestTypeDef,
     _OptionalPutConformancePackRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef",
     {
         "ConformancePackName": str,
     },
 )
 _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
@@ -2762,22 +2606,20 @@
         "Filters": ConformancePackEvaluationFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetConformancePackComplianceDetailsRequestRequestTypeDef(
     _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef,
     _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeConformancePackComplianceResponseTypeDef = TypedDict(
     "DescribeConformancePackComplianceResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleComplianceList": List[ConformancePackRuleComplianceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2813,55 +2655,29 @@
         "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeRemediationExceptionsRequestRequestTypeDef(
     _RequiredDescribeRemediationExceptionsRequestRequestTypeDef,
     _OptionalDescribeRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
-
 FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
     "FailedDeleteRemediationExceptionsBatchTypeDef",
     {
         "FailureMessage": str,
         "FailedItems": List[RemediationExceptionResourceKeyTypeDef],
     },
     total=False,
 )
 
-_RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
-    {
-        "ConfigRuleName": str,
-        "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
-    },
-)
-_OptionalPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRemediationExceptionsRequestRequestTypeDef",
-    {
-        "Message": str,
-        "ExpirationTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class PutRemediationExceptionsRequestRequestTypeDef(
-    _RequiredPutRemediationExceptionsRequestRequestTypeDef,
-    _OptionalPutRemediationExceptionsRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
@@ -2869,22 +2685,20 @@
     {
         "Filters": ConfigRuleComplianceFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
     _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
@@ -2892,22 +2706,20 @@
     {
         "Filters": AggregateConformancePackComplianceFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
     _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
 ):
     pass
 
-
 DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
     TypedDict(
         "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
         {
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
@@ -2955,22 +2767,20 @@
     {
         "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
 ):
     pass
 
-
 DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -3049,22 +2859,20 @@
     {
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
     _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
 ):
     pass
 
-
 DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -3084,22 +2892,20 @@
     {
         "ComplianceType": ComplianceTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
     _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
     "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
@@ -3107,22 +2913,20 @@
     {
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
 ):
     pass
 
-
 GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "ResourceEvaluationId": str,
@@ -3141,48 +2945,20 @@
     "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
     _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
 ):
     pass
 
-
-_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
-    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
 _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
@@ -3192,44 +2968,40 @@
         "resourceName": str,
         "includeDeletedResources": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
     _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
     TypedDict(
         "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
         {
             "Expression": str,
             "ConfigurationAggregatorName": str,
         },
@@ -3242,44 +3014,40 @@
             "MaxResults": int,
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
-
 class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
     _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
     "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
     _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
 ):
     pass
 
-
 DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef = TypedDict(
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "Filters": DescribeConfigRulesFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3372,51 +3140,143 @@
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
         "OrderingTimestamp": datetime,
         "ResourceEvaluationId": str,
     },
     total=False,
 )
 
-_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEvaluationsRequestRequestTypeDef",
+_RequiredEvaluationTypeDef = TypedDict(
+    "_RequiredEvaluationTypeDef",
     {
-        "ResultToken": str,
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": TimestampTypeDef,
     },
 )
-_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEvaluationsRequestRequestTypeDef",
+_OptionalEvaluationTypeDef = TypedDict(
+    "_OptionalEvaluationTypeDef",
     {
-        "Evaluations": Sequence[Union[EvaluationTypeDef, EvaluationOutputTypeDef]],
-        "TestMode": bool,
+        "Annotation": str,
     },
     total=False,
 )
 
+class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
+    pass
 
-class PutEvaluationsRequestRequestTypeDef(
-    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+_RequiredExternalEvaluationTypeDef = TypedDict(
+    "_RequiredExternalEvaluationTypeDef",
+    {
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": TimestampTypeDef,
+    },
+)
+_OptionalExternalEvaluationTypeDef = TypedDict(
+    "_OptionalExternalEvaluationTypeDef",
+    {
+        "Annotation": str,
+    },
+    total=False,
+)
+
+class ExternalEvaluationTypeDef(
+    _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
 ):
     pass
 
+_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    {
+        "laterTime": TimestampTypeDef,
+        "earlierTime": TimestampTypeDef,
+        "chronologicalOrder": ChronologicalOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
+    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+):
+    pass
 
-ExecutionControlsTypeDef = TypedDict(
-    "ExecutionControlsTypeDef",
+_RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
     {
-        "SsmControls": SsmControlsTypeDef,
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+_OptionalGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestRequestTypeDef",
+    {
+        "laterTime": TimestampTypeDef,
+        "earlierTime": TimestampTypeDef,
+        "chronologicalOrder": ChronologicalOrderType,
+        "limit": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-PutExternalEvaluationRequestRequestTypeDef = TypedDict(
-    "PutExternalEvaluationRequestRequestTypeDef",
+class GetResourceConfigHistoryRequestRequestTypeDef(
+    _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
+    _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
+):
+    pass
+
+_RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
-        "ExternalEvaluation": ExternalEvaluationTypeDef,
+        "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
     },
 )
+_OptionalPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRemediationExceptionsRequestRequestTypeDef",
+    {
+        "Message": str,
+        "ExpirationTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class PutRemediationExceptionsRequestRequestTypeDef(
+    _RequiredPutRemediationExceptionsRequestRequestTypeDef,
+    _OptionalPutRemediationExceptionsRequestRequestTypeDef,
+):
+    pass
+
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ExecutionControlsTypeDef = TypedDict(
+    "ExecutionControlsTypeDef",
+    {
+        "SsmControls": SsmControlsTypeDef,
+    },
+    total=False,
+)
 
 QueryInfoTypeDef = TypedDict(
     "QueryInfoTypeDef",
     {
         "SelectFields": List[FieldInfoTypeDef],
     },
     total=False,
@@ -3435,22 +3295,20 @@
         "GroupByKey": ResourceCountGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetAggregateDiscoveredResourceCountsRequestRequestTypeDef(
     _RequiredGetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     _OptionalGetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
 ):
     pass
 
-
 GetAggregateDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     {
         "TotalDiscoveredResources": int,
         "GroupByKey": str,
         "GroupedResourceCounts": List[GroupedResourceCountTypeDef],
         "NextToken": str,
@@ -3479,22 +3337,20 @@
     {
         "Filters": StatusDetailFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef = TypedDict(
@@ -3503,22 +3359,20 @@
         "Filters": StatusDetailFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
 ):
     pass
 
-
 GetOrganizationConfigRuleDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     {
         "OrganizationConfigRuleDetailedStatus": List[MemberAccountStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3535,22 +3389,20 @@
     {
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef = TypedDict(
@@ -3559,22 +3411,20 @@
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
 ):
     pass
 
-
 GetOrganizationConformancePackDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     {
         "OrganizationConformancePackDetailedStatuses": List[
             OrganizationConformancePackDetailedStatusTypeDef
         ],
         "NextToken": str,
@@ -3609,22 +3459,20 @@
         "EvaluationContext": EvaluationContextTypeDef,
         "EvaluationTimeout": int,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartResourceEvaluationRequestRequestTypeDef(
     _RequiredStartResourceEvaluationRequestRequestTypeDef,
     _OptionalStartResourceEvaluationRequestRequestTypeDef,
 ):
     pass
 
-
 GetStoredQueryResponseTypeDef = TypedDict(
     "GetStoredQueryResponseTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3641,22 +3489,20 @@
     {
         "Filters": ResourceFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceType": ResourceTypeType,
     },
 )
@@ -3666,22 +3512,20 @@
         "Filters": ResourceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAggregateDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "resourceIdentifiers": List[ResourceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3725,77 +3569,50 @@
     "_OptionalPutAggregationAuthorizationRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutAggregationAuthorizationRequestRequestTypeDef(
     _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
     _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
     },
 )
 _OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
     "_OptionalPutStoredQueryRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutStoredQueryRequestRequestTypeDef(
     _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "AccountAggregationSources": Sequence[
-            Union[AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef]
-        ],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutConfigurationAggregatorRequestRequestTypeDef(
-    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
-    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
-):
-    pass
-
-
+OrganizationAggregationSourceUnionTypeDef = Union[
+    OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
+]
 _RequiredOrganizationConfigRuleTypeDef = TypedDict(
     "_RequiredOrganizationConfigRuleTypeDef",
     {
         "OrganizationConfigRuleName": str,
         "OrganizationConfigRuleArn": str,
     },
 )
@@ -3807,21 +3624,25 @@
         "ExcludedAccounts": List[str],
         "LastUpdateTime": datetime,
         "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     },
     total=False,
 )
 
-
 class OrganizationConfigRuleTypeDef(
     _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
 ):
     pass
 
-
+OrganizationCustomRuleMetadataUnionTypeDef = Union[
+    OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
+]
+OrganizationManagedRuleMetadataUnionTypeDef = Union[
+    OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
+]
 _RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
@@ -3831,22 +3652,20 @@
         "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
         "ExcludedAccounts": Sequence[str],
         "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
     },
     total=False,
 )
 
-
 class PutOrganizationConfigRuleRequestRequestTypeDef(
     _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
     _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
 ):
     pass
 
-
 RecordingGroupOutputTypeDef = TypedDict(
     "RecordingGroupOutputTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
         "resourceTypes": List[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
@@ -3893,24 +3712,14 @@
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
-ResourceEvaluationFiltersTypeDef = TypedDict(
-    "ResourceEvaluationFiltersTypeDef",
-    {
-        "EvaluationMode": EvaluationModeType,
-        "TimeWindow": TimeWindowTypeDef,
-        "EvaluationContextIdentifier": str,
-    },
-    total=False,
-)
-
 _RequiredSourceOutputTypeDef = TypedDict(
     "_RequiredSourceOutputTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceOutputTypeDef = TypedDict(
@@ -3919,19 +3728,17 @@
         "SourceIdentifier": str,
         "SourceDetails": List[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
-
 class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
     pass
 
-
 _RequiredSourceTypeDef = TypedDict(
     "_RequiredSourceTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
@@ -3940,18 +3747,38 @@
         "SourceIdentifier": str,
         "SourceDetails": Sequence[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
-
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
 
+_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "AccountAggregationSources": Sequence[AccountAggregationSourceUnionTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutConfigurationAggregatorRequestRequestTypeDef(
+    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
+    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
+):
+    pass
 
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4144,34 +3971,51 @@
     "_OptionalConformancePackEvaluationResultTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
-
 class ConformancePackEvaluationResultTypeDef(
     _RequiredConformancePackEvaluationResultTypeDef, _OptionalConformancePackEvaluationResultTypeDef
 ):
     pass
 
-
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "EvaluationResultIdentifier": EvaluationResultIdentifierTypeDef,
         "ComplianceType": ComplianceTypeType,
         "ResultRecordedTime": datetime,
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
+EvaluationUnionTypeDef = Union[EvaluationTypeDef, EvaluationOutputTypeDef]
+PutExternalEvaluationRequestRequestTypeDef = TypedDict(
+    "PutExternalEvaluationRequestRequestTypeDef",
+    {
+        "ConfigRuleName": str,
+        "ExternalEvaluation": ExternalEvaluationTypeDef,
+    },
+)
+
+ResourceEvaluationFiltersTypeDef = TypedDict(
+    "ResourceEvaluationFiltersTypeDef",
+    {
+        "EvaluationMode": EvaluationModeType,
+        "TimeWindow": TimeWindowTypeDef,
+        "EvaluationContextIdentifier": str,
+    },
+    total=False,
+)
+
 SelectAggregateResourceConfigResponseTypeDef = TypedDict(
     "SelectAggregateResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4246,21 +4090,19 @@
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
     },
     total=False,
 )
 
-
 class RemediationConfigurationOutputTypeDef(
     _RequiredRemediationConfigurationOutputTypeDef, _OptionalRemediationConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredRemediationConfigurationTypeDef = TypedDict(
     "_RequiredRemediationConfigurationTypeDef",
     {
         "ConfigRuleName": str,
         "TargetType": Literal["SSM_DOCUMENT"],
         "TargetId": str,
     },
@@ -4277,40 +4119,19 @@
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
     },
     total=False,
 )
 
-
 class RemediationConfigurationTypeDef(
     _RequiredRemediationConfigurationTypeDef, _OptionalRemediationConfigurationTypeDef
 ):
     pass
 
-
-ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
-    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
-    {
-        "Filters": ResourceEvaluationFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
-    "ListResourceEvaluationsRequestRequestTypeDef",
-    {
-        "Filters": ResourceEvaluationFiltersTypeDef,
-        "Limit": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 _RequiredConfigRuleOutputTypeDef = TypedDict(
     "_RequiredConfigRuleOutputTypeDef",
     {
         "Source": SourceOutputTypeDef,
     },
 )
 _OptionalConfigRuleOutputTypeDef = TypedDict(
@@ -4326,19 +4147,17 @@
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
         "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
     pass
 
-
 _RequiredConfigRuleTypeDef = TypedDict(
     "_RequiredConfigRuleTypeDef",
     {
         "Source": SourceTypeDef,
     },
 )
 _OptionalConfigRuleTypeDef = TypedDict(
@@ -4354,19 +4173,17 @@
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
         "EvaluationModes": Sequence[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class ConfigRuleTypeDef(_RequiredConfigRuleTypeDef, _OptionalConfigRuleTypeDef):
     pass
 
-
 GetAggregateConfigRuleComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     {
         "GroupByKey": str,
         "AggregateComplianceCounts": List[AggregateComplianceCountTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4441,22 +4258,64 @@
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEvaluationsRequestRequestTypeDef",
+    {
+        "ResultToken": str,
+    },
+)
+_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEvaluationsRequestRequestTypeDef",
+    {
+        "Evaluations": Sequence[EvaluationUnionTypeDef],
+        "TestMode": bool,
+    },
+    total=False,
+)
+
+class PutEvaluationsRequestRequestTypeDef(
+    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+):
+    pass
+
+ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
+    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+    {
+        "Filters": ResourceEvaluationFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
+    "ListResourceEvaluationsRequestRequestTypeDef",
+    {
+        "Filters": ResourceEvaluationFiltersTypeDef,
+        "Limit": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
         "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigurationRecorderUnionTypeDef = Union[
+    ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
+]
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
@@ -4473,53 +4332,53 @@
     {
         "FailureMessage": str,
         "FailedItems": List[RemediationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
-PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutRemediationConfigurationsRequestRequestTypeDef",
-    {
-        "RemediationConfigurations": Sequence[
-            Union[RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef]
-        ],
-    },
-)
-
+RemediationConfigurationUnionTypeDef = Union[
+    RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef
+]
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
         "ConfigRules": List[ConfigRuleOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigRuleUnionTypeDef = Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef]
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
     {
         "ConfigRule": ConfigRuleTypeDef,
     },
 )
 _OptionalPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigRuleRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutConfigRuleRequestRequestTypeDef(
     _RequiredPutConfigRuleRequestRequestTypeDef, _OptionalPutConfigRuleRequestRequestTypeDef
 ):
     pass
 
-
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutRemediationConfigurationsRequestRequestTypeDef",
+    {
+        "RemediationConfigurations": Sequence[RemediationConfigurationUnionTypeDef],
+    },
+)
```

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/type_defs.pyi` & `mypy-boto3-config-1.28.16/mypy_boto3_config/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_config.type_defs import AccountAggregationSourceOutputTypeDef
 
-    data: AccountAggregationSourceOutputTypeDef = {...}
+    data: AccountAggregationSourceOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,14 +52,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
@@ -134,19 +135,18 @@
     "RemediationExceptionTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
     "EvaluationContextTypeDef",
     "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
-    "EvaluationTypeDef",
+    "TimestampTypeDef",
     "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
     "SsmControlsTypeDef",
-    "ExternalEvaluationTypeDef",
     "FieldInfoTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
@@ -155,15 +155,14 @@
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     "ResourceCountTypeDef",
     "StatusDetailFiltersTypeDef",
     "MemberAccountStatusTypeDef",
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     "OrganizationConformancePackDetailedStatusTypeDef",
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
-    "GetResourceConfigHistoryRequestRequestTypeDef",
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     "ResourceDetailsTypeDef",
     "GetStoredQueryRequestRequestTypeDef",
     "StoredQueryTypeDef",
     "ResourceFiltersTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
@@ -182,22 +181,22 @@
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
     "ResourceValueTypeDef",
     "StaticValueOutputTypeDef",
     "StaticValueTypeDef",
-    "TimeWindowTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AccountAggregationSourceUnionTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigResponseTypeDef",
@@ -239,15 +238,14 @@
     "PutConformancePackRequestRequestTypeDef",
     "GetConformancePackComplianceDetailsRequestRequestTypeDef",
     "DescribeConformancePackComplianceResponseTypeDef",
     "DescribeConformancePackStatusResponseTypeDef",
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     "DescribeRemediationExceptionsRequestRequestTypeDef",
     "FailedDeleteRemediationExceptionsBatchTypeDef",
-    "PutRemediationExceptionsRequestRequestTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
     "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
     "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
     "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
     "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
@@ -261,15 +259,14 @@
     "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
     "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
     "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     "DescribeConfigRulesRequestRequestTypeDef",
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
@@ -277,17 +274,21 @@
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
     "PutEvaluationsResponseTypeDef",
     "EvaluationResultIdentifierTypeDef",
-    "PutEvaluationsRequestRequestTypeDef",
+    "EvaluationTypeDef",
+    "ExternalEvaluationTypeDef",
+    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    "GetResourceConfigHistoryRequestRequestTypeDef",
+    "PutRemediationExceptionsRequestRequestTypeDef",
+    "TimeWindowTypeDef",
     "ExecutionControlsTypeDef",
-    "PutExternalEvaluationRequestRequestTypeDef",
     "QueryInfoTypeDef",
     "GetAggregateDiscoveredResourceCountsRequestRequestTypeDef",
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     "GetDiscoveredResourceCountsResponseTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
@@ -302,25 +303,27 @@
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
     "PutStoredQueryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "PutConfigurationAggregatorRequestRequestTypeDef",
+    "OrganizationAggregationSourceUnionTypeDef",
     "OrganizationConfigRuleTypeDef",
+    "OrganizationCustomRuleMetadataUnionTypeDef",
+    "OrganizationManagedRuleMetadataUnionTypeDef",
     "PutOrganizationConfigRuleRequestRequestTypeDef",
     "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
     "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
-    "ResourceEvaluationFiltersTypeDef",
     "SourceOutputTypeDef",
     "SourceTypeDef",
+    "PutConfigurationAggregatorRequestRequestTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     "AggregateComplianceByConfigRuleTypeDef",
     "ComplianceByConfigRuleTypeDef",
@@ -335,43 +338,50 @@
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
     "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
+    "EvaluationUnionTypeDef",
+    "PutExternalEvaluationRequestRequestTypeDef",
+    "ResourceEvaluationFiltersTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
     "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
     "RemediationConfigurationOutputTypeDef",
     "RemediationConfigurationTypeDef",
-    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
-    "ListResourceEvaluationsRequestRequestTypeDef",
     "ConfigRuleOutputTypeDef",
     "ConfigRuleTypeDef",
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     "DescribeComplianceByConfigRuleResponseTypeDef",
     "DescribeComplianceByResourceResponseTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     "GetConformancePackComplianceDetailsResponseTypeDef",
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     "GetComplianceDetailsByResourceResponseTypeDef",
+    "PutEvaluationsRequestRequestTypeDef",
+    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+    "ListResourceEvaluationsRequestRequestTypeDef",
     "DescribeConfigurationRecordersResponseTypeDef",
+    "ConfigurationRecorderUnionTypeDef",
     "PutConfigurationRecorderRequestRequestTypeDef",
     "DescribeRemediationConfigurationsResponseTypeDef",
     "FailedRemediationBatchTypeDef",
-    "PutRemediationConfigurationsRequestRequestTypeDef",
+    "RemediationConfigurationUnionTypeDef",
     "DescribeConfigRulesResponseTypeDef",
+    "ConfigRuleUnionTypeDef",
     "PutConfigRuleRequestRequestTypeDef",
     "PutRemediationConfigurationsResponseTypeDef",
+    "PutRemediationConfigurationsRequestRequestTypeDef",
 )
 
 _RequiredAccountAggregationSourceOutputTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceOutputTypeDef",
     {
         "AccountIds": List[str],
     },
@@ -381,19 +391,21 @@
     {
         "AllAwsRegions": bool,
         "AwsRegions": List[str],
     },
     total=False,
 )
 
+
 class AccountAggregationSourceOutputTypeDef(
     _RequiredAccountAggregationSourceOutputTypeDef, _OptionalAccountAggregationSourceOutputTypeDef
 ):
     pass
 
+
 _RequiredAccountAggregationSourceTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 _OptionalAccountAggregationSourceTypeDef = TypedDict(
@@ -401,19 +413,21 @@
     {
         "AllAwsRegions": bool,
         "AwsRegions": Sequence[str],
     },
     total=False,
 )
 
+
 class AccountAggregationSourceTypeDef(
     _RequiredAccountAggregationSourceTypeDef, _OptionalAccountAggregationSourceTypeDef
 ):
     pass
 
+
 AggregateConformancePackComplianceTypeDef = TypedDict(
     "AggregateConformancePackComplianceTypeDef",
     {
         "ComplianceType": ConformancePackComplianceTypeType,
         "CompliantRuleCount": int,
         "NonCompliantRuleCount": int,
         "TotalRuleCount": int,
@@ -463,19 +477,21 @@
     "_OptionalAggregateResourceIdentifierTypeDef",
     {
         "ResourceName": str,
     },
     total=False,
 )
 
+
 class AggregateResourceIdentifierTypeDef(
     _RequiredAggregateResourceIdentifierTypeDef, _OptionalAggregateResourceIdentifierTypeDef
 ):
     pass
 
+
 AggregatedSourceStatusTypeDef = TypedDict(
     "AggregatedSourceStatusTypeDef",
     {
         "SourceId": str,
         "SourceType": AggregatedSourceTypeType,
         "AwsRegion": str,
         "LastUpdateStatus": AggregatedSourceStatusTypeType,
@@ -661,20 +677,22 @@
     {
         "AwsRegions": List[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
+
 class OrganizationAggregationSourceOutputTypeDef(
     _RequiredOrganizationAggregationSourceOutputTypeDef,
     _OptionalOrganizationAggregationSourceOutputTypeDef,
 ):
     pass
 
+
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "resourceName": str,
         "relationshipName": str,
@@ -749,19 +767,21 @@
     "_OptionalTemplateSSMDocumentDetailsTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
+
 class TemplateSSMDocumentDetailsTypeDef(
     _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
 ):
     pass
 
+
 ConformancePackEvaluationFiltersTypeDef = TypedDict(
     "ConformancePackEvaluationFiltersTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "ComplianceType": ConformancePackComplianceTypeType,
         "ResourceType": str,
         "ResourceIds": Sequence[str],
@@ -795,19 +815,21 @@
     {
         "ConformancePackStatusReason": str,
         "LastUpdateCompletedTime": datetime,
     },
     total=False,
 )
 
+
 class ConformancePackStatusDetailTypeDef(
     _RequiredConformancePackStatusDetailTypeDef, _OptionalConformancePackStatusDetailTypeDef
 ):
     pass
 
+
 _RequiredCustomPolicyDetailsTypeDef = TypedDict(
     "_RequiredCustomPolicyDetailsTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
 )
@@ -815,19 +837,21 @@
     "_OptionalCustomPolicyDetailsTypeDef",
     {
         "EnableDebugLogDelivery": bool,
     },
     total=False,
 )
 
+
 class CustomPolicyDetailsTypeDef(
     _RequiredCustomPolicyDetailsTypeDef, _OptionalCustomPolicyDetailsTypeDef
 ):
     pass
 
+
 DeleteAggregationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteAggregationAuthorizationRequestRequestTypeDef",
     {
         "AuthorizedAccountId": str,
         "AuthorizedAwsRegion": str,
     },
 )
@@ -906,20 +930,22 @@
     "_OptionalDeleteRemediationConfigurationRequestRequestTypeDef",
     {
         "ResourceType": str,
     },
     total=False,
 )
 
+
 class DeleteRemediationConfigurationRequestRequestTypeDef(
     _RequiredDeleteRemediationConfigurationRequestRequestTypeDef,
     _OptionalDeleteRemediationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 RemediationExceptionResourceKeyTypeDef = TypedDict(
     "RemediationExceptionResourceKeyTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
     },
     total=False,
@@ -1025,20 +1051,22 @@
         "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeConfigurationAggregatorsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -1120,19 +1148,21 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+
 class OrganizationConfigRuleStatusTypeDef(
     _RequiredOrganizationConfigRuleStatusTypeDef, _OptionalOrganizationConfigRuleStatusTypeDef
 ):
     pass
 
+
 DescribeOrganizationConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1162,20 +1192,22 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+
 class OrganizationConformancePackStatusTypeDef(
     _RequiredOrganizationConformancePackStatusTypeDef,
     _OptionalOrganizationConformancePackStatusTypeDef,
 ):
     pass
 
+
 DescribeOrganizationConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1220,19 +1252,21 @@
     {
         "Message": str,
         "ExpirationTime": datetime,
     },
     total=False,
 )
 
+
 class RemediationExceptionTypeDef(
     _RequiredRemediationExceptionTypeDef, _OptionalRemediationExceptionTypeDef
 ):
     pass
 
+
 DescribeRetentionConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -1267,17 +1301,19 @@
     "_OptionalEvaluationOutputTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
+
 class EvaluationOutputTypeDef(_RequiredEvaluationOutputTypeDef, _OptionalEvaluationOutputTypeDef):
     pass
 
+
 EvaluationResultQualifierTypeDef = TypedDict(
     "EvaluationResultQualifierTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceType": str,
         "ResourceId": str,
         "EvaluationMode": EvaluationModeType,
@@ -1295,37 +1331,20 @@
     "_OptionalEvaluationStatusTypeDef",
     {
         "FailureReason": str,
     },
     total=False,
 )
 
+
 class EvaluationStatusTypeDef(_RequiredEvaluationStatusTypeDef, _OptionalEvaluationStatusTypeDef):
     pass
 
-_RequiredEvaluationTypeDef = TypedDict(
-    "_RequiredEvaluationTypeDef",
-    {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": Union[datetime, str],
-    },
-)
-_OptionalEvaluationTypeDef = TypedDict(
-    "_OptionalEvaluationTypeDef",
-    {
-        "Annotation": str,
-    },
-    total=False,
-)
-
-class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
-    pass
 
+TimestampTypeDef = Union[datetime, str]
 ExclusionByResourceTypesOutputTypeDef = TypedDict(
     "ExclusionByResourceTypesOutputTypeDef",
     {
         "resourceTypes": List[ResourceTypeType],
     },
     total=False,
 )
@@ -1343,36 +1362,14 @@
     {
         "ConcurrentExecutionRatePercentage": int,
         "ErrorPercentage": int,
     },
     total=False,
 )
 
-_RequiredExternalEvaluationTypeDef = TypedDict(
-    "_RequiredExternalEvaluationTypeDef",
-    {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": Union[datetime, str],
-    },
-)
-_OptionalExternalEvaluationTypeDef = TypedDict(
-    "_OptionalExternalEvaluationTypeDef",
-    {
-        "Annotation": str,
-    },
-    total=False,
-)
-
-class ExternalEvaluationTypeDef(
-    _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
-):
-    pass
-
 FieldInfoTypeDef = TypedDict(
     "FieldInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -1392,20 +1389,22 @@
         "ComplianceType": ComplianceTypeType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceCountFiltersTypeDef = TypedDict(
     "ResourceCountFiltersTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "AccountId": str,
         "Region": str,
     },
@@ -1432,20 +1431,22 @@
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
+
 GetComplianceDetailsByResourceRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
@@ -1473,20 +1474,22 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
+
 GetCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetCustomRulePolicyRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
     total=False,
 )
@@ -1533,19 +1536,21 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+
 class MemberAccountStatusTypeDef(
     _RequiredMemberAccountStatusTypeDef, _OptionalMemberAccountStatusTypeDef
 ):
     pass
 
+
 OrganizationResourceDetailedStatusFiltersTypeDef = TypedDict(
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     {
         "AccountId": str,
         "Status": OrganizationResourceDetailedStatusType,
     },
     total=False,
@@ -1565,52 +1570,29 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+
 class OrganizationConformancePackDetailedStatusTypeDef(
     _RequiredOrganizationConformancePackDetailedStatusTypeDef,
     _OptionalOrganizationConformancePackDetailedStatusTypeDef,
 ):
     pass
 
+
 GetOrganizationCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 
-_RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestRequestTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "limit": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class GetResourceConfigHistoryRequestRequestTypeDef(
-    _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
-    _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
-):
-    pass
-
 GetResourceEvaluationSummaryRequestRequestTypeDef = TypedDict(
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     {
         "ResourceEvaluationId": str,
     },
 )
 
@@ -1626,17 +1608,19 @@
     "_OptionalResourceDetailsTypeDef",
     {
         "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
     },
     total=False,
 )
 
+
 class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
     pass
 
+
 GetStoredQueryRequestRequestTypeDef = TypedDict(
     "GetStoredQueryRequestRequestTypeDef",
     {
         "QueryName": str,
     },
 )
 
@@ -1653,17 +1637,19 @@
         "QueryArn": str,
         "Description": str,
         "Expression": str,
     },
     total=False,
 )
 
+
 class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
     pass
 
+
 ResourceFiltersTypeDef = TypedDict(
     "ResourceFiltersTypeDef",
     {
         "AccountId": str,
         "ResourceId": str,
         "ResourceName": str,
         "Region": str,
@@ -1685,20 +1671,22 @@
         "limit": int,
         "includeDeletedResources": bool,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "resourceName": str,
         "resourceDeletionTime": datetime,
@@ -1737,19 +1725,21 @@
     "_OptionalStoredQueryMetadataTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class StoredQueryMetadataTypeDef(
     _RequiredStoredQueryMetadataTypeDef, _OptionalStoredQueryMetadataTypeDef
 ):
     pass
 
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1757,20 +1747,22 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -1787,19 +1779,21 @@
     {
         "AwsRegions": Sequence[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
+
 class OrganizationAggregationSourceTypeDef(
     _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
 ):
     pass
 
+
 OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef = TypedDict(
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     {
         "Description": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeNoSNType],
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
@@ -1830,20 +1824,22 @@
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
+
 class OrganizationCustomRuleMetadataOutputTypeDef(
     _RequiredOrganizationCustomRuleMetadataOutputTypeDef,
     _OptionalOrganizationCustomRuleMetadataOutputTypeDef,
 ):
     pass
 
+
 _RequiredOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
     "_RequiredOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
 _OptionalOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
@@ -1856,20 +1852,22 @@
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
+
 class OrganizationManagedRuleMetadataOutputTypeDef(
     _RequiredOrganizationManagedRuleMetadataOutputTypeDef,
     _OptionalOrganizationManagedRuleMetadataOutputTypeDef,
 ):
     pass
 
+
 _RequiredOrganizationCustomPolicyRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomPolicyRuleMetadataTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
 )
@@ -1885,20 +1883,22 @@
         "TagKeyScope": str,
         "TagValueScope": str,
         "DebugLogDeliveryAccounts": Sequence[str],
     },
     total=False,
 )
 
+
 class OrganizationCustomPolicyRuleMetadataTypeDef(
     _RequiredOrganizationCustomPolicyRuleMetadataTypeDef,
     _OptionalOrganizationCustomPolicyRuleMetadataTypeDef,
 ):
     pass
 
+
 _RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomRuleMetadataTypeDef",
     {
         "LambdaFunctionArn": str,
         "OrganizationConfigRuleTriggerTypes": Sequence[OrganizationConfigRuleTriggerTypeType],
     },
 )
@@ -1912,19 +1912,21 @@
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
+
 class OrganizationCustomRuleMetadataTypeDef(
     _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
 ):
     pass
 
+
 _RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationManagedRuleMetadataTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
 _OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
@@ -1937,19 +1939,21 @@
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
+
 class OrganizationManagedRuleMetadataTypeDef(
     _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
 ):
     pass
 
+
 _RequiredPutResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceConfigRequestRequestTypeDef",
     {
         "ResourceType": str,
         "SchemaVersionId": str,
         "ResourceId": str,
         "Configuration": str,
@@ -1960,19 +1964,21 @@
     {
         "ResourceName": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class PutResourceConfigRequestRequestTypeDef(
     _RequiredPutResourceConfigRequestRequestTypeDef, _OptionalPutResourceConfigRequestRequestTypeDef
 ):
     pass
 
+
 PutRetentionConfigurationRequestRequestTypeDef = TypedDict(
     "PutRetentionConfigurationRequestRequestTypeDef",
     {
         "RetentionPeriodInDays": int,
     },
 )
 
@@ -2013,23 +2019,14 @@
 StaticValueTypeDef = TypedDict(
     "StaticValueTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-TimeWindowTypeDef = TypedDict(
-    "TimeWindowTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredSelectAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectAggregateResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
         "ConfigurationAggregatorName": str,
     },
 )
@@ -2039,20 +2036,22 @@
         "Limit": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SelectAggregateResourceConfigRequestRequestTypeDef(
     _RequiredSelectAggregateResourceConfigRequestRequestTypeDef,
     _OptionalSelectAggregateResourceConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSelectResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestRequestTypeDef = TypedDict(
@@ -2060,20 +2059,22 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SelectResourceConfigRequestRequestTypeDef(
     _RequiredSelectResourceConfigRequestRequestTypeDef,
     _OptionalSelectResourceConfigRequestRequestTypeDef,
 ):
     pass
 
+
 SourceDetailTypeDef = TypedDict(
     "SourceDetailTypeDef",
     {
         "EventSource": Literal["aws.config"],
         "MessageType": MessageTypeType,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
     },
@@ -2106,14 +2107,17 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AccountAggregationSourceUnionTypeDef = Union[
+    AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef
+]
 AggregateComplianceByConformancePackTypeDef = TypedDict(
     "AggregateComplianceByConformancePackTypeDef",
     {
         "ConformancePackName": str,
         "Compliance": AggregateConformancePackComplianceTypeDef,
         "AccountId": str,
         "AwsRegion": str,
@@ -2142,20 +2146,22 @@
         "Filters": AggregateConformancePackComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef(
     _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -2165,20 +2171,22 @@
         "GroupByKey": AggregateConformancePackComplianceSummaryGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
+
 BatchGetAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifiers": Sequence[AggregateResourceIdentifierTypeDef],
     },
 )
@@ -2334,20 +2342,22 @@
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeRemediationExecutionStatusRequestRequestTypeDef(
     _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef,
     _OptionalDescribeRemediationExecutionStatusRequestRequestTypeDef,
 ):
     pass
 
+
 StartRemediationExecutionRequestRequestTypeDef = TypedDict(
     "StartRemediationExecutionRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
     },
 )
@@ -2392,20 +2402,22 @@
         "Filters": ConfigRuleComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef(
     _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -2415,20 +2427,22 @@
         "GroupByKey": ConfigRuleComplianceSummaryGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeConfigRuleEvaluationStatusResponseTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     {
         "ConfigRulesEvaluationStatus": List[ConfigRuleEvaluationStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2517,20 +2531,22 @@
         "Filters": ConformancePackComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeConformancePackComplianceRequestRequestTypeDef(
     _RequiredDescribeConformancePackComplianceRequestRequestTypeDef,
     _OptionalDescribeConformancePackComplianceRequestRequestTypeDef,
 ):
     pass
 
+
 ListConformancePackComplianceScoresResponseTypeDef = TypedDict(
     "ListConformancePackComplianceScoresResponseTypeDef",
     {
         "NextToken": str,
         "ConformancePackComplianceScores": List[ConformancePackComplianceScoreTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2572,19 +2588,21 @@
         "DeliveryS3KeyPrefix": str,
         "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
         "ExcludedAccounts": List[str],
     },
     total=False,
 )
 
+
 class OrganizationConformancePackTypeDef(
     _RequiredOrganizationConformancePackTypeDef, _OptionalOrganizationConformancePackTypeDef
 ):
     pass
 
+
 _RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
     "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
@@ -2596,20 +2614,22 @@
         "DeliveryS3KeyPrefix": str,
         "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
         "ExcludedAccounts": Sequence[str],
     },
     total=False,
 )
 
+
 class PutOrganizationConformancePackRequestRequestTypeDef(
     _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
     _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredConformancePackDetailTypeDef = TypedDict(
     "_RequiredConformancePackDetailTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackArn": str,
         "ConformancePackId": str,
     },
@@ -2623,19 +2643,21 @@
         "LastUpdateRequestedTime": datetime,
         "CreatedBy": str,
         "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
+
 class ConformancePackDetailTypeDef(
     _RequiredConformancePackDetailTypeDef, _OptionalConformancePackDetailTypeDef
 ):
     pass
 
+
 _RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
     "_RequiredPutConformancePackRequestRequestTypeDef",
     {
         "ConformancePackName": str,
     },
 )
 _OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
@@ -2647,20 +2669,22 @@
         "DeliveryS3KeyPrefix": str,
         "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
         "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
+
 class PutConformancePackRequestRequestTypeDef(
     _RequiredPutConformancePackRequestRequestTypeDef,
     _OptionalPutConformancePackRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef",
     {
         "ConformancePackName": str,
     },
 )
 _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
@@ -2669,20 +2693,22 @@
         "Filters": ConformancePackEvaluationFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetConformancePackComplianceDetailsRequestRequestTypeDef(
     _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef,
     _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeConformancePackComplianceResponseTypeDef = TypedDict(
     "DescribeConformancePackComplianceResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleComplianceList": List[ConformancePackRuleComplianceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2718,51 +2744,31 @@
         "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeRemediationExceptionsRequestRequestTypeDef(
     _RequiredDescribeRemediationExceptionsRequestRequestTypeDef,
     _OptionalDescribeRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
+
 FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
     "FailedDeleteRemediationExceptionsBatchTypeDef",
     {
         "FailureMessage": str,
         "FailedItems": List[RemediationExceptionResourceKeyTypeDef],
     },
     total=False,
 )
 
-_RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
-    {
-        "ConfigRuleName": str,
-        "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
-    },
-)
-_OptionalPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRemediationExceptionsRequestRequestTypeDef",
-    {
-        "Message": str,
-        "ExpirationTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class PutRemediationExceptionsRequestRequestTypeDef(
-    _RequiredPutRemediationExceptionsRequestRequestTypeDef,
-    _OptionalPutRemediationExceptionsRequestRequestTypeDef,
-):
-    pass
-
 _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
@@ -2770,20 +2776,22 @@
     {
         "Filters": ConfigRuleComplianceFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
     _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
@@ -2791,20 +2799,22 @@
     {
         "Filters": AggregateConformancePackComplianceFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
     _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
 ):
     pass
 
+
 DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
     TypedDict(
         "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
         {
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
@@ -2852,20 +2862,22 @@
     {
         "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
 ):
     pass
 
+
 DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2944,20 +2956,22 @@
     {
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
     _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
 ):
     pass
 
+
 DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2977,20 +2991,22 @@
     {
         "ComplianceType": ComplianceTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
     _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
     "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
@@ -2998,20 +3014,22 @@
     {
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
 ):
     pass
 
+
 GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "ResourceEvaluationId": str,
@@ -3030,43 +3048,21 @@
     "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
     _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
 ):
     pass
 
-_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
-    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-):
-    pass
 
 _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
@@ -3077,40 +3073,44 @@
         "resourceName": str,
         "includeDeletedResources": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
     _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
     TypedDict(
         "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
         {
             "Expression": str,
             "ConfigurationAggregatorName": str,
         },
@@ -3123,40 +3123,44 @@
             "MaxResults": int,
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
+
 class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
     _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
     "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
     _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
 ):
     pass
 
+
 DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef = TypedDict(
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "Filters": DescribeConfigRulesFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3249,49 +3253,153 @@
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
         "OrderingTimestamp": datetime,
         "ResourceEvaluationId": str,
     },
     total=False,
 )
 
-_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEvaluationsRequestRequestTypeDef",
+_RequiredEvaluationTypeDef = TypedDict(
+    "_RequiredEvaluationTypeDef",
     {
-        "ResultToken": str,
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": TimestampTypeDef,
     },
 )
-_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEvaluationsRequestRequestTypeDef",
+_OptionalEvaluationTypeDef = TypedDict(
+    "_OptionalEvaluationTypeDef",
     {
-        "Evaluations": Sequence[Union[EvaluationTypeDef, EvaluationOutputTypeDef]],
-        "TestMode": bool,
+        "Annotation": str,
     },
     total=False,
 )
 
-class PutEvaluationsRequestRequestTypeDef(
-    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+
+class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
+    pass
+
+
+_RequiredExternalEvaluationTypeDef = TypedDict(
+    "_RequiredExternalEvaluationTypeDef",
+    {
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": TimestampTypeDef,
+    },
+)
+_OptionalExternalEvaluationTypeDef = TypedDict(
+    "_OptionalExternalEvaluationTypeDef",
+    {
+        "Annotation": str,
+    },
+    total=False,
+)
+
+
+class ExternalEvaluationTypeDef(
+    _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
 ):
     pass
 
-ExecutionControlsTypeDef = TypedDict(
-    "ExecutionControlsTypeDef",
+
+_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     {
-        "SsmControls": SsmControlsTypeDef,
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    {
+        "laterTime": TimestampTypeDef,
+        "earlierTime": TimestampTypeDef,
+        "chronologicalOrder": ChronologicalOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-PutExternalEvaluationRequestRequestTypeDef = TypedDict(
-    "PutExternalEvaluationRequestRequestTypeDef",
+
+class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
+    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+_OptionalGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestRequestTypeDef",
+    {
+        "laterTime": TimestampTypeDef,
+        "earlierTime": TimestampTypeDef,
+        "chronologicalOrder": ChronologicalOrderType,
+        "limit": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class GetResourceConfigHistoryRequestRequestTypeDef(
+    _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
+    _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
-        "ExternalEvaluation": ExternalEvaluationTypeDef,
+        "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
     },
 )
+_OptionalPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRemediationExceptionsRequestRequestTypeDef",
+    {
+        "Message": str,
+        "ExpirationTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class PutRemediationExceptionsRequestRequestTypeDef(
+    _RequiredPutRemediationExceptionsRequestRequestTypeDef,
+    _OptionalPutRemediationExceptionsRequestRequestTypeDef,
+):
+    pass
+
+
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ExecutionControlsTypeDef = TypedDict(
+    "ExecutionControlsTypeDef",
+    {
+        "SsmControls": SsmControlsTypeDef,
+    },
+    total=False,
+)
 
 QueryInfoTypeDef = TypedDict(
     "QueryInfoTypeDef",
     {
         "SelectFields": List[FieldInfoTypeDef],
     },
     total=False,
@@ -3310,20 +3418,22 @@
         "GroupByKey": ResourceCountGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetAggregateDiscoveredResourceCountsRequestRequestTypeDef(
     _RequiredGetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     _OptionalGetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
 ):
     pass
 
+
 GetAggregateDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     {
         "TotalDiscoveredResources": int,
         "GroupByKey": str,
         "GroupedResourceCounts": List[GroupedResourceCountTypeDef],
         "NextToken": str,
@@ -3352,20 +3462,22 @@
     {
         "Filters": StatusDetailFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef = TypedDict(
@@ -3374,20 +3486,22 @@
         "Filters": StatusDetailFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
 ):
     pass
 
+
 GetOrganizationConfigRuleDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     {
         "OrganizationConfigRuleDetailedStatus": List[MemberAccountStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3404,20 +3518,22 @@
     {
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef = TypedDict(
@@ -3426,20 +3542,22 @@
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
 ):
     pass
 
+
 GetOrganizationConformancePackDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     {
         "OrganizationConformancePackDetailedStatuses": List[
             OrganizationConformancePackDetailedStatusTypeDef
         ],
         "NextToken": str,
@@ -3474,20 +3592,22 @@
         "EvaluationContext": EvaluationContextTypeDef,
         "EvaluationTimeout": int,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartResourceEvaluationRequestRequestTypeDef(
     _RequiredStartResourceEvaluationRequestRequestTypeDef,
     _OptionalStartResourceEvaluationRequestRequestTypeDef,
 ):
     pass
 
+
 GetStoredQueryResponseTypeDef = TypedDict(
     "GetStoredQueryResponseTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3504,20 +3624,22 @@
     {
         "Filters": ResourceFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceType": ResourceTypeType,
     },
 )
@@ -3527,20 +3649,22 @@
         "Filters": ResourceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAggregateDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "resourceIdentifiers": List[ResourceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3584,71 +3708,54 @@
     "_OptionalPutAggregationAuthorizationRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutAggregationAuthorizationRequestRequestTypeDef(
     _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
     _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
     },
 )
 _OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
     "_OptionalPutStoredQueryRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutStoredQueryRequestRequestTypeDef(
     _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "AccountAggregationSources": Sequence[
-            Union[AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef]
-        ],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutConfigurationAggregatorRequestRequestTypeDef(
-    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
-    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
-):
-    pass
-
+OrganizationAggregationSourceUnionTypeDef = Union[
+    OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
+]
 _RequiredOrganizationConfigRuleTypeDef = TypedDict(
     "_RequiredOrganizationConfigRuleTypeDef",
     {
         "OrganizationConfigRuleName": str,
         "OrganizationConfigRuleArn": str,
     },
 )
@@ -3660,19 +3767,27 @@
         "ExcludedAccounts": List[str],
         "LastUpdateTime": datetime,
         "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     },
     total=False,
 )
 
+
 class OrganizationConfigRuleTypeDef(
     _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
 ):
     pass
 
+
+OrganizationCustomRuleMetadataUnionTypeDef = Union[
+    OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
+]
+OrganizationManagedRuleMetadataUnionTypeDef = Union[
+    OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
+]
 _RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
@@ -3682,20 +3797,22 @@
         "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
         "ExcludedAccounts": Sequence[str],
         "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
     },
     total=False,
 )
 
+
 class PutOrganizationConfigRuleRequestRequestTypeDef(
     _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
     _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
 ):
     pass
 
+
 RecordingGroupOutputTypeDef = TypedDict(
     "RecordingGroupOutputTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
         "resourceTypes": List[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
@@ -3742,24 +3859,14 @@
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
-ResourceEvaluationFiltersTypeDef = TypedDict(
-    "ResourceEvaluationFiltersTypeDef",
-    {
-        "EvaluationMode": EvaluationModeType,
-        "TimeWindow": TimeWindowTypeDef,
-        "EvaluationContextIdentifier": str,
-    },
-    total=False,
-)
-
 _RequiredSourceOutputTypeDef = TypedDict(
     "_RequiredSourceOutputTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceOutputTypeDef = TypedDict(
@@ -3768,17 +3875,19 @@
         "SourceIdentifier": str,
         "SourceDetails": List[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
+
 class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
     pass
 
+
 _RequiredSourceTypeDef = TypedDict(
     "_RequiredSourceTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
@@ -3787,17 +3896,43 @@
         "SourceIdentifier": str,
         "SourceDetails": Sequence[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
+
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
 
+
+_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "AccountAggregationSources": Sequence[AccountAggregationSourceUnionTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutConfigurationAggregatorRequestRequestTypeDef(
+    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
+    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3989,32 +4124,53 @@
     "_OptionalConformancePackEvaluationResultTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
+
 class ConformancePackEvaluationResultTypeDef(
     _RequiredConformancePackEvaluationResultTypeDef, _OptionalConformancePackEvaluationResultTypeDef
 ):
     pass
 
+
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "EvaluationResultIdentifier": EvaluationResultIdentifierTypeDef,
         "ComplianceType": ComplianceTypeType,
         "ResultRecordedTime": datetime,
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
+EvaluationUnionTypeDef = Union[EvaluationTypeDef, EvaluationOutputTypeDef]
+PutExternalEvaluationRequestRequestTypeDef = TypedDict(
+    "PutExternalEvaluationRequestRequestTypeDef",
+    {
+        "ConfigRuleName": str,
+        "ExternalEvaluation": ExternalEvaluationTypeDef,
+    },
+)
+
+ResourceEvaluationFiltersTypeDef = TypedDict(
+    "ResourceEvaluationFiltersTypeDef",
+    {
+        "EvaluationMode": EvaluationModeType,
+        "TimeWindow": TimeWindowTypeDef,
+        "EvaluationContextIdentifier": str,
+    },
+    total=False,
+)
+
 SelectAggregateResourceConfigResponseTypeDef = TypedDict(
     "SelectAggregateResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4089,19 +4245,21 @@
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
     },
     total=False,
 )
 
+
 class RemediationConfigurationOutputTypeDef(
     _RequiredRemediationConfigurationOutputTypeDef, _OptionalRemediationConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredRemediationConfigurationTypeDef = TypedDict(
     "_RequiredRemediationConfigurationTypeDef",
     {
         "ConfigRuleName": str,
         "TargetType": Literal["SSM_DOCUMENT"],
         "TargetId": str,
     },
@@ -4118,37 +4276,20 @@
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
     },
     total=False,
 )
 
+
 class RemediationConfigurationTypeDef(
     _RequiredRemediationConfigurationTypeDef, _OptionalRemediationConfigurationTypeDef
 ):
     pass
 
-ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
-    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
-    {
-        "Filters": ResourceEvaluationFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
-    "ListResourceEvaluationsRequestRequestTypeDef",
-    {
-        "Filters": ResourceEvaluationFiltersTypeDef,
-        "Limit": int,
-        "NextToken": str,
-    },
-    total=False,
-)
 
 _RequiredConfigRuleOutputTypeDef = TypedDict(
     "_RequiredConfigRuleOutputTypeDef",
     {
         "Source": SourceOutputTypeDef,
     },
 )
@@ -4165,17 +4306,19 @@
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
         "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
     pass
 
+
 _RequiredConfigRuleTypeDef = TypedDict(
     "_RequiredConfigRuleTypeDef",
     {
         "Source": SourceTypeDef,
     },
 )
 _OptionalConfigRuleTypeDef = TypedDict(
@@ -4191,17 +4334,19 @@
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
         "EvaluationModes": Sequence[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class ConfigRuleTypeDef(_RequiredConfigRuleTypeDef, _OptionalConfigRuleTypeDef):
     pass
 
+
 GetAggregateConfigRuleComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     {
         "GroupByKey": str,
         "AggregateComplianceCounts": List[AggregateComplianceCountTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4276,22 +4421,66 @@
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEvaluationsRequestRequestTypeDef",
+    {
+        "ResultToken": str,
+    },
+)
+_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEvaluationsRequestRequestTypeDef",
+    {
+        "Evaluations": Sequence[EvaluationUnionTypeDef],
+        "TestMode": bool,
+    },
+    total=False,
+)
+
+
+class PutEvaluationsRequestRequestTypeDef(
+    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+):
+    pass
+
+
+ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
+    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+    {
+        "Filters": ResourceEvaluationFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
+    "ListResourceEvaluationsRequestRequestTypeDef",
+    {
+        "Filters": ResourceEvaluationFiltersTypeDef,
+        "Limit": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
         "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigurationRecorderUnionTypeDef = Union[
+    ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
+]
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
@@ -4308,51 +4497,55 @@
     {
         "FailureMessage": str,
         "FailedItems": List[RemediationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
-PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutRemediationConfigurationsRequestRequestTypeDef",
-    {
-        "RemediationConfigurations": Sequence[
-            Union[RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef]
-        ],
-    },
-)
-
+RemediationConfigurationUnionTypeDef = Union[
+    RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef
+]
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
         "ConfigRules": List[ConfigRuleOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigRuleUnionTypeDef = Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef]
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
     {
         "ConfigRule": ConfigRuleTypeDef,
     },
 )
 _OptionalPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigRuleRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutConfigRuleRequestRequestTypeDef(
     _RequiredPutConfigRuleRequestRequestTypeDef, _OptionalPutConfigRuleRequestRequestTypeDef
 ):
     pass
 
+
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutRemediationConfigurationsRequestRequestTypeDef",
+    {
+        "RemediationConfigurations": Sequence[RemediationConfigurationUnionTypeDef],
+    },
+)
```

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/PKG-INFO` & `mypy-boto3-config-1.28.16/mypy_boto3_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ConfigService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 config type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 config type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
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
@@ -497,20 +497,20 @@
 )
 
 
 def check_value(value: AggregateConformancePackComplianceSummaryGroupKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_config.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_config.type_defs import (
     AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
@@ -587,19 +587,18 @@
     RemediationExceptionTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
     EvaluationContextTypeDef,
     EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
-    EvaluationTypeDef,
+    TimestampTypeDef,
     ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
     SsmControlsTypeDef,
-    ExternalEvaluationTypeDef,
     FieldInfoTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     GetComplianceDetailsByResourceRequestRequestTypeDef,
     GetComplianceSummaryByResourceTypeRequestRequestTypeDef,
@@ -608,15 +607,14 @@
     GetDiscoveredResourceCountsRequestRequestTypeDef,
     ResourceCountTypeDef,
     StatusDetailFiltersTypeDef,
     MemberAccountStatusTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
-    GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
     ResourceDetailsTypeDef,
     GetStoredQueryRequestRequestTypeDef,
     StoredQueryTypeDef,
     ResourceFiltersTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
@@ -635,22 +633,22 @@
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
     ResourceValueTypeDef,
     StaticValueOutputTypeDef,
     StaticValueTypeDef,
-    TimeWindowTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
@@ -692,15 +690,14 @@
     PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
     FailedDeleteRemediationExceptionsBatchTypeDef,
-    PutRemediationExceptionsRequestRequestTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
     DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
     DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
     DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
     DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
@@ -714,15 +711,14 @@
     DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
     DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
     GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
@@ -730,17 +726,21 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     EvaluationResultIdentifierTypeDef,
-    PutEvaluationsRequestRequestTypeDef,
+    EvaluationTypeDef,
+    ExternalEvaluationTypeDef,
+    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    GetResourceConfigHistoryRequestRequestTypeDef,
+    PutRemediationExceptionsRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ExecutionControlsTypeDef,
-    PutExternalEvaluationRequestRequestTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
@@ -755,25 +755,27 @@
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
     PutStoredQueryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    PutConfigurationAggregatorRequestRequestTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationConfigRuleTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     PutOrganizationConfigRuleRequestRequestTypeDef,
     RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
     RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
-    ResourceEvaluationFiltersTypeDef,
     SourceOutputTypeDef,
     SourceTypeDef,
+    PutConfigurationAggregatorRequestRequestTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
     GetComplianceSummaryByConfigRuleResponseTypeDef,
     AggregateComplianceByConfigRuleTypeDef,
     ComplianceByConfigRuleTypeDef,
@@ -788,47 +790,54 @@
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
+    EvaluationUnionTypeDef,
+    PutExternalEvaluationRequestRequestTypeDef,
+    ResourceEvaluationFiltersTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
     ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
-    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
-    ListResourceEvaluationsRequestRequestTypeDef,
     ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetComplianceSummaryByResourceTypeResponseTypeDef,
     DescribeAggregateComplianceByConfigRulesResponseTypeDef,
     DescribeComplianceByConfigRuleResponseTypeDef,
     DescribeComplianceByResourceResponseTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetConformancePackComplianceDetailsResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
     GetComplianceDetailsByResourceResponseTypeDef,
+    PutEvaluationsRequestRequestTypeDef,
+    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
+    ListResourceEvaluationsRequestRequestTypeDef,
     DescribeConfigurationRecordersResponseTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     PutConfigurationRecorderRequestRequestTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     FailedRemediationBatchTypeDef,
-    PutRemediationConfigurationsRequestRequestTypeDef,
+    RemediationConfigurationUnionTypeDef,
     DescribeConfigRulesResponseTypeDef,
+    ConfigRuleUnionTypeDef,
     PutConfigRuleRequestRequestTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
+    PutRemediationConfigurationsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountAggregationSourceOutputTypeDef:
+def get_value() -> AccountAggregationSourceOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/SOURCES.txt` & `mypy-boto3-config-1.28.16/mypy_boto3_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15.post1/setup.py` & `mypy-boto3-config-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-config",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.ConfigService 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 config type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 config type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_config": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

