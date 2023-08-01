# Comparing `tmp/mypy-boto3-emr-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-emr-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:06 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-1.28.16.tar", last modified: Tue Aug  1 11:36:45 2023, max compression
```

## Comparing `mypy-boto3-emr-1.28.15.post1.tar` & `mypy-boto3-emr-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.237143 mypy-boto3-emr-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-07-29 10:03:06.233143 mypy-boto3-emr-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.225143 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44339 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44265 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85114 2023-07-29 09:44:59.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    84996 2023-07-29 09:44:58.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.233143 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:03:06.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:06.237143 mypy-boto3-emr-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.920894 mypy-boto3-emr-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-08-01 11:36:45.912894 mypy-boto3-emr-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23036 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.912894 mypy-boto3-emr-1.28.16/mypy_boto3_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43884 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43810 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-08-01 11:17:33.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85641 2023-08-01 11:17:36.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85523 2023-08-01 11:17:34.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.912894 mypy-boto3-emr-1.28.16/mypy_boto3_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-08-01 11:36:45.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:36:45.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:45.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:45.000000 mypy-boto3-emr-1.28.16/mypy_boto3_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:45.920894 mypy-boto3-emr-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:17:32.000000 mypy-boto3-emr-1.28.16/setup.py
```

### Comparing `mypy-boto3-emr-1.28.15.post1/LICENSE` & `mypy-boto3-emr-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15.post1/PKG-INFO` & `mypy-boto3-emr-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EMR 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 emr type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 emr type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
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
@@ -416,20 +416,20 @@
 )
 
 
 def check_value(value: ActionOnFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_emr.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_emr.type_defs import (
     ResponseMetadataTypeDef,
     TagTypeDef,
     ApplicationOutputTypeDef,
     ApplicationTypeDef,
@@ -449,23 +449,24 @@
     Ec2InstanceAttributesTypeDef,
     KerberosAttributesTypeDef,
     PlacementGroupConfigTypeDef,
     CommandTypeDef,
     ComputeLimitsTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
+    ConfigurationUnionTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
     DeleteStudioInputRequestTypeDef,
     DeleteStudioSessionMappingInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterInputRequestTypeDef,
-    DescribeJobFlowsInputRequestTypeDef,
+    TimestampTypeDef,
     DescribeNotebookExecutionInputRequestTypeDef,
     DescribeReleaseLabelInputRequestTypeDef,
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
@@ -493,19 +494,17 @@
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
     PlacementTypeOutputTypeDef,
     PaginatorConfigTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
-    ListClustersInputRequestTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
     ListInstanceGroupsInputRequestTypeDef,
     ListInstancesInputRequestTypeDef,
-    ListNotebookExecutionsInputRequestTypeDef,
     ReleaseLabelFilterTypeDef,
     ListSecurityConfigurationsInputRequestTypeDef,
     SecurityConfigurationSummaryTypeDef,
     ListStepsInputRequestTypeDef,
     ListStudioSessionMappingsInputRequestTypeDef,
     SessionMappingSummaryTypeDef,
     ListStudiosInputRequestTypeDef,
@@ -543,14 +542,15 @@
     ListReleaseLabelsOutputTypeDef,
     ModifyClusterOutputTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
     StudioTypeDef,
+    ApplicationUnionTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
     BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
     BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
@@ -560,14 +560,17 @@
     ClusterStatusTypeDef,
     ListBootstrapActionsOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
+    DescribeJobFlowsInputRequestTypeDef,
+    ListClustersInputRequestTypeDef,
+    ListNotebookExecutionsInputRequestTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigOutputTypeDef,
     HadoopJarStepConfigTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
@@ -596,16 +599,18 @@
     NotebookExecutionTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
     DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
+    BlockPublicAccessConfigurationUnionTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
+    BootstrapActionConfigUnionTypeDef,
     ScalingTriggerOutputTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
@@ -623,40 +628,41 @@
     StepTypeDef,
     ScalingRuleOutputTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
     StepDetailTypeDef,
-    AddJobFlowStepsInputRequestTypeDef,
+    StepConfigUnionTypeDef,
     ModifyInstanceFleetInputRequestTypeDef,
     ModifyInstanceGroupsInputRequestTypeDef,
     ListInstancesOutputTypeDef,
     InstanceFleetTypeDef,
     ListStepsOutputTypeDef,
     DescribeStepOutputTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyTypeDef,
     InstanceFleetConfigTypeDef,
     JobFlowDetailTypeDef,
+    AddJobFlowStepsInputRequestTypeDef,
     ListInstanceFleetsOutputTypeDef,
     InstanceGroupTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     InstanceGroupConfigTypeDef,
     PutAutoScalingPolicyInputRequestTypeDef,
     AddInstanceFleetInputRequestTypeDef,
     DescribeJobFlowsOutputTypeDef,
     ListInstanceGroupsOutputTypeDef,
     AddInstanceGroupsInputRequestTypeDef,
     JobFlowInstancesConfigTypeDef,
     RunJobFlowInputRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-1.28.15.post1/README.md` & `mypy-boto3-emr-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
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
@@ -384,20 +384,20 @@
 )
 
 
 def check_value(value: ActionOnFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_emr.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_emr.type_defs import (
     ResponseMetadataTypeDef,
     TagTypeDef,
     ApplicationOutputTypeDef,
     ApplicationTypeDef,
@@ -417,23 +417,24 @@
     Ec2InstanceAttributesTypeDef,
     KerberosAttributesTypeDef,
     PlacementGroupConfigTypeDef,
     CommandTypeDef,
     ComputeLimitsTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
+    ConfigurationUnionTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
     DeleteStudioInputRequestTypeDef,
     DeleteStudioSessionMappingInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterInputRequestTypeDef,
-    DescribeJobFlowsInputRequestTypeDef,
+    TimestampTypeDef,
     DescribeNotebookExecutionInputRequestTypeDef,
     DescribeReleaseLabelInputRequestTypeDef,
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
@@ -461,19 +462,17 @@
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
     PlacementTypeOutputTypeDef,
     PaginatorConfigTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
-    ListClustersInputRequestTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
     ListInstanceGroupsInputRequestTypeDef,
     ListInstancesInputRequestTypeDef,
-    ListNotebookExecutionsInputRequestTypeDef,
     ReleaseLabelFilterTypeDef,
     ListSecurityConfigurationsInputRequestTypeDef,
     SecurityConfigurationSummaryTypeDef,
     ListStepsInputRequestTypeDef,
     ListStudioSessionMappingsInputRequestTypeDef,
     SessionMappingSummaryTypeDef,
     ListStudiosInputRequestTypeDef,
@@ -511,14 +510,15 @@
     ListReleaseLabelsOutputTypeDef,
     ModifyClusterOutputTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
     StudioTypeDef,
+    ApplicationUnionTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
     BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
     BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
@@ -528,14 +528,17 @@
     ClusterStatusTypeDef,
     ListBootstrapActionsOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
+    DescribeJobFlowsInputRequestTypeDef,
+    ListClustersInputRequestTypeDef,
+    ListNotebookExecutionsInputRequestTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigOutputTypeDef,
     HadoopJarStepConfigTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
@@ -564,16 +567,18 @@
     NotebookExecutionTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
     DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
+    BlockPublicAccessConfigurationUnionTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
+    BootstrapActionConfigUnionTypeDef,
     ScalingTriggerOutputTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
@@ -591,40 +596,41 @@
     StepTypeDef,
     ScalingRuleOutputTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
     StepDetailTypeDef,
-    AddJobFlowStepsInputRequestTypeDef,
+    StepConfigUnionTypeDef,
     ModifyInstanceFleetInputRequestTypeDef,
     ModifyInstanceGroupsInputRequestTypeDef,
     ListInstancesOutputTypeDef,
     InstanceFleetTypeDef,
     ListStepsOutputTypeDef,
     DescribeStepOutputTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyTypeDef,
     InstanceFleetConfigTypeDef,
     JobFlowDetailTypeDef,
+    AddJobFlowStepsInputRequestTypeDef,
     ListInstanceFleetsOutputTypeDef,
     InstanceGroupTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     InstanceGroupConfigTypeDef,
     PutAutoScalingPolicyInputRequestTypeDef,
     AddInstanceFleetInputRequestTypeDef,
     DescribeJobFlowsOutputTypeDef,
     ListInstanceGroupsOutputTypeDef,
     AddInstanceGroupsInputRequestTypeDef,
     JobFlowInstancesConfigTypeDef,
     RunJobFlowInputRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__init__.py` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__init__.pyi` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__main__.py` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMR 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.EMR 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR\nOther"
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

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/client.py` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_emr.client import EMRClient
 
     session = Session()
     client: EMRClient = session.client("emr")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthModeType,
     ClusterStateType,
     IdentityTypeType,
@@ -45,25 +44,21 @@
     ListStudioSessionMappingsPaginator,
     ListStudiosPaginator,
 )
 from .type_defs import (
     AddInstanceFleetOutputTypeDef,
     AddInstanceGroupsOutputTypeDef,
     AddJobFlowStepsOutputTypeDef,
-    ApplicationOutputTypeDef,
-    ApplicationTypeDef,
+    ApplicationUnionTypeDef,
     AutoScalingPolicyTypeDef,
     AutoTerminationPolicyTypeDef,
-    BlockPublicAccessConfigurationOutputTypeDef,
-    BlockPublicAccessConfigurationTypeDef,
-    BootstrapActionConfigOutputTypeDef,
-    BootstrapActionConfigTypeDef,
+    BlockPublicAccessConfigurationUnionTypeDef,
+    BootstrapActionConfigUnionTypeDef,
     CancelStepsOutputTypeDef,
-    ConfigurationOutputTypeDef,
-    ConfigurationTypeDef,
+    ConfigurationUnionTypeDef,
     CreateSecurityConfigurationOutputTypeDef,
     CreateStudioOutputTypeDef,
     DescribeClusterOutputTypeDef,
     DescribeJobFlowsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     DescribeSecurityConfigurationOutputTypeDef,
@@ -99,18 +94,18 @@
     NotebookS3LocationFromInputTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
     PlacementGroupConfigTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     ReleaseLabelFilterTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
-    StepConfigOutputTypeDef,
-    StepConfigTypeDef,
+    StepConfigUnionTypeDef,
     SupportedProductConfigTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import ClusterRunningWaiter, ClusterTerminatedWaiter, StepCompleteWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -171,15 +166,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#add_instance_groups)
         """
 
     def add_job_flow_steps(
         self,
         *,
         JobFlowId: str,
-        Steps: Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
+        Steps: Sequence[StepConfigUnionTypeDef],
         ExecutionRoleArn: str = ...
     ) -> AddJobFlowStepsOutputTypeDef:
         """
         AddJobFlowSteps adds new steps to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_job_flow_steps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#add_job_flow_steps)
@@ -314,16 +309,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#describe_cluster)
         """
 
     def describe_job_flows(
         self,
         *,
-        CreatedAfter: Union[datetime, str] = ...,
-        CreatedBefore: Union[datetime, str] = ...,
+        CreatedAfter: TimestampTypeDef = ...,
+        CreatedBefore: TimestampTypeDef = ...,
         JobFlowIds: Sequence[str] = ...,
         JobFlowStates: Sequence[JobFlowExecutionStateType] = ...
     ) -> DescribeJobFlowsOutputTypeDef:
         """
         This API is no longer supported and will eventually be removed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_job_flows)
@@ -460,16 +455,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_bootstrap_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_bootstrap_actions)
         """
 
     def list_clusters(
         self,
         *,
-        CreatedAfter: Union[datetime, str] = ...,
-        CreatedBefore: Union[datetime, str] = ...,
+        CreatedAfter: TimestampTypeDef = ...,
+        CreatedBefore: TimestampTypeDef = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
         Marker: str = ...
     ) -> ListClustersOutputTypeDef:
         """
         Provides the status of all clusters visible to this Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_clusters)
