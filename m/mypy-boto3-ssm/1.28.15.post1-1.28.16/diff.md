# Comparing `tmp/mypy-boto3-ssm-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ssm-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:16 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-1.28.16.tar", last modified: Tue Aug  1 11:37:55 2023, max compression
```

## Comparing `mypy-boto3-ssm-1.28.15.post1.tar` & `mypy-boto3-ssm-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.565421 mypy-boto3-ssm-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46806 2023-07-29 10:04:16.565421 mypy-boto3-ssm-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45329 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.561421 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   133465 2023-07-29 10:00:02.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   133272 2023-07-29 10:00:02.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-07-29 10:00:04.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    28170 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    59274 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    59225 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   214204 2023-07-29 10:00:13.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   213962 2023-07-29 10:00:06.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.565421 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46806 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:16.565421 mypy-boto3-ssm-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.896719 mypy-boto3-ssm-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:36.000000 mypy-boto3-ssm-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47336 2023-08-01 11:37:55.888719 mypy-boto3-ssm-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    45868 2023-08-01 11:33:36.000000 mypy-boto3-ssm-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.888719 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-08-01 11:33:36.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-08-01 11:33:36.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:33:36.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131484 2023-08-01 11:33:37.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131291 2023-08-01 11:33:36.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-08-01 11:33:38.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28170 2023-08-01 11:33:38.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    59201 2023-08-01 11:33:38.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59152 2023-08-01 11:33:37.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:36.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   215349 2023-08-01 11:33:48.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   215107 2023-08-01 11:33:45.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:36.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-01 11:33:38.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-01 11:33:38.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.888719 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47336 2023-08-01 11:37:55.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:37:55.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:55.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:55.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:55.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:55.000000 mypy-boto3-ssm-1.28.16/mypy_boto3_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:55.896719 mypy-boto3-ssm-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:33:35.000000 mypy-boto3-ssm-1.28.16/setup.py
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/LICENSE` & `mypy-boto3-ssm-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15.post1/PKG-INFO` & `mypy-boto3-ssm-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SSM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ssm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ssm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -633,20 +633,20 @@
 )
 
 
 def check_value(value: AssociationComplianceSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ssm.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
     TagTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
@@ -655,41 +655,40 @@
     AssociationOverviewTypeDef,
     AssociationStatusOutputTypeDef,
     TargetOutputTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
-    AssociationStatusTypeDef,
+    TimestampTypeDef,
     AttachmentContentTypeDef,
     AttachmentInformationTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
+    BlobTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
     NotificationConfigOutputTypeDef,
     ComplianceExecutionSummaryOutputTypeDef,
-    ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
     TargetTypeDef,
     DocumentRequiresTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
     MetadataValueTypeDef,
-    PatchSourceOutputTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
@@ -766,14 +765,15 @@
     OpsResultAttributeTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
+    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
@@ -790,15 +790,14 @@
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
     MaintenanceWindowLambdaParametersOutputTypeDef,
-    MaintenanceWindowLambdaParametersTypeDef,
     NotificationConfigTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
     OpsItemIdentityTypeDef,
     ParameterInlinePolicyTypeDef,
@@ -874,33 +873,32 @@
     AssociationTypeDef,
     MaintenanceWindowTargetTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
     ListAssociationsRequestRequestTypeDef,
-    UpdateAssociationStatusRequestRequestTypeDef,
+    AssociationStatusTypeDef,
+    ComplianceExecutionSummaryTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
+    MaintenanceWindowLambdaParametersTypeDef,
     GetCommandInvocationResultTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
     MaintenanceWindowRunCommandParametersOutputTypeDef,
     ComplianceItemTypeDef,
-    PutComplianceItemsRequestRequestTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    TargetUnionTypeDef,
     CreateDocumentRequestRequestTypeDef,
     DocumentIdentifierTypeDef,
     GetDocumentResultTypeDef,
     OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
     OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
@@ -913,15 +911,14 @@
     DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
     DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
@@ -933,16 +930,14 @@
     ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
-    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
-    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
     DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef,
     DescribePatchBaselinesRequestRequestTypeDef,
     DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef,
     DescribePatchGroupsRequestRequestTypeDef,
     DescribeAvailablePatchesResultTypeDef,
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef,
@@ -994,14 +989,15 @@
     GetInventoryRequestRequestTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
+    PatchSourceUnionTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
@@ -1012,14 +1008,16 @@
     ListOpsItemEventsRequestRequestTypeDef,
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
     MaintenanceWindowRunCommandParametersTypeDef,
+    NotificationConfigUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     OpsEntityTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
     PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
@@ -1030,24 +1028,35 @@
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
     MaintenanceWindowTaskTypeDef,
     TargetLocationOutputTypeDef,
-    SendCommandRequestRequestTypeDef,
+    AlarmConfigurationUnionTypeDef,
     TargetLocationTypeDef,
     ListAssociationsResultTypeDef,
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
+    AssociationStatusUnionTypeDef,
+    UpdateAssociationStatusRequestRequestTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
+    PutComplianceItemsRequestRequestTypeDef,
     ListCommandInvocationsResultTypeDef,
     MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
+    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
+    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    SendCommandRequestRequestTypeDef,
+    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     ListDocumentsResultTypeDef,
     DescribeOpsItemsResponseTypeDef,
     GetOpsItemResponseTypeDef,
     DescribePatchGroupsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -1064,14 +1073,15 @@
     MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
     PatchRuleOutputTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchRuleTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
     ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
     DescribeAssociationExecutionsResultTypeDef,
     ListCommandsResultTypeDef,
     SendCommandResultTypeDef,
@@ -1079,25 +1089,24 @@
     DescribeMaintenanceWindowTasksResultTypeDef,
     AssociationDescriptionTypeDef,
     AssociationVersionInfoTypeDef,
     CreateAssociationBatchRequestEntryOutputTypeDef,
     RunbookOutputTypeDef,
     StepExecutionTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
-    CreateAssociationRequestRequestTypeDef,
     RunbookTypeDef,
-    StartAutomationExecutionRequestRequestTypeDef,
-    UpdateAssociationRequestRequestTypeDef,
+    TargetLocationUnionTypeDef,
     GetMaintenanceWindowTaskResultTypeDef,
     UpdateMaintenanceWindowTaskResultTypeDef,
     ListComplianceSummariesResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListDocumentMetadataHistoryResponseTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
     RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
     UpdateMaintenanceWindowTaskRequestRequestTypeDef,
     PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
     ResourceDataSyncItemTypeDef,
     CreateResourceDataSyncRequestRequestTypeDef,
     UpdateResourceDataSyncRequestRequestTypeDef,
@@ -1106,30 +1115,36 @@
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     ListAssociationVersionsResultTypeDef,
     FailedCreateAssociationTypeDef,
     AutomationExecutionMetadataTypeDef,
     AutomationExecutionTypeDef,
     DescribeAutomationStepExecutionsResultTypeDef,
-    CreateAssociationBatchRequestRequestTypeDef,
-    StartChangeRequestExecutionRequestRequestTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
+    RunbookUnionTypeDef,
+    CreateAssociationRequestRequestTypeDef,
+    StartAutomationExecutionRequestRequestTypeDef,
+    UpdateAssociationRequestRequestTypeDef,
     GetPatchBaselineResultTypeDef,
     UpdatePatchBaselineResultTypeDef,
     BaselineOverrideTypeDef,
     CreatePatchBaselineRequestRequestTypeDef,
+    PatchRuleGroupUnionTypeDef,
     UpdatePatchBaselineRequestRequestTypeDef,
     ListResourceDataSyncResultTypeDef,
     CreateAssociationBatchResultTypeDef,
     DescribeAutomationExecutionsResultTypeDef,
     GetAutomationExecutionResultTypeDef,
+    CreateAssociationBatchRequestRequestTypeDef,
+    StartChangeRequestExecutionRequestRequestTypeDef,
     GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSharingInfoTypeDef:
+def get_value() -> AccountSharingInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/README.md` & `mypy-boto3-ssm-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -601,20 +601,20 @@
 )
 
 
 def check_value(value: AssociationComplianceSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ssm.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
     TagTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
@@ -623,41 +623,40 @@
     AssociationOverviewTypeDef,
     AssociationStatusOutputTypeDef,
     TargetOutputTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
-    AssociationStatusTypeDef,
+    TimestampTypeDef,
     AttachmentContentTypeDef,
     AttachmentInformationTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
+    BlobTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
     NotificationConfigOutputTypeDef,
     ComplianceExecutionSummaryOutputTypeDef,
-    ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
     TargetTypeDef,
     DocumentRequiresTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
     MetadataValueTypeDef,
-    PatchSourceOutputTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
@@ -734,14 +733,15 @@
     OpsResultAttributeTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
+    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
@@ -758,15 +758,14 @@
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
     MaintenanceWindowLambdaParametersOutputTypeDef,
-    MaintenanceWindowLambdaParametersTypeDef,
     NotificationConfigTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
     OpsItemIdentityTypeDef,
     ParameterInlinePolicyTypeDef,
@@ -842,33 +841,32 @@
     AssociationTypeDef,
     MaintenanceWindowTargetTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
     ListAssociationsRequestRequestTypeDef,
-    UpdateAssociationStatusRequestRequestTypeDef,
+    AssociationStatusTypeDef,
+    ComplianceExecutionSummaryTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
+    MaintenanceWindowLambdaParametersTypeDef,
     GetCommandInvocationResultTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
     MaintenanceWindowRunCommandParametersOutputTypeDef,
     ComplianceItemTypeDef,
-    PutComplianceItemsRequestRequestTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    TargetUnionTypeDef,
     CreateDocumentRequestRequestTypeDef,
     DocumentIdentifierTypeDef,
     GetDocumentResultTypeDef,
     OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
     OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
@@ -881,15 +879,14 @@
     DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
     DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
@@ -901,16 +898,14 @@
     ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
-    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
-    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
     DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef,
     DescribePatchBaselinesRequestRequestTypeDef,
     DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef,
     DescribePatchGroupsRequestRequestTypeDef,
     DescribeAvailablePatchesResultTypeDef,
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef,
@@ -962,14 +957,15 @@
     GetInventoryRequestRequestTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
+    PatchSourceUnionTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
@@ -980,14 +976,16 @@
     ListOpsItemEventsRequestRequestTypeDef,
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
     MaintenanceWindowRunCommandParametersTypeDef,
+    NotificationConfigUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     OpsEntityTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
     PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
@@ -998,24 +996,35 @@
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
     MaintenanceWindowTaskTypeDef,
     TargetLocationOutputTypeDef,
-    SendCommandRequestRequestTypeDef,
+    AlarmConfigurationUnionTypeDef,
     TargetLocationTypeDef,
     ListAssociationsResultTypeDef,
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
+    AssociationStatusUnionTypeDef,
+    UpdateAssociationStatusRequestRequestTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
+    PutComplianceItemsRequestRequestTypeDef,
     ListCommandInvocationsResultTypeDef,
     MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
+    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
+    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    SendCommandRequestRequestTypeDef,
+    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     ListDocumentsResultTypeDef,
     DescribeOpsItemsResponseTypeDef,
     GetOpsItemResponseTypeDef,
     DescribePatchGroupsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -1032,14 +1041,15 @@
     MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
     PatchRuleOutputTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchRuleTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
     ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
     DescribeAssociationExecutionsResultTypeDef,
     ListCommandsResultTypeDef,
     SendCommandResultTypeDef,
@@ -1047,25 +1057,24 @@
     DescribeMaintenanceWindowTasksResultTypeDef,
     AssociationDescriptionTypeDef,
     AssociationVersionInfoTypeDef,
     CreateAssociationBatchRequestEntryOutputTypeDef,
     RunbookOutputTypeDef,
     StepExecutionTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
-    CreateAssociationRequestRequestTypeDef,
     RunbookTypeDef,
-    StartAutomationExecutionRequestRequestTypeDef,
-    UpdateAssociationRequestRequestTypeDef,
+    TargetLocationUnionTypeDef,
     GetMaintenanceWindowTaskResultTypeDef,
     UpdateMaintenanceWindowTaskResultTypeDef,
     ListComplianceSummariesResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListDocumentMetadataHistoryResponseTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
     RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
     UpdateMaintenanceWindowTaskRequestRequestTypeDef,
     PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
     ResourceDataSyncItemTypeDef,
     CreateResourceDataSyncRequestRequestTypeDef,
     UpdateResourceDataSyncRequestRequestTypeDef,
@@ -1074,30 +1083,36 @@
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     ListAssociationVersionsResultTypeDef,
     FailedCreateAssociationTypeDef,
     AutomationExecutionMetadataTypeDef,
     AutomationExecutionTypeDef,
     DescribeAutomationStepExecutionsResultTypeDef,
-    CreateAssociationBatchRequestRequestTypeDef,
-    StartChangeRequestExecutionRequestRequestTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
+    RunbookUnionTypeDef,
+    CreateAssociationRequestRequestTypeDef,
+    StartAutomationExecutionRequestRequestTypeDef,
+    UpdateAssociationRequestRequestTypeDef,
     GetPatchBaselineResultTypeDef,
     UpdatePatchBaselineResultTypeDef,
     BaselineOverrideTypeDef,
     CreatePatchBaselineRequestRequestTypeDef,
+    PatchRuleGroupUnionTypeDef,
     UpdatePatchBaselineRequestRequestTypeDef,
     ListResourceDataSyncResultTypeDef,
     CreateAssociationBatchResultTypeDef,
     DescribeAutomationExecutionsResultTypeDef,
     GetAutomationExecutionResultTypeDef,
+    CreateAssociationBatchRequestRequestTypeDef,
+    StartChangeRequestExecutionRequestRequestTypeDef,
     GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSharingInfoTypeDef:
+def get_value() -> AccountSharingInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__init__.py` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__init__.pyi` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__main__.py` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSM 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.SSM 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
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

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/client.py` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_ssm.client import SSMClient
 
     session = Session()
     client: SSMClient = session.client("ssm")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationSyncComplianceType,
     ComplianceUploadTypeType,
@@ -90,35 +89,31 @@
     ListOpsItemEventsPaginator,
     ListOpsItemRelatedItemsPaginator,
     ListOpsMetadataPaginator,
     ListResourceComplianceSummariesPaginator,
     ListResourceDataSyncPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationOutputTypeDef,
-    AlarmConfigurationTypeDef,
+    AlarmConfigurationUnionTypeDef,
     AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationExecutionFilterTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
-    AssociationStatusOutputTypeDef,
-    AssociationStatusTypeDef,
+    AssociationStatusUnionTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     BaselineOverrideTypeDef,
     CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
-    ComplianceExecutionSummaryOutputTypeDef,
-    ComplianceExecutionSummaryTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     CreateActivationResultTypeDef,
-    CreateAssociationBatchRequestEntryOutputTypeDef,
-    CreateAssociationBatchRequestEntryTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
     CreateAssociationBatchResultTypeDef,
     CreateAssociationResultTypeDef,
     CreateDocumentResultTypeDef,
     CreateMaintenanceWindowResultTypeDef,
     CreateOpsItemResponseTypeDef,
     CreateOpsMetadataResultTypeDef,
     CreatePatchBaselineResultTypeDef,
@@ -213,67 +208,59 @@
     ListOpsItemRelatedItemsResponseTypeDef,
     ListOpsMetadataResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     ListTagsForResourceResultTypeDef,
     LoggingInfoTypeDef,
     MaintenanceWindowFilterTypeDef,
-    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     MetadataValueTypeDef,
-    NotificationConfigOutputTypeDef,
-    NotificationConfigTypeDef,
+    NotificationConfigUnionTypeDef,
     OpsAggregatorTypeDef,
     OpsFilterTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemFilterTypeDef,
     OpsItemNotificationTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsResultAttributeTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
-    PatchFilterGroupOutputTypeDef,
-    PatchFilterGroupTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchOrchestratorFilterTypeDef,
-    PatchRuleGroupOutputTypeDef,
-    PatchRuleGroupTypeDef,
-    PatchSourceOutputTypeDef,
-    PatchSourceTypeDef,
+    PatchRuleGroupUnionTypeDef,
+    PatchSourceUnionTypeDef,
     PutInventoryResultTypeDef,
     PutParameterResultTypeDef,
     PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupResultTypeDef,
     RegisterTargetWithMaintenanceWindowResultTypeDef,
     RegisterTaskWithMaintenanceWindowResultTypeDef,
     RegistrationMetadataItemTypeDef,
     RelatedOpsItemTypeDef,
     ResetServiceSettingResultTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     ResourceDataSyncSourceTypeDef,
     ResultAttributeTypeDef,
     ResumeSessionResponseTypeDef,
-    RunbookOutputTypeDef,
-    RunbookTypeDef,
+    RunbookUnionTypeDef,
     SendCommandResultTypeDef,
     SessionFilterTypeDef,
     StartAutomationExecutionResultTypeDef,
     StartChangeRequestExecutionResultTypeDef,
     StartSessionResponseTypeDef,
     StepExecutionFilterTypeDef,
     TagTypeDef,
-    TargetLocationOutputTypeDef,
-    TargetLocationTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
+    TargetLocationUnionTypeDef,
+    TargetUnionTypeDef,
     TerminateSessionResponseTypeDef,
+    TimestampTypeDef,
     UnlabelParameterVersionResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
     UpdateDocumentResultTypeDef,
     UpdateMaintenanceWindowResultTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
@@ -511,15 +498,15 @@
     def create_activation(
         self,
         *,
         IamRole: str,
         Description: str = ...,
         DefaultInstanceName: str = ...,
         RegistrationLimit: int = ...,
-        ExpirationDate: Union[datetime, str] = ...,
+        ExpirationDate: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RegistrationMetadata: Sequence[RegistrationMetadataItemTypeDef] = ...
     ) -> CreateActivationResultTypeDef:
         """
         Generates an activation code and activation ID you can use to register your on-
         premises servers, edge devices, or virtual machine (VM) with Amazon Web Services
         Systems Manager.
@@ -531,48 +518,41 @@
     def create_association(
         self,
         *,
         Name: str,
         DocumentVersion: str = ...,
         InstanceId: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         AssociationName: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_association)
         """
 
     def create_association_batch(
-        self,
-        *,
-        Entries: Sequence[
-            Union[
-                CreateAssociationBatchRequestEntryTypeDef,
-                CreateAssociationBatchRequestEntryOutputTypeDef,
-            ]
-        ]
+        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryUnionTypeDef]
     ) -> CreateAssociationBatchResultTypeDef:
         """
         Associates the specified Amazon Web Services Systems Manager document (SSM
         document) with the specified managed nodes or targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_association_batch)
@@ -632,18 +612,18 @@
         OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,
         Notifications: Sequence[OpsItemNotificationTypeDef] = ...,
         Priority: int = ...,
         RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Category: str = ...,
         Severity: str = ...,
-        ActualStartTime: Union[datetime, str] = ...,
-        ActualEndTime: Union[datetime, str] = ...,
-        PlannedStartTime: Union[datetime, str] = ...,
-        PlannedEndTime: Union[datetime, str] = ...,
+        ActualStartTime: TimestampTypeDef = ...,
+        ActualEndTime: TimestampTypeDef = ...,
+        PlannedStartTime: TimestampTypeDef = ...,
+        PlannedEndTime: TimestampTypeDef = ...,
         AccountId: str = ...
     ) -> CreateOpsItemResponseTypeDef:
         """
         Creates a new OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_ops_item)
