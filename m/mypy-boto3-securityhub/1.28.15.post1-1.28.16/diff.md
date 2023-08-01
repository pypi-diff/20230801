# Comparing `tmp/mypy-boto3-securityhub-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-securityhub-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securityhub-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:09 2023, max compression
+gzip compressed data, was "mypy-boto3-securityhub-1.28.16.tar", last modified: Tue Aug  1 11:37:49 2023, max compression
```

## Comparing `mypy-boto3-securityhub-1.28.15.post1.tar` & `mypy-boto3-securityhub-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:09.333392 mypy-boto3-securityhub-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    61545 2023-07-29 10:04:09.329392 mypy-boto3-securityhub-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    60036 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:09.325392 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52477 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52388 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18429 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   402830 2023-07-29 09:59:13.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   402757 2023-07-29 09:59:03.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:09.329392 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    61545 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:09.333392 mypy-boto3-securityhub-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:48.988737 mypy-boto3-securityhub-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:32:27.000000 mypy-boto3-securityhub-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    61722 2023-08-01 11:37:48.984737 mypy-boto3-securityhub-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60222 2023-08-01 11:32:27.000000 mypy-boto3-securityhub-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:48.984737 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-08-01 11:32:27.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-08-01 11:32:27.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 11:32:27.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51904 2023-08-01 11:32:28.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51815 2023-08-01 11:32:28.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-08-01 11:32:28.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-08-01 11:32:28.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-08-01 11:32:28.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-08-01 11:32:28.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:32:27.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   403431 2023-08-01 11:32:43.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   403358 2023-08-01 11:32:38.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:32:27.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:48.984737 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    61722 2023-08-01 11:37:48.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-01 11:37:48.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:48.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:48.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:48.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:37:48.000000 mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:48.988737 mypy-boto3-securityhub-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 11:32:27.000000 mypy-boto3-securityhub-1.28.16/setup.py
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/LICENSE` & `mypy-boto3-securityhub-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15.post1/PKG-INFO` & `mypy-boto3-securityhub-1.28.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SecurityHub 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 securityhub type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
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
@@ -406,20 +406,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_securityhub.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_securityhub.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccountDetailsTypeDef,
     ActionLocalIpDetailsTypeDef,
@@ -823,14 +823,15 @@
     FindingHistoryUpdateTypeDef,
     FindingProviderSeverityTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
+    TimestampTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
     GetInsightsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
@@ -1016,15 +1017,14 @@
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
     AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
-    GetFindingHistoryRequestRequestTypeDef,
     AwsSnsTopicDetailsOutputTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
     AwsWafRateBasedRuleDetailsOutputTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
@@ -1080,15 +1080,14 @@
     InviteMembersResponseTypeDef,
     DateFilterTypeDef,
     DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
     DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
-    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
     GetInsightsRequestGetInsightsPaginateTypeDef,
     ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListMembersRequestListMembersPaginateTypeDef,
     ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
@@ -1100,14 +1099,16 @@
     ListFindingAggregatorsResponseTypeDef,
     FindingHistoryRecordTypeDef,
     FindingProviderFieldsOutputTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
+    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    GetFindingHistoryRequestRequestTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
     NetworkPathComponentDetailsOutputTypeDef,
     NetworkPathComponentDetailsTypeDef,
@@ -1241,14 +1242,15 @@
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionOutputTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionOutputTypeDef,
     PortProbeActionTypeDef,
+    AutomationRulesActionUnionTypeDef,
     AwsAthenaWorkGroupDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsOutputTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
@@ -1274,17 +1276,18 @@
     AwsStepFunctionStateMachineDetailsOutputTypeDef,
     AwsStepFunctionStateMachineDetailsTypeDef,
     AwsWafv2RulesActionDetailsOutputTypeDef,
     AwsWafv2WebAclActionDetailsOutputTypeDef,
     AwsWafv2RulesActionDetailsTypeDef,
     AwsWafv2WebAclActionDetailsTypeDef,
     AutomationRulesConfigTypeDef,
-    CreateAutomationRuleRequestRequestTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
     InsightTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentOutputTypeDef,
     NetworkPathComponentTypeDef,
@@ -1296,14 +1299,15 @@
     RuleGroupSourceStatelessRulesDetailsTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef,
     RuleGroupSourceCustomActionsDetailsOutputTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
+    CreateAutomationRuleRequestRequestTypeDef,
     AwsBackupBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
     AwsCloudFrontDistributionDetailsOutputTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
     AwsGuardDutyDetectorDetailsOutputTypeDef,
     AwsGuardDutyDetectorDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef,