@@ -516,16 +511,16 @@
         """
 
     def list_notebook_executions(
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
-        From: Union[datetime, str] = ...,
-        To: Union[datetime, str] = ...,
+        From: TimestampTypeDef = ...,
+        To: TimestampTypeDef = ...,
         Marker: str = ...,
         ExecutionEngineId: str = ...
     ) -> ListNotebookExecutionsOutputTypeDef:
         """
         Provides summaries of all notebook executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_notebook_executions)
@@ -658,19 +653,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_auto_termination_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_auto_termination_policy)
         """
 
     def put_block_public_access_configuration(
-        self,
-        *,
-        BlockPublicAccessConfiguration: Union[
-            BlockPublicAccessConfigurationTypeDef, BlockPublicAccessConfigurationOutputTypeDef
-        ]
+        self, *, BlockPublicAccessConfiguration: BlockPublicAccessConfigurationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon EMR block public access configuration for your
         Amazon Web Services account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_block_public_access_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_block_public_access_configuration)
@@ -726,22 +717,20 @@
         Name: str,
         Instances: JobFlowInstancesConfigTypeDef,
         LogUri: str = ...,
         LogEncryptionKmsKeyId: str = ...,
         AdditionalInfo: str = ...,
         AmiVersion: str = ...,
         ReleaseLabel: str = ...,
-        Steps: Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]] = ...,
-        BootstrapActions: Sequence[
-            Union[BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef]
-        ] = ...,
+        Steps: Sequence[StepConfigUnionTypeDef] = ...,
+        BootstrapActions: Sequence[BootstrapActionConfigUnionTypeDef] = ...,
         SupportedProducts: Sequence[str] = ...,
         NewSupportedProducts: Sequence[SupportedProductConfigTypeDef] = ...,
-        Applications: Sequence[Union[ApplicationTypeDef, ApplicationOutputTypeDef]] = ...,
-        Configurations: Sequence[Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]] = ...,
+        Applications: Sequence[ApplicationUnionTypeDef] = ...,
+        Configurations: Sequence[ConfigurationUnionTypeDef] = ...,
         VisibleToAllUsers: bool = ...,
         JobFlowRole: str = ...,
         ServiceRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SecurityConfiguration: str = ...,
         AutoScalingRole: str = ...,
         ScaleDownBehavior: ScaleDownBehaviorType = ...,
```

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/client.pyi` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_emr.client import EMRClient
 
     session = Session()
     client: EMRClient = session.client("emr")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthModeType,
     ClusterStateType,
     IdentityTypeType,
@@ -45,25 +44,21 @@
     ListStudioSessionMappingsPaginator,
     ListStudiosPaginator,
 )
 from .type_defs import (
     AddInstanceFleetOutputTypeDef,
     AddInstanceGroupsOutputTypeDef,
     AddJobFlowStepsOutputTypeDef,
-    ApplicationOutputTypeDef,
-    ApplicationTypeDef,
+    ApplicationUnionTypeDef,
     AutoScalingPolicyTypeDef,
     AutoTerminationPolicyTypeDef,
-    BlockPublicAccessConfigurationOutputTypeDef,
-    BlockPublicAccessConfigurationTypeDef,
-    BootstrapActionConfigOutputTypeDef,
-    BootstrapActionConfigTypeDef,
+    BlockPublicAccessConfigurationUnionTypeDef,
+    BootstrapActionConfigUnionTypeDef,
     CancelStepsOutputTypeDef,
-    ConfigurationOutputTypeDef,
-    ConfigurationTypeDef,
+    ConfigurationUnionTypeDef,
     CreateSecurityConfigurationOutputTypeDef,
     CreateStudioOutputTypeDef,
     DescribeClusterOutputTypeDef,
     DescribeJobFlowsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     DescribeSecurityConfigurationOutputTypeDef,
@@ -99,18 +94,18 @@
     NotebookS3LocationFromInputTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
     PlacementGroupConfigTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     ReleaseLabelFilterTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
-    StepConfigOutputTypeDef,
-    StepConfigTypeDef,
+    StepConfigUnionTypeDef,
     SupportedProductConfigTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import ClusterRunningWaiter, ClusterTerminatedWaiter, StepCompleteWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -164,15 +159,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_instance_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#add_instance_groups)
         """
     def add_job_flow_steps(
         self,
         *,
         JobFlowId: str,
-        Steps: Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
+        Steps: Sequence[StepConfigUnionTypeDef],
         ExecutionRoleArn: str = ...
     ) -> AddJobFlowStepsOutputTypeDef:
         """
         AddJobFlowSteps adds new steps to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_job_flow_steps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#add_job_flow_steps)
@@ -295,16 +290,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#describe_cluster)
         """
     def describe_job_flows(
         self,
         *,
-        CreatedAfter: Union[datetime, str] = ...,
-        CreatedBefore: Union[datetime, str] = ...,
+        CreatedAfter: TimestampTypeDef = ...,
+        CreatedBefore: TimestampTypeDef = ...,
         JobFlowIds: Sequence[str] = ...,
         JobFlowStates: Sequence[JobFlowExecutionStateType] = ...
     ) -> DescribeJobFlowsOutputTypeDef:
         """
         This API is no longer supported and will eventually be removed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_job_flows)
@@ -428,16 +423,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_bootstrap_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_bootstrap_actions)
         """
     def list_clusters(
         self,
         *,
-        CreatedAfter: Union[datetime, str] = ...,
-        CreatedBefore: Union[datetime, str] = ...,
+        CreatedAfter: TimestampTypeDef = ...,
+        CreatedBefore: TimestampTypeDef = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
         Marker: str = ...
     ) -> ListClustersOutputTypeDef:
         """
         Provides the status of all clusters visible to this Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_clusters)
@@ -480,16 +475,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_instances)
         """
     def list_notebook_executions(
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
-        From: Union[datetime, str] = ...,
-        To: Union[datetime, str] = ...,
+        From: TimestampTypeDef = ...,
+        To: TimestampTypeDef = ...,
         Marker: str = ...,
         ExecutionEngineId: str = ...
     ) -> ListNotebookExecutionsOutputTypeDef:
         """
         Provides summaries of all notebook executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_notebook_executions)
@@ -610,19 +605,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_auto_termination_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_auto_termination_policy)
         """
     def put_block_public_access_configuration(
-        self,
-        *,
-        BlockPublicAccessConfiguration: Union[
-            BlockPublicAccessConfigurationTypeDef, BlockPublicAccessConfigurationOutputTypeDef
-        ]
+        self, *, BlockPublicAccessConfiguration: BlockPublicAccessConfigurationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon EMR block public access configuration for your
         Amazon Web Services account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_block_public_access_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_block_public_access_configuration)