@@ -666,23 +646,23 @@
         """
 
     def create_patch_baseline(
         self,
         *,
         Name: str,
         OperatingSystem: OperatingSystemType = ...,
-        GlobalFilters: Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef] = ...,
-        ApprovalRules: Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef] = ...,
+        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
+        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]] = ...,
+        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
@@ -1129,15 +1109,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_maintenance_window_executions)
         """
 
     def describe_maintenance_window_schedule(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
@@ -1189,15 +1169,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_maintenance_windows)
         """
 
     def describe_maintenance_windows_for_target(
         self,
         *,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        Targets: Sequence[TargetUnionTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated with.
@@ -1867,17 +1847,15 @@
 
     def put_compliance_items(
         self,
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
-        ExecutionSummary: Union[
-            ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
-        ],
+        ExecutionSummary: ComplianceExecutionSummaryUnionTypeDef,
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
         UploadType: ComplianceUploadTypeType = ...
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
@@ -1949,15 +1927,15 @@
         """
 
     def register_target_with_maintenance_window(
         self,
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        Targets: Sequence[TargetUnionTypeDef],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
@@ -1968,36 +1946,29 @@
 
     def register_task_with_maintenance_window(
         self,
         *,
         WindowId: str,
         TaskArn: str,
         TaskType: MaintenanceWindowTaskTypeType,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ServiceRoleArn: str = ...,
         TaskParameters: Mapping[
-            str,
-            Union[
-                MaintenanceWindowTaskParameterValueExpressionTypeDef,
-                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-            ],
-        ] = ...,
-        TaskInvocationParameters: Union[
-            MaintenanceWindowTaskInvocationParametersTypeDef,
-            MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
         ] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#register_task_with_maintenance_window)
         """
@@ -2044,30 +2015,30 @@
         """
 
     def send_command(
         self,
         *,
         DocumentName: str,
         InstanceIds: Sequence[str] = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         DocumentVersion: str = ...,
         DocumentHash: str = ...,
         DocumentHashType: DocumentHashTypeType = ...,
         TimeoutSeconds: int = ...,
         Comment: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         OutputS3Region: str = ...,
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
-        NotificationConfig: Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef] = ...,
+        NotificationConfig: NotificationConfigUnionTypeDef = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#send_command)
         """
@@ -2085,42 +2056,42 @@
         *,
         DocumentName: str,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ClientToken: str = ...,
         Mode: ExecutionModeType = ...,
         TargetParameterName: str = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
-        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#start_automation_execution)
         """
 
     def start_change_request_execution(
         self,
         *,
         DocumentName: str,
-        Runbooks: Sequence[Union[RunbookTypeDef, RunbookOutputTypeDef]],
-        ScheduledTime: Union[datetime, str] = ...,
+        Runbooks: Sequence[RunbookUnionTypeDef],
+        ScheduledTime: TimestampTypeDef = ...,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ScheduledEndTime: Union[datetime, str] = ...,
+        ScheduledEndTime: TimestampTypeDef = ...,
         ChangeDetails: str = ...
     ) -> StartChangeRequestExecutionResultTypeDef:
         """
         Creates a change request for Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_change_request_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#start_change_request_execution)
@@ -2176,42 +2147,38 @@
         *,
         AssociationId: str,
         Parameters: Mapping[str, Sequence[str]] = ...,
         DocumentVersion: str = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         Name: str = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         AssociationName: str = ...,
         AssociationVersion: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_association)
         """
 
     def update_association_status(
-        self,
-        *,
-        Name: str,
-        InstanceId: str,
-        AssociationStatus: Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
+        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusUnionTypeDef
     ) -> UpdateAssociationStatusResultTypeDef:
         """
         Updates the status of the Amazon Web Services Systems Manager document (SSM
         document) associated with the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_association_status)
@@ -2282,15 +2249,15 @@
         """
 
     def update_maintenance_window_target(
         self,
         *,
         WindowId: str,
         WindowTargetId: str,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
@@ -2300,37 +2267,30 @@
         """
 
     def update_maintenance_window_task(
         self,
         *,
         WindowId: str,
         WindowTaskId: str,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         TaskArn: str = ...,
         ServiceRoleArn: str = ...,
         TaskParameters: Mapping[
-            str,
-            Union[
-                MaintenanceWindowTaskParameterValueExpressionTypeDef,
-                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-            ],
-        ] = ...,
-        TaskInvocationParameters: Union[
-            MaintenanceWindowTaskInvocationParametersTypeDef,
-            MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
         ] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_maintenance_window_task)
         """
@@ -2354,18 +2314,18 @@
         Notifications: Sequence[OpsItemNotificationTypeDef] = ...,
         Priority: int = ...,
         RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,
         Status: OpsItemStatusType = ...,
         Title: str = ...,
         Category: str = ...,
         Severity: str = ...,
-        ActualStartTime: Union[datetime, str] = ...,
-        ActualEndTime: Union[datetime, str] = ...,
-        PlannedStartTime: Union[datetime, str] = ...,
-        PlannedEndTime: Union[datetime, str] = ...,
+        ActualStartTime: TimestampTypeDef = ...,
+        ActualEndTime: TimestampTypeDef = ...,
+        PlannedStartTime: TimestampTypeDef = ...,
+        PlannedEndTime: TimestampTypeDef = ...,
         OpsItemArn: str = ...
     ) -> Dict[str, Any]:
         """
         Edit or change an OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_ops_item)
@@ -2387,23 +2347,23 @@
         """
 
     def update_patch_baseline(
         self,
         *,
         BaselineId: str,
         Name: str = ...,
-        GlobalFilters: Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef] = ...,
-        ApprovalRules: Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef] = ...,
+        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
+        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]] = ...,
+        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
         Replace: bool = ...
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_patch_baseline)
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/client.pyi` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_ssm.client import SSMClient
 
     session = Session()
     client: SSMClient = session.client("ssm")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationSyncComplianceType,
     ComplianceUploadTypeType,
@@ -90,35 +89,31 @@
     ListOpsItemEventsPaginator,
     ListOpsItemRelatedItemsPaginator,
     ListOpsMetadataPaginator,
     ListResourceComplianceSummariesPaginator,
     ListResourceDataSyncPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationOutputTypeDef,
-    AlarmConfigurationTypeDef,
+    AlarmConfigurationUnionTypeDef,
     AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationExecutionFilterTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
-    AssociationStatusOutputTypeDef,
-    AssociationStatusTypeDef,
+    AssociationStatusUnionTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     BaselineOverrideTypeDef,
     CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
-    ComplianceExecutionSummaryOutputTypeDef,
-    ComplianceExecutionSummaryTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     CreateActivationResultTypeDef,
-    CreateAssociationBatchRequestEntryOutputTypeDef,
-    CreateAssociationBatchRequestEntryTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
     CreateAssociationBatchResultTypeDef,
     CreateAssociationResultTypeDef,
     CreateDocumentResultTypeDef,
     CreateMaintenanceWindowResultTypeDef,
     CreateOpsItemResponseTypeDef,
     CreateOpsMetadataResultTypeDef,
     CreatePatchBaselineResultTypeDef,
@@ -213,67 +208,59 @@
     ListOpsItemRelatedItemsResponseTypeDef,
     ListOpsMetadataResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     ListTagsForResourceResultTypeDef,
     LoggingInfoTypeDef,
     MaintenanceWindowFilterTypeDef,
-    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     MetadataValueTypeDef,
-    NotificationConfigOutputTypeDef,
-    NotificationConfigTypeDef,
+    NotificationConfigUnionTypeDef,
     OpsAggregatorTypeDef,
     OpsFilterTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemFilterTypeDef,
     OpsItemNotificationTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsResultAttributeTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
-    PatchFilterGroupOutputTypeDef,
-    PatchFilterGroupTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchOrchestratorFilterTypeDef,
-    PatchRuleGroupOutputTypeDef,
-    PatchRuleGroupTypeDef,
-    PatchSourceOutputTypeDef,
-    PatchSourceTypeDef,
+    PatchRuleGroupUnionTypeDef,
+    PatchSourceUnionTypeDef,
     PutInventoryResultTypeDef,
     PutParameterResultTypeDef,
     PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupResultTypeDef,
     RegisterTargetWithMaintenanceWindowResultTypeDef,
     RegisterTaskWithMaintenanceWindowResultTypeDef,
     RegistrationMetadataItemTypeDef,
     RelatedOpsItemTypeDef,
     ResetServiceSettingResultTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     ResourceDataSyncSourceTypeDef,
     ResultAttributeTypeDef,
     ResumeSessionResponseTypeDef,
-    RunbookOutputTypeDef,
-    RunbookTypeDef,
+    RunbookUnionTypeDef,
     SendCommandResultTypeDef,
     SessionFilterTypeDef,
     StartAutomationExecutionResultTypeDef,
     StartChangeRequestExecutionResultTypeDef,
     StartSessionResponseTypeDef,
     StepExecutionFilterTypeDef,
     TagTypeDef,
-    TargetLocationOutputTypeDef,
-    TargetLocationTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
+    TargetLocationUnionTypeDef,
+    TargetUnionTypeDef,
     TerminateSessionResponseTypeDef,
+    TimestampTypeDef,
     UnlabelParameterVersionResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
     UpdateDocumentResultTypeDef,
     UpdateMaintenanceWindowResultTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
@@ -500,15 +487,15 @@
     def create_activation(
         self,
         *,
         IamRole: str,
         Description: str = ...,
         DefaultInstanceName: str = ...,
         RegistrationLimit: int = ...,
-        ExpirationDate: Union[datetime, str] = ...,
+        ExpirationDate: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RegistrationMetadata: Sequence[RegistrationMetadataItemTypeDef] = ...
     ) -> CreateActivationResultTypeDef:
         """
         Generates an activation code and activation ID you can use to register your on-
         premises servers, edge devices, or virtual machine (VM) with Amazon Web Services
         Systems Manager.
@@ -519,47 +506,40 @@
     def create_association(
         self,
         *,
         Name: str,
         DocumentVersion: str = ...,
         InstanceId: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         AssociationName: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_association)
         """
     def create_association_batch(
-        self,
-        *,
-        Entries: Sequence[
-            Union[
-                CreateAssociationBatchRequestEntryTypeDef,
-                CreateAssociationBatchRequestEntryOutputTypeDef,
-            ]
-        ]
+        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryUnionTypeDef]
     ) -> CreateAssociationBatchResultTypeDef:
         """
         Associates the specified Amazon Web Services Systems Manager document (SSM
         document) with the specified managed nodes or targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_association_batch)
@@ -616,18 +596,18 @@
         OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,
         Notifications: Sequence[OpsItemNotificationTypeDef] = ...,
         Priority: int = ...,
         RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Category: str = ...,
         Severity: str = ...,
-        ActualStartTime: Union[datetime, str] = ...,
-        ActualEndTime: Union[datetime, str] = ...,
-        PlannedStartTime: Union[datetime, str] = ...,
-        PlannedEndTime: Union[datetime, str] = ...,
+        ActualStartTime: TimestampTypeDef = ...,
+        ActualEndTime: TimestampTypeDef = ...,
+        PlannedStartTime: TimestampTypeDef = ...,
+        PlannedEndTime: TimestampTypeDef = ...,
         AccountId: str = ...
     ) -> CreateOpsItemResponseTypeDef:
         """
         Creates a new OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_ops_item)
@@ -648,23 +628,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_ops_metadata)
         """
     def create_patch_baseline(
         self,
         *,
         Name: str,
         OperatingSystem: OperatingSystemType = ...,
-        GlobalFilters: Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef] = ...,
-        ApprovalRules: Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef] = ...,
+        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
+        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]] = ...,
+        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
@@ -1074,15 +1054,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_maintenance_window_executions)
         """
     def describe_maintenance_window_schedule(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
@@ -1130,15 +1110,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_maintenance_windows)
         """
     def describe_maintenance_windows_for_target(
         self,
         *,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        Targets: Sequence[TargetUnionTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated with.
@@ -1755,17 +1735,15 @@
         """
     def put_compliance_items(
         self,
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
-        ExecutionSummary: Union[
-            ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
-        ],
+        ExecutionSummary: ComplianceExecutionSummaryUnionTypeDef,
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
         UploadType: ComplianceUploadTypeType = ...
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
@@ -1831,15 +1809,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#register_patch_baseline_for_patch_group)
         """
     def register_target_with_maintenance_window(
         self,
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        Targets: Sequence[TargetUnionTypeDef],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
@@ -1849,36 +1827,29 @@
         """
     def register_task_with_maintenance_window(
         self,
         *,
         WindowId: str,
         TaskArn: str,
         TaskType: MaintenanceWindowTaskTypeType,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ServiceRoleArn: str = ...,
         TaskParameters: Mapping[
-            str,
-            Union[
-                MaintenanceWindowTaskParameterValueExpressionTypeDef,
-                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-            ],
-        ] = ...,
-        TaskInvocationParameters: Union[
-            MaintenanceWindowTaskInvocationParametersTypeDef,
-            MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
         ] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#register_task_with_maintenance_window)
         """
@@ -1920,30 +1891,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#send_automation_signal)
         """
     def send_command(
         self,
         *,
         DocumentName: str,
         InstanceIds: Sequence[str] = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         DocumentVersion: str = ...,
         DocumentHash: str = ...,
         DocumentHashType: DocumentHashTypeType = ...,
         TimeoutSeconds: int = ...,
         Comment: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         OutputS3Region: str = ...,
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
-        NotificationConfig: Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef] = ...,
+        NotificationConfig: NotificationConfigUnionTypeDef = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#send_command)
         """
@@ -1959,41 +1930,41 @@
         *,
         DocumentName: str,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ClientToken: str = ...,
         Mode: ExecutionModeType = ...,
         TargetParameterName: str = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
-        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#start_automation_execution)
         """
     def start_change_request_execution(
         self,
         *,
         DocumentName: str,
-        Runbooks: Sequence[Union[RunbookTypeDef, RunbookOutputTypeDef]],
-        ScheduledTime: Union[datetime, str] = ...,
+        Runbooks: Sequence[RunbookUnionTypeDef],
+        ScheduledTime: TimestampTypeDef = ...,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ScheduledEndTime: Union[datetime, str] = ...,
+        ScheduledEndTime: TimestampTypeDef = ...,
         ChangeDetails: str = ...
     ) -> StartChangeRequestExecutionResultTypeDef:
         """
         Creates a change request for Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_change_request_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#start_change_request_execution)
@@ -2044,41 +2015,37 @@
         *,
         AssociationId: str,
         Parameters: Mapping[str, Sequence[str]] = ...,
         DocumentVersion: str = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         Name: str = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         AssociationName: str = ...,
         AssociationVersion: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_association)
         """
     def update_association_status(
-        self,
-        *,
-        Name: str,
-        InstanceId: str,
-        AssociationStatus: Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
+        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusUnionTypeDef
     ) -> UpdateAssociationStatusResultTypeDef:
         """
         Updates the status of the Amazon Web Services Systems Manager document (SSM
         document) associated with the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_association_status)
@@ -2144,15 +2111,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_maintenance_window)
         """
     def update_maintenance_window_target(
         self,
         *,
         WindowId: str,
         WindowTargetId: str,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
@@ -2161,37 +2128,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_maintenance_window_target)
         """
     def update_maintenance_window_task(
         self,
         *,
         WindowId: str,
         WindowTaskId: str,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         TaskArn: str = ...,
         ServiceRoleArn: str = ...,
         TaskParameters: Mapping[
-            str,
-            Union[
-                MaintenanceWindowTaskParameterValueExpressionTypeDef,
-                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-            ],
-        ] = ...,
-        TaskInvocationParameters: Union[
-            MaintenanceWindowTaskInvocationParametersTypeDef,
-            MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
         ] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_maintenance_window_task)
         """
@@ -2213,18 +2173,18 @@
         Notifications: Sequence[OpsItemNotificationTypeDef] = ...,
         Priority: int = ...,
         RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,
         Status: OpsItemStatusType = ...,
         Title: str = ...,
         Category: str = ...,
         Severity: str = ...,
-        ActualStartTime: Union[datetime, str] = ...,
-        ActualEndTime: Union[datetime, str] = ...,
-        PlannedStartTime: Union[datetime, str] = ...,
-        PlannedEndTime: Union[datetime, str] = ...,
+        ActualStartTime: TimestampTypeDef = ...,
+        ActualEndTime: TimestampTypeDef = ...,
+        PlannedStartTime: TimestampTypeDef = ...,
+        PlannedEndTime: TimestampTypeDef = ...,
         OpsItemArn: str = ...
     ) -> Dict[str, Any]:
         """
         Edit or change an OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_ops_item)
@@ -2244,23 +2204,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_ops_metadata)
         """
     def update_patch_baseline(
         self,
         *,
         BaselineId: str,
         Name: str = ...,
-        GlobalFilters: Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef] = ...,
-        ApprovalRules: Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef] = ...,
+        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
+        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]] = ...,
+        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
         Replace: bool = ...
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_patch_baseline)
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/literals.py` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/literals.pyi` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/paginator.py` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     list_ops_item_events_paginator: ListOpsItemEventsPaginator = client.get_paginator("list_ops_item_events")
     list_ops_item_related_items_paginator: ListOpsItemRelatedItemsPaginator = client.get_paginator("list_ops_item_related_items")
     list_ops_metadata_paginator: ListOpsMetadataPaginator = client.get_paginator("list_ops_metadata")
     list_resource_compliance_summaries_paginator: ListResourceComplianceSummariesPaginator = client.get_paginator("list_resource_compliance_summaries")
     list_resource_data_sync_paginator: ListResourceDataSyncPaginator = client.get_paginator("list_resource_data_sync")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     MaintenanceWindowResourceTypeType,
     OperatingSystemType,
     PatchPropertyType,