@@ -1346,19 +1350,20 @@
     ResourceDetailsOutputTypeDef,
     ResourceDetailsTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     AwsSecurityFindingOutputTypeDef,
     AwsSecurityFindingTypeDef,
     GetFindingsResponseTypeDef,
+    AwsSecurityFindingUnionTypeDef,
     BatchImportFindingsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/README.md` & `mypy-boto3-securityhub-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
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
@@ -374,20 +374,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_securityhub.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_securityhub.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccountDetailsTypeDef,
     ActionLocalIpDetailsTypeDef,
@@ -791,14 +791,15 @@
     FindingHistoryUpdateTypeDef,
     FindingProviderSeverityTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
+    TimestampTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
     GetInsightsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
@@ -984,15 +985,14 @@
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
     AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
-    GetFindingHistoryRequestRequestTypeDef,
     AwsSnsTopicDetailsOutputTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
     AwsWafRateBasedRuleDetailsOutputTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
@@ -1048,15 +1048,14 @@
     InviteMembersResponseTypeDef,
     DateFilterTypeDef,
     DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
     DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
-    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
     GetInsightsRequestGetInsightsPaginateTypeDef,
     ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListMembersRequestListMembersPaginateTypeDef,
     ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
@@ -1068,14 +1067,16 @@
     ListFindingAggregatorsResponseTypeDef,
     FindingHistoryRecordTypeDef,
     FindingProviderFieldsOutputTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
+    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    GetFindingHistoryRequestRequestTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
     NetworkPathComponentDetailsOutputTypeDef,
     NetworkPathComponentDetailsTypeDef,
@@ -1209,14 +1210,15 @@
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionOutputTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionOutputTypeDef,
     PortProbeActionTypeDef,
+    AutomationRulesActionUnionTypeDef,
     AwsAthenaWorkGroupDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsOutputTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
@@ -1242,17 +1244,18 @@
     AwsStepFunctionStateMachineDetailsOutputTypeDef,
     AwsStepFunctionStateMachineDetailsTypeDef,
     AwsWafv2RulesActionDetailsOutputTypeDef,
     AwsWafv2WebAclActionDetailsOutputTypeDef,
     AwsWafv2RulesActionDetailsTypeDef,
     AwsWafv2WebAclActionDetailsTypeDef,
     AutomationRulesConfigTypeDef,
-    CreateAutomationRuleRequestRequestTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
     InsightTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentOutputTypeDef,
     NetworkPathComponentTypeDef,
@@ -1264,14 +1267,15 @@
     RuleGroupSourceStatelessRulesDetailsTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef,
     RuleGroupSourceCustomActionsDetailsOutputTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
+    CreateAutomationRuleRequestRequestTypeDef,
     AwsBackupBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
     AwsCloudFrontDistributionDetailsOutputTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
     AwsGuardDutyDetectorDetailsOutputTypeDef,
     AwsGuardDutyDetectorDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef,
@@ -1314,19 +1318,20 @@
     ResourceDetailsOutputTypeDef,
     ResourceDetailsTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     AwsSecurityFindingOutputTypeDef,
     AwsSecurityFindingTypeDef,
     GetFindingsResponseTypeDef,
+    AwsSecurityFindingUnionTypeDef,
     BatchImportFindingsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__init__.py` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__init__.pyi` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__main__.py` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityHub 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.SecurityHub 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\nOther"
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

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/client.py` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_securityhub.client import SecurityHubClient
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableStandardsType,
     ControlFindingGeneratorType,
     ControlStatusType,
@@ -42,23 +41,19 @@
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
     ListSecurityControlDefinitionsPaginator,
     ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
-    AutomationRulesActionOutputTypeDef,
-    AutomationRulesActionTypeDef,
-    AutomationRulesFindingFiltersOutputTypeDef,
-    AutomationRulesFindingFiltersTypeDef,
-    AwsSecurityFindingFiltersOutputTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AutomationRulesActionUnionTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
-    AwsSecurityFindingOutputTypeDef,
-    AwsSecurityFindingTypeDef,
+    AwsSecurityFindingUnionTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchImportFindingsResponseTypeDef,
@@ -105,14 +100,15 @@
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
     StandardsControlAssociationIdTypeDef,
     StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