@@ -672,22 +663,20 @@
         Name: str,
         Instances: JobFlowInstancesConfigTypeDef,
         LogUri: str = ...,
         LogEncryptionKmsKeyId: str = ...,
         AdditionalInfo: str = ...,
         AmiVersion: str = ...,
         ReleaseLabel: str = ...,
-        Steps: Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]] = ...,
-        BootstrapActions: Sequence[
-            Union[BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef]
-        ] = ...,
+        Steps: Sequence[StepConfigUnionTypeDef] = ...,
+        BootstrapActions: Sequence[BootstrapActionConfigUnionTypeDef] = ...,
         SupportedProducts: Sequence[str] = ...,
         NewSupportedProducts: Sequence[SupportedProductConfigTypeDef] = ...,
-        Applications: Sequence[Union[ApplicationTypeDef, ApplicationOutputTypeDef]] = ...,
-        Configurations: Sequence[Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]] = ...,
+        Applications: Sequence[ApplicationUnionTypeDef] = ...,
+        Configurations: Sequence[ConfigurationUnionTypeDef] = ...,
         VisibleToAllUsers: bool = ...,
         JobFlowRole: str = ...,
         ServiceRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SecurityConfiguration: str = ...,
         AutoScalingRole: str = ...,
         ScaleDownBehavior: ScaleDownBehaviorType = ...,