@@ -195,16 +195,15 @@
     PaginatorConfigTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     ResultAttributeTypeDef,
     SessionFilterTypeDef,
     StepExecutionFilterTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
+    TargetUnionTypeDef,
 )
 
 __all__ = (
     "DescribeActivationsPaginator",
     "DescribeAssociationExecutionTargetsPaginator",
     "DescribeAssociationExecutionsPaginator",
     "DescribeAutomationExecutionsPaginator",
@@ -573,15 +572,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
@@ -649,15 +648,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
     """
 
     def paginate(
         self,
         *,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        Targets: Sequence[TargetUnionTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/paginator.pyi` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     list_ops_item_events_paginator: ListOpsItemEventsPaginator = client.get_paginator("list_ops_item_events")
     list_ops_item_related_items_paginator: ListOpsItemRelatedItemsPaginator = client.get_paginator("list_ops_item_related_items")
     list_ops_metadata_paginator: ListOpsMetadataPaginator = client.get_paginator("list_ops_metadata")
     list_resource_compliance_summaries_paginator: ListResourceComplianceSummariesPaginator = client.get_paginator("list_resource_compliance_summaries")
     list_resource_data_sync_paginator: ListResourceDataSyncPaginator = client.get_paginator("list_resource_data_sync")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     MaintenanceWindowResourceTypeType,
     OperatingSystemType,
     PatchPropertyType,
@@ -195,16 +195,15 @@
     PaginatorConfigTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     ResultAttributeTypeDef,
     SessionFilterTypeDef,
     StepExecutionFilterTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
+    TargetUnionTypeDef,
 )
 
 __all__ = (
     "DescribeActivationsPaginator",
     "DescribeAssociationExecutionTargetsPaginator",
     "DescribeAssociationExecutionsPaginator",
     "DescribeAutomationExecutionsPaginator",
@@ -553,15 +552,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
@@ -625,15 +624,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
     """
 
     def paginate(
         self,
         *,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        Targets: Sequence[TargetUnionTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/type_defs.py` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ssm.type_defs import AccountSharingInfoTypeDef
 
-    data: AccountSharingInfoTypeDef = {...}
+    data: AccountSharingInfoTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -101,56 +101,54 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountSharingInfoTypeDef",
     "TagTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
     "AssociationStatusOutputTypeDef",
     "TargetOutputTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
-    "AssociationStatusTypeDef",
+    "TimestampTypeDef",
     "AttachmentContentTypeDef",
     "AttachmentInformationTypeDef",
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
+    "BlobTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
     "NotificationConfigOutputTypeDef",
     "ComplianceExecutionSummaryOutputTypeDef",
-    "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
     "TargetTypeDef",
     "DocumentRequiresTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
     "MetadataValueTypeDef",
-    "PatchSourceOutputTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
@@ -227,14 +225,15 @@
     "OpsResultAttributeTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
+    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
@@ -251,15 +250,14 @@
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
     "MaintenanceWindowLambdaParametersOutputTypeDef",
-    "MaintenanceWindowLambdaParametersTypeDef",
     "NotificationConfigTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
     "OpsItemIdentityTypeDef",
     "ParameterInlinePolicyTypeDef",
@@ -335,33 +333,32 @@
     "AssociationTypeDef",
     "MaintenanceWindowTargetTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
     "ListAssociationsRequestRequestTypeDef",
-    "UpdateAssociationStatusRequestRequestTypeDef",
+    "AssociationStatusTypeDef",
+    "ComplianceExecutionSummaryTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
+    "MaintenanceWindowLambdaParametersTypeDef",
     "GetCommandInvocationResultTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
     "MaintenanceWindowRunCommandParametersOutputTypeDef",
     "ComplianceItemTypeDef",
-    "PutComplianceItemsRequestRequestTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    "TargetUnionTypeDef",
     "CreateDocumentRequestRequestTypeDef",
     "DocumentIdentifierTypeDef",
     "GetDocumentResultTypeDef",
     "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
     "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
@@ -374,15 +371,14 @@
     "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
@@ -394,16 +390,14 @@
     "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     "DescribePatchBaselinesRequestRequestTypeDef",
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     "DescribePatchGroupsRequestRequestTypeDef",
     "DescribeAvailablePatchesResultTypeDef",
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
@@ -455,14 +449,15 @@
     "GetInventoryRequestRequestTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
+    "PatchSourceUnionTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
@@ -473,14 +468,16 @@
     "ListOpsItemEventsRequestRequestTypeDef",
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
     "MaintenanceWindowRunCommandParametersTypeDef",
+    "NotificationConfigUnionTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionUnionTypeDef",
     "OpsEntityTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
     "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
@@ -491,24 +488,35 @@
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     "MaintenanceWindowTaskTypeDef",
     "TargetLocationOutputTypeDef",
-    "SendCommandRequestRequestTypeDef",
+    "AlarmConfigurationUnionTypeDef",
     "TargetLocationTypeDef",
     "ListAssociationsResultTypeDef",
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
+    "AssociationStatusUnionTypeDef",
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    "ComplianceExecutionSummaryUnionTypeDef",
+    "PutComplianceItemsRequestRequestTypeDef",
     "ListCommandInvocationsResultTypeDef",
     "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    "SendCommandRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "ListDocumentsResultTypeDef",
     "DescribeOpsItemsResponseTypeDef",
     "GetOpsItemResponseTypeDef",
     "DescribePatchGroupsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
@@ -525,14 +533,15 @@
     "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
     "PatchRuleOutputTypeDef",
+    "PatchFilterGroupUnionTypeDef",
     "PatchRuleTypeDef",
     "ResourceDataSyncSourceWithStateTypeDef",
     "ResourceDataSyncSourceTypeDef",
     "DescribeSessionsResponseTypeDef",
     "DescribeAssociationExecutionsResultTypeDef",
     "ListCommandsResultTypeDef",
     "SendCommandResultTypeDef",
@@ -540,25 +549,24 @@
     "DescribeMaintenanceWindowTasksResultTypeDef",
     "AssociationDescriptionTypeDef",
     "AssociationVersionInfoTypeDef",
     "CreateAssociationBatchRequestEntryOutputTypeDef",
     "RunbookOutputTypeDef",
     "StepExecutionTypeDef",
     "CreateAssociationBatchRequestEntryTypeDef",
-    "CreateAssociationRequestRequestTypeDef",
     "RunbookTypeDef",
-    "StartAutomationExecutionRequestRequestTypeDef",
-    "UpdateAssociationRequestRequestTypeDef",
+    "TargetLocationUnionTypeDef",
     "GetMaintenanceWindowTaskResultTypeDef",
     "UpdateMaintenanceWindowTaskResultTypeDef",
     "ListComplianceSummariesResultTypeDef",
     "ListResourceComplianceSummariesResultTypeDef",
     "ListDocumentMetadataHistoryResponseTypeDef",
     "DescribeInstanceAssociationsStatusResultTypeDef",
     "DescribeInventoryDeletionsResultTypeDef",
+    "MaintenanceWindowTaskInvocationParametersUnionTypeDef",
     "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
     "PatchRuleGroupOutputTypeDef",
     "PatchRuleGroupTypeDef",
     "ResourceDataSyncItemTypeDef",
     "CreateResourceDataSyncRequestRequestTypeDef",
     "UpdateResourceDataSyncRequestRequestTypeDef",
@@ -567,25 +575,31 @@
     "UpdateAssociationResultTypeDef",
     "UpdateAssociationStatusResultTypeDef",
     "ListAssociationVersionsResultTypeDef",
     "FailedCreateAssociationTypeDef",
     "AutomationExecutionMetadataTypeDef",
     "AutomationExecutionTypeDef",
     "DescribeAutomationStepExecutionsResultTypeDef",
-    "CreateAssociationBatchRequestRequestTypeDef",
-    "StartChangeRequestExecutionRequestRequestTypeDef",
+    "CreateAssociationBatchRequestEntryUnionTypeDef",
+    "RunbookUnionTypeDef",
+    "CreateAssociationRequestRequestTypeDef",
+    "StartAutomationExecutionRequestRequestTypeDef",
+    "UpdateAssociationRequestRequestTypeDef",
     "GetPatchBaselineResultTypeDef",
     "UpdatePatchBaselineResultTypeDef",
     "BaselineOverrideTypeDef",
     "CreatePatchBaselineRequestRequestTypeDef",
+    "PatchRuleGroupUnionTypeDef",
     "UpdatePatchBaselineRequestRequestTypeDef",
     "ListResourceDataSyncResultTypeDef",
     "CreateAssociationBatchResultTypeDef",
     "DescribeAutomationExecutionsResultTypeDef",
     "GetAutomationExecutionResultTypeDef",
+    "CreateAssociationBatchRequestRequestTypeDef",
+    "StartChangeRequestExecutionRequestRequestTypeDef",
     "GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
 )
 
 AccountSharingInfoTypeDef = TypedDict(
     "AccountSharingInfoTypeDef",
     {
         "AccountId": str,
@@ -660,21 +674,19 @@
     "_OptionalAssociationStatusOutputTypeDef",
     {
         "AdditionalInfo": str,
     },
     total=False,
 )
 
-
 class AssociationStatusOutputTypeDef(
     _RequiredAssociationStatusOutputTypeDef, _OptionalAssociationStatusOutputTypeDef
 ):
     pass
 
-
 TargetOutputTypeDef = TypedDict(
     "TargetOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
     },
     total=False,
@@ -710,37 +722,15 @@
     "AssociationFilterTypeDef",
     {
         "key": AssociationFilterKeyType,
         "value": str,
     },
 )
 
-_RequiredAssociationStatusTypeDef = TypedDict(
-    "_RequiredAssociationStatusTypeDef",
-    {
-        "Date": Union[datetime, str],
-        "Name": AssociationStatusNameType,
-        "Message": str,
-    },
-)
-_OptionalAssociationStatusTypeDef = TypedDict(
-    "_OptionalAssociationStatusTypeDef",
-    {
-        "AdditionalInfo": str,
-    },
-    total=False,
-)
-
-
-class AssociationStatusTypeDef(
-    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 AttachmentContentTypeDef = TypedDict(
     "AttachmentContentTypeDef",
     {
         "Name": str,
         "Size": int,
         "Hash": str,
         "HashType": Literal["Sha256"],
@@ -801,35 +791,34 @@
     {
         "Name": str,
         "Products": Sequence[str],
         "Configuration": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCancelCommandRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCommandRequestRequestTypeDef",
     {
         "CommandId": str,
     },
 )
 _OptionalCancelCommandRequestRequestTypeDef = TypedDict(
     "_OptionalCancelCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CancelCommandRequestRequestTypeDef(
     _RequiredCancelCommandRequestRequestTypeDef, _OptionalCancelCommandRequestRequestTypeDef
 ):
     pass
 
-
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
@@ -890,44 +879,20 @@
     {
         "ExecutionId": str,
         "ExecutionType": str,
     },
     total=False,
 )
 
-
 class ComplianceExecutionSummaryOutputTypeDef(
     _RequiredComplianceExecutionSummaryOutputTypeDef,
     _OptionalComplianceExecutionSummaryOutputTypeDef,
 ):
     pass
 
-
-_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
-    "_RequiredComplianceExecutionSummaryTypeDef",
-    {
-        "ExecutionTime": Union[datetime, str],
-    },
-)
-_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
-    "_OptionalComplianceExecutionSummaryTypeDef",
-    {
-        "ExecutionId": str,
-        "ExecutionType": str,
-    },
-    total=False,
-)
-
-
-class ComplianceExecutionSummaryTypeDef(
-    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
-):
-    pass
-
-
 _RequiredComplianceItemEntryTypeDef = TypedDict(
     "_RequiredComplianceItemEntryTypeDef",
     {
         "Severity": ComplianceSeverityType,
         "Status": ComplianceStatusType,
     },
 )
@@ -937,21 +902,19 @@
         "Id": str,
         "Title": str,
         "Details": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ComplianceItemEntryTypeDef(
     _RequiredComplianceItemEntryTypeDef, _OptionalComplianceItemEntryTypeDef
 ):
     pass
 
-
 ComplianceStringFilterTypeDef = TypedDict(
     "ComplianceStringFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "Type": ComplianceQueryOperatorTypeType,
     },
@@ -1000,19 +963,17 @@
         "Version": str,
         "RequireType": str,
         "VersionName": str,
     },
     total=False,
 )
 
-
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
-
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
     total=False,
@@ -1037,23 +998,14 @@
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-PatchSourceOutputTypeDef = TypedDict(
-    "PatchSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Products": List[str],
-        "Configuration": str,
-    },
-)
-
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -1079,21 +1031,19 @@
         "DocumentVersion": str,
         "VersionName": str,
         "Force": bool,
     },
     total=False,
 )
 
-
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteInventoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInventoryRequestRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalDeleteInventoryRequestRequestTypeDef = TypedDict(
@@ -1102,21 +1052,19 @@
         "SchemaDeleteOption": InventorySchemaDeleteOptionType,
         "DryRun": bool,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteInventoryRequestRequestTypeDef(
     _RequiredDeleteInventoryRequestRequestTypeDef, _OptionalDeleteInventoryRequestRequestTypeDef
 ):
     pass
 
-
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
@@ -1158,22 +1106,20 @@
     "_OptionalDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
     },
     total=False,
 )
 
-
 class DeleteResourceDataSyncRequestRequestTypeDef(
     _RequiredDeleteResourceDataSyncRequestRequestTypeDef,
     _OptionalDeleteResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "PolicyId": str,
         "PolicyHash": str,
     },
@@ -1205,22 +1151,20 @@
     "_OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "Safe": bool,
     },
     total=False,
 )
 
-
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -1314,22 +1258,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeDocumentPermissionRequestRequestTypeDef(
     _RequiredDescribeDocumentPermissionRequestRequestTypeDef,
     _OptionalDescribeDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeDocumentRequestRequestTypeDef = TypedDict(
@@ -1337,21 +1279,19 @@
     {
         "DocumentVersion": str,
         "VersionName": str,
     },
     total=False,
 )
 
-
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
@@ -1359,22 +1299,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEffectiveInstanceAssociationsRequestRequestTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceAssociationTypeDef = TypedDict(
     "InstanceAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
@@ -1393,22 +1331,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
@@ -1416,22 +1352,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeInstanceAssociationsStatusRequestRequestTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceInformationFilterTypeDef = TypedDict(
     "InstanceInformationFilterTypeDef",
     {
         "key": InstanceInformationFilterKeyType,
         "valueSet": Sequence[str],
     },
 )
@@ -1483,21 +1417,19 @@
         "CriticalNonCompliantCount": int,
         "SecurityNonCompliantCount": int,
         "OtherNonCompliantCount": int,
     },
     total=False,
 )
 
-
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
-
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
@@ -1505,22 +1437,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPatchComplianceDataTypeDef = TypedDict(
     "_RequiredPatchComplianceDataTypeDef",
     {
         "Title": str,
         "KBId": str,
         "Classification": str,
         "Severity": str,
@@ -1532,21 +1462,19 @@
     "_OptionalPatchComplianceDataTypeDef",
     {
         "CVEIds": str,
     },
     total=False,
 )
 
-
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
-
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1652,21 +1580,19 @@
     {
         "Option": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-
 class ParameterStringFilterTypeDef(
     _RequiredParameterStringFilterTypeDef, _OptionalParameterStringFilterTypeDef
 ):
     pass
 
-
 ParametersFilterTypeDef = TypedDict(
     "ParametersFilterTypeDef",
     {
         "Key": ParametersFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -1703,22 +1629,20 @@
         "PatchSet": PatchSetType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
-
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
 )
@@ -1842,21 +1766,19 @@
     "_OptionalGetCalendarStateRequestRequestTypeDef",
     {
         "AtTime": str,
     },
     total=False,
 )
 
-
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1873,22 +1795,20 @@
     "_OptionalGetCommandInvocationRequestRequestTypeDef",
     {
         "PluginName": str,
     },
     total=False,
 )
 
-
 class GetCommandInvocationRequestRequestTypeDef(
     _RequiredGetCommandInvocationRequestRequestTypeDef,
     _OptionalGetCommandInvocationRequestRequestTypeDef,
 ):
     pass
 
-
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
@@ -1912,21 +1832,19 @@
         "VersionName": str,
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
     },
     total=False,
 )
 
-
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredInventoryFilterTypeDef = TypedDict(
     "_RequiredInventoryFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -1934,19 +1852,17 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Type": InventoryQueryOperatorTypeType,
     },
     total=False,
 )
 
-
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
-
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
@@ -2020,40 +1936,36 @@
     "_OptionalLoggingInfoTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-
 class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
     pass
 
-
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalGetOpsItemRequestRequestTypeDef = TypedDict(
     "_OptionalGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemArn": str,
     },
     total=False,
 )
 
-
 class GetOpsItemRequestRequestTypeDef(
     _RequiredGetOpsItemRequestRequestTypeDef, _OptionalGetOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalGetOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -2061,21 +1973,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2083,19 +1993,17 @@
     "_OptionalOpsFilterTypeDef",
     {
         "Type": OpsFilterOperatorTypeType,
     },
     total=False,
 )
 
-
 class OpsFilterTypeDef(_RequiredOpsFilterTypeDef, _OptionalOpsFilterTypeDef):
     pass
 
-
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
@@ -2111,43 +2019,39 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetParameterHistoryRequestRequestTypeDef(
     _RequiredGetParameterHistoryRequestRequestTypeDef,
     _OptionalGetParameterHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetParameterRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterRequestRequestTypeDef = TypedDict(
     "_OptionalGetParameterRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
-
 class GetParameterRequestRequestTypeDef(
     _RequiredGetParameterRequestRequestTypeDef, _OptionalGetParameterRequestRequestTypeDef
 ):
     pass
 
-
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Value": str,
         "Version": int,
@@ -2170,50 +2074,55 @@
     "_OptionalGetParametersRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
-
 class GetParametersRequestRequestTypeDef(
     _RequiredGetParametersRequestRequestTypeDef, _OptionalGetParametersRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
-
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
+PatchSourceOutputTypeDef = TypedDict(
+    "PatchSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Products": List[str],
+        "Configuration": str,
+    },
+)
+
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -2221,22 +2130,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesResponseEntryTypeDef = TypedDict(
     "GetResourcePoliciesResponseEntryTypeDef",
     {
         "PolicyId": str,
         "PolicyHash": str,
         "Policy": str,
     },
@@ -2322,19 +2229,17 @@
         "ContentHash": str,
         "Content": Sequence[Mapping[str, str]],
         "Context": Mapping[str, str],
     },
     total=False,
 )
 
-
 class InventoryItemTypeDef(_RequiredInventoryItemTypeDef, _OptionalInventoryItemTypeDef):
     pass
 
-
 _RequiredInventoryResultItemTypeDef = TypedDict(
     "_RequiredInventoryResultItemTypeDef",
     {
         "TypeName": str,
         "SchemaVersion": str,
         "Content": List[Dict[str, str]],
     },
@@ -2344,21 +2249,19 @@
     {
         "CaptureTime": str,
         "ContentHash": str,
     },
     total=False,
 )
 
-
 class InventoryResultItemTypeDef(
     _RequiredInventoryResultItemTypeDef, _OptionalInventoryResultItemTypeDef
 ):
     pass
 
-
 _RequiredLabelParameterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredLabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "Labels": Sequence[str],
     },
 )
@@ -2366,22 +2269,20 @@
     "_OptionalLabelParameterVersionRequestRequestTypeDef",
     {
         "ParameterVersion": int,
     },
     total=False,
 )
 
-
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestRequestTypeDef = TypedDict(
@@ -2389,22 +2290,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociationVersionsRequestRequestTypeDef(
     _RequiredListAssociationVersionsRequestRequestTypeDef,
     _OptionalListAssociationVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDocumentMetadataHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentMetadataHistoryRequestRequestTypeDef",
     {
         "Name": str,
         "Metadata": Literal["DocumentReviews"],
     },
 )
@@ -2414,22 +2313,20 @@
         "DocumentVersion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -2437,22 +2334,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
     },
@@ -2529,24 +2424,14 @@
         "ClientContext": str,
         "Qualifier": str,
         "Payload": bytes,
     },
     total=False,
 )
 
-MaintenanceWindowLambdaParametersTypeDef = TypedDict(
-    "MaintenanceWindowLambdaParametersTypeDef",
-    {
-        "ClientContext": str,
-        "Qualifier": str,
-        "Payload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 NotificationConfigTypeDef = TypedDict(
     "NotificationConfigTypeDef",
     {
         "NotificationArn": str,
         "NotificationEvents": Sequence[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
@@ -2583,22 +2468,20 @@
         "AccountIdsToAdd": Sequence[str],
         "AccountIdsToRemove": Sequence[str],
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
-
 class ModifyDocumentPermissionRequestRequestTypeDef(
     _RequiredModifyDocumentPermissionRequestRequestTypeDef,
     _OptionalModifyDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
-
 OpsEntityItemTypeDef = TypedDict(
     "OpsEntityItemTypeDef",
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
@@ -2650,21 +2533,19 @@
     {
         "PolicyId": str,
         "PolicyHash": str,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
@@ -2726,22 +2607,20 @@
     "_OptionalSendAutomationSignalRequestRequestTypeDef",
     {
         "Payload": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class SendAutomationSignalRequestRequestTypeDef(
     _RequiredSendAutomationSignalRequestRequestTypeDef,
     _OptionalSendAutomationSignalRequestRequestTypeDef,
 ):
     pass
 
-
 SessionManagerOutputUrlTypeDef = TypedDict(
     "SessionManagerOutputUrlTypeDef",
     {
         "S3OutputUrl": str,
         "CloudWatchOutputUrl": str,
     },
     total=False,
@@ -2766,43 +2645,39 @@
         "DocumentName": str,
         "Reason": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_OptionalStopAutomationExecutionRequestRequestTypeDef",
     {
         "Type": StopTypeType,
     },
     total=False,
 )
 
-
 class StopAutomationExecutionRequestRequestTypeDef(
     _RequiredStopAutomationExecutionRequestRequestTypeDef,
     _OptionalStopAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
-
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -2844,22 +2719,20 @@
         "AllowUnassociatedTargets": bool,
         "Enabled": bool,
         "Replace": bool,
     },
     total=False,
 )
 
-
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
@@ -2918,22 +2791,20 @@
         "ScheduleOffset": int,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -2949,63 +2820,57 @@
         "Tier": ParameterTierType,
         "Policies": str,
         "DataType": str,
     },
     total=False,
 )
 
-
 class PutParameterRequestRequestTypeDef(
     _RequiredPutParameterRequestRequestTypeDef, _OptionalPutParameterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAlarmConfigurationOutputTypeDef = TypedDict(
     "_RequiredAlarmConfigurationOutputTypeDef",
     {
         "Alarms": List[AlarmTypeDef],
     },
 )
 _OptionalAlarmConfigurationOutputTypeDef = TypedDict(
     "_OptionalAlarmConfigurationOutputTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
-
 class AlarmConfigurationOutputTypeDef(
     _RequiredAlarmConfigurationOutputTypeDef, _OptionalAlarmConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredAlarmConfigurationTypeDef = TypedDict(
     "_RequiredAlarmConfigurationTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
 )
 _OptionalAlarmConfigurationTypeDef = TypedDict(
     "_OptionalAlarmConfigurationTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
-
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
-
 AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
     "AssociateOpsItemRelatedItemResponseTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3480,22 +3345,20 @@
         "Filters": Sequence[AssociationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 AssociationExecutionTargetTypeDef = TypedDict(
     "AssociationExecutionTargetTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "ResourceId": str,
@@ -3521,40 +3384,70 @@
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 ListAssociationsRequestRequestTypeDef = TypedDict(
     "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
-    "UpdateAssociationStatusRequestRequestTypeDef",
+_RequiredAssociationStatusTypeDef = TypedDict(
+    "_RequiredAssociationStatusTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationStatus": AssociationStatusTypeDef,
+        "Date": TimestampTypeDef,
+        "Name": AssociationStatusNameType,
+        "Message": str,
+    },
+)
+_OptionalAssociationStatusTypeDef = TypedDict(
+    "_OptionalAssociationStatusTypeDef",
+    {
+        "AdditionalInfo": str,
+    },
+    total=False,
+)
+
+class AssociationStatusTypeDef(
+    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+):
+    pass
+
+_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryTypeDef",
+    {
+        "ExecutionTime": TimestampTypeDef,
     },
 )
+_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryTypeDef",
+    {
+        "ExecutionId": str,
+        "ExecutionType": str,
+    },
+    total=False,
+)
+
+class ComplianceExecutionSummaryTypeDef(
+    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
+):
+    pass
 
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
@@ -3568,31 +3461,39 @@
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
     },
     total=False,
 )
 
-
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
-
 DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+MaintenanceWindowLambdaParametersTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersTypeDef",
+    {
+        "ClientContext": str,
+        "Qualifier": str,
+        "Payload": BlobTypeDef,
+    },
+    total=False,
+)
+
 GetCommandInvocationResultTypeDef = TypedDict(
     "GetCommandInvocationResultTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "Comment": str,
         "DocumentName": str,
@@ -3691,41 +3592,14 @@
         "Severity": ComplianceSeverityType,
         "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "Details": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": str,
-        "ComplianceType": str,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
-        "Items": Sequence[ComplianceItemEntryTypeDef],
-    },
-)
-_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ItemContentHash": str,
-        "UploadType": ComplianceUploadTypeType,
-    },
-    total=False,
-)
-
-
-class PutComplianceItemsRequestRequestTypeDef(
-    _RequiredPutComplianceItemsRequestRequestTypeDef,
-    _OptionalPutComplianceItemsRequestRequestTypeDef,
-):
-    pass
-
-
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
@@ -3780,106 +3654,27 @@
 )
 _OptionalCreateActivationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateActivationRequestRequestTypeDef",
     {
         "Description": str,
         "DefaultInstanceName": str,
         "RegistrationLimit": int,
-        "ExpirationDate": Union[datetime, str],
+        "ExpirationDate": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "RegistrationMetadata": Sequence[RegistrationMetadataItemTypeDef],
     },
     total=False,
 )
 
-
 class CreateActivationRequestRequestTypeDef(
     _RequiredCreateActivationRequestRequestTypeDef, _OptionalCreateActivationRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-    },
-)
-_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-    },
-)
-_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
-    {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
-        "Replace": bool,
-    },
-    total=False,
-)
-
-
-class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-):
-    pass
-
-
+TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 _RequiredCreateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3894,21 +3689,19 @@
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDocumentRequestRequestTypeDef(
     _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
 ):
     pass
 
-
 DocumentIdentifierTypeDef = TypedDict(
     "DocumentIdentifierTypeDef",
     {
         "Name": str,
         "CreatedDate": datetime,
         "DisplayName": str,
         "Owner": str,
@@ -3986,30 +3779,28 @@
         "OperationalData": Mapping[str, OpsItemDataValueTypeDef],
         "Notifications": Sequence[OpsItemNotificationTypeDef],
         "Priority": int,
         "RelatedOpsItems": Sequence[RelatedOpsItemTypeDef],
         "Tags": Sequence[TagTypeDef],
         "Category": str,
         "Severity": str,
-        "ActualStartTime": Union[datetime, str],
-        "ActualEndTime": Union[datetime, str],
-        "PlannedStartTime": Union[datetime, str],
-        "PlannedEndTime": Union[datetime, str],
+        "ActualStartTime": TimestampTypeDef,
+        "ActualEndTime": TimestampTypeDef,
+        "PlannedStartTime": TimestampTypeDef,
+        "PlannedEndTime": TimestampTypeDef,
         "AccountId": str,
     },
     total=False,
 )
 
-
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 OpsItemTypeDef = TypedDict(
     "OpsItemTypeDef",
     {
         "CreatedBy": str,
         "OpsItemType": str,
         "CreatedTime": datetime,
         "Description": str,
@@ -4050,30 +3841,28 @@
         "Notifications": Sequence[OpsItemNotificationTypeDef],
         "Priority": int,
         "RelatedOpsItems": Sequence[RelatedOpsItemTypeDef],
         "Status": OpsItemStatusType,
         "Title": str,
         "Category": str,
         "Severity": str,
-        "ActualStartTime": Union[datetime, str],
-        "ActualEndTime": Union[datetime, str],
-        "PlannedStartTime": Union[datetime, str],
-        "PlannedEndTime": Union[datetime, str],
+        "ActualStartTime": TimestampTypeDef,
+        "ActualEndTime": TimestampTypeDef,
+        "PlannedStartTime": TimestampTypeDef,
+        "PlannedEndTime": TimestampTypeDef,
         "OpsItemArn": str,
     },
     total=False,
 )
 
-
 class UpdateOpsItemRequestRequestTypeDef(
     _RequiredUpdateOpsItemRequestRequestTypeDef, _OptionalUpdateOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalCreateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -4081,21 +3870,19 @@
     {
         "Metadata": Mapping[str, MetadataValueTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-
 GetOpsMetadataResultTypeDef = TypedDict(
     "GetOpsMetadataResultTypeDef",
     {
         "ResourceId": str,
         "Metadata": Dict[str, MetadataValueTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4113,21 +3900,19 @@
     {
         "MetadataToUpdate": Mapping[str, MetadataValueTypeDef],
         "KeysToDelete": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-
 DescribeActivationsRequestRequestTypeDef = TypedDict(
     "DescribeActivationsRequestRequestTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -4155,22 +3940,20 @@
     {
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
         {
             "AssociationId": str,
         },
     )
@@ -4182,22 +3965,20 @@
             "Filters": Sequence[AssociationExecutionFilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
-
 class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
     _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
 ):
     pass
 
-
 DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4213,120 +3994,89 @@
     "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
     "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
 ):
     pass
 
-
 DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     {
         "DeletionId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -4335,22 +4085,20 @@
     {
         "PatchSet": PatchSetType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
     _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
 ):
     pass
 
-
 GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
     "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     {
         "TypeName": str,
         "Aggregator": bool,
         "SubType": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4369,66 +4117,60 @@
     {
         "WithDecryption": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
     _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
     _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
     "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
     _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
     "ListAssociationsRequestListAssociationsPaginateTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4487,22 +4229,20 @@
     "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
     _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4529,22 +4269,20 @@
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
@@ -4554,22 +4292,20 @@
         "NextToken": str,
         "MaxResults": int,
         "ReverseOrder": bool,
     },
     total=False,
 )
 
-
 class DescribeAutomationStepExecutionsRequestRequestTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4596,22 +4332,20 @@
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
@@ -4620,49 +4354,20 @@
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchesRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
-    TypedDict(
-        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-        {
-            "WindowId": str,
-            "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-            "ResourceType": MaintenanceWindowResourceTypeType,
-            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4747,22 +4452,20 @@
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
@@ -4771,22 +4474,20 @@
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4822,22 +4523,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -4847,22 +4546,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
@@ -4870,22 +4567,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
@@ -4894,22 +4589,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
@@ -4917,22 +4610,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
@@ -4941,22 +4632,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
@@ -4964,22 +4653,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
@@ -4988,22 +4675,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTargetsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
@@ -5011,22 +4696,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
@@ -5035,22 +4718,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -5145,22 +4826,20 @@
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
     _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetParametersByPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetParametersByPathRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalGetParametersByPathRequestRequestTypeDef = TypedDict(
@@ -5171,22 +4850,20 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetParametersByPathRequestRequestTypeDef(
     _RequiredGetParametersByPathRequestRequestTypeDef,
     _OptionalGetParametersByPathRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5233,22 +4910,20 @@
     {
         "Filters": Sequence[SessionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestRequestTypeDef = TypedDict(
@@ -5257,21 +4932,19 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[SessionFilterTypeDef],
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
-
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5356,19 +5029,17 @@
     "_OptionalDocumentReviewsTypeDef",
     {
         "Comment": Sequence[DocumentReviewCommentSourceTypeDef],
     },
     total=False,
 )
 
-
 class DocumentReviewsTypeDef(_RequiredDocumentReviewsTypeDef, _OptionalDocumentReviewsTypeDef):
     pass
 
-
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5395,22 +5066,20 @@
     {
         "PluginName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetCommandInvocationRequestCommandExecutedWaitTypeDef(
     _RequiredGetCommandInvocationRequestCommandExecutedWaitTypeDef,
     _OptionalGetCommandInvocationRequestCommandExecutedWaitTypeDef,
 ):
     pass
 
-
 InventoryGroupTypeDef = TypedDict(
     "InventoryGroupTypeDef",
     {
         "Name": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
 )
@@ -5428,22 +5097,20 @@
         "Filters": Sequence[InventoryFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInventoryEntriesRequestRequestTypeDef(
     _RequiredListInventoryEntriesRequestRequestTypeDef,
     _OptionalListInventoryEntriesRequestRequestTypeDef,
 ):
     pass
 
-
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -5523,14 +5190,15 @@
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PatchSourceUnionTypeDef = Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5618,21 +5286,19 @@
     {
         "Version": str,
         "DisplayName": str,
     },
     total=False,
 )
 
-
 class InventoryItemSchemaTypeDef(
     _RequiredInventoryItemSchemaTypeDef, _OptionalInventoryItemSchemaTypeDef
 ):
     pass
 
-
 PutInventoryRequestRequestTypeDef = TypedDict(
     "PutInventoryRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Items": Sequence[InventoryItemTypeDef],
     },
 )
@@ -5728,14 +5394,19 @@
         "Parameters": Mapping[str, Sequence[str]],
         "ServiceRoleArn": str,
         "TimeoutSeconds": int,
     },
     total=False,
 )
 
+NotificationConfigUnionTypeDef = Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef]
+MaintenanceWindowTaskParameterValueExpressionUnionTypeDef = Union[
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+]
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
@@ -5833,44 +5504,40 @@
     "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     {
         "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
-
 class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
 ):
     pass
 
-
 _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationalUnits": Sequence[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
-
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
-
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
     },
@@ -5881,21 +5548,19 @@
         "Prefix": str,
         "AWSKMSKeyARN": str,
         "DestinationDataSharing": ResourceDataSyncDestinationDataSharingTypeDef,
     },
     total=False,
 )
 
-
 class ResourceDataSyncS3DestinationTypeDef(
     _RequiredResourceDataSyncS3DestinationTypeDef, _OptionalResourceDataSyncS3DestinationTypeDef
 ):
     pass
 
-
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "SessionId": str,
         "Target": str,
         "Status": SessionStatusType,
         "StartDate": datetime,
@@ -6041,51 +5706,15 @@
         "TargetLocationMaxErrors": str,
         "ExecutionRoleName": str,
         "TargetLocationAlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredSendCommandRequestRequestTypeDef = TypedDict(
-    "_RequiredSendCommandRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalSendCommandRequestRequestTypeDef = TypedDict(
-    "_OptionalSendCommandRequestRequestTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "DocumentVersion": str,
-        "DocumentHash": str,
-        "DocumentHashType": DocumentHashTypeType,
-        "TimeoutSeconds": int,
-        "Comment": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "OutputS3Region": str,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "ServiceRoleArn": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class SendCommandRequestRequestTypeDef(
-    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
-):
-    pass
-
-
+AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
 TargetLocationTypeDef = TypedDict(
     "TargetLocationTypeDef",
     {
         "Accounts": Sequence[str],
         "Regions": Sequence[str],
         "TargetLocationMaxConcurrency": str,
         "TargetLocationMaxErrors": str,
@@ -6118,14 +5747,52 @@
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AssociationStatusUnionTypeDef = Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
+UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationStatus": AssociationStatusTypeDef,
+    },
+)
+
+ComplianceExecutionSummaryUnionTypeDef = Union[
+    ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
+]
+_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": str,
+        "ComplianceType": str,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "Items": Sequence[ComplianceItemEntryTypeDef],
+    },
+)
+_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ItemContentHash": str,
+        "UploadType": ComplianceUploadTypeType,
+    },
+    total=False,
+)
+
+class PutComplianceItemsRequestRequestTypeDef(
+    _RequiredPutComplianceItemsRequestRequestTypeDef,
+    _OptionalPutComplianceItemsRequestRequestTypeDef,
+):
+    pass
+
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6172,14 +5839,169 @@
         "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
+DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
+    TypedDict(
+        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+        {
+            "WindowId": str,
+            "Targets": Sequence[TargetUnionTypeDef],
+            "ResourceType": MaintenanceWindowResourceTypeType,
+            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+):
+    pass
+
+_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": Sequence[TargetUnionTypeDef],
+    },
+)
+_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSendCommandRequestRequestTypeDef = TypedDict(
+    "_RequiredSendCommandRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalSendCommandRequestRequestTypeDef = TypedDict(
+    "_OptionalSendCommandRequestRequestTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "Targets": Sequence[TargetUnionTypeDef],
+        "DocumentVersion": str,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "TimeoutSeconds": int,
+        "Comment": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "OutputS3Region": str,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "ServiceRoleArn": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class SendCommandRequestRequestTypeDef(
+    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "Replace": bool,
+    },
+    total=False,
+)
+
+class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+):
+    pass
+
 ListDocumentsResultTypeDef = TypedDict(
     "ListDocumentsResultTypeDef",
     {
         "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6254,22 +6076,20 @@
     "_OptionalUpdateDocumentMetadataRequestRequestTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
-
 class UpdateDocumentMetadataRequestRequestTypeDef(
     _RequiredUpdateDocumentMetadataRequestRequestTypeDef,
     _OptionalUpdateDocumentMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6424,19 +6244,18 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
-
 class PatchRuleOutputTypeDef(_RequiredPatchRuleOutputTypeDef, _OptionalPatchRuleOutputTypeDef):
     pass
 
-
+PatchFilterGroupUnionTypeDef = Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef]
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
     },
 )
 _OptionalPatchRuleTypeDef = TypedDict(
@@ -6446,19 +6265,17 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
-
 class PatchRuleTypeDef(_RequiredPatchRuleTypeDef, _OptionalPatchRuleTypeDef):
     pass
 
-
 ResourceDataSyncSourceWithStateTypeDef = TypedDict(
     "ResourceDataSyncSourceWithStateTypeDef",
     {
         "SourceType": str,
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
         "SourceRegions": List[str],
         "IncludeFutureRegions": bool,
@@ -6481,21 +6298,19 @@
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
         "IncludeFutureRegions": bool,
         "EnableAllOpsDataSources": bool,
     },
     total=False,
 )
 
-
 class ResourceDataSyncSourceTypeDef(
     _RequiredResourceDataSyncSourceTypeDef, _OptionalResourceDataSyncSourceTypeDef
 ):
     pass
 
-
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6633,22 +6448,20 @@
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class CreateAssociationBatchRequestEntryOutputTypeDef(
     _RequiredCreateAssociationBatchRequestEntryOutputTypeDef,
     _OptionalCreateAssociationBatchRequestEntryOutputTypeDef,
 ):
     pass
 
-
 _RequiredRunbookOutputTypeDef = TypedDict(
     "_RequiredRunbookOutputTypeDef",
     {
         "DocumentName": str,
     },
 )
 _OptionalRunbookOutputTypeDef = TypedDict(
@@ -6662,19 +6475,17 @@
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetLocations": List[TargetLocationOutputTypeDef],
     },
     total=False,
 )
 
-
 class RunbookOutputTypeDef(_RequiredRunbookOutputTypeDef, _OptionalRunbookOutputTypeDef):
     pass
 
-
 StepExecutionTypeDef = TypedDict(
     "StepExecutionTypeDef",
     {
         "StepName": str,
         "Action": str,
         "TimeoutSeconds": int,
         "OnFailure": str,
@@ -6728,61 +6539,20 @@
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateAssociationBatchRequestEntryTypeDef(
     _RequiredCreateAssociationBatchRequestEntryTypeDef,
     _OptionalCreateAssociationBatchRequestEntryTypeDef,
 ):
     pass
 
-
-_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAssociationRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAssociationRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "InstanceId": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "AssociationName": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateAssociationRequestRequestTypeDef(
-    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredRunbookTypeDef = TypedDict(
     "_RequiredRunbookTypeDef",
     {
         "DocumentName": str,
     },
 )
 _OptionalRunbookTypeDef = TypedDict(
@@ -6796,91 +6566,18 @@
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetLocations": Sequence[TargetLocationTypeDef],
     },
     total=False,
 )
 
-
 class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
     pass
 
-
-_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ClientToken": str,
-        "Mode": ExecutionModeType,
-        "TargetParameterName": str,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class StartAutomationExecutionRequestRequestTypeDef(
-    _RequiredStartAutomationExecutionRequestRequestTypeDef,
-    _OptionalStartAutomationExecutionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAssociationRequestRequestTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAssociationRequestRequestTypeDef",
-    {
-        "Parameters": Mapping[str, Sequence[str]],
-        "DocumentVersion": str,
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "Name": str,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "AssociationName": str,
-        "AssociationVersion": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateAssociationRequestRequestTypeDef(
-    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
-):
-    pass
-
-
+TargetLocationUnionTypeDef = Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]
 GetMaintenanceWindowTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
         "Targets": List[TargetOutputTypeDef],
         "TaskArn": str,
@@ -6966,98 +6663,86 @@
     {
         "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MaintenanceWindowTaskInvocationParametersUnionTypeDef = Union[
+    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+]
 _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
     },
 )
 _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        "Targets": Sequence[TargetUnionTypeDef],
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[
-            str,
-            Union[
-                MaintenanceWindowTaskParameterValueExpressionTypeDef,
-                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-            ],
-        ],
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "ClientToken": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
     _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
     _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        "Targets": Sequence[TargetUnionTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[
-            str,
-            Union[
-                MaintenanceWindowTaskParameterValueExpressionTypeDef,
-                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-            ],
-        ],
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "Replace": bool,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
 ):
     pass
 
-
 PatchRuleGroupOutputTypeDef = TypedDict(
     "PatchRuleGroupOutputTypeDef",
     {
         "PatchRules": List[PatchRuleOutputTypeDef],
     },
 )
 
@@ -7097,22 +6782,20 @@
         "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
     total=False,
 )
 
-
 class CreateResourceDataSyncRequestRequestTypeDef(
     _RequiredCreateResourceDataSyncRequestRequestTypeDef,
     _OptionalCreateResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "UpdateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
@@ -7251,56 +6934,122 @@
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssociationBatchRequestRequestTypeDef = TypedDict(
-    "CreateAssociationBatchRequestRequestTypeDef",
+CreateAssociationBatchRequestEntryUnionTypeDef = Union[
+    CreateAssociationBatchRequestEntryTypeDef, CreateAssociationBatchRequestEntryOutputTypeDef
+]
+RunbookUnionTypeDef = Union[RunbookTypeDef, RunbookOutputTypeDef]
+_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAssociationRequestRequestTypeDef",
     {
-        "Entries": Sequence[
-            Union[
-                CreateAssociationBatchRequestEntryTypeDef,
-                CreateAssociationBatchRequestEntryOutputTypeDef,
-            ]
-        ],
+        "Name": str,
+    },
+)
+_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAssociationRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "InstanceId": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "AssociationName": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
+    total=False,
 )
 
-_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+class CreateAssociationRequestRequestTypeDef(
+    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
+):
+    pass
+
+_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
     {
         "DocumentName": str,
-        "Runbooks": Sequence[Union[RunbookTypeDef, RunbookOutputTypeDef]],
     },
 )
-_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
     {
-        "ScheduledTime": Union[datetime, str],
         "DocumentVersion": str,
         "Parameters": Mapping[str, Sequence[str]],
-        "ChangeRequestName": str,
         "ClientToken": str,
-        "AutoApprove": bool,
+        "Mode": ExecutionModeType,
+        "TargetParameterName": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
-        "ScheduledEndTime": Union[datetime, str],
-        "ChangeDetails": str,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class StartChangeRequestExecutionRequestRequestTypeDef(
-    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
-    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+class StartAutomationExecutionRequestRequestTypeDef(
+    _RequiredStartAutomationExecutionRequestRequestTypeDef,
+    _OptionalStartAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAssociationRequestRequestTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAssociationRequestRequestTypeDef",
+    {
+        "Parameters": Mapping[str, Sequence[str]],
+        "DocumentVersion": str,
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "Name": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "AssociationName": str,
+        "AssociationVersion": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateAssociationRequestRequestTypeDef(
+    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
+):
+    pass
 
 GetPatchBaselineResultTypeDef = TypedDict(
     "GetPatchBaselineResultTypeDef",
     {
         "BaselineId": str,
         "Name": str,
         "OperatingSystem": OperatingSystemType,
@@ -7371,29 +7120,28 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]],
+        "Sources": Sequence[PatchSourceUnionTypeDef],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePatchBaselineRequestRequestTypeDef(
     _RequiredCreatePatchBaselineRequestRequestTypeDef,
     _OptionalCreatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
+PatchRuleGroupUnionTypeDef = Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef]
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
@@ -7404,28 +7152,26 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]],
+        "Sources": Sequence[PatchSourceUnionTypeDef],
         "Replace": bool,
     },
     total=False,
 )
 
-
 class UpdatePatchBaselineRequestRequestTypeDef(
     _RequiredUpdatePatchBaselineRequestRequestTypeDef,
     _OptionalUpdatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7453,14 +7199,50 @@
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAssociationBatchRequestRequestTypeDef = TypedDict(
+    "CreateAssociationBatchRequestRequestTypeDef",
+    {
+        "Entries": Sequence[CreateAssociationBatchRequestEntryUnionTypeDef],
+    },
+)
+
+_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+        "Runbooks": Sequence[RunbookUnionTypeDef],
+    },
+)
+_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "ScheduledTime": TimestampTypeDef,
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ChangeRequestName": str,
+        "ClientToken": str,
+        "AutoApprove": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ScheduledEndTime": TimestampTypeDef,
+        "ChangeDetails": str,
+    },
+    total=False,
+)
+
+class StartChangeRequestExecutionRequestRequestTypeDef(
+    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
+    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+):
+    pass
+
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "SnapshotId": str,
     },
 )
@@ -7468,13 +7250,12 @@
     "_OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "BaselineOverride": BaselineOverrideTypeDef,
     },
     total=False,
 )
 
-
 class GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef(
     _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
     _OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/type_defs.pyi` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ssm.type_defs import AccountSharingInfoTypeDef
 
-    data: AccountSharingInfoTypeDef = {...}
+    data: AccountSharingInfoTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -101,55 +101,55 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountSharingInfoTypeDef",
     "TagTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
     "AssociationStatusOutputTypeDef",
     "TargetOutputTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
-    "AssociationStatusTypeDef",
+    "TimestampTypeDef",
     "AttachmentContentTypeDef",
     "AttachmentInformationTypeDef",
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
+    "BlobTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
     "NotificationConfigOutputTypeDef",
     "ComplianceExecutionSummaryOutputTypeDef",
-    "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
     "TargetTypeDef",
     "DocumentRequiresTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
     "MetadataValueTypeDef",
-    "PatchSourceOutputTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
@@ -226,14 +226,15 @@
     "OpsResultAttributeTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
+    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
@@ -250,15 +251,14 @@
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
     "MaintenanceWindowLambdaParametersOutputTypeDef",
-    "MaintenanceWindowLambdaParametersTypeDef",
     "NotificationConfigTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
     "OpsItemIdentityTypeDef",
     "ParameterInlinePolicyTypeDef",
@@ -334,33 +334,32 @@
     "AssociationTypeDef",
     "MaintenanceWindowTargetTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
     "ListAssociationsRequestRequestTypeDef",
-    "UpdateAssociationStatusRequestRequestTypeDef",
+    "AssociationStatusTypeDef",
+    "ComplianceExecutionSummaryTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
+    "MaintenanceWindowLambdaParametersTypeDef",
     "GetCommandInvocationResultTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
     "MaintenanceWindowRunCommandParametersOutputTypeDef",
     "ComplianceItemTypeDef",
-    "PutComplianceItemsRequestRequestTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    "TargetUnionTypeDef",
     "CreateDocumentRequestRequestTypeDef",
     "DocumentIdentifierTypeDef",
     "GetDocumentResultTypeDef",
     "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
     "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
@@ -373,15 +372,14 @@
     "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
@@ -393,16 +391,14 @@
     "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     "DescribePatchBaselinesRequestRequestTypeDef",
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     "DescribePatchGroupsRequestRequestTypeDef",
     "DescribeAvailablePatchesResultTypeDef",
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
@@ -454,14 +450,15 @@
     "GetInventoryRequestRequestTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
+    "PatchSourceUnionTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
@@ -472,14 +469,16 @@
     "ListOpsItemEventsRequestRequestTypeDef",
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
     "MaintenanceWindowRunCommandParametersTypeDef",
+    "NotificationConfigUnionTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionUnionTypeDef",
     "OpsEntityTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
     "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
@@ -490,24 +489,35 @@
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     "MaintenanceWindowTaskTypeDef",
     "TargetLocationOutputTypeDef",
-    "SendCommandRequestRequestTypeDef",
+    "AlarmConfigurationUnionTypeDef",
     "TargetLocationTypeDef",
     "ListAssociationsResultTypeDef",
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
+    "AssociationStatusUnionTypeDef",
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    "ComplianceExecutionSummaryUnionTypeDef",
+    "PutComplianceItemsRequestRequestTypeDef",
     "ListCommandInvocationsResultTypeDef",
     "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    "SendCommandRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "ListDocumentsResultTypeDef",
     "DescribeOpsItemsResponseTypeDef",
     "GetOpsItemResponseTypeDef",
     "DescribePatchGroupsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
@@ -524,14 +534,15 @@
     "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
     "PatchRuleOutputTypeDef",
+    "PatchFilterGroupUnionTypeDef",
     "PatchRuleTypeDef",
     "ResourceDataSyncSourceWithStateTypeDef",
     "ResourceDataSyncSourceTypeDef",
     "DescribeSessionsResponseTypeDef",
     "DescribeAssociationExecutionsResultTypeDef",
     "ListCommandsResultTypeDef",
     "SendCommandResultTypeDef",
@@ -539,25 +550,24 @@
     "DescribeMaintenanceWindowTasksResultTypeDef",
     "AssociationDescriptionTypeDef",
     "AssociationVersionInfoTypeDef",
     "CreateAssociationBatchRequestEntryOutputTypeDef",
     "RunbookOutputTypeDef",
     "StepExecutionTypeDef",
     "CreateAssociationBatchRequestEntryTypeDef",
-    "CreateAssociationRequestRequestTypeDef",
     "RunbookTypeDef",
-    "StartAutomationExecutionRequestRequestTypeDef",
-    "UpdateAssociationRequestRequestTypeDef",
+    "TargetLocationUnionTypeDef",
     "GetMaintenanceWindowTaskResultTypeDef",
     "UpdateMaintenanceWindowTaskResultTypeDef",
     "ListComplianceSummariesResultTypeDef",
     "ListResourceComplianceSummariesResultTypeDef",
     "ListDocumentMetadataHistoryResponseTypeDef",
     "DescribeInstanceAssociationsStatusResultTypeDef",
     "DescribeInventoryDeletionsResultTypeDef",
+    "MaintenanceWindowTaskInvocationParametersUnionTypeDef",
     "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
     "PatchRuleGroupOutputTypeDef",
     "PatchRuleGroupTypeDef",
     "ResourceDataSyncItemTypeDef",
     "CreateResourceDataSyncRequestRequestTypeDef",
     "UpdateResourceDataSyncRequestRequestTypeDef",
@@ -566,25 +576,31 @@
     "UpdateAssociationResultTypeDef",
     "UpdateAssociationStatusResultTypeDef",
     "ListAssociationVersionsResultTypeDef",
     "FailedCreateAssociationTypeDef",
     "AutomationExecutionMetadataTypeDef",
     "AutomationExecutionTypeDef",
     "DescribeAutomationStepExecutionsResultTypeDef",
-    "CreateAssociationBatchRequestRequestTypeDef",
-    "StartChangeRequestExecutionRequestRequestTypeDef",
+    "CreateAssociationBatchRequestEntryUnionTypeDef",
+    "RunbookUnionTypeDef",
+    "CreateAssociationRequestRequestTypeDef",
+    "StartAutomationExecutionRequestRequestTypeDef",
+    "UpdateAssociationRequestRequestTypeDef",
     "GetPatchBaselineResultTypeDef",
     "UpdatePatchBaselineResultTypeDef",
     "BaselineOverrideTypeDef",
     "CreatePatchBaselineRequestRequestTypeDef",
+    "PatchRuleGroupUnionTypeDef",
     "UpdatePatchBaselineRequestRequestTypeDef",
     "ListResourceDataSyncResultTypeDef",
     "CreateAssociationBatchResultTypeDef",
     "DescribeAutomationExecutionsResultTypeDef",
     "GetAutomationExecutionResultTypeDef",
+    "CreateAssociationBatchRequestRequestTypeDef",
+    "StartChangeRequestExecutionRequestRequestTypeDef",
     "GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
 )
 
 AccountSharingInfoTypeDef = TypedDict(
     "AccountSharingInfoTypeDef",
     {
         "AccountId": str,
@@ -659,19 +675,21 @@
     "_OptionalAssociationStatusOutputTypeDef",
     {
         "AdditionalInfo": str,
     },
     total=False,
 )
 
+
 class AssociationStatusOutputTypeDef(
     _RequiredAssociationStatusOutputTypeDef, _OptionalAssociationStatusOutputTypeDef
 ):
     pass
 
+
 TargetOutputTypeDef = TypedDict(
     "TargetOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
     },
     total=False,
@@ -707,35 +725,15 @@
     "AssociationFilterTypeDef",
     {
         "key": AssociationFilterKeyType,
         "value": str,
     },
 )
 
-_RequiredAssociationStatusTypeDef = TypedDict(
-    "_RequiredAssociationStatusTypeDef",
-    {
-        "Date": Union[datetime, str],
-        "Name": AssociationStatusNameType,
-        "Message": str,
-    },
-)
-_OptionalAssociationStatusTypeDef = TypedDict(
-    "_OptionalAssociationStatusTypeDef",
-    {
-        "AdditionalInfo": str,
-    },
-    total=False,
-)
-
-class AssociationStatusTypeDef(
-    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 AttachmentContentTypeDef = TypedDict(
     "AttachmentContentTypeDef",
     {
         "Name": str,
         "Size": int,
         "Hash": str,
         "HashType": Literal["Sha256"],
@@ -796,33 +794,36 @@
     {
         "Name": str,
         "Products": Sequence[str],
         "Configuration": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCancelCommandRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCommandRequestRequestTypeDef",
     {
         "CommandId": str,
     },
 )
 _OptionalCancelCommandRequestRequestTypeDef = TypedDict(
     "_OptionalCancelCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CancelCommandRequestRequestTypeDef(
     _RequiredCancelCommandRequestRequestTypeDef, _OptionalCancelCommandRequestRequestTypeDef
 ):
     pass
 
+
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
@@ -883,39 +884,21 @@
     {
         "ExecutionId": str,
         "ExecutionType": str,
     },
     total=False,
 )
 
+
 class ComplianceExecutionSummaryOutputTypeDef(
     _RequiredComplianceExecutionSummaryOutputTypeDef,
     _OptionalComplianceExecutionSummaryOutputTypeDef,
 ):
     pass
 
-_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
-    "_RequiredComplianceExecutionSummaryTypeDef",
-    {
-        "ExecutionTime": Union[datetime, str],
-    },
-)
-_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
-    "_OptionalComplianceExecutionSummaryTypeDef",
-    {
-        "ExecutionId": str,
-        "ExecutionType": str,
-    },
-    total=False,
-)
-
-class ComplianceExecutionSummaryTypeDef(
-    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
-):
-    pass
 
 _RequiredComplianceItemEntryTypeDef = TypedDict(
     "_RequiredComplianceItemEntryTypeDef",
     {
         "Severity": ComplianceSeverityType,
         "Status": ComplianceStatusType,
     },
@@ -926,19 +909,21 @@
         "Id": str,
         "Title": str,
         "Details": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ComplianceItemEntryTypeDef(
     _RequiredComplianceItemEntryTypeDef, _OptionalComplianceItemEntryTypeDef
 ):
     pass
 
+
 ComplianceStringFilterTypeDef = TypedDict(
     "ComplianceStringFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "Type": ComplianceQueryOperatorTypeType,
     },
@@ -987,17 +972,19 @@
         "Version": str,
         "RequireType": str,
         "VersionName": str,
     },
     total=False,
 )
 
+
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
+
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
     total=False,
@@ -1022,23 +1009,14 @@
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-PatchSourceOutputTypeDef = TypedDict(
-    "PatchSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Products": List[str],
-        "Configuration": str,
-    },
-)
-
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -1064,19 +1042,21 @@
         "DocumentVersion": str,
         "VersionName": str,
         "Force": bool,
     },
     total=False,
 )
 