+    TimestampTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     WorkflowUpdateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -238,17 +234,15 @@
         is currently enabled or disabled in a standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
         """
 
     def batch_import_findings(
-        self,
-        *,
-        Findings: Sequence[Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]]
+        self, *, Findings: Sequence[AwsSecurityFindingUnionTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
         Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
@@ -329,18 +323,16 @@
 
     def create_automation_rule(
         self,
         *,
         RuleOrder: int,
         RuleName: str,
         Description: str,
-        Criteria: Union[
-            AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
-        ],
-        Actions: Sequence[Union[AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef]],
+        Criteria: AutomationRulesFindingFiltersUnionTypeDef,
+        Actions: Sequence[AutomationRulesActionUnionTypeDef],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
         IsTerminal: bool = ...
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
@@ -355,19 +347,15 @@
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_finding_aggregator)
         """
 
     def create_insight(
-        self,
-        *,
-        Name: str,
-        Filters: Union[AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef],
-        GroupByAttribute: str
+        self, *, Name: str, Filters: AwsSecurityFindingFiltersUnionTypeDef, GroupByAttribute: str
     ) -> CreateInsightResponseTypeDef:
         """
         Creates a custom insight in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_insight)
         """
@@ -623,32 +611,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_aggregator)
         """
 
     def get_finding_history(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingHistoryResponseTypeDef:
         """
         Returns history for a Security Hub finding in the last 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_history)
         """
 
     def get_findings(
         self,
         *,
-        Filters: Union[
-            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
-        ] = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
@@ -837,15 +823,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_finding_aggregator)
         """
 
     def update_findings(
         self,
         *,
-        Filters: Union[AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef],
+        Filters: AwsSecurityFindingFiltersUnionTypeDef,
         Note: NoteUpdateTypeDef = ...,
         RecordState: RecordStateType = ...
     ) -> Dict[str, Any]:
         """
         `UpdateFindings` is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
@@ -853,17 +839,15 @@
         """
 
     def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
-        Filters: Union[
-            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
-        ] = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         GroupByAttribute: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_insight)
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/client.pyi` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_securityhub.client import SecurityHubClient
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableStandardsType,
     ControlFindingGeneratorType,
     ControlStatusType,
@@ -42,23 +41,19 @@
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
     ListSecurityControlDefinitionsPaginator,
     ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
-    AutomationRulesActionOutputTypeDef,
-    AutomationRulesActionTypeDef,
-    AutomationRulesFindingFiltersOutputTypeDef,
-    AutomationRulesFindingFiltersTypeDef,
-    AwsSecurityFindingFiltersOutputTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AutomationRulesActionUnionTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
-    AwsSecurityFindingOutputTypeDef,
-    AwsSecurityFindingTypeDef,
+    AwsSecurityFindingUnionTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchImportFindingsResponseTypeDef,
@@ -105,14 +100,15 @@
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
     StandardsControlAssociationIdTypeDef,
     StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
+    TimestampTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     WorkflowUpdateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -225,17 +221,15 @@
         For a batch of security controls and standards, identifies whether each control
         is currently enabled or disabled in a standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
         """
     def batch_import_findings(
-        self,
-        *,
-        Findings: Sequence[Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]]
+        self, *, Findings: Sequence[AwsSecurityFindingUnionTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
         Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
@@ -309,18 +303,16 @@
         """
     def create_automation_rule(
         self,
         *,
         RuleOrder: int,
         RuleName: str,
         Description: str,
-        Criteria: Union[
-            AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
-        ],
-        Actions: Sequence[Union[AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef]],
+        Criteria: AutomationRulesFindingFiltersUnionTypeDef,
+        Actions: Sequence[AutomationRulesActionUnionTypeDef],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
         IsTerminal: bool = ...
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
@@ -333,19 +325,15 @@
         """
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_finding_aggregator)
         """
     def create_insight(
-        self,
-        *,
-        Name: str,
-        Filters: Union[AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef],
-        GroupByAttribute: str
+        self, *, Name: str, Filters: AwsSecurityFindingFiltersUnionTypeDef, GroupByAttribute: str
     ) -> CreateInsightResponseTypeDef:
         """
         Creates a custom insight in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_insight)
         """
@@ -574,31 +562,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_aggregator)
         """
     def get_finding_history(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingHistoryResponseTypeDef:
         """
         Returns history for a Security Hub finding in the last 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_history)
         """
     def get_findings(
         self,
         *,
-        Filters: Union[
-            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
-        ] = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
@@ -767,32 +753,30 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_finding_aggregator)
         """
     def update_findings(
         self,
         *,
-        Filters: Union[AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef],
+        Filters: AwsSecurityFindingFiltersUnionTypeDef,
         Note: NoteUpdateTypeDef = ...,
         RecordState: RecordStateType = ...
     ) -> Dict[str, Any]:
         """
         `UpdateFindings` is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_findings)
         """
     def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
-        Filters: Union[
-            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
-        ] = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         GroupByAttribute: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_insight)
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/literals.py` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/literals.pyi` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/paginator.py` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,20 @@
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
     list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    AwsSecurityFindingFiltersOutputTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     GetFindingHistoryResponseTypeDef,