```

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/literals.py` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/literals.pyi` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/paginator.py` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     list_notebook_executions_paginator: ListNotebookExecutionsPaginator = client.get_paginator("list_notebook_executions")
     list_security_configurations_paginator: ListSecurityConfigurationsPaginator = client.get_paginator("list_security_configurations")
     list_steps_paginator: ListStepsPaginator = client.get_paginator("list_steps")
     list_studio_session_mappings_paginator: ListStudioSessionMappingsPaginator = client.get_paginator("list_studio_session_mappings")
     list_studios_paginator: ListStudiosPaginator = client.get_paginator("list_studios")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ClusterStateType,
     IdentityTypeType,
     InstanceFleetTypeType,
@@ -59,14 +58,15 @@
     ListInstancesOutputTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStepsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBootstrapActionsPaginator",
     "ListClustersPaginator",
     "ListInstanceFleetsPaginator",
     "ListInstanceGroupsPaginator",
@@ -109,16 +109,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listclusterspaginator)
     """
 
     def paginate(
         self,
         *,
-        CreatedAfter: Union[datetime, str] = ...,
-        CreatedBefore: Union[datetime, str] = ...,
+        CreatedAfter: TimestampTypeDef = ...,
+        CreatedBefore: TimestampTypeDef = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listclusterspaginator)
         """
@@ -184,16 +184,16 @@
     """
 
     def paginate(
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
-        From: Union[datetime, str] = ...,
-        To: Union[datetime, str] = ...,
+        From: TimestampTypeDef = ...,
+        To: TimestampTypeDef = ...,
         ExecutionEngineId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNotebookExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListNotebookExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listnotebookexecutionspaginator)
         """
```

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/paginator.pyi` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     list_notebook_executions_paginator: ListNotebookExecutionsPaginator = client.get_paginator("list_notebook_executions")
     list_security_configurations_paginator: ListSecurityConfigurationsPaginator = client.get_paginator("list_security_configurations")
     list_steps_paginator: ListStepsPaginator = client.get_paginator("list_steps")
     list_studio_session_mappings_paginator: ListStudioSessionMappingsPaginator = client.get_paginator("list_studio_session_mappings")
     list_studios_paginator: ListStudiosPaginator = client.get_paginator("list_studios")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ClusterStateType,
     IdentityTypeType,
     InstanceFleetTypeType,
@@ -59,14 +58,15 @@
     ListInstancesOutputTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStepsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBootstrapActionsPaginator",
     "ListClustersPaginator",
     "ListInstanceFleetsPaginator",
     "ListInstanceGroupsPaginator",
@@ -105,16 +105,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listclusterspaginator)
     """
 
     def paginate(
         self,
         *,
-        CreatedAfter: Union[datetime, str] = ...,
-        CreatedBefore: Union[datetime, str] = ...,
+        CreatedAfter: TimestampTypeDef = ...,
+        CreatedBefore: TimestampTypeDef = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listclusterspaginator)
         """
@@ -176,16 +176,16 @@
     """
 
     def paginate(
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
-        From: Union[datetime, str] = ...,
-        To: Union[datetime, str] = ...,
+        From: TimestampTypeDef = ...,
+        To: TimestampTypeDef = ...,
         ExecutionEngineId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNotebookExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListNotebookExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listnotebookexecutionspaginator)
         """
```

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/type_defs.py` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_emr.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -85,23 +85,24 @@
     "Ec2InstanceAttributesTypeDef",
     "KerberosAttributesTypeDef",
     "PlacementGroupConfigTypeDef",
     "CommandTypeDef",
     "ComputeLimitsTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
+    "ConfigurationUnionTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
     "DeleteStudioInputRequestTypeDef",
     "DeleteStudioSessionMappingInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterInputRequestTypeDef",
-    "DescribeJobFlowsInputRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeNotebookExecutionInputRequestTypeDef",
     "DescribeReleaseLabelInputRequestTypeDef",
     "OSReleaseTypeDef",
     "SimplifiedApplicationTypeDef",
     "DescribeSecurityConfigurationInputRequestTypeDef",
     "DescribeStepInputRequestTypeDef",
     "DescribeStudioInputRequestTypeDef",
@@ -129,19 +130,17 @@
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
     "PlacementTypeOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
-    "ListClustersInputRequestTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
     "ListInstanceGroupsInputRequestTypeDef",
     "ListInstancesInputRequestTypeDef",
-    "ListNotebookExecutionsInputRequestTypeDef",
     "ReleaseLabelFilterTypeDef",
     "ListSecurityConfigurationsInputRequestTypeDef",
     "SecurityConfigurationSummaryTypeDef",
     "ListStepsInputRequestTypeDef",
     "ListStudioSessionMappingsInputRequestTypeDef",
     "SessionMappingSummaryTypeDef",
     "ListStudiosInputRequestTypeDef",
@@ -179,14 +178,15 @@
     "ListReleaseLabelsOutputTypeDef",
     "ModifyClusterOutputTypeDef",
     "RunJobFlowOutputTypeDef",
     "StartNotebookExecutionOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
     "StudioTypeDef",
+    "ApplicationUnionTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
     "BlockPublicAccessConfigurationOutputTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
     "BootstrapActionConfigOutputTypeDef",
     "BootstrapActionConfigTypeDef",
@@ -196,14 +196,17 @@
     "ClusterStatusTypeDef",
     "ListBootstrapActionsOutputTypeDef",
     "ManagedScalingPolicyTypeDef",
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
     "DescribeStepInputStepCompleteWaitTypeDef",
+    "DescribeJobFlowsInputRequestTypeDef",
+    "ListClustersInputRequestTypeDef",
+    "ListNotebookExecutionsInputRequestTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
     "HadoopJarStepConfigOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
@@ -232,16 +235,18 @@
     "NotebookExecutionTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
     "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
+    "BlockPublicAccessConfigurationUnionTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
+    "BootstrapActionConfigUnionTypeDef",
     "ScalingTriggerOutputTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
@@ -259,25 +264,26 @@
     "StepTypeDef",
     "ScalingRuleOutputTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
     "StepDetailTypeDef",