+
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteInventoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInventoryRequestRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalDeleteInventoryRequestRequestTypeDef = TypedDict(
@@ -1085,19 +1065,21 @@
         "SchemaDeleteOption": InventorySchemaDeleteOptionType,
         "DryRun": bool,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteInventoryRequestRequestTypeDef(
     _RequiredDeleteInventoryRequestRequestTypeDef, _OptionalDeleteInventoryRequestRequestTypeDef
 ):
     pass
 
+
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
@@ -1139,20 +1121,22 @@
     "_OptionalDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
     },
     total=False,
 )
 
+
 class DeleteResourceDataSyncRequestRequestTypeDef(
     _RequiredDeleteResourceDataSyncRequestRequestTypeDef,
     _OptionalDeleteResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "PolicyId": str,
         "PolicyHash": str,
     },
@@ -1184,20 +1168,22 @@
     "_OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "Safe": bool,
     },
     total=False,
 )
 
+
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -1291,20 +1277,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeDocumentPermissionRequestRequestTypeDef(
     _RequiredDescribeDocumentPermissionRequestRequestTypeDef,
     _OptionalDescribeDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeDocumentRequestRequestTypeDef = TypedDict(
@@ -1312,19 +1300,21 @@
     {
         "DocumentVersion": str,
         "VersionName": str,
     },
     total=False,
 )
 
+
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
@@ -1332,20 +1322,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEffectiveInstanceAssociationsRequestRequestTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceAssociationTypeDef = TypedDict(
     "InstanceAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
@@ -1364,20 +1356,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
@@ -1385,20 +1379,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeInstanceAssociationsStatusRequestRequestTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceInformationFilterTypeDef = TypedDict(
     "InstanceInformationFilterTypeDef",
     {
         "key": InstanceInformationFilterKeyType,
         "valueSet": Sequence[str],
     },
 )
@@ -1450,19 +1446,21 @@
         "CriticalNonCompliantCount": int,
         "SecurityNonCompliantCount": int,
         "OtherNonCompliantCount": int,
     },
     total=False,
 )
 