@@ -69,14 +67,15 @@
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriterionTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsPaginator",
     "DescribeStandardsControlsPaginator",
@@ -89,25 +88,22 @@
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
     "ListSecurityControlDefinitionsPaginator",
     "ListStandardsControlAssociationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeActionTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
@@ -117,60 +113,56 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
         """
 
-
 class DescribeProductsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
     """
 
     def paginate(
         self, *, ProductArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
         """
 
-
 class DescribeStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
         """
 
-
 class DescribeStandardsControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
     """
 
     def paginate(
         self, *, StandardsSubscriptionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStandardsControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
         """
 
-
 class GetEnabledStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
@@ -180,161 +172,149 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
         """
 
-
 class GetFindingHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
     """
 
     def paginate(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
         """
 
-
 class GetFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        Filters: Union[
-            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
-        ] = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
 
-
 class GetInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
     """
 
     def paginate(
         self, *, InsightArns: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
         """
 
-
 class ListEnabledProductsForImportPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnabledProductsForImportResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
         """
 
-
 class ListFindingAggregatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
         """
 
-
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
         """
 
-
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
     """
 
     def paginate(
         self, *, OnlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
         """
 
-
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
 
-
 class ListSecurityControlDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
     """
 
     def paginate(
         self, *, StandardsArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityControlDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
         """
 
-
 class ListStandardsControlAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/paginator.pyi` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,22 +43,20 @@
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
     list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    AwsSecurityFindingFiltersOutputTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     GetFindingHistoryResponseTypeDef,
@@ -69,14 +67,15 @@
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriterionTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsPaginator",
     "DescribeStandardsControlsPaginator",
@@ -89,22 +88,25 @@
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
     "ListSecurityControlDefinitionsPaginator",
     "ListStandardsControlAssociationsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeActionTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
@@ -114,56 +116,60 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
         """
 
+
 class DescribeProductsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
     """
 
     def paginate(
         self, *, ProductArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
         """
 
+
 class DescribeStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
         """
 
+
 class DescribeStandardsControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
     """
 
     def paginate(
         self, *, StandardsSubscriptionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStandardsControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
         """
 
+
 class GetEnabledStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
@@ -173,151 +179,159 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
         """
 
+
 class GetFindingHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
     """
 
     def paginate(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
         """
 
+
 class GetFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        Filters: Union[
-            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
-        ] = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
 
+
 class GetInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
     """
 
     def paginate(
         self, *, InsightArns: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
         """
 
+
 class ListEnabledProductsForImportPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnabledProductsForImportResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
         """
 
+
 class ListFindingAggregatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
         """
 
+
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
         """
 
+
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
     """
 
     def paginate(
         self, *, OnlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
         """
 
+
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
 
+
 class ListSecurityControlDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
     """
 
     def paginate(
         self, *, StandardsArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityControlDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
         """
 
+
 class ListStandardsControlAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/type_defs.py` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_securityhub.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
-    data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
+    data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -464,14 +464,15 @@
     "FindingHistoryUpdateTypeDef",
     "FindingProviderSeverityTypeDef",
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     "FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef",
     "InvitationTypeDef",
     "GetEnabledStandardsRequestRequestTypeDef",
     "GetFindingAggregatorRequestRequestTypeDef",
+    "TimestampTypeDef",
     "SortCriterionTypeDef",
     "GetInsightResultsRequestRequestTypeDef",
     "GetInsightsRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "InsightResultValueTypeDef",
     "InviteMembersRequestRequestTypeDef",
@@ -657,15 +658,14 @@
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
-    "GetFindingHistoryRequestRequestTypeDef",
     "AwsSnsTopicDetailsOutputTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     "AwsWafRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
@@ -721,15 +721,14 @@
     "InviteMembersResponseTypeDef",
     "DateFilterTypeDef",
     "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
     "DescribeProductsRequestDescribeProductsPaginateTypeDef",
     "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
     "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
-    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
     "GetInsightsRequestGetInsightsPaginateTypeDef",
     "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
     "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
     "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListMembersRequestListMembersPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
@@ -741,14 +740,16 @@
     "ListFindingAggregatorsResponseTypeDef",
     "FindingHistoryRecordTypeDef",
     "FindingProviderFieldsOutputTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
+    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    "GetFindingHistoryRequestRequestTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
     "ListSecurityControlDefinitionsResponseTypeDef",
     "ListStandardsControlAssociationsResponseTypeDef",
     "NetworkPathComponentDetailsOutputTypeDef",
     "NetworkPathComponentDetailsTypeDef",
@@ -882,14 +883,15 @@
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
     "StatelessCustomActionDefinitionOutputTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
     "PortProbeActionOutputTypeDef",
     "PortProbeActionTypeDef",
+    "AutomationRulesActionUnionTypeDef",
     "AwsAthenaWorkGroupDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     "AwsCertificateManagerCertificateDetailsOutputTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
@@ -915,17 +917,18 @@
     "AwsStepFunctionStateMachineDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineDetailsTypeDef",
     "AwsWafv2RulesActionDetailsOutputTypeDef",
     "AwsWafv2WebAclActionDetailsOutputTypeDef",
     "AwsWafv2RulesActionDetailsTypeDef",
     "AwsWafv2WebAclActionDetailsTypeDef",
     "AutomationRulesConfigTypeDef",
-    "CreateAutomationRuleRequestRequestTypeDef",
+    "AutomationRulesFindingFiltersUnionTypeDef",
     "UpdateAutomationRulesRequestItemTypeDef",
     "InsightTypeDef",
+    "AwsSecurityFindingFiltersUnionTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
     "NetworkPathComponentOutputTypeDef",
     "NetworkPathComponentTypeDef",
@@ -937,14 +940,15 @@
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
     "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
+    "CreateAutomationRuleRequestRequestTypeDef",
     "AwsBackupBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
     "AwsCloudFrontDistributionDetailsOutputTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
     "AwsGuardDutyDetectorDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
@@ -987,14 +991,15 @@
     "ResourceDetailsOutputTypeDef",
     "ResourceDetailsTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "AwsSecurityFindingOutputTypeDef",
     "AwsSecurityFindingTypeDef",
     "GetFindingsResponseTypeDef",
+    "AwsSecurityFindingUnionTypeDef",
     "BatchImportFindingsRequestRequestTypeDef",
 )
 
 AcceptAdministratorInvitationRequestRequestTypeDef = TypedDict(
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     {
         "AdministratorId": str,
@@ -5145,14 +5150,15 @@
 GetFindingAggregatorRequestRequestTypeDef = TypedDict(
     "GetFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 SortCriterionTypeDef = TypedDict(
     "SortCriterionTypeDef",
     {
         "Field": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -7922,38 +7928,14 @@
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetFindingHistoryRequestRequestTypeDef",
-    {
-        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
-    },
-)
-_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetFindingHistoryRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class GetFindingHistoryRequestRequestTypeDef(
-    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
-):
-    pass
-
-
 AwsSnsTopicDetailsOutputTypeDef = TypedDict(
     "AwsSnsTopicDetailsOutputTypeDef",
     {
         "KmsMasterKeyId": str,
         "Subscription": List[AwsSnsTopicSubscriptionTypeDef],
         "TopicName": str,
         "Owner": str,
@@ -8615,38 +8597,14 @@
     {
         "StandardsSubscriptionArns": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
-    {
-        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
-    },
-)
-_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
-    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-):
-    pass
-
-
 GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
     "GetInsightsRequestGetInsightsPaginateTypeDef",
     {
         "InsightArns": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -8831,14 +8789,62 @@
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
+    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestRequestTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class GetFindingHistoryRequestRequestTypeDef(
+    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
+):
+    pass
+
+
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[ResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -11161,14 +11167,17 @@
     {
         "PortProbeDetails": Sequence[PortProbeDetailTypeDef],
         "Blocked": bool,
     },
     total=False,
 )
 
+AutomationRulesActionUnionTypeDef = Union[
+    AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef
+]
 AwsAthenaWorkGroupDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
         "State": str,
         "Configuration": AwsAthenaWorkGroupConfigurationDetailsTypeDef,
@@ -11757,44 +11766,17 @@
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
-_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
-    {
-        "RuleOrder": int,
-        "RuleName": str,
-        "Description": str,
-        "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": Sequence[
-            Union[AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef]
-        ],
-    },
-)
-_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "RuleStatus": RuleStatusType,
-        "IsTerminal": bool,
-    },
-    total=False,
-)
-
-
-class CreateAutomationRuleRequestRequestTypeDef(
-    _RequiredCreateAutomationRuleRequestRequestTypeDef,
-    _OptionalCreateAutomationRuleRequestRequestTypeDef,
-):
-    pass
-
-
+AutomationRulesFindingFiltersUnionTypeDef = Union[
+    AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
+]
 _RequiredUpdateAutomationRulesRequestItemTypeDef = TypedDict(
     "_RequiredUpdateAutomationRulesRequestItemTypeDef",
     {
         "RuleArn": str,
     },
 )
 _OptionalUpdateAutomationRulesRequestItemTypeDef = TypedDict(
@@ -11825,14 +11807,17 @@
         "InsightArn": str,
         "Name": str,
         "Filters": AwsSecurityFindingFiltersOutputTypeDef,
         "GroupByAttribute": str,
     },
 )
 
+AwsSecurityFindingFiltersUnionTypeDef = Union[
+    AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+]
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
@@ -12042,14 +12027,42 @@
         "AwsApiCallAction": AwsApiCallActionTypeDef,
         "DnsRequestAction": DnsRequestActionTypeDef,
         "PortProbeAction": PortProbeActionTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionUnionTypeDef],
+    },
+)
+_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "RuleStatus": RuleStatusType,
+        "IsTerminal": bool,
+    },
+    total=False,
+)
+
+
+class CreateAutomationRuleRequestRequestTypeDef(
+    _RequiredCreateAutomationRuleRequestRequestTypeDef,
+    _OptionalCreateAutomationRuleRequestRequestTypeDef,
+):
+    pass
+
+
 AwsBackupBackupPlanDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupPlanDetailsOutputTypeDef",
     {
         "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "VersionId": str,
@@ -12960,13 +12973,14 @@
     {
         "Findings": List[AwsSecurityFindingOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AwsSecurityFindingUnionTypeDef = Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]
 BatchImportFindingsRequestRequestTypeDef = TypedDict(
     "BatchImportFindingsRequestRequestTypeDef",
     {
-        "Findings": Sequence[Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]],
+        "Findings": Sequence[AwsSecurityFindingUnionTypeDef],
     },
 )
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/type_defs.pyi` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_securityhub.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
-    data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
+    data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -463,14 +463,15 @@
     "FindingHistoryUpdateTypeDef",
     "FindingProviderSeverityTypeDef",
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     "FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef",
     "InvitationTypeDef",
     "GetEnabledStandardsRequestRequestTypeDef",
     "GetFindingAggregatorRequestRequestTypeDef",
+    "TimestampTypeDef",
     "SortCriterionTypeDef",
     "GetInsightResultsRequestRequestTypeDef",
     "GetInsightsRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "InsightResultValueTypeDef",
     "InviteMembersRequestRequestTypeDef",
@@ -656,15 +657,14 @@
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
-    "GetFindingHistoryRequestRequestTypeDef",
     "AwsSnsTopicDetailsOutputTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     "AwsWafRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
@@ -720,15 +720,14 @@
     "InviteMembersResponseTypeDef",
     "DateFilterTypeDef",
     "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
     "DescribeProductsRequestDescribeProductsPaginateTypeDef",
     "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
     "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
-    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
     "GetInsightsRequestGetInsightsPaginateTypeDef",
     "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
     "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
     "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListMembersRequestListMembersPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
@@ -740,14 +739,16 @@
     "ListFindingAggregatorsResponseTypeDef",
     "FindingHistoryRecordTypeDef",
     "FindingProviderFieldsOutputTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
+    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    "GetFindingHistoryRequestRequestTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
     "ListSecurityControlDefinitionsResponseTypeDef",
     "ListStandardsControlAssociationsResponseTypeDef",
     "NetworkPathComponentDetailsOutputTypeDef",
     "NetworkPathComponentDetailsTypeDef",
@@ -881,14 +882,15 @@
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
     "StatelessCustomActionDefinitionOutputTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
     "PortProbeActionOutputTypeDef",
     "PortProbeActionTypeDef",
+    "AutomationRulesActionUnionTypeDef",
     "AwsAthenaWorkGroupDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     "AwsCertificateManagerCertificateDetailsOutputTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
@@ -914,17 +916,18 @@
     "AwsStepFunctionStateMachineDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineDetailsTypeDef",
     "AwsWafv2RulesActionDetailsOutputTypeDef",
     "AwsWafv2WebAclActionDetailsOutputTypeDef",
     "AwsWafv2RulesActionDetailsTypeDef",
     "AwsWafv2WebAclActionDetailsTypeDef",
     "AutomationRulesConfigTypeDef",
-    "CreateAutomationRuleRequestRequestTypeDef",
+    "AutomationRulesFindingFiltersUnionTypeDef",
     "UpdateAutomationRulesRequestItemTypeDef",
     "InsightTypeDef",
+    "AwsSecurityFindingFiltersUnionTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
     "NetworkPathComponentOutputTypeDef",
     "NetworkPathComponentTypeDef",
@@ -936,14 +939,15 @@
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
     "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
+    "CreateAutomationRuleRequestRequestTypeDef",
     "AwsBackupBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
     "AwsCloudFrontDistributionDetailsOutputTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
     "AwsGuardDutyDetectorDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
@@ -986,14 +990,15 @@
     "ResourceDetailsOutputTypeDef",
     "ResourceDetailsTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "AwsSecurityFindingOutputTypeDef",
     "AwsSecurityFindingTypeDef",
     "GetFindingsResponseTypeDef",
+    "AwsSecurityFindingUnionTypeDef",
     "BatchImportFindingsRequestRequestTypeDef",
 )
 
 AcceptAdministratorInvitationRequestRequestTypeDef = TypedDict(
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     {
         "AdministratorId": str,
@@ -5122,14 +5127,15 @@
 GetFindingAggregatorRequestRequestTypeDef = TypedDict(
     "GetFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 SortCriterionTypeDef = TypedDict(
     "SortCriterionTypeDef",
     {
         "Field": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -7883,36 +7889,14 @@
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetFindingHistoryRequestRequestTypeDef",
-    {
-        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
-    },
-)
-_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetFindingHistoryRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class GetFindingHistoryRequestRequestTypeDef(
-    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
-):
-    pass
-
 AwsSnsTopicDetailsOutputTypeDef = TypedDict(
     "AwsSnsTopicDetailsOutputTypeDef",
     {
         "KmsMasterKeyId": str,
         "Subscription": List[AwsSnsTopicSubscriptionTypeDef],
         "TopicName": str,
         "Owner": str,
@@ -8568,36 +8552,14 @@
     {
         "StandardsSubscriptionArns": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
-    {
-        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
-    },
-)
-_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
-    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-):
-    pass
-
 GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
     "GetInsightsRequestGetInsightsPaginateTypeDef",
     {
         "InsightArns": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -8780,14 +8742,58 @@
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
+    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestRequestTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class GetFindingHistoryRequestRequestTypeDef(
+    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
+):
+    pass
+
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[ResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -11104,14 +11110,17 @@
     {
         "PortProbeDetails": Sequence[PortProbeDetailTypeDef],
         "Blocked": bool,
     },
     total=False,
 )
 
+AutomationRulesActionUnionTypeDef = Union[
+    AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef
+]
 AwsAthenaWorkGroupDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
         "State": str,
         "Configuration": AwsAthenaWorkGroupConfigurationDetailsTypeDef,
@@ -11700,42 +11709,17 @@
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
-_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
-    {
-        "RuleOrder": int,
-        "RuleName": str,
-        "Description": str,
-        "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": Sequence[
-            Union[AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef]
-        ],
-    },
-)
-_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "RuleStatus": RuleStatusType,
-        "IsTerminal": bool,
-    },
-    total=False,
-)
-
-class CreateAutomationRuleRequestRequestTypeDef(
-    _RequiredCreateAutomationRuleRequestRequestTypeDef,
-    _OptionalCreateAutomationRuleRequestRequestTypeDef,
-):
-    pass
-
+AutomationRulesFindingFiltersUnionTypeDef = Union[
+    AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
+]
 _RequiredUpdateAutomationRulesRequestItemTypeDef = TypedDict(
     "_RequiredUpdateAutomationRulesRequestItemTypeDef",
     {
         "RuleArn": str,
     },
 )
 _OptionalUpdateAutomationRulesRequestItemTypeDef = TypedDict(
@@ -11764,14 +11748,17 @@
         "InsightArn": str,
         "Name": str,
         "Filters": AwsSecurityFindingFiltersOutputTypeDef,
         "GroupByAttribute": str,
     },
 )
 
+AwsSecurityFindingFiltersUnionTypeDef = Union[
+    AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+]
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
@@ -11977,14 +11964,40 @@
         "AwsApiCallAction": AwsApiCallActionTypeDef,
         "DnsRequestAction": DnsRequestActionTypeDef,
         "PortProbeAction": PortProbeActionTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionUnionTypeDef],
+    },
+)
+_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "RuleStatus": RuleStatusType,
+        "IsTerminal": bool,
+    },
+    total=False,
+)
+
+class CreateAutomationRuleRequestRequestTypeDef(
+    _RequiredCreateAutomationRuleRequestRequestTypeDef,
+    _OptionalCreateAutomationRuleRequestRequestTypeDef,
+):
+    pass
+
 AwsBackupBackupPlanDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupPlanDetailsOutputTypeDef",
     {
         "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "VersionId": str,
@@ -12887,13 +12900,14 @@
     {
         "Findings": List[AwsSecurityFindingOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AwsSecurityFindingUnionTypeDef = Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]
 BatchImportFindingsRequestRequestTypeDef = TypedDict(
     "BatchImportFindingsRequestRequestTypeDef",
     {
-        "Findings": Sequence[Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]],
+        "Findings": Sequence[AwsSecurityFindingUnionTypeDef],
     },
 )
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/PKG-INFO` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SecurityHub 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 securityhub type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
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
@@ -406,20 +406,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_securityhub.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_securityhub.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccountDetailsTypeDef,
     ActionLocalIpDetailsTypeDef,
@@ -823,14 +823,15 @@
     FindingHistoryUpdateTypeDef,
     FindingProviderSeverityTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
+    TimestampTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
     GetInsightsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
@@ -1016,15 +1017,14 @@
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
     AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
-    GetFindingHistoryRequestRequestTypeDef,
     AwsSnsTopicDetailsOutputTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
     AwsWafRateBasedRuleDetailsOutputTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
@@ -1080,15 +1080,14 @@
     InviteMembersResponseTypeDef,
     DateFilterTypeDef,
     DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
     DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
-    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
     GetInsightsRequestGetInsightsPaginateTypeDef,
     ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListMembersRequestListMembersPaginateTypeDef,
     ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
@@ -1100,14 +1099,16 @@
     ListFindingAggregatorsResponseTypeDef,
     FindingHistoryRecordTypeDef,
     FindingProviderFieldsOutputTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
+    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    GetFindingHistoryRequestRequestTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
     NetworkPathComponentDetailsOutputTypeDef,
     NetworkPathComponentDetailsTypeDef,
@@ -1241,14 +1242,15 @@
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionOutputTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionOutputTypeDef,
     PortProbeActionTypeDef,
+    AutomationRulesActionUnionTypeDef,
     AwsAthenaWorkGroupDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsOutputTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
@@ -1274,17 +1276,18 @@
     AwsStepFunctionStateMachineDetailsOutputTypeDef,
     AwsStepFunctionStateMachineDetailsTypeDef,
     AwsWafv2RulesActionDetailsOutputTypeDef,
     AwsWafv2WebAclActionDetailsOutputTypeDef,
     AwsWafv2RulesActionDetailsTypeDef,
     AwsWafv2WebAclActionDetailsTypeDef,
     AutomationRulesConfigTypeDef,
-    CreateAutomationRuleRequestRequestTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
     InsightTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentOutputTypeDef,
     NetworkPathComponentTypeDef,
@@ -1296,14 +1299,15 @@
     RuleGroupSourceStatelessRulesDetailsTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef,
     RuleGroupSourceCustomActionsDetailsOutputTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
+    CreateAutomationRuleRequestRequestTypeDef,
     AwsBackupBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
     AwsCloudFrontDistributionDetailsOutputTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
     AwsGuardDutyDetectorDetailsOutputTypeDef,
     AwsGuardDutyDetectorDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef,
@@ -1346,19 +1350,20 @@
     ResourceDetailsOutputTypeDef,
     ResourceDetailsTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     AwsSecurityFindingOutputTypeDef,
     AwsSecurityFindingTypeDef,
     GetFindingsResponseTypeDef,
+    AwsSecurityFindingUnionTypeDef,
     BatchImportFindingsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/SOURCES.txt` & `mypy-boto3-securityhub-1.28.16/mypy_boto3_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15.post1/setup.py` & `mypy-boto3-securityhub-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securityhub",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.SecurityHub 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 securityhub type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_securityhub": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