-    "AddJobFlowStepsInputRequestTypeDef",
+    "StepConfigUnionTypeDef",
     "ModifyInstanceFleetInputRequestTypeDef",
     "ModifyInstanceGroupsInputRequestTypeDef",
     "ListInstancesOutputTypeDef",
     "InstanceFleetTypeDef",
     "ListStepsOutputTypeDef",
     "DescribeStepOutputTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyTypeDef",
     "InstanceFleetConfigTypeDef",
     "JobFlowDetailTypeDef",
+    "AddJobFlowStepsInputRequestTypeDef",
     "ListInstanceFleetsOutputTypeDef",
     "InstanceGroupTypeDef",
     "PutAutoScalingPolicyOutputTypeDef",
     "InstanceGroupConfigTypeDef",
     "PutAutoScalingPolicyInputRequestTypeDef",
     "AddInstanceFleetInputRequestTypeDef",
     "DescribeJobFlowsOutputTypeDef",
@@ -605,14 +611,15 @@
         "Classification": str,
         "Configurations": Sequence[Dict[str, Any]],
         "Properties": Mapping[str, str],
     },
     total=False,
 )
 
+ConfigurationUnionTypeDef = Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]
 CreateSecurityConfigurationInputRequestTypeDef = TypedDict(
     "CreateSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
         "SecurityConfiguration": str,
     },
 )
@@ -701,25 +708,15 @@
 DescribeClusterInputRequestTypeDef = TypedDict(
     "DescribeClusterInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 
-DescribeJobFlowsInputRequestTypeDef = TypedDict(
-    "DescribeJobFlowsInputRequestTypeDef",
-    {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "JobFlowIds": Sequence[str],
-        "JobFlowStates": Sequence[JobFlowExecutionStateType],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeNotebookExecutionInputRequestTypeDef = TypedDict(
     "DescribeNotebookExecutionInputRequestTypeDef",
     {
         "NotebookExecutionId": str,
     },
 )
 
@@ -1136,25 +1133,14 @@
 class ListBootstrapActionsInputRequestTypeDef(
     _RequiredListBootstrapActionsInputRequestTypeDef,
     _OptionalListBootstrapActionsInputRequestTypeDef,
 ):
     pass
 
 
-ListClustersInputRequestTypeDef = TypedDict(
-    "ListClustersInputRequestTypeDef",
-    {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "ClusterStates": Sequence[ClusterStateType],
-        "Marker": str,
-    },
-    total=False,
-)
-
 _RequiredListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceFleetsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceFleetsInputRequestTypeDef = TypedDict(
@@ -1215,27 +1201,14 @@
 
 class ListInstancesInputRequestTypeDef(
     _RequiredListInstancesInputRequestTypeDef, _OptionalListInstancesInputRequestTypeDef
 ):
     pass
 
 
-ListNotebookExecutionsInputRequestTypeDef = TypedDict(
-    "ListNotebookExecutionsInputRequestTypeDef",
-    {
-        "EditorId": str,
-        "Status": NotebookExecutionStatusType,
-        "From": Union[datetime, str],
-        "To": Union[datetime, str],
-        "Marker": str,
-        "ExecutionEngineId": str,
-    },
-    total=False,
-)
-
 ReleaseLabelFilterTypeDef = TypedDict(
     "ReleaseLabelFilterTypeDef",
     {
         "Prefix": str,
         "Application": str,
     },
     total=False,
@@ -1774,14 +1747,15 @@
         "IdpAuthUrl": str,
         "IdpRelayStateParameterName": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+ApplicationUnionTypeDef = Union[ApplicationTypeDef, ApplicationOutputTypeDef]
 AutoScalingPolicyStatusTypeDef = TypedDict(
     "AutoScalingPolicyStatusTypeDef",
     {
         "State": AutoScalingPolicyStateType,
         "StateChangeReason": AutoScalingPolicyStateChangeReasonTypeDef,
     },
     total=False,
@@ -2039,14 +2013,49 @@
 class DescribeStepInputStepCompleteWaitTypeDef(
     _RequiredDescribeStepInputStepCompleteWaitTypeDef,
     _OptionalDescribeStepInputStepCompleteWaitTypeDef,
 ):
     pass
 
 
+DescribeJobFlowsInputRequestTypeDef = TypedDict(
+    "DescribeJobFlowsInputRequestTypeDef",
+    {
+        "CreatedAfter": TimestampTypeDef,
+        "CreatedBefore": TimestampTypeDef,
+        "JobFlowIds": Sequence[str],
+        "JobFlowStates": Sequence[JobFlowExecutionStateType],
+    },
+    total=False,
+)
+
+ListClustersInputRequestTypeDef = TypedDict(
+    "ListClustersInputRequestTypeDef",
+    {
+        "CreatedAfter": TimestampTypeDef,
+        "CreatedBefore": TimestampTypeDef,
+        "ClusterStates": Sequence[ClusterStateType],
+        "Marker": str,
+    },
+    total=False,
+)
+
+ListNotebookExecutionsInputRequestTypeDef = TypedDict(
+    "ListNotebookExecutionsInputRequestTypeDef",
+    {
+        "EditorId": str,
+        "Status": NotebookExecutionStatusType,
+        "From": TimestampTypeDef,
+        "To": TimestampTypeDef,
+        "Marker": str,
+        "ExecutionEngineId": str,
+    },
+    total=False,
+)
+
 DescribeReleaseLabelOutputTypeDef = TypedDict(
     "DescribeReleaseLabelOutputTypeDef",
     {
         "ReleaseLabel": str,
         "Applications": List[SimplifiedApplicationTypeDef],
         "NextToken": str,
         "AvailableOSReleases": List[OSReleaseTypeDef],
@@ -2248,16 +2257,16 @@
 ):
     pass
 
 
 ListClustersInputListClustersPaginateTypeDef = TypedDict(
     "ListClustersInputListClustersPaginateTypeDef",
     {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
+        "CreatedAfter": TimestampTypeDef,
+        "CreatedBefore": TimestampTypeDef,
         "ClusterStates": Sequence[ClusterStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
@@ -2332,16 +2341,16 @@
 
 
 ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
     "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     {
         "EditorId": str,
         "Status": NotebookExecutionStatusType,
-        "From": Union[datetime, str],
-        "To": Union[datetime, str],
+        "From": TimestampTypeDef,
+        "To": TimestampTypeDef,
         "ExecutionEngineId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
@@ -2575,14 +2584,17 @@
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationOutputTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BlockPublicAccessConfigurationUnionTypeDef = Union[
+    BlockPublicAccessConfigurationTypeDef, BlockPublicAccessConfigurationOutputTypeDef
+]
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
     },
 )
 
@@ -2590,14 +2602,17 @@
     "BootstrapActionDetailTypeDef",
     {
         "BootstrapActionConfig": BootstrapActionConfigOutputTypeDef,
     },
     total=False,
 )
 
+BootstrapActionConfigUnionTypeDef = Union[
+    BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef
+]
 ScalingTriggerOutputTypeDef = TypedDict(
     "ScalingTriggerOutputTypeDef",
     {
         "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionOutputTypeDef,
     },
 )
 
@@ -2957,36 +2972,15 @@
     "StepDetailTypeDef",
     {
         "StepConfig": StepConfigOutputTypeDef,
         "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
     },
 )
 
-_RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
-    "_RequiredAddJobFlowStepsInputRequestTypeDef",
-    {
-        "JobFlowId": str,
-        "Steps": Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
-    },
-)
-_OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
-    "_OptionalAddJobFlowStepsInputRequestTypeDef",
-    {
-        "ExecutionRoleArn": str,
-    },
-    total=False,
-)
-
-
-class AddJobFlowStepsInputRequestTypeDef(
-    _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
-):
-    pass
-
-
+StepConfigUnionTypeDef = Union[StepConfigTypeDef, StepConfigOutputTypeDef]
 ModifyInstanceFleetInputRequestTypeDef = TypedDict(
     "ModifyInstanceFleetInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceFleet": InstanceFleetModifyConfigTypeDef,
     },
 )
@@ -3116,14 +3110,36 @@
 )
 
 
 class JobFlowDetailTypeDef(_RequiredJobFlowDetailTypeDef, _OptionalJobFlowDetailTypeDef):
     pass
 
 
+_RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
+    "_RequiredAddJobFlowStepsInputRequestTypeDef",
+    {
+        "JobFlowId": str,
+        "Steps": Sequence[StepConfigUnionTypeDef],
+    },
+)
+_OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
+    "_OptionalAddJobFlowStepsInputRequestTypeDef",
+    {
+        "ExecutionRoleArn": str,
+    },
+    total=False,
+)
+
+
+class AddJobFlowStepsInputRequestTypeDef(
+    _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
+):
+    pass
+
+
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3271,22 +3287,20 @@
     "_OptionalRunJobFlowInputRequestTypeDef",
     {
         "LogUri": str,
         "LogEncryptionKmsKeyId": str,
         "AdditionalInfo": str,
         "AmiVersion": str,
         "ReleaseLabel": str,
-        "Steps": Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
-        "BootstrapActions": Sequence[
-            Union[BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef]
-        ],
+        "Steps": Sequence[StepConfigUnionTypeDef],
+        "BootstrapActions": Sequence[BootstrapActionConfigUnionTypeDef],
         "SupportedProducts": Sequence[str],
         "NewSupportedProducts": Sequence[SupportedProductConfigTypeDef],
-        "Applications": Sequence[Union[ApplicationTypeDef, ApplicationOutputTypeDef]],
-        "Configurations": Sequence[Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]],
+        "Applications": Sequence[ApplicationUnionTypeDef],
+        "Configurations": Sequence[ConfigurationUnionTypeDef],
         "VisibleToAllUsers": bool,
         "JobFlowRole": str,
         "ServiceRole": str,
         "Tags": Sequence[TagTypeDef],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