+
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
+
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
@@ -1470,20 +1468,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPatchComplianceDataTypeDef = TypedDict(
     "_RequiredPatchComplianceDataTypeDef",
     {
         "Title": str,
         "KBId": str,
         "Classification": str,
         "Severity": str,
@@ -1495,19 +1495,21 @@
     "_OptionalPatchComplianceDataTypeDef",
     {
         "CVEIds": str,
     },
     total=False,
 )
 
+
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
+
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1613,19 +1615,21 @@
     {
         "Option": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+
 class ParameterStringFilterTypeDef(
     _RequiredParameterStringFilterTypeDef, _OptionalParameterStringFilterTypeDef
 ):
     pass
 
+
 ParametersFilterTypeDef = TypedDict(
     "ParametersFilterTypeDef",
     {
         "Key": ParametersFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -1662,20 +1666,22 @@
         "PatchSet": PatchSetType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
+
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
 )
@@ -1799,19 +1805,21 @@
     "_OptionalGetCalendarStateRequestRequestTypeDef",
     {
         "AtTime": str,
     },
     total=False,
 )
 
+
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1828,20 +1836,22 @@
     "_OptionalGetCommandInvocationRequestRequestTypeDef",
     {
         "PluginName": str,
     },
     total=False,
 )
 
+
 class GetCommandInvocationRequestRequestTypeDef(
     _RequiredGetCommandInvocationRequestRequestTypeDef,
     _OptionalGetCommandInvocationRequestRequestTypeDef,
 ):
     pass
 
+
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
@@ -1865,19 +1875,21 @@
         "VersionName": str,
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
     },
     total=False,
 )
 