```

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/type_defs.pyi` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_emr.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -84,23 +84,24 @@
     "Ec2InstanceAttributesTypeDef",
     "KerberosAttributesTypeDef",
     "PlacementGroupConfigTypeDef",
     "CommandTypeDef",
     "ComputeLimitsTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
+    "ConfigurationUnionTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
     "DeleteStudioInputRequestTypeDef",
     "DeleteStudioSessionMappingInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterInputRequestTypeDef",
-    "DescribeJobFlowsInputRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeNotebookExecutionInputRequestTypeDef",
     "DescribeReleaseLabelInputRequestTypeDef",
     "OSReleaseTypeDef",
     "SimplifiedApplicationTypeDef",
     "DescribeSecurityConfigurationInputRequestTypeDef",
     "DescribeStepInputRequestTypeDef",
     "DescribeStudioInputRequestTypeDef",
@@ -128,19 +129,17 @@
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
     "PlacementTypeOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
-    "ListClustersInputRequestTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
     "ListInstanceGroupsInputRequestTypeDef",
     "ListInstancesInputRequestTypeDef",
-    "ListNotebookExecutionsInputRequestTypeDef",
     "ReleaseLabelFilterTypeDef",
     "ListSecurityConfigurationsInputRequestTypeDef",
     "SecurityConfigurationSummaryTypeDef",
     "ListStepsInputRequestTypeDef",
     "ListStudioSessionMappingsInputRequestTypeDef",
     "SessionMappingSummaryTypeDef",
     "ListStudiosInputRequestTypeDef",
@@ -178,14 +177,15 @@
     "ListReleaseLabelsOutputTypeDef",
     "ModifyClusterOutputTypeDef",
     "RunJobFlowOutputTypeDef",
     "StartNotebookExecutionOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
     "StudioTypeDef",
+    "ApplicationUnionTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
     "BlockPublicAccessConfigurationOutputTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
     "BootstrapActionConfigOutputTypeDef",
     "BootstrapActionConfigTypeDef",
@@ -195,14 +195,17 @@
     "ClusterStatusTypeDef",
     "ListBootstrapActionsOutputTypeDef",
     "ManagedScalingPolicyTypeDef",
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
     "DescribeStepInputStepCompleteWaitTypeDef",
+    "DescribeJobFlowsInputRequestTypeDef",
+    "ListClustersInputRequestTypeDef",
+    "ListNotebookExecutionsInputRequestTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
     "HadoopJarStepConfigOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
@@ -231,16 +234,18 @@
     "NotebookExecutionTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
     "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
+    "BlockPublicAccessConfigurationUnionTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
+    "BootstrapActionConfigUnionTypeDef",
     "ScalingTriggerOutputTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
@@ -258,25 +263,26 @@
     "StepTypeDef",
     "ScalingRuleOutputTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
     "StepDetailTypeDef",
-    "AddJobFlowStepsInputRequestTypeDef",
+    "StepConfigUnionTypeDef",
     "ModifyInstanceFleetInputRequestTypeDef",
     "ModifyInstanceGroupsInputRequestTypeDef",
     "ListInstancesOutputTypeDef",
     "InstanceFleetTypeDef",
     "ListStepsOutputTypeDef",
     "DescribeStepOutputTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyTypeDef",
     "InstanceFleetConfigTypeDef",
     "JobFlowDetailTypeDef",
+    "AddJobFlowStepsInputRequestTypeDef",
     "ListInstanceFleetsOutputTypeDef",
     "InstanceGroupTypeDef",
     "PutAutoScalingPolicyOutputTypeDef",
     "InstanceGroupConfigTypeDef",
     "PutAutoScalingPolicyInputRequestTypeDef",
     "AddInstanceFleetInputRequestTypeDef",
     "DescribeJobFlowsOutputTypeDef",
@@ -590,14 +596,15 @@
         "Classification": str,
         "Configurations": Sequence[Dict[str, Any]],
         "Properties": Mapping[str, str],
     },
     total=False,
 )
 
+ConfigurationUnionTypeDef = Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]
 CreateSecurityConfigurationInputRequestTypeDef = TypedDict(
     "CreateSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
         "SecurityConfiguration": str,
     },
 )
@@ -682,25 +689,15 @@
 DescribeClusterInputRequestTypeDef = TypedDict(
     "DescribeClusterInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 
-DescribeJobFlowsInputRequestTypeDef = TypedDict(
-    "DescribeJobFlowsInputRequestTypeDef",
-    {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "JobFlowIds": Sequence[str],
-        "JobFlowStates": Sequence[JobFlowExecutionStateType],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeNotebookExecutionInputRequestTypeDef = TypedDict(
     "DescribeNotebookExecutionInputRequestTypeDef",
     {
         "NotebookExecutionId": str,
     },
 )
 
@@ -1103,25 +1100,14 @@
 
 class ListBootstrapActionsInputRequestTypeDef(
     _RequiredListBootstrapActionsInputRequestTypeDef,
     _OptionalListBootstrapActionsInputRequestTypeDef,
 ):
     pass
 
-ListClustersInputRequestTypeDef = TypedDict(
-    "ListClustersInputRequestTypeDef",
-    {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "ClusterStates": Sequence[ClusterStateType],
-        "Marker": str,
-    },
-    total=False,
-)
-
 _RequiredListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceFleetsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceFleetsInputRequestTypeDef = TypedDict(
@@ -1176,27 +1162,14 @@
 )
 
 class ListInstancesInputRequestTypeDef(
     _RequiredListInstancesInputRequestTypeDef, _OptionalListInstancesInputRequestTypeDef
 ):
     pass
 
-ListNotebookExecutionsInputRequestTypeDef = TypedDict(
-    "ListNotebookExecutionsInputRequestTypeDef",
-    {
-        "EditorId": str,
-        "Status": NotebookExecutionStatusType,
-        "From": Union[datetime, str],
-        "To": Union[datetime, str],
-        "Marker": str,
-        "ExecutionEngineId": str,
-    },
-    total=False,
-)
-
 ReleaseLabelFilterTypeDef = TypedDict(
     "ReleaseLabelFilterTypeDef",
     {
         "Prefix": str,
         "Application": str,
     },
     total=False,
@@ -1719,14 +1692,15 @@
         "IdpAuthUrl": str,
         "IdpRelayStateParameterName": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+ApplicationUnionTypeDef = Union[ApplicationTypeDef, ApplicationOutputTypeDef]
 AutoScalingPolicyStatusTypeDef = TypedDict(
     "AutoScalingPolicyStatusTypeDef",
     {
         "State": AutoScalingPolicyStateType,
         "StateChangeReason": AutoScalingPolicyStateChangeReasonTypeDef,
     },
     total=False,
@@ -1968,14 +1942,49 @@
 
 class DescribeStepInputStepCompleteWaitTypeDef(
     _RequiredDescribeStepInputStepCompleteWaitTypeDef,
     _OptionalDescribeStepInputStepCompleteWaitTypeDef,
 ):
     pass
 
+DescribeJobFlowsInputRequestTypeDef = TypedDict(
+    "DescribeJobFlowsInputRequestTypeDef",
+    {
+        "CreatedAfter": TimestampTypeDef,
+        "CreatedBefore": TimestampTypeDef,
+        "JobFlowIds": Sequence[str],
+        "JobFlowStates": Sequence[JobFlowExecutionStateType],
+    },
+    total=False,
+)
+
+ListClustersInputRequestTypeDef = TypedDict(
+    "ListClustersInputRequestTypeDef",
+    {
+        "CreatedAfter": TimestampTypeDef,
+        "CreatedBefore": TimestampTypeDef,
+        "ClusterStates": Sequence[ClusterStateType],
+        "Marker": str,
+    },
+    total=False,
+)
+
+ListNotebookExecutionsInputRequestTypeDef = TypedDict(
+    "ListNotebookExecutionsInputRequestTypeDef",
+    {
+        "EditorId": str,
+        "Status": NotebookExecutionStatusType,
+        "From": TimestampTypeDef,
+        "To": TimestampTypeDef,
+        "Marker": str,
+        "ExecutionEngineId": str,
+    },
+    total=False,
+)
+
 DescribeReleaseLabelOutputTypeDef = TypedDict(
     "DescribeReleaseLabelOutputTypeDef",
     {
         "ReleaseLabel": str,
         "Applications": List[SimplifiedApplicationTypeDef],
         "NextToken": str,
         "AvailableOSReleases": List[OSReleaseTypeDef],
@@ -2167,16 +2176,16 @@
     _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
 ):
     pass
 
 ListClustersInputListClustersPaginateTypeDef = TypedDict(
     "ListClustersInputListClustersPaginateTypeDef",
     {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
+        "CreatedAfter": TimestampTypeDef,
+        "CreatedBefore": TimestampTypeDef,
         "ClusterStates": Sequence[ClusterStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
@@ -2245,16 +2254,16 @@
     pass
 
 ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
     "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     {
         "EditorId": str,
         "Status": NotebookExecutionStatusType,
-        "From": Union[datetime, str],
-        "To": Union[datetime, str],
+        "From": TimestampTypeDef,
+        "To": TimestampTypeDef,
         "ExecutionEngineId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
@@ -2480,14 +2489,17 @@
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationOutputTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BlockPublicAccessConfigurationUnionTypeDef = Union[
+    BlockPublicAccessConfigurationTypeDef, BlockPublicAccessConfigurationOutputTypeDef
+]
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
     },
 )
 
@@ -2495,14 +2507,17 @@
     "BootstrapActionDetailTypeDef",
     {
         "BootstrapActionConfig": BootstrapActionConfigOutputTypeDef,
     },
     total=False,
 )
 
+BootstrapActionConfigUnionTypeDef = Union[
+    BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef
+]
 ScalingTriggerOutputTypeDef = TypedDict(
     "ScalingTriggerOutputTypeDef",
     {
         "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionOutputTypeDef,
     },
 )
 
@@ -2848,34 +2863,15 @@
     "StepDetailTypeDef",
     {
         "StepConfig": StepConfigOutputTypeDef,
         "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
     },
 )
 
-_RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
-    "_RequiredAddJobFlowStepsInputRequestTypeDef",
-    {
-        "JobFlowId": str,
-        "Steps": Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
-    },
-)
-_OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
-    "_OptionalAddJobFlowStepsInputRequestTypeDef",
-    {
-        "ExecutionRoleArn": str,
-    },
-    total=False,
-)
-
-class AddJobFlowStepsInputRequestTypeDef(
-    _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
-):
-    pass
-
+StepConfigUnionTypeDef = Union[StepConfigTypeDef, StepConfigOutputTypeDef]
 ModifyInstanceFleetInputRequestTypeDef = TypedDict(
     "ModifyInstanceFleetInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceFleet": InstanceFleetModifyConfigTypeDef,
     },
 )
@@ -3001,14 +2997,34 @@
     },
     total=False,
 )
 
 class JobFlowDetailTypeDef(_RequiredJobFlowDetailTypeDef, _OptionalJobFlowDetailTypeDef):
     pass
 