+
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredInventoryFilterTypeDef = TypedDict(
     "_RequiredInventoryFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -1885,17 +1897,19 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Type": InventoryQueryOperatorTypeType,
     },
     total=False,
 )
 
+
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
+
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
@@ -1969,36 +1983,40 @@
     "_OptionalLoggingInfoTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
+
 class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
     pass
 
+
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalGetOpsItemRequestRequestTypeDef = TypedDict(
     "_OptionalGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemArn": str,
     },
     total=False,
 )
 
+
 class GetOpsItemRequestRequestTypeDef(
     _RequiredGetOpsItemRequestRequestTypeDef, _OptionalGetOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalGetOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -2006,19 +2024,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2026,17 +2046,19 @@
     "_OptionalOpsFilterTypeDef",
     {
         "Type": OpsFilterOperatorTypeType,
     },
     total=False,
 )
 
+
 class OpsFilterTypeDef(_RequiredOpsFilterTypeDef, _OptionalOpsFilterTypeDef):
     pass
 
+
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
@@ -2052,39 +2074,43 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetParameterHistoryRequestRequestTypeDef(
     _RequiredGetParameterHistoryRequestRequestTypeDef,
     _OptionalGetParameterHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetParameterRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterRequestRequestTypeDef = TypedDict(
     "_OptionalGetParameterRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
+
 class GetParameterRequestRequestTypeDef(
     _RequiredGetParameterRequestRequestTypeDef, _OptionalGetParameterRequestRequestTypeDef
 ):
     pass
 
+
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Value": str,
         "Version": int,
@@ -2107,46 +2133,59 @@
     "_OptionalGetParametersRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
+
 class GetParametersRequestRequestTypeDef(
     _RequiredGetParametersRequestRequestTypeDef, _OptionalGetParametersRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
+
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
+
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
+PatchSourceOutputTypeDef = TypedDict(
+    "PatchSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Products": List[str],
+        "Configuration": str,
+    },
+)
+
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -2154,20 +2193,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesResponseEntryTypeDef = TypedDict(
     "GetResourcePoliciesResponseEntryTypeDef",
     {
         "PolicyId": str,
         "PolicyHash": str,
         "Policy": str,
     },
@@ -2253,17 +2294,19 @@
         "ContentHash": str,
         "Content": Sequence[Mapping[str, str]],
         "Context": Mapping[str, str],
     },
     total=False,
 )
 
+
 class InventoryItemTypeDef(_RequiredInventoryItemTypeDef, _OptionalInventoryItemTypeDef):
     pass
 
+
 _RequiredInventoryResultItemTypeDef = TypedDict(
     "_RequiredInventoryResultItemTypeDef",
     {
         "TypeName": str,
         "SchemaVersion": str,
         "Content": List[Dict[str, str]],
     },
@@ -2273,19 +2316,21 @@
     {
         "CaptureTime": str,
         "ContentHash": str,
     },
     total=False,
 )
 
+
 class InventoryResultItemTypeDef(
     _RequiredInventoryResultItemTypeDef, _OptionalInventoryResultItemTypeDef
 ):
     pass
 
+
 _RequiredLabelParameterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredLabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "Labels": Sequence[str],
     },
 )