+_RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
+    "_RequiredAddJobFlowStepsInputRequestTypeDef",
+    {
+        "JobFlowId": str,
+        "Steps": Sequence[StepConfigUnionTypeDef],
+    },
+)
+_OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
+    "_OptionalAddJobFlowStepsInputRequestTypeDef",
+    {
+        "ExecutionRoleArn": str,
+    },
+    total=False,
+)
+
+class AddJobFlowStepsInputRequestTypeDef(
+    _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
+):
+    pass
+
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3154,22 +3170,20 @@
     "_OptionalRunJobFlowInputRequestTypeDef",
     {
         "LogUri": str,
         "LogEncryptionKmsKeyId": str,
         "AdditionalInfo": str,
         "AmiVersion": str,
         "ReleaseLabel": str,
-        "Steps": Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
-        "BootstrapActions": Sequence[
-            Union[BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef]
-        ],
+        "Steps": Sequence[StepConfigUnionTypeDef],
+        "BootstrapActions": Sequence[BootstrapActionConfigUnionTypeDef],
         "SupportedProducts": Sequence[str],
         "NewSupportedProducts": Sequence[SupportedProductConfigTypeDef],
-        "Applications": Sequence[Union[ApplicationTypeDef, ApplicationOutputTypeDef]],
-        "Configurations": Sequence[Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]],
+        "Applications": Sequence[ApplicationUnionTypeDef],
+        "Configurations": Sequence[ConfigurationUnionTypeDef],
         "VisibleToAllUsers": bool,
         "JobFlowRole": str,
         "ServiceRole": str,
         "Tags": Sequence[TagTypeDef],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
```

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/waiter.py` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/waiter.pyi` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/PKG-INFO` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EMR 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 emr type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 emr type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
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
@@ -416,20 +416,20 @@
 )
 
 
 def check_value(value: ActionOnFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_emr.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_emr.type_defs import (
     ResponseMetadataTypeDef,
     TagTypeDef,
     ApplicationOutputTypeDef,
     ApplicationTypeDef,
@@ -449,23 +449,24 @@
     Ec2InstanceAttributesTypeDef,
     KerberosAttributesTypeDef,
     PlacementGroupConfigTypeDef,
     CommandTypeDef,
     ComputeLimitsTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
+    ConfigurationUnionTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
     DeleteStudioInputRequestTypeDef,
     DeleteStudioSessionMappingInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterInputRequestTypeDef,
-    DescribeJobFlowsInputRequestTypeDef,
+    TimestampTypeDef,
     DescribeNotebookExecutionInputRequestTypeDef,
     DescribeReleaseLabelInputRequestTypeDef,
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
@@ -493,19 +494,17 @@
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
     PlacementTypeOutputTypeDef,
     PaginatorConfigTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
-    ListClustersInputRequestTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
     ListInstanceGroupsInputRequestTypeDef,
     ListInstancesInputRequestTypeDef,
-    ListNotebookExecutionsInputRequestTypeDef,
     ReleaseLabelFilterTypeDef,
     ListSecurityConfigurationsInputRequestTypeDef,
     SecurityConfigurationSummaryTypeDef,
     ListStepsInputRequestTypeDef,
     ListStudioSessionMappingsInputRequestTypeDef,
     SessionMappingSummaryTypeDef,
     ListStudiosInputRequestTypeDef,
@@ -543,14 +542,15 @@
     ListReleaseLabelsOutputTypeDef,
     ModifyClusterOutputTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
     StudioTypeDef,
+    ApplicationUnionTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
     BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
     BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
@@ -560,14 +560,17 @@
     ClusterStatusTypeDef,
     ListBootstrapActionsOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
+    DescribeJobFlowsInputRequestTypeDef,
+    ListClustersInputRequestTypeDef,
+    ListNotebookExecutionsInputRequestTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigOutputTypeDef,
     HadoopJarStepConfigTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
@@ -596,16 +599,18 @@
     NotebookExecutionTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
     DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
+    BlockPublicAccessConfigurationUnionTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
+    BootstrapActionConfigUnionTypeDef,
     ScalingTriggerOutputTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
@@ -623,40 +628,41 @@
     StepTypeDef,
     ScalingRuleOutputTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
     StepDetailTypeDef,
-    AddJobFlowStepsInputRequestTypeDef,
+    StepConfigUnionTypeDef,
     ModifyInstanceFleetInputRequestTypeDef,
     ModifyInstanceGroupsInputRequestTypeDef,
     ListInstancesOutputTypeDef,
     InstanceFleetTypeDef,
     ListStepsOutputTypeDef,
     DescribeStepOutputTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyTypeDef,
     InstanceFleetConfigTypeDef,
     JobFlowDetailTypeDef,
+    AddJobFlowStepsInputRequestTypeDef,
     ListInstanceFleetsOutputTypeDef,
     InstanceGroupTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     InstanceGroupConfigTypeDef,
     PutAutoScalingPolicyInputRequestTypeDef,
     AddInstanceFleetInputRequestTypeDef,
     DescribeJobFlowsOutputTypeDef,
     ListInstanceGroupsOutputTypeDef,
     AddInstanceGroupsInputRequestTypeDef,
     JobFlowInstancesConfigTypeDef,
     RunJobFlowInputRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/SOURCES.txt` & `mypy-boto3-emr-1.28.16/mypy_boto3_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15.post1/setup.py` & `mypy-boto3-emr-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.EMR 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 emr type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 emr type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_emr": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