@@ -2293,20 +2338,22 @@
     "_OptionalLabelParameterVersionRequestRequestTypeDef",
     {
         "ParameterVersion": int,
     },
     total=False,
 )
 
+
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestRequestTypeDef = TypedDict(
@@ -2314,20 +2361,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociationVersionsRequestRequestTypeDef(
     _RequiredListAssociationVersionsRequestRequestTypeDef,
     _OptionalListAssociationVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDocumentMetadataHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentMetadataHistoryRequestRequestTypeDef",
     {
         "Name": str,
         "Metadata": Literal["DocumentReviews"],
     },
 )
@@ -2337,20 +2386,22 @@
         "DocumentVersion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -2358,20 +2409,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
     },
@@ -2448,24 +2501,14 @@
         "ClientContext": str,
         "Qualifier": str,
         "Payload": bytes,
     },
     total=False,
 )
 
-MaintenanceWindowLambdaParametersTypeDef = TypedDict(
-    "MaintenanceWindowLambdaParametersTypeDef",
-    {
-        "ClientContext": str,
-        "Qualifier": str,
-        "Payload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 NotificationConfigTypeDef = TypedDict(
     "NotificationConfigTypeDef",
     {
         "NotificationArn": str,
         "NotificationEvents": Sequence[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
@@ -2502,20 +2545,22 @@
         "AccountIdsToAdd": Sequence[str],
         "AccountIdsToRemove": Sequence[str],
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
+
 class ModifyDocumentPermissionRequestRequestTypeDef(
     _RequiredModifyDocumentPermissionRequestRequestTypeDef,
     _OptionalModifyDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
+
 OpsEntityItemTypeDef = TypedDict(
     "OpsEntityItemTypeDef",
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
@@ -2567,19 +2612,21 @@
     {
         "PolicyId": str,
         "PolicyHash": str,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
@@ -2641,20 +2688,22 @@
     "_OptionalSendAutomationSignalRequestRequestTypeDef",
     {
         "Payload": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class SendAutomationSignalRequestRequestTypeDef(
     _RequiredSendAutomationSignalRequestRequestTypeDef,
     _OptionalSendAutomationSignalRequestRequestTypeDef,
 ):
     pass
 
+
 SessionManagerOutputUrlTypeDef = TypedDict(
     "SessionManagerOutputUrlTypeDef",
     {
         "S3OutputUrl": str,
         "CloudWatchOutputUrl": str,
     },
     total=False,
@@ -2679,39 +2728,43 @@
         "DocumentName": str,
         "Reason": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_OptionalStopAutomationExecutionRequestRequestTypeDef",
     {
         "Type": StopTypeType,
     },
     total=False,
 )
 
+
 class StopAutomationExecutionRequestRequestTypeDef(
     _RequiredStopAutomationExecutionRequestRequestTypeDef,
     _OptionalStopAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
+
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -2753,20 +2806,22 @@
         "AllowUnassociatedTargets": bool,
         "Enabled": bool,
         "Replace": bool,
     },
     total=False,
 )
 
+
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
@@ -2825,20 +2880,22 @@
         "ScheduleOffset": int,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -2854,57 +2911,63 @@
         "Tier": ParameterTierType,
         "Policies": str,
         "DataType": str,
     },
     total=False,
 )
 
+
 class PutParameterRequestRequestTypeDef(
     _RequiredPutParameterRequestRequestTypeDef, _OptionalPutParameterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAlarmConfigurationOutputTypeDef = TypedDict(
     "_RequiredAlarmConfigurationOutputTypeDef",
     {
         "Alarms": List[AlarmTypeDef],
     },
 )
 _OptionalAlarmConfigurationOutputTypeDef = TypedDict(
     "_OptionalAlarmConfigurationOutputTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
+
 class AlarmConfigurationOutputTypeDef(
     _RequiredAlarmConfigurationOutputTypeDef, _OptionalAlarmConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredAlarmConfigurationTypeDef = TypedDict(
     "_RequiredAlarmConfigurationTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
 )
 _OptionalAlarmConfigurationTypeDef = TypedDict(
     "_OptionalAlarmConfigurationTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
+
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
+
 AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
     "AssociateOpsItemRelatedItemResponseTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3379,20 +3442,22 @@
         "Filters": Sequence[AssociationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 AssociationExecutionTargetTypeDef = TypedDict(
     "AssociationExecutionTargetTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "ResourceId": str,
@@ -3418,38 +3483,76 @@
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 ListAssociationsRequestRequestTypeDef = TypedDict(
     "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
-    "UpdateAssociationStatusRequestRequestTypeDef",
+_RequiredAssociationStatusTypeDef = TypedDict(
+    "_RequiredAssociationStatusTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationStatus": AssociationStatusTypeDef,
+        "Date": TimestampTypeDef,
+        "Name": AssociationStatusNameType,
+        "Message": str,
+    },
+)
+_OptionalAssociationStatusTypeDef = TypedDict(
+    "_OptionalAssociationStatusTypeDef",
+    {
+        "AdditionalInfo": str,
+    },
+    total=False,
+)
+
+
+class AssociationStatusTypeDef(
+    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+):
+    pass
+
+
+_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryTypeDef",
+    {
+        "ExecutionTime": TimestampTypeDef,
     },
 )
+_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryTypeDef",
+    {
+        "ExecutionId": str,
+        "ExecutionType": str,
+    },
+    total=False,
+)
+
+
+class ComplianceExecutionSummaryTypeDef(
+    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
+):
+    pass
+
 
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
@@ -3463,29 +3566,41 @@
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
     },
     total=False,
 )
 
+
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
+
 DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+MaintenanceWindowLambdaParametersTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersTypeDef",
+    {
+        "ClientContext": str,
+        "Qualifier": str,
+        "Payload": BlobTypeDef,
+    },
+    total=False,
+)
+
 GetCommandInvocationResultTypeDef = TypedDict(
     "GetCommandInvocationResultTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "Comment": str,
         "DocumentName": str,
@@ -3584,39 +3699,14 @@
         "Severity": ComplianceSeverityType,
         "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "Details": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": str,
-        "ComplianceType": str,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
-        "Items": Sequence[ComplianceItemEntryTypeDef],
-    },
-)
-_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ItemContentHash": str,
-        "UploadType": ComplianceUploadTypeType,
-    },
-    total=False,
-)
-
-class PutComplianceItemsRequestRequestTypeDef(
-    _RequiredPutComplianceItemsRequestRequestTypeDef,
-    _OptionalPutComplianceItemsRequestRequestTypeDef,
-):
-    pass
-
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
@@ -3671,98 +3761,29 @@
 )
 _OptionalCreateActivationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateActivationRequestRequestTypeDef",
     {
         "Description": str,
         "DefaultInstanceName": str,
         "RegistrationLimit": int,
-        "ExpirationDate": Union[datetime, str],
+        "ExpirationDate": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "RegistrationMetadata": Sequence[RegistrationMetadataItemTypeDef],
     },
     total=False,
 )
 
+
 class CreateActivationRequestRequestTypeDef(
     _RequiredCreateActivationRequestRequestTypeDef, _OptionalCreateActivationRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-):
-    pass
-
-_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-    },
-)
-_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-    },
-)
-_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
-    {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
-        "Replace": bool,
-    },
-    total=False,
-)
-
-class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-):
-    pass
 
+TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 _RequiredCreateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3777,19 +3798,21 @@
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDocumentRequestRequestTypeDef(
     _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
 ):
     pass
 
+
 DocumentIdentifierTypeDef = TypedDict(
     "DocumentIdentifierTypeDef",
     {
         "Name": str,
         "CreatedDate": datetime,
         "DisplayName": str,
         "Owner": str,
@@ -3867,28 +3890,30 @@
         "OperationalData": Mapping[str, OpsItemDataValueTypeDef],
         "Notifications": Sequence[OpsItemNotificationTypeDef],
         "Priority": int,
         "RelatedOpsItems": Sequence[RelatedOpsItemTypeDef],
         "Tags": Sequence[TagTypeDef],
         "Category": str,
         "Severity": str,
-        "ActualStartTime": Union[datetime, str],
-        "ActualEndTime": Union[datetime, str],
-        "PlannedStartTime": Union[datetime, str],
-        "PlannedEndTime": Union[datetime, str],
+        "ActualStartTime": TimestampTypeDef,
+        "ActualEndTime": TimestampTypeDef,
+        "PlannedStartTime": TimestampTypeDef,
+        "PlannedEndTime": TimestampTypeDef,
         "AccountId": str,
     },
     total=False,
 )
 
+
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 OpsItemTypeDef = TypedDict(
     "OpsItemTypeDef",
     {
         "CreatedBy": str,
         "OpsItemType": str,
         "CreatedTime": datetime,
         "Description": str,
@@ -3929,28 +3954,30 @@
         "Notifications": Sequence[OpsItemNotificationTypeDef],
         "Priority": int,
         "RelatedOpsItems": Sequence[RelatedOpsItemTypeDef],
         "Status": OpsItemStatusType,
         "Title": str,
         "Category": str,
         "Severity": str,
-        "ActualStartTime": Union[datetime, str],
-        "ActualEndTime": Union[datetime, str],
-        "PlannedStartTime": Union[datetime, str],
-        "PlannedEndTime": Union[datetime, str],
+        "ActualStartTime": TimestampTypeDef,
+        "ActualEndTime": TimestampTypeDef,
+        "PlannedStartTime": TimestampTypeDef,
+        "PlannedEndTime": TimestampTypeDef,
         "OpsItemArn": str,
     },
     total=False,
 )
 
+
 class UpdateOpsItemRequestRequestTypeDef(
     _RequiredUpdateOpsItemRequestRequestTypeDef, _OptionalUpdateOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalCreateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -3958,19 +3985,21 @@
     {
         "Metadata": Mapping[str, MetadataValueTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
 GetOpsMetadataResultTypeDef = TypedDict(
     "GetOpsMetadataResultTypeDef",
     {
         "ResourceId": str,
         "Metadata": Dict[str, MetadataValueTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3988,19 +4017,21 @@
     {
         "MetadataToUpdate": Mapping[str, MetadataValueTypeDef],
         "KeysToDelete": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
 DescribeActivationsRequestRequestTypeDef = TypedDict(
     "DescribeActivationsRequestRequestTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -4028,20 +4059,22 @@
     {
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
         {
             "AssociationId": str,
         },
     )
@@ -4053,20 +4086,22 @@
             "Filters": Sequence[AssociationExecutionFilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
+
 class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
     _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
 ):
     pass
 
+
 DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4082,110 +4117,97 @@
     "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
     "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
 ):
     pass
 
+
 DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     {
         "DeletionId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -4194,20 +4216,22 @@
     {
         "PatchSet": PatchSetType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
     _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
 ):
     pass
 
+
 GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
     "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     {
         "TypeName": str,
         "Aggregator": bool,
         "SubType": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4226,60 +4250,66 @@
     {
         "WithDecryption": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
     _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
     _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
     "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
     _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
     "ListAssociationsRequestListAssociationsPaginateTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4338,20 +4368,22 @@
     "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
     _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4378,20 +4410,22 @@
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
@@ -4401,20 +4435,22 @@
         "NextToken": str,
         "MaxResults": int,
         "ReverseOrder": bool,
     },
     total=False,
 )
 
+
 class DescribeAutomationStepExecutionsRequestRequestTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4441,20 +4477,22 @@
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
@@ -4463,46 +4501,21 @@
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchesRequestRequestTypeDef,
 ):
     pass
 
-DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
-    TypedDict(
-        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-        {
-            "WindowId": str,
-            "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-            "ResourceType": MaintenanceWindowResourceTypeType,
-            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
 
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4588,20 +4601,22 @@
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
@@ -4610,20 +4625,22 @@
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4659,20 +4676,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -4682,20 +4701,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
@@ -4703,20 +4724,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
@@ -4725,20 +4748,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
@@ -4746,20 +4771,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
@@ -4768,20 +4795,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
@@ -4789,20 +4818,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
@@ -4811,20 +4842,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTargetsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
@@ -4832,20 +4865,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
@@ -4854,20 +4889,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4962,20 +4999,22 @@
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
     _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetParametersByPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetParametersByPathRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalGetParametersByPathRequestRequestTypeDef = TypedDict(
@@ -4986,20 +5025,22 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetParametersByPathRequestRequestTypeDef(
     _RequiredGetParametersByPathRequestRequestTypeDef,
     _OptionalGetParametersByPathRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5046,20 +5087,22 @@
     {
         "Filters": Sequence[SessionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestRequestTypeDef = TypedDict(
@@ -5068,19 +5111,21 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[SessionFilterTypeDef],
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
+
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5165,17 +5210,19 @@
     "_OptionalDocumentReviewsTypeDef",
     {
         "Comment": Sequence[DocumentReviewCommentSourceTypeDef],
     },
     total=False,
 )
 
+
 class DocumentReviewsTypeDef(_RequiredDocumentReviewsTypeDef, _OptionalDocumentReviewsTypeDef):
     pass
 
+
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5202,20 +5249,22 @@
     {
         "PluginName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetCommandInvocationRequestCommandExecutedWaitTypeDef(
     _RequiredGetCommandInvocationRequestCommandExecutedWaitTypeDef,
     _OptionalGetCommandInvocationRequestCommandExecutedWaitTypeDef,
 ):
     pass
 
+
 InventoryGroupTypeDef = TypedDict(
     "InventoryGroupTypeDef",
     {
         "Name": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
 )
@@ -5233,20 +5282,22 @@
         "Filters": Sequence[InventoryFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInventoryEntriesRequestRequestTypeDef(
     _RequiredListInventoryEntriesRequestRequestTypeDef,
     _OptionalListInventoryEntriesRequestRequestTypeDef,
 ):
     pass
 
+
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -5326,14 +5377,15 @@
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PatchSourceUnionTypeDef = Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5421,19 +5473,21 @@
     {
         "Version": str,
         "DisplayName": str,
     },
     total=False,
 )
 
+
 class InventoryItemSchemaTypeDef(
     _RequiredInventoryItemSchemaTypeDef, _OptionalInventoryItemSchemaTypeDef
 ):
     pass
 
+
 PutInventoryRequestRequestTypeDef = TypedDict(
     "PutInventoryRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Items": Sequence[InventoryItemTypeDef],
     },
 )
@@ -5529,14 +5583,19 @@
         "Parameters": Mapping[str, Sequence[str]],
         "ServiceRoleArn": str,
         "TimeoutSeconds": int,
     },
     total=False,
 )
 
+NotificationConfigUnionTypeDef = Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef]
+MaintenanceWindowTaskParameterValueExpressionUnionTypeDef = Union[
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+]
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
@@ -5634,40 +5693,44 @@
     "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     {
         "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
+
 class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
 ):
     pass
 
+
 _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationalUnits": Sequence[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
+
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
+
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
     },
@@ -5678,19 +5741,21 @@
         "Prefix": str,
         "AWSKMSKeyARN": str,
         "DestinationDataSharing": ResourceDataSyncDestinationDataSharingTypeDef,
     },
     total=False,
 )
 
+
 class ResourceDataSyncS3DestinationTypeDef(
     _RequiredResourceDataSyncS3DestinationTypeDef, _OptionalResourceDataSyncS3DestinationTypeDef
 ):
     pass
 
+
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "SessionId": str,
         "Target": str,
         "Status": SessionStatusType,
         "StartDate": datetime,
@@ -5836,49 +5901,15 @@
         "TargetLocationMaxErrors": str,
         "ExecutionRoleName": str,
         "TargetLocationAlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredSendCommandRequestRequestTypeDef = TypedDict(
-    "_RequiredSendCommandRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalSendCommandRequestRequestTypeDef = TypedDict(
-    "_OptionalSendCommandRequestRequestTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "DocumentVersion": str,
-        "DocumentHash": str,
-        "DocumentHashType": DocumentHashTypeType,
-        "TimeoutSeconds": int,
-        "Comment": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "OutputS3Region": str,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "ServiceRoleArn": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class SendCommandRequestRequestTypeDef(
-    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
-):
-    pass
-
+AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
 TargetLocationTypeDef = TypedDict(
     "TargetLocationTypeDef",
     {
         "Accounts": Sequence[str],
         "Regions": Sequence[str],
         "TargetLocationMaxConcurrency": str,
         "TargetLocationMaxErrors": str,
@@ -5911,14 +5942,54 @@
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AssociationStatusUnionTypeDef = Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
+UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationStatus": AssociationStatusTypeDef,
+    },
+)
+
+ComplianceExecutionSummaryUnionTypeDef = Union[
+    ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
+]
+_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": str,
+        "ComplianceType": str,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "Items": Sequence[ComplianceItemEntryTypeDef],
+    },
+)
+_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ItemContentHash": str,
+        "UploadType": ComplianceUploadTypeType,
+    },
+    total=False,
+)
+
+
+class PutComplianceItemsRequestRequestTypeDef(
+    _RequiredPutComplianceItemsRequestRequestTypeDef,
+    _OptionalPutComplianceItemsRequestRequestTypeDef,
+):
+    pass
+
+
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5965,14 +6036,179 @@
         "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
+DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
+    TypedDict(
+        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+        {
+            "WindowId": str,
+            "Targets": Sequence[TargetUnionTypeDef],
+            "ResourceType": MaintenanceWindowResourceTypeType,
+            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": Sequence[TargetUnionTypeDef],
+    },
+)
+_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSendCommandRequestRequestTypeDef = TypedDict(
+    "_RequiredSendCommandRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalSendCommandRequestRequestTypeDef = TypedDict(
+    "_OptionalSendCommandRequestRequestTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "Targets": Sequence[TargetUnionTypeDef],
+        "DocumentVersion": str,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "TimeoutSeconds": int,
+        "Comment": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "OutputS3Region": str,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "ServiceRoleArn": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class SendCommandRequestRequestTypeDef(
+    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "Replace": bool,
+    },
+    total=False,
+)
+
+
+class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+):
+    pass
+
+
 ListDocumentsResultTypeDef = TypedDict(
     "ListDocumentsResultTypeDef",
     {
         "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6047,20 +6283,22 @@
     "_OptionalUpdateDocumentMetadataRequestRequestTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
+
 class UpdateDocumentMetadataRequestRequestTypeDef(
     _RequiredUpdateDocumentMetadataRequestRequestTypeDef,
     _OptionalUpdateDocumentMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6215,17 +6453,20 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
+
 class PatchRuleOutputTypeDef(_RequiredPatchRuleOutputTypeDef, _OptionalPatchRuleOutputTypeDef):
     pass
 
+
+PatchFilterGroupUnionTypeDef = Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef]
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
     },
 )
 _OptionalPatchRuleTypeDef = TypedDict(
@@ -6235,17 +6476,19 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
+
 class PatchRuleTypeDef(_RequiredPatchRuleTypeDef, _OptionalPatchRuleTypeDef):
     pass
 
+
 ResourceDataSyncSourceWithStateTypeDef = TypedDict(
     "ResourceDataSyncSourceWithStateTypeDef",
     {
         "SourceType": str,
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
         "SourceRegions": List[str],
         "IncludeFutureRegions": bool,
@@ -6268,19 +6511,21 @@
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
         "IncludeFutureRegions": bool,
         "EnableAllOpsDataSources": bool,
     },
     total=False,
 )
 
+
 class ResourceDataSyncSourceTypeDef(
     _RequiredResourceDataSyncSourceTypeDef, _OptionalResourceDataSyncSourceTypeDef
 ):
     pass
 
+
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6418,20 +6663,22 @@
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class CreateAssociationBatchRequestEntryOutputTypeDef(
     _RequiredCreateAssociationBatchRequestEntryOutputTypeDef,
     _OptionalCreateAssociationBatchRequestEntryOutputTypeDef,
 ):
     pass
 
+
 _RequiredRunbookOutputTypeDef = TypedDict(
     "_RequiredRunbookOutputTypeDef",
     {
         "DocumentName": str,
     },
 )
 _OptionalRunbookOutputTypeDef = TypedDict(
@@ -6445,17 +6692,19 @@
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetLocations": List[TargetLocationOutputTypeDef],
     },
     total=False,
 )
 
+
 class RunbookOutputTypeDef(_RequiredRunbookOutputTypeDef, _OptionalRunbookOutputTypeDef):
     pass
 
+
 StepExecutionTypeDef = TypedDict(
     "StepExecutionTypeDef",
     {
         "StepName": str,
         "Action": str,
         "TimeoutSeconds": int,
         "OnFailure": str,
@@ -6509,56 +6758,21 @@
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateAssociationBatchRequestEntryTypeDef(
     _RequiredCreateAssociationBatchRequestEntryTypeDef,
     _OptionalCreateAssociationBatchRequestEntryTypeDef,
 ):
     pass
 
-_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAssociationRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAssociationRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "InstanceId": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "AssociationName": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateAssociationRequestRequestTypeDef(
-    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
-):
-    pass
 
 _RequiredRunbookTypeDef = TypedDict(
     "_RequiredRunbookTypeDef",
     {
         "DocumentName": str,
     },
 )
@@ -6573,85 +6787,20 @@
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetLocations": Sequence[TargetLocationTypeDef],
     },
     total=False,
 )
 
-class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
-    pass
-
-_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ClientToken": str,
-        "Mode": ExecutionModeType,
-        "TargetParameterName": str,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
 
-class StartAutomationExecutionRequestRequestTypeDef(
-    _RequiredStartAutomationExecutionRequestRequestTypeDef,
-    _OptionalStartAutomationExecutionRequestRequestTypeDef,
-):
+class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
     pass
 
-_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAssociationRequestRequestTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAssociationRequestRequestTypeDef",
-    {
-        "Parameters": Mapping[str, Sequence[str]],
-        "DocumentVersion": str,
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "Name": str,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        "AssociationName": str,
-        "AssociationVersion": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateAssociationRequestRequestTypeDef(
-    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
-):
-    pass
 
+TargetLocationUnionTypeDef = Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]
 GetMaintenanceWindowTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
         "Targets": List[TargetOutputTypeDef],
         "TaskArn": str,
@@ -6737,94 +6886,90 @@
     {
         "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MaintenanceWindowTaskInvocationParametersUnionTypeDef = Union[
+    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+]
 _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
     },
 )
 _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        "Targets": Sequence[TargetUnionTypeDef],
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[
-            str,
-            Union[
-                MaintenanceWindowTaskParameterValueExpressionTypeDef,
-                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-            ],
-        ],
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "ClientToken": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
     _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
     _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        "Targets": Sequence[TargetUnionTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[
-            str,
-            Union[
-                MaintenanceWindowTaskParameterValueExpressionTypeDef,
-                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-            ],
-        ],
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "Replace": bool,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
 ):
     pass
 
+
 PatchRuleGroupOutputTypeDef = TypedDict(
     "PatchRuleGroupOutputTypeDef",
     {
         "PatchRules": List[PatchRuleOutputTypeDef],
     },
 )
 
@@ -6864,20 +7009,22 @@
         "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
     total=False,
 )
 
+
 class CreateResourceDataSyncRequestRequestTypeDef(
     _RequiredCreateResourceDataSyncRequestRequestTypeDef,
     _OptionalCreateResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "UpdateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
@@ -7016,55 +7163,129 @@
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssociationBatchRequestRequestTypeDef = TypedDict(
-    "CreateAssociationBatchRequestRequestTypeDef",
+CreateAssociationBatchRequestEntryUnionTypeDef = Union[
+    CreateAssociationBatchRequestEntryTypeDef, CreateAssociationBatchRequestEntryOutputTypeDef
+]
+RunbookUnionTypeDef = Union[RunbookTypeDef, RunbookOutputTypeDef]
+_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAssociationRequestRequestTypeDef",
     {
-        "Entries": Sequence[
-            Union[
-                CreateAssociationBatchRequestEntryTypeDef,
-                CreateAssociationBatchRequestEntryOutputTypeDef,
-            ]
-        ],
+        "Name": str,
+    },
+)
+_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAssociationRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "InstanceId": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "AssociationName": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
+    total=False,
 )
 
-_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+
+class CreateAssociationRequestRequestTypeDef(
+    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
     {
         "DocumentName": str,
-        "Runbooks": Sequence[Union[RunbookTypeDef, RunbookOutputTypeDef]],
     },
 )
-_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
     {
-        "ScheduledTime": Union[datetime, str],
         "DocumentVersion": str,
         "Parameters": Mapping[str, Sequence[str]],
-        "ChangeRequestName": str,
         "ClientToken": str,
-        "AutoApprove": bool,
+        "Mode": ExecutionModeType,
+        "TargetParameterName": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
-        "ScheduledEndTime": Union[datetime, str],
-        "ChangeDetails": str,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-class StartChangeRequestExecutionRequestRequestTypeDef(
-    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
-    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+
+class StartAutomationExecutionRequestRequestTypeDef(
+    _RequiredStartAutomationExecutionRequestRequestTypeDef,
+    _OptionalStartAutomationExecutionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAssociationRequestRequestTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAssociationRequestRequestTypeDef",
+    {
+        "Parameters": Mapping[str, Sequence[str]],
+        "DocumentVersion": str,
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "Name": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "AssociationName": str,
+        "AssociationVersion": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateAssociationRequestRequestTypeDef(
+    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
 ):
     pass
 
+
 GetPatchBaselineResultTypeDef = TypedDict(
     "GetPatchBaselineResultTypeDef",
     {
         "BaselineId": str,
         "Name": str,
         "OperatingSystem": OperatingSystemType,
         "GlobalFilters": PatchFilterGroupOutputTypeDef,
@@ -7134,27 +7355,30 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]],
+        "Sources": Sequence[PatchSourceUnionTypeDef],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePatchBaselineRequestRequestTypeDef(
     _RequiredCreatePatchBaselineRequestRequestTypeDef,
     _OptionalCreatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
+
+PatchRuleGroupUnionTypeDef = Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef]
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
@@ -7165,26 +7389,28 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]],
+        "Sources": Sequence[PatchSourceUnionTypeDef],
         "Replace": bool,
     },
     total=False,
 )
 
+
 class UpdatePatchBaselineRequestRequestTypeDef(
     _RequiredUpdatePatchBaselineRequestRequestTypeDef,
     _OptionalUpdatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
+
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7212,14 +7438,52 @@
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAssociationBatchRequestRequestTypeDef = TypedDict(
+    "CreateAssociationBatchRequestRequestTypeDef",
+    {
+        "Entries": Sequence[CreateAssociationBatchRequestEntryUnionTypeDef],
+    },
+)
+
+_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+        "Runbooks": Sequence[RunbookUnionTypeDef],
+    },
+)
+_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "ScheduledTime": TimestampTypeDef,
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ChangeRequestName": str,
+        "ClientToken": str,
+        "AutoApprove": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ScheduledEndTime": TimestampTypeDef,
+        "ChangeDetails": str,
+    },
+    total=False,
+)
+
+
+class StartChangeRequestExecutionRequestRequestTypeDef(
+    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
+    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "SnapshotId": str,
     },
 )
@@ -7227,12 +7491,13 @@
     "_OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "BaselineOverride": BaselineOverrideTypeDef,
     },
     total=False,
 )
 
+
 class GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef(
     _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
     _OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/waiter.py` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/waiter.pyi` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/PKG-INFO` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SSM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ssm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ssm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -633,20 +633,20 @@
 )
 
 
 def check_value(value: AssociationComplianceSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ssm.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
     TagTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
@@ -655,41 +655,40 @@
     AssociationOverviewTypeDef,
     AssociationStatusOutputTypeDef,
     TargetOutputTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
-    AssociationStatusTypeDef,
+    TimestampTypeDef,
     AttachmentContentTypeDef,
     AttachmentInformationTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
+    BlobTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
     NotificationConfigOutputTypeDef,
     ComplianceExecutionSummaryOutputTypeDef,
-    ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
     TargetTypeDef,
     DocumentRequiresTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
     MetadataValueTypeDef,
-    PatchSourceOutputTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
@@ -766,14 +765,15 @@
     OpsResultAttributeTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
+    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
@@ -790,15 +790,14 @@
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
     MaintenanceWindowLambdaParametersOutputTypeDef,
-    MaintenanceWindowLambdaParametersTypeDef,
     NotificationConfigTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
     OpsItemIdentityTypeDef,
     ParameterInlinePolicyTypeDef,
@@ -874,33 +873,32 @@
     AssociationTypeDef,
     MaintenanceWindowTargetTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
     ListAssociationsRequestRequestTypeDef,
-    UpdateAssociationStatusRequestRequestTypeDef,
+    AssociationStatusTypeDef,
+    ComplianceExecutionSummaryTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
+    MaintenanceWindowLambdaParametersTypeDef,
     GetCommandInvocationResultTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
     MaintenanceWindowRunCommandParametersOutputTypeDef,
     ComplianceItemTypeDef,
-    PutComplianceItemsRequestRequestTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    TargetUnionTypeDef,
     CreateDocumentRequestRequestTypeDef,
     DocumentIdentifierTypeDef,
     GetDocumentResultTypeDef,
     OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
     OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
@@ -913,15 +911,14 @@
     DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
     DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
@@ -933,16 +930,14 @@
     ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
-    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
-    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
     DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef,
     DescribePatchBaselinesRequestRequestTypeDef,
     DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef,
     DescribePatchGroupsRequestRequestTypeDef,
     DescribeAvailablePatchesResultTypeDef,
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef,
@@ -994,14 +989,15 @@
     GetInventoryRequestRequestTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
+    PatchSourceUnionTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
@@ -1012,14 +1008,16 @@
     ListOpsItemEventsRequestRequestTypeDef,
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
     MaintenanceWindowRunCommandParametersTypeDef,
+    NotificationConfigUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     OpsEntityTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
     PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
@@ -1030,24 +1028,35 @@
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
     MaintenanceWindowTaskTypeDef,
     TargetLocationOutputTypeDef,
-    SendCommandRequestRequestTypeDef,
+    AlarmConfigurationUnionTypeDef,
     TargetLocationTypeDef,
     ListAssociationsResultTypeDef,
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
+    AssociationStatusUnionTypeDef,
+    UpdateAssociationStatusRequestRequestTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
+    PutComplianceItemsRequestRequestTypeDef,
     ListCommandInvocationsResultTypeDef,
     MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
+    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
+    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    SendCommandRequestRequestTypeDef,
+    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     ListDocumentsResultTypeDef,
     DescribeOpsItemsResponseTypeDef,
     GetOpsItemResponseTypeDef,
     DescribePatchGroupsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -1064,14 +1073,15 @@
     MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
     PatchRuleOutputTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchRuleTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
     ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
     DescribeAssociationExecutionsResultTypeDef,
     ListCommandsResultTypeDef,
     SendCommandResultTypeDef,
@@ -1079,25 +1089,24 @@
     DescribeMaintenanceWindowTasksResultTypeDef,
     AssociationDescriptionTypeDef,
     AssociationVersionInfoTypeDef,
     CreateAssociationBatchRequestEntryOutputTypeDef,
     RunbookOutputTypeDef,
     StepExecutionTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
-    CreateAssociationRequestRequestTypeDef,
     RunbookTypeDef,
-    StartAutomationExecutionRequestRequestTypeDef,
-    UpdateAssociationRequestRequestTypeDef,
+    TargetLocationUnionTypeDef,
     GetMaintenanceWindowTaskResultTypeDef,
     UpdateMaintenanceWindowTaskResultTypeDef,
     ListComplianceSummariesResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListDocumentMetadataHistoryResponseTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
     RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
     UpdateMaintenanceWindowTaskRequestRequestTypeDef,
     PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
     ResourceDataSyncItemTypeDef,
     CreateResourceDataSyncRequestRequestTypeDef,
     UpdateResourceDataSyncRequestRequestTypeDef,
@@ -1106,30 +1115,36 @@
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     ListAssociationVersionsResultTypeDef,
     FailedCreateAssociationTypeDef,
     AutomationExecutionMetadataTypeDef,
     AutomationExecutionTypeDef,
     DescribeAutomationStepExecutionsResultTypeDef,
-    CreateAssociationBatchRequestRequestTypeDef,
-    StartChangeRequestExecutionRequestRequestTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
+    RunbookUnionTypeDef,
+    CreateAssociationRequestRequestTypeDef,
+    StartAutomationExecutionRequestRequestTypeDef,
+    UpdateAssociationRequestRequestTypeDef,
     GetPatchBaselineResultTypeDef,
     UpdatePatchBaselineResultTypeDef,
     BaselineOverrideTypeDef,
     CreatePatchBaselineRequestRequestTypeDef,
+    PatchRuleGroupUnionTypeDef,
     UpdatePatchBaselineRequestRequestTypeDef,
     ListResourceDataSyncResultTypeDef,
     CreateAssociationBatchResultTypeDef,
     DescribeAutomationExecutionsResultTypeDef,
     GetAutomationExecutionResultTypeDef,
+    CreateAssociationBatchRequestRequestTypeDef,
+    StartChangeRequestExecutionRequestRequestTypeDef,
     GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSharingInfoTypeDef:
+def get_value() -> AccountSharingInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/SOURCES.txt` & `mypy-boto3-ssm-1.28.16/mypy_boto3_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15.post1/setup.py` & `mypy-boto3-ssm-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SSM 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 ssm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ssm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ssm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

