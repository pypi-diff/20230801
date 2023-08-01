# Comparing `tmp/mypy-boto3-codedeploy-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-codedeploy-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codedeploy-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:45 2023, max compression
+gzip compressed data, was "mypy-boto3-codedeploy-1.28.16.tar", last modified: Tue Aug  1 11:36:25 2023, max compression
```

## Comparing `mypy-boto3-codedeploy-1.28.15.post1.tar` & `mypy-boto3-codedeploy-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:45.361065 mypy-boto3-codedeploy-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:41.000000 mypy-boto3-codedeploy-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-07-29 10:02:45.353065 mypy-boto3-codedeploy-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-07-29 09:40:41.000000 mypy-boto3-codedeploy-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:45.349065 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-29 09:40:41.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-29 09:40:41.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:40:41.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47150 2023-07-29 09:40:42.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47086 2023-07-29 09:40:41.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-29 09:40:42.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-07-29 09:40:42.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-29 09:40:42.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-07-29 09:40:42.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:41.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53049 2023-07-29 09:40:44.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53016 2023-07-29 09:40:43.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:41.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-29 09:40:42.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-29 09:40:42.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:45.353065 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-07-29 10:02:45.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-29 10:02:45.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:45.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:45.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:45.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:45.000000 mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:45.361065 mypy-boto3-codedeploy-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:40:41.000000 mypy-boto3-codedeploy-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.852928 mypy-boto3-codedeploy-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-08-01 11:36:25.852928 mypy-boto3-codedeploy-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.844928 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46294 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46230 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-08-01 11:13:14.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53952 2023-08-01 11:13:16.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53919 2023-08-01 11:13:14.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.852928 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-08-01 11:36:25.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 11:36:25.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:25.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:25.000000 mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:25.852928 mypy-boto3-codedeploy-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:13:13.000000 mypy-boto3-codedeploy-1.28.16/setup.py
```

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/LICENSE` & `mypy-boto3-codedeploy-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/PKG-INFO` & `mypy-boto3-codedeploy-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codedeploy
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeDeploy 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeDeploy 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codedeploy type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codedeploy type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codedeploy)](https://pepy.tech/project/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
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
@@ -407,20 +407,20 @@
 )
 
 
 def check_value(value: ApplicationRevisionSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codedeploy.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
     AlarmTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
@@ -439,22 +439,21 @@
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
     MinimumHealthyHostsTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
-    TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
     LastDeploymentInfoTypeDef,
+    TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
     TargetGroupInfoTypeDef,
@@ -473,36 +472,38 @@
     PaginatorConfigTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
     ListApplicationsInputRequestTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
-    TimeRangeTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
     TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
     TimeBasedCanaryTypeDef,
     TimeBasedLinearTypeDef,
+    TimestampTypeDef,
+    TriggerConfigTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
     InstanceInfoTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationsOutputTypeDef,
     CreateApplicationOutputTypeDef,
     CreateDeploymentConfigOutputTypeDef,
     CreateDeploymentGroupOutputTypeDef,
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
@@ -533,24 +534,27 @@
     ListApplicationsInputListApplicationsPaginateTypeDef,
     ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
-    ListDeploymentsInputListDeploymentsPaginateTypeDef,
-    ListDeploymentsInputRequestTypeDef,
     RevisionLocationTypeDef,
     TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
     TrafficRoutingConfigTypeDef,
+    TimeRangeTypeDef,
+    TriggerConfigUnionTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
     GetOnPremisesInstanceOutputTypeDef,
+    AlarmConfigurationUnionTypeDef,
     TargetInstancesOutputTypeDef,
+    EC2TagSetUnionTypeDef,
     TargetInstancesTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
     BatchGetApplicationRevisionsInputRequestTypeDef,
     GetApplicationRevisionInputRequestTypeDef,
@@ -558,34 +562,38 @@
     ListApplicationRevisionsOutputTypeDef,
     RegisterApplicationRevisionInputRequestTypeDef,
     RevisionInfoTypeDef,
     LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
     CreateDeploymentConfigInputRequestTypeDef,
     DeploymentConfigInfoTypeDef,
+    ListDeploymentsInputListDeploymentsPaginateTypeDef,
+    ListDeploymentsInputRequestTypeDef,
     CreateDeploymentInputRequestTypeDef,
+    TargetInstancesUnionTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
     CreateDeploymentGroupInputRequestTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     UpdateDeploymentGroupInputRequestTypeDef,
     GetDeploymentConfigOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     GetDeploymentTargetOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     GetDeploymentOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/README.md` & `mypy-boto3-codedeploy-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codedeploy)](https://pepy.tech/project/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
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
@@ -375,20 +375,20 @@
 )
 
 
 def check_value(value: ApplicationRevisionSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codedeploy.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
     AlarmTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
@@ -407,22 +407,21 @@
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
     MinimumHealthyHostsTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
-    TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
     LastDeploymentInfoTypeDef,
+    TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
     TargetGroupInfoTypeDef,
@@ -441,36 +440,38 @@
     PaginatorConfigTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
     ListApplicationsInputRequestTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
-    TimeRangeTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
     TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
     TimeBasedCanaryTypeDef,
     TimeBasedLinearTypeDef,
+    TimestampTypeDef,
+    TriggerConfigTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
     InstanceInfoTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationsOutputTypeDef,
     CreateApplicationOutputTypeDef,
     CreateDeploymentConfigOutputTypeDef,
     CreateDeploymentGroupOutputTypeDef,
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
@@ -501,24 +502,27 @@
     ListApplicationsInputListApplicationsPaginateTypeDef,
     ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
-    ListDeploymentsInputListDeploymentsPaginateTypeDef,
-    ListDeploymentsInputRequestTypeDef,
     RevisionLocationTypeDef,
     TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
     TrafficRoutingConfigTypeDef,
+    TimeRangeTypeDef,
+    TriggerConfigUnionTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
     GetOnPremisesInstanceOutputTypeDef,
+    AlarmConfigurationUnionTypeDef,
     TargetInstancesOutputTypeDef,
+    EC2TagSetUnionTypeDef,
     TargetInstancesTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
     BatchGetApplicationRevisionsInputRequestTypeDef,
     GetApplicationRevisionInputRequestTypeDef,
@@ -526,34 +530,38 @@
     ListApplicationRevisionsOutputTypeDef,
     RegisterApplicationRevisionInputRequestTypeDef,
     RevisionInfoTypeDef,
     LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
     CreateDeploymentConfigInputRequestTypeDef,
     DeploymentConfigInfoTypeDef,
+    ListDeploymentsInputListDeploymentsPaginateTypeDef,
+    ListDeploymentsInputRequestTypeDef,
     CreateDeploymentInputRequestTypeDef,
+    TargetInstancesUnionTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
     CreateDeploymentGroupInputRequestTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     UpdateDeploymentGroupInputRequestTypeDef,
     GetDeploymentConfigOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     GetDeploymentTargetOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     GetDeploymentOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/__init__.py` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/__init__.pyi` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/__main__.py` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeDeploy 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CodeDeploy 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy\nOther"
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

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/client.py` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_codedeploy.client import CodeDeployClient
 
     session = Session()
     client: CodeDeployClient = session.client("codedeploy")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApplicationRevisionSortByType,
     ComputePlatformType,
     DeploymentStatusType,
@@ -41,18 +41,16 @@
     ListDeploymentInstancesPaginator,
     ListDeploymentsPaginator,
     ListDeploymentTargetsPaginator,
     ListGitHubAccountTokenNamesPaginator,
     ListOnPremisesInstancesPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationOutputTypeDef,
-    AlarmConfigurationTypeDef,
-    AutoRollbackConfigurationOutputTypeDef,
-    AutoRollbackConfigurationTypeDef,
+    AlarmConfigurationUnionTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     BatchGetApplicationsOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
@@ -61,16 +59,15 @@
     CreateDeploymentConfigOutputTypeDef,
     CreateDeploymentGroupOutputTypeDef,
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
-    EC2TagSetOutputTypeDef,
-    EC2TagSetTypeDef,
+    EC2TagSetUnionTypeDef,
     ECSServiceTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationOutputTypeDef,
     GetApplicationRevisionOutputTypeDef,
     GetDeploymentConfigOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
@@ -83,30 +80,26 @@
     ListDeploymentGroupsOutputTypeDef,
     ListDeploymentInstancesOutputTypeDef,
     ListDeploymentsOutputTypeDef,
     ListDeploymentTargetsOutputTypeDef,
     ListGitHubAccountTokenNamesOutputTypeDef,
     ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoadBalancerInfoOutputTypeDef,
-    LoadBalancerInfoTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     MinimumHealthyHostsTypeDef,
-    OnPremisesTagSetOutputTypeDef,
-    OnPremisesTagSetTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RevisionLocationTypeDef,
     StopDeploymentOutputTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
-    TargetInstancesOutputTypeDef,
-    TargetInstancesTypeDef,
+    TargetInstancesUnionTypeDef,
     TimeRangeTypeDef,
     TrafficRoutingConfigTypeDef,
-    TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
+    TriggerConfigUnionTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
 )
 from .waiter import DeploymentSuccessfulWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -384,23 +377,19 @@
         *,
         applicationName: str,
         deploymentGroupName: str = ...,
         revision: RevisionLocationTypeDef = ...,
         deploymentConfigName: str = ...,
         description: str = ...,
         ignoreApplicationStopFailures: bool = ...,
-        targetInstances: Union[TargetInstancesTypeDef, TargetInstancesOutputTypeDef] = ...,
-        autoRollbackConfiguration: Union[
-            AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
-        ] = ...,
+        targetInstances: TargetInstancesUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         updateOutdatedInstancesOnly: bool = ...,
         fileExistsBehavior: FileExistsBehaviorType = ...,
-        overrideAlarmConfiguration: Union[
-            AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef
-        ] = ...
+        overrideAlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> CreateDeploymentOutputTypeDef:
         """
         Deploys an application revision through the specified deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/client/#create_deployment)
         """
@@ -426,28 +415,24 @@
         applicationName: str,
         deploymentGroupName: str,
         serviceRoleArn: str,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
-        triggerConfigurations: Sequence[
-            Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
-        ] = ...,
-        alarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...,
-        autoRollbackConfiguration: Union[
-            AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
-        ] = ...,
+        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef] = ...,
-        ec2TagSet: Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef] = ...,
+        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
+        ec2TagSet: EC2TagSetUnionTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef] = ...,
+        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDeploymentGroupOutputTypeDef:
         """
         Creates a deployment group to which application revisions are deployed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/client/#create_deployment_group)
@@ -825,28 +810,24 @@
         currentDeploymentGroupName: str,
         newDeploymentGroupName: str = ...,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
         serviceRoleArn: str = ...,
-        triggerConfigurations: Sequence[
-            Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
-        ] = ...,
-        alarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...,
-        autoRollbackConfiguration: Union[
-            AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
-        ] = ...,
+        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef] = ...,
-        ec2TagSet: Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef] = ...,
+        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
+        ec2TagSet: EC2TagSetUnionTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef] = ...
+        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...
     ) -> UpdateDeploymentGroupOutputTypeDef:
         """
         Changes information about a deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.update_deployment_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/client/#update_deployment_group)
         """
```

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/client.pyi` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_codedeploy.client import CodeDeployClient
 
     session = Session()
     client: CodeDeployClient = session.client("codedeploy")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApplicationRevisionSortByType,
     ComputePlatformType,
     DeploymentStatusType,
@@ -41,18 +41,16 @@
     ListDeploymentInstancesPaginator,
     ListDeploymentsPaginator,
     ListDeploymentTargetsPaginator,
     ListGitHubAccountTokenNamesPaginator,
     ListOnPremisesInstancesPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationOutputTypeDef,
-    AlarmConfigurationTypeDef,
-    AutoRollbackConfigurationOutputTypeDef,
-    AutoRollbackConfigurationTypeDef,
+    AlarmConfigurationUnionTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     BatchGetApplicationsOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
@@ -61,16 +59,15 @@
     CreateDeploymentConfigOutputTypeDef,
     CreateDeploymentGroupOutputTypeDef,
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
-    EC2TagSetOutputTypeDef,
-    EC2TagSetTypeDef,
+    EC2TagSetUnionTypeDef,
     ECSServiceTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationOutputTypeDef,
     GetApplicationRevisionOutputTypeDef,
     GetDeploymentConfigOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
@@ -83,30 +80,26 @@
     ListDeploymentGroupsOutputTypeDef,
     ListDeploymentInstancesOutputTypeDef,
     ListDeploymentsOutputTypeDef,
     ListDeploymentTargetsOutputTypeDef,
     ListGitHubAccountTokenNamesOutputTypeDef,
     ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoadBalancerInfoOutputTypeDef,
-    LoadBalancerInfoTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     MinimumHealthyHostsTypeDef,
-    OnPremisesTagSetOutputTypeDef,
-    OnPremisesTagSetTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RevisionLocationTypeDef,
     StopDeploymentOutputTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
-    TargetInstancesOutputTypeDef,
-    TargetInstancesTypeDef,
+    TargetInstancesUnionTypeDef,
     TimeRangeTypeDef,
     TrafficRoutingConfigTypeDef,
-    TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
+    TriggerConfigUnionTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
 )
 from .waiter import DeploymentSuccessfulWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -367,23 +360,19 @@
         *,
         applicationName: str,
         deploymentGroupName: str = ...,
         revision: RevisionLocationTypeDef = ...,
         deploymentConfigName: str = ...,
         description: str = ...,
         ignoreApplicationStopFailures: bool = ...,
-        targetInstances: Union[TargetInstancesTypeDef, TargetInstancesOutputTypeDef] = ...,
-        autoRollbackConfiguration: Union[
-            AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
-        ] = ...,
+        targetInstances: TargetInstancesUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         updateOutdatedInstancesOnly: bool = ...,
         fileExistsBehavior: FileExistsBehaviorType = ...,
-        overrideAlarmConfiguration: Union[
-            AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef
-        ] = ...
+        overrideAlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> CreateDeploymentOutputTypeDef:
         """
         Deploys an application revision through the specified deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/client/#create_deployment)
         """
@@ -407,28 +396,24 @@
         applicationName: str,
         deploymentGroupName: str,
         serviceRoleArn: str,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
-        triggerConfigurations: Sequence[
-            Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
-        ] = ...,
-        alarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...,
-        autoRollbackConfiguration: Union[
-            AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
-        ] = ...,
+        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef] = ...,
-        ec2TagSet: Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef] = ...,
+        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
+        ec2TagSet: EC2TagSetUnionTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef] = ...,
+        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDeploymentGroupOutputTypeDef:
         """
         Creates a deployment group to which application revisions are deployed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/client/#create_deployment_group)
@@ -771,28 +756,24 @@
         currentDeploymentGroupName: str,
         newDeploymentGroupName: str = ...,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
         serviceRoleArn: str = ...,
-        triggerConfigurations: Sequence[
-            Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
-        ] = ...,
-        alarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...,
-        autoRollbackConfiguration: Union[
-            AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
-        ] = ...,
+        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef] = ...,
-        ec2TagSet: Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef] = ...,
+        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
+        ec2TagSet: EC2TagSetUnionTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef] = ...
+        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...
     ) -> UpdateDeploymentGroupOutputTypeDef:
         """
         Changes information about a deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.update_deployment_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/client/#update_deployment_group)
         """
```

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/literals.py` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/literals.pyi` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/paginator.py` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/paginator.pyi` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/type_defs.py` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codedeploy.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,15 +52,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "AlarmTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
     "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
@@ -77,22 +76,21 @@
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
     "MinimumHealthyHostsTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
-    "TriggerConfigOutputTypeDef",
-    "TriggerConfigTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     "LastDeploymentInfoTypeDef",
+    "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
     "TargetGroupInfoTypeDef",
@@ -111,36 +109,38 @@
     "PaginatorConfigTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
     "ListApplicationsInputRequestTypeDef",
     "ListDeploymentConfigsInputRequestTypeDef",
     "ListDeploymentGroupsInputRequestTypeDef",
     "ListDeploymentInstancesInputRequestTypeDef",
     "ListDeploymentTargetsInputRequestTypeDef",
-    "TimeRangeTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
     "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
     "TimeBasedCanaryTypeDef",
     "TimeBasedLinearTypeDef",
+    "TimestampTypeDef",
+    "TriggerConfigTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
     "InstanceInfoTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
+    "AutoRollbackConfigurationUnionTypeDef",
     "BatchGetApplicationsOutputTypeDef",
     "CreateApplicationOutputTypeDef",
     "CreateDeploymentConfigOutputTypeDef",
     "CreateDeploymentGroupOutputTypeDef",
     "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
     "DeleteGitHubAccountTokenOutputTypeDef",
@@ -171,24 +171,27 @@
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
-    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
-    "ListDeploymentsInputRequestTypeDef",
     "RevisionLocationTypeDef",
     "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
     "TrafficRoutingConfigTypeDef",
+    "TimeRangeTypeDef",
+    "TriggerConfigUnionTypeDef",
     "BatchGetOnPremisesInstancesOutputTypeDef",
     "GetOnPremisesInstanceOutputTypeDef",
+    "AlarmConfigurationUnionTypeDef",
     "TargetInstancesOutputTypeDef",
+    "EC2TagSetUnionTypeDef",
     "TargetInstancesTypeDef",
+    "OnPremisesTagSetUnionTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
     "BatchGetApplicationRevisionsInputRequestTypeDef",
     "GetApplicationRevisionInputRequestTypeDef",
@@ -196,22 +199,26 @@
     "ListApplicationRevisionsOutputTypeDef",
     "RegisterApplicationRevisionInputRequestTypeDef",
     "RevisionInfoTypeDef",
     "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
     "CreateDeploymentConfigInputRequestTypeDef",
     "DeploymentConfigInfoTypeDef",
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    "ListDeploymentsInputRequestTypeDef",
     "CreateDeploymentInputRequestTypeDef",
+    "TargetInstancesUnionTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
     "CreateDeploymentGroupInputRequestTypeDef",
+    "LoadBalancerInfoUnionTypeDef",
     "UpdateDeploymentGroupInputRequestTypeDef",
     "GetDeploymentConfigOutputTypeDef",
     "BatchGetDeploymentTargetsOutputTypeDef",
     "GetDeploymentTargetOutputTypeDef",
     "BatchGetDeploymentGroupsOutputTypeDef",
     "GetDeploymentGroupOutputTypeDef",
     "BatchGetDeploymentsOutputTypeDef",
@@ -419,34 +426,14 @@
         "Key": str,
         "Value": str,
         "Type": TagFilterTypeType,
     },
     total=False,
 )
 
-TriggerConfigOutputTypeDef = TypedDict(
-    "TriggerConfigOutputTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": List[TriggerEventTypeType],
-    },
-    total=False,
-)
-
-TriggerConfigTypeDef = TypedDict(
-    "TriggerConfigTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": Sequence[TriggerEventTypeType],
-    },
-    total=False,
-)
-
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -488,14 +475,24 @@
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
+TriggerConfigOutputTypeDef = TypedDict(
+    "TriggerConfigOutputTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": List[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 DeploymentOverviewTypeDef = TypedDict(
     "DeploymentOverviewTypeDef",
     {
         "Pending": int,
         "InProgress": int,
         "Succeeded": int,
         "Failed": int,
@@ -687,22 +684,20 @@
         "s3KeyPrefix": str,
         "deployed": ListStateFilterActionType,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationRevisionsInputRequestTypeDef(
     _RequiredListApplicationRevisionsInputRequestTypeDef,
     _OptionalListApplicationRevisionsInputRequestTypeDef,
 ):
     pass
 
-
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -725,22 +720,20 @@
     "_OptionalListDeploymentGroupsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListDeploymentGroupsInputRequestTypeDef(
     _RequiredListDeploymentGroupsInputRequestTypeDef,
     _OptionalListDeploymentGroupsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDeploymentInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 _OptionalListDeploymentInstancesInputRequestTypeDef = TypedDict(
@@ -749,41 +742,30 @@
         "nextToken": str,
         "instanceStatusFilter": Sequence[InstanceStatusType],
         "instanceTypeFilter": Sequence[InstanceTypeType],
     },
     total=False,
 )
 
-
 class ListDeploymentInstancesInputRequestTypeDef(
     _RequiredListDeploymentInstancesInputRequestTypeDef,
     _OptionalListDeploymentInstancesInputRequestTypeDef,
 ):
     pass
 
-
 ListDeploymentTargetsInputRequestTypeDef = TypedDict(
     "ListDeploymentTargetsInputRequestTypeDef",
     {
         "deploymentId": str,
         "nextToken": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "start": Union[datetime, str],
-        "end": Union[datetime, str],
-    },
-    total=False,
-)
-
 ListGitHubAccountTokenNamesInputRequestTypeDef = TypedDict(
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -798,21 +780,19 @@
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-
 PutLifecycleEventHookExecutionStatusInputRequestTypeDef = TypedDict(
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     {
         "deploymentId": str,
         "lifecycleEventHookExecutionId": str,
         "status": LifecycleEventStatusType,
     },
@@ -839,22 +819,20 @@
     {
         "iamSessionArn": str,
         "iamUserArn": str,
     },
     total=False,
 )
 
-
 class RegisterOnPremisesInstanceInputRequestTypeDef(
     _RequiredRegisterOnPremisesInstanceInputRequestTypeDef,
     _OptionalRegisterOnPremisesInstanceInputRequestTypeDef,
 ):
     pass
 
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
         "version": str,
@@ -881,21 +859,19 @@
     "_OptionalStopDeploymentInputRequestTypeDef",
     {
         "autoRollbackEnabled": bool,
     },
     total=False,
 )
 
-
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
-
 TrafficRouteOutputTypeDef = TypedDict(
     "TrafficRouteOutputTypeDef",
     {
         "listenerArns": List[str],
     },
     total=False,
 )
@@ -922,14 +898,25 @@
     {
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
+TriggerConfigTypeDef = TypedDict(
+    "TriggerConfigTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": Sequence[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -962,21 +949,19 @@
     {
         "computePlatform": ComputePlatformType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateApplicationInputRequestTypeDef(
     _RequiredCreateApplicationInputRequestTypeDef, _OptionalCreateApplicationInputRequestTypeDef
 ):
     pass
 
-
 InstanceInfoTypeDef = TypedDict(
     "InstanceInfoTypeDef",
     {
         "instanceName": str,
         "iamSessionArn": str,
         "iamUserArn": str,
         "instanceArn": str,
@@ -1019,14 +1004,17 @@
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
         "alarms": Sequence[AlarmTypeDef],
     },
     total=False,
 )
 
+AutoRollbackConfigurationUnionTypeDef = Union[
+    AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
+]
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1290,22 +1278,20 @@
     "_OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
-
 _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
     "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
@@ -1317,22 +1303,20 @@
         "s3KeyPrefix": str,
         "deployed": ListStateFilterActionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
     _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
     _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
 ):
     pass
 
-
 ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1355,22 +1339,20 @@
     "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
     _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     {
         "deploymentId": str,
     },
 )
 _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
@@ -1379,22 +1361,20 @@
         "instanceStatusFilter": Sequence[InstanceStatusType],
         "instanceTypeFilter": Sequence[InstanceTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
     _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
 ):
     pass
 
-
 ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
     "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     {
         "deploymentId": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1415,40 +1395,14 @@
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
-    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "externalId": str,
-        "includeOnlyStatuses": Sequence[DeploymentStatusType],
-        "createTimeRange": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDeploymentsInputRequestTypeDef = TypedDict(
-    "ListDeploymentsInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "externalId": str,
-        "includeOnlyStatuses": Sequence[DeploymentStatusType],
-        "createTimeRange": TimeRangeTypeDef,
-        "nextToken": str,
-    },
-    total=False,
-)
-
 RevisionLocationTypeDef = TypedDict(
     "RevisionLocationTypeDef",
     {
         "revisionType": RevisionLocationTypeType,
         "s3Location": S3LocationTypeDef,
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
@@ -1483,14 +1437,24 @@
         "type": TrafficRoutingTypeType,
         "timeBasedCanary": TimeBasedCanaryTypeDef,
         "timeBasedLinear": TimeBasedLinearTypeDef,
     },
     total=False,
 )
 
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "start": TimestampTypeDef,
+        "end": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesOutputTypeDef",
     {
         "instanceInfos": List[InstanceInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1499,34 +1463,37 @@
     "GetOnPremisesInstanceOutputTypeDef",
     {
         "instanceInfo": InstanceInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
 TargetInstancesOutputTypeDef = TypedDict(
     "TargetInstancesOutputTypeDef",
     {
         "tagFilters": List[EC2TagFilterTypeDef],
         "autoScalingGroups": List[str],
         "ec2TagSet": EC2TagSetOutputTypeDef,
     },
     total=False,
 )
 
+EC2TagSetUnionTypeDef = Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef]
 TargetInstancesTypeDef = TypedDict(
     "TargetInstancesTypeDef",
     {
         "tagFilters": Sequence[EC2TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
         "ec2TagSet": EC2TagSetTypeDef,
     },
     total=False,
 )
 
+OnPremisesTagSetUnionTypeDef = Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef]
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
         "deploymentId": str,
         "targetId": str,
         "lastUpdatedAt": datetime,
         "lifecycleEvents": List[LifecycleEventTypeDef],
@@ -1638,22 +1605,20 @@
     "_OptionalRegisterApplicationRevisionInputRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class RegisterApplicationRevisionInputRequestTypeDef(
     _RequiredRegisterApplicationRevisionInputRequestTypeDef,
     _OptionalRegisterApplicationRevisionInputRequestTypeDef,
 ):
     pass
 
-
 RevisionInfoTypeDef = TypedDict(
     "RevisionInfoTypeDef",
     {
         "revisionLocation": RevisionLocationTypeDef,
         "genericRevisionInfo": GenericRevisionInfoTypeDef,
     },
     total=False,
@@ -1691,35 +1656,59 @@
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
-
 class CreateDeploymentConfigInputRequestTypeDef(
     _RequiredCreateDeploymentConfigInputRequestTypeDef,
     _OptionalCreateDeploymentConfigInputRequestTypeDef,
 ):
     pass
 
-
 DeploymentConfigInfoTypeDef = TypedDict(
     "DeploymentConfigInfoTypeDef",
     {
         "deploymentConfigId": str,
         "deploymentConfigName": str,
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "createTime": datetime,
         "computePlatform": ComputePlatformType,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
     },
     total=False,
 )
 
+ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "externalId": str,
+        "includeOnlyStatuses": Sequence[DeploymentStatusType],
+        "createTimeRange": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentsInputRequestTypeDef = TypedDict(
+    "ListDeploymentsInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "externalId": str,
+        "includeOnlyStatuses": Sequence[DeploymentStatusType],
+        "createTimeRange": TimeRangeTypeDef,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredCreateDeploymentInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalCreateDeploymentInputRequestTypeDef = TypedDict(
@@ -1735,21 +1724,20 @@
         "updateOutdatedInstancesOnly": bool,
         "fileExistsBehavior": FileExistsBehaviorType,
         "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateDeploymentInputRequestTypeDef(
     _RequiredCreateDeploymentInputRequestTypeDef, _OptionalCreateDeploymentInputRequestTypeDef
 ):
     pass
 
-
+TargetInstancesUnionTypeDef = Union[TargetInstancesTypeDef, TargetInstancesOutputTypeDef]
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1862,37 +1850,36 @@
 _OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_OptionalCreateDeploymentGroupInputRequestTypeDef",
     {
         "deploymentConfigName": str,
         "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
-        "triggerConfigurations": Sequence[Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]],
+        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
         "alarmConfiguration": AlarmConfigurationTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "deploymentStyle": DeploymentStyleTypeDef,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "ec2TagSet": EC2TagSetTypeDef,
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeploymentGroupInputRequestTypeDef(
     _RequiredCreateDeploymentGroupInputRequestTypeDef,
     _OptionalCreateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
-
+LoadBalancerInfoUnionTypeDef = Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef]
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
@@ -1901,36 +1888,34 @@
     {
         "newDeploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
         "serviceRoleArn": str,
-        "triggerConfigurations": Sequence[Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]],
+        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
         "alarmConfiguration": AlarmConfigurationTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "deploymentStyle": DeploymentStyleTypeDef,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "ec2TagSet": EC2TagSetTypeDef,
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDeploymentGroupInputRequestTypeDef(
     _RequiredUpdateDeploymentGroupInputRequestTypeDef,
     _OptionalUpdateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
-
 GetDeploymentConfigOutputTypeDef = TypedDict(
     "GetDeploymentConfigOutputTypeDef",
     {
         "deploymentConfigInfo": DeploymentConfigInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/type_defs.pyi` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codedeploy.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,14 +52,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
     "AlarmTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
     "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
@@ -76,22 +77,21 @@
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
     "MinimumHealthyHostsTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
-    "TriggerConfigOutputTypeDef",
-    "TriggerConfigTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     "LastDeploymentInfoTypeDef",
+    "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
     "TargetGroupInfoTypeDef",
@@ -110,36 +110,38 @@
     "PaginatorConfigTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
     "ListApplicationsInputRequestTypeDef",
     "ListDeploymentConfigsInputRequestTypeDef",
     "ListDeploymentGroupsInputRequestTypeDef",
     "ListDeploymentInstancesInputRequestTypeDef",
     "ListDeploymentTargetsInputRequestTypeDef",
-    "TimeRangeTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
     "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
     "TimeBasedCanaryTypeDef",
     "TimeBasedLinearTypeDef",
+    "TimestampTypeDef",
+    "TriggerConfigTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
     "InstanceInfoTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
+    "AutoRollbackConfigurationUnionTypeDef",
     "BatchGetApplicationsOutputTypeDef",
     "CreateApplicationOutputTypeDef",
     "CreateDeploymentConfigOutputTypeDef",
     "CreateDeploymentGroupOutputTypeDef",
     "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
     "DeleteGitHubAccountTokenOutputTypeDef",
@@ -170,24 +172,27 @@
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
-    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
-    "ListDeploymentsInputRequestTypeDef",
     "RevisionLocationTypeDef",
     "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
     "TrafficRoutingConfigTypeDef",
+    "TimeRangeTypeDef",
+    "TriggerConfigUnionTypeDef",
     "BatchGetOnPremisesInstancesOutputTypeDef",
     "GetOnPremisesInstanceOutputTypeDef",
+    "AlarmConfigurationUnionTypeDef",
     "TargetInstancesOutputTypeDef",
+    "EC2TagSetUnionTypeDef",
     "TargetInstancesTypeDef",
+    "OnPremisesTagSetUnionTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
     "BatchGetApplicationRevisionsInputRequestTypeDef",
     "GetApplicationRevisionInputRequestTypeDef",
@@ -195,22 +200,26 @@
     "ListApplicationRevisionsOutputTypeDef",
     "RegisterApplicationRevisionInputRequestTypeDef",
     "RevisionInfoTypeDef",
     "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
     "CreateDeploymentConfigInputRequestTypeDef",
     "DeploymentConfigInfoTypeDef",
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    "ListDeploymentsInputRequestTypeDef",
     "CreateDeploymentInputRequestTypeDef",
+    "TargetInstancesUnionTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
     "CreateDeploymentGroupInputRequestTypeDef",
+    "LoadBalancerInfoUnionTypeDef",
     "UpdateDeploymentGroupInputRequestTypeDef",
     "GetDeploymentConfigOutputTypeDef",
     "BatchGetDeploymentTargetsOutputTypeDef",
     "GetDeploymentTargetOutputTypeDef",
     "BatchGetDeploymentGroupsOutputTypeDef",
     "GetDeploymentGroupOutputTypeDef",
     "BatchGetDeploymentsOutputTypeDef",
@@ -418,34 +427,14 @@
         "Key": str,
         "Value": str,
         "Type": TagFilterTypeType,
     },
     total=False,
 )
 
-TriggerConfigOutputTypeDef = TypedDict(
-    "TriggerConfigOutputTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": List[TriggerEventTypeType],
-    },
-    total=False,
-)
-
-TriggerConfigTypeDef = TypedDict(
-    "TriggerConfigTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": Sequence[TriggerEventTypeType],
-    },
-    total=False,
-)
-
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -487,14 +476,24 @@
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
+TriggerConfigOutputTypeDef = TypedDict(
+    "TriggerConfigOutputTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": List[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 DeploymentOverviewTypeDef = TypedDict(
     "DeploymentOverviewTypeDef",
     {
         "Pending": int,
         "InProgress": int,
         "Succeeded": int,
         "Failed": int,
@@ -686,20 +685,22 @@
         "s3KeyPrefix": str,
         "deployed": ListStateFilterActionType,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationRevisionsInputRequestTypeDef(
     _RequiredListApplicationRevisionsInputRequestTypeDef,
     _OptionalListApplicationRevisionsInputRequestTypeDef,
 ):
     pass
 
+
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -722,20 +723,22 @@
     "_OptionalListDeploymentGroupsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListDeploymentGroupsInputRequestTypeDef(
     _RequiredListDeploymentGroupsInputRequestTypeDef,
     _OptionalListDeploymentGroupsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDeploymentInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 _OptionalListDeploymentInstancesInputRequestTypeDef = TypedDict(
@@ -744,39 +747,32 @@
         "nextToken": str,
         "instanceStatusFilter": Sequence[InstanceStatusType],
         "instanceTypeFilter": Sequence[InstanceTypeType],
     },
     total=False,
 )
 
+
 class ListDeploymentInstancesInputRequestTypeDef(
     _RequiredListDeploymentInstancesInputRequestTypeDef,
     _OptionalListDeploymentInstancesInputRequestTypeDef,
 ):
     pass
 
+
 ListDeploymentTargetsInputRequestTypeDef = TypedDict(
     "ListDeploymentTargetsInputRequestTypeDef",
     {
         "deploymentId": str,
         "nextToken": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "start": Union[datetime, str],
-        "end": Union[datetime, str],
-    },
-    total=False,
-)
-
 ListGitHubAccountTokenNamesInputRequestTypeDef = TypedDict(
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -791,19 +787,21 @@
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+
 PutLifecycleEventHookExecutionStatusInputRequestTypeDef = TypedDict(
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     {
         "deploymentId": str,
         "lifecycleEventHookExecutionId": str,
         "status": LifecycleEventStatusType,
     },
@@ -830,20 +828,22 @@
     {
         "iamSessionArn": str,
         "iamUserArn": str,
     },
     total=False,
 )
 
+
 class RegisterOnPremisesInstanceInputRequestTypeDef(
     _RequiredRegisterOnPremisesInstanceInputRequestTypeDef,
     _OptionalRegisterOnPremisesInstanceInputRequestTypeDef,
 ):
     pass
 
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
         "version": str,
@@ -870,19 +870,21 @@
     "_OptionalStopDeploymentInputRequestTypeDef",
     {
         "autoRollbackEnabled": bool,
     },
     total=False,
 )
 
+
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
+
 TrafficRouteOutputTypeDef = TypedDict(
     "TrafficRouteOutputTypeDef",
     {
         "listenerArns": List[str],
     },
     total=False,
 )
@@ -909,14 +911,25 @@
     {
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
+TriggerConfigTypeDef = TypedDict(
+    "TriggerConfigTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": Sequence[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -949,19 +962,21 @@
     {
         "computePlatform": ComputePlatformType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateApplicationInputRequestTypeDef(
     _RequiredCreateApplicationInputRequestTypeDef, _OptionalCreateApplicationInputRequestTypeDef
 ):
     pass
 
+
 InstanceInfoTypeDef = TypedDict(
     "InstanceInfoTypeDef",
     {
         "instanceName": str,
         "iamSessionArn": str,
         "iamUserArn": str,
         "instanceArn": str,
@@ -1004,14 +1019,17 @@
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
         "alarms": Sequence[AlarmTypeDef],
     },
     total=False,
 )
 
+AutoRollbackConfigurationUnionTypeDef = Union[
+    AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
+]
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1275,20 +1293,22 @@
     "_OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
+
 _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
     "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
@@ -1300,20 +1320,22 @@
         "s3KeyPrefix": str,
         "deployed": ListStateFilterActionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
     _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
     _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
 ):
     pass
 
+
 ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1336,20 +1358,22 @@
     "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
     _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     {
         "deploymentId": str,
     },
 )
 _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
@@ -1358,20 +1382,22 @@
         "instanceStatusFilter": Sequence[InstanceStatusType],
         "instanceTypeFilter": Sequence[InstanceTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
     _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
 ):
     pass
 
+
 ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
     "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     {
         "deploymentId": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1392,40 +1418,14 @@
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
-    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "externalId": str,
-        "includeOnlyStatuses": Sequence[DeploymentStatusType],
-        "createTimeRange": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDeploymentsInputRequestTypeDef = TypedDict(
-    "ListDeploymentsInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "externalId": str,
-        "includeOnlyStatuses": Sequence[DeploymentStatusType],
-        "createTimeRange": TimeRangeTypeDef,
-        "nextToken": str,
-    },
-    total=False,
-)
-
 RevisionLocationTypeDef = TypedDict(
     "RevisionLocationTypeDef",
     {
         "revisionType": RevisionLocationTypeType,
         "s3Location": S3LocationTypeDef,
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
@@ -1460,14 +1460,24 @@
         "type": TrafficRoutingTypeType,
         "timeBasedCanary": TimeBasedCanaryTypeDef,
         "timeBasedLinear": TimeBasedLinearTypeDef,
     },
     total=False,
 )
 
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "start": TimestampTypeDef,
+        "end": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesOutputTypeDef",
     {
         "instanceInfos": List[InstanceInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1476,34 +1486,37 @@
     "GetOnPremisesInstanceOutputTypeDef",
     {
         "instanceInfo": InstanceInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
 TargetInstancesOutputTypeDef = TypedDict(
     "TargetInstancesOutputTypeDef",
     {
         "tagFilters": List[EC2TagFilterTypeDef],
         "autoScalingGroups": List[str],
         "ec2TagSet": EC2TagSetOutputTypeDef,
     },
     total=False,
 )
 
+EC2TagSetUnionTypeDef = Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef]
 TargetInstancesTypeDef = TypedDict(
     "TargetInstancesTypeDef",
     {
         "tagFilters": Sequence[EC2TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
         "ec2TagSet": EC2TagSetTypeDef,
     },
     total=False,
 )
 
+OnPremisesTagSetUnionTypeDef = Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef]
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
         "deploymentId": str,
         "targetId": str,
         "lastUpdatedAt": datetime,
         "lifecycleEvents": List[LifecycleEventTypeDef],
@@ -1615,20 +1628,22 @@
     "_OptionalRegisterApplicationRevisionInputRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class RegisterApplicationRevisionInputRequestTypeDef(
     _RequiredRegisterApplicationRevisionInputRequestTypeDef,
     _OptionalRegisterApplicationRevisionInputRequestTypeDef,
 ):
     pass
 
+
 RevisionInfoTypeDef = TypedDict(
     "RevisionInfoTypeDef",
     {
         "revisionLocation": RevisionLocationTypeDef,
         "genericRevisionInfo": GenericRevisionInfoTypeDef,
     },
     total=False,
@@ -1666,33 +1681,61 @@
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
+
 class CreateDeploymentConfigInputRequestTypeDef(
     _RequiredCreateDeploymentConfigInputRequestTypeDef,
     _OptionalCreateDeploymentConfigInputRequestTypeDef,
 ):
     pass
 
+
 DeploymentConfigInfoTypeDef = TypedDict(
     "DeploymentConfigInfoTypeDef",
     {
         "deploymentConfigId": str,
         "deploymentConfigName": str,
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "createTime": datetime,
         "computePlatform": ComputePlatformType,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
     },
     total=False,
 )
 
+ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "externalId": str,
+        "includeOnlyStatuses": Sequence[DeploymentStatusType],
+        "createTimeRange": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentsInputRequestTypeDef = TypedDict(
+    "ListDeploymentsInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "externalId": str,
+        "includeOnlyStatuses": Sequence[DeploymentStatusType],
+        "createTimeRange": TimeRangeTypeDef,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredCreateDeploymentInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalCreateDeploymentInputRequestTypeDef = TypedDict(
@@ -1708,19 +1751,22 @@
         "updateOutdatedInstancesOnly": bool,
         "fileExistsBehavior": FileExistsBehaviorType,
         "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateDeploymentInputRequestTypeDef(
     _RequiredCreateDeploymentInputRequestTypeDef, _OptionalCreateDeploymentInputRequestTypeDef
 ):
     pass
 
+
+TargetInstancesUnionTypeDef = Union[TargetInstancesTypeDef, TargetInstancesOutputTypeDef]
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1833,35 +1879,38 @@
 _OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_OptionalCreateDeploymentGroupInputRequestTypeDef",
     {
         "deploymentConfigName": str,
         "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
-        "triggerConfigurations": Sequence[Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]],
+        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
         "alarmConfiguration": AlarmConfigurationTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "deploymentStyle": DeploymentStyleTypeDef,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "ec2TagSet": EC2TagSetTypeDef,
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeploymentGroupInputRequestTypeDef(
     _RequiredCreateDeploymentGroupInputRequestTypeDef,
     _OptionalCreateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
+
+LoadBalancerInfoUnionTypeDef = Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef]
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
@@ -1870,34 +1919,36 @@
     {
         "newDeploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
         "serviceRoleArn": str,
-        "triggerConfigurations": Sequence[Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]],
+        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
         "alarmConfiguration": AlarmConfigurationTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "deploymentStyle": DeploymentStyleTypeDef,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "ec2TagSet": EC2TagSetTypeDef,
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDeploymentGroupInputRequestTypeDef(
     _RequiredUpdateDeploymentGroupInputRequestTypeDef,
     _OptionalUpdateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
+
 GetDeploymentConfigOutputTypeDef = TypedDict(
     "GetDeploymentConfigOutputTypeDef",
     {
         "deploymentConfigInfo": DeploymentConfigInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/waiter.py` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy/waiter.pyi` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy.egg-info/PKG-INFO` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codedeploy
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeDeploy 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeDeploy 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codedeploy type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codedeploy type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codedeploy)](https://pepy.tech/project/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
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
@@ -407,20 +407,20 @@
 )
 
 
 def check_value(value: ApplicationRevisionSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codedeploy.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
     AlarmTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
@@ -439,22 +439,21 @@
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
     MinimumHealthyHostsTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
-    TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
     LastDeploymentInfoTypeDef,
+    TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
     TargetGroupInfoTypeDef,
@@ -473,36 +472,38 @@
     PaginatorConfigTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
     ListApplicationsInputRequestTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
-    TimeRangeTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
     TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
     TimeBasedCanaryTypeDef,
     TimeBasedLinearTypeDef,
+    TimestampTypeDef,
+    TriggerConfigTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
     InstanceInfoTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationsOutputTypeDef,
     CreateApplicationOutputTypeDef,
     CreateDeploymentConfigOutputTypeDef,
     CreateDeploymentGroupOutputTypeDef,
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
@@ -533,24 +534,27 @@
     ListApplicationsInputListApplicationsPaginateTypeDef,
     ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
-    ListDeploymentsInputListDeploymentsPaginateTypeDef,
-    ListDeploymentsInputRequestTypeDef,
     RevisionLocationTypeDef,
     TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
     TrafficRoutingConfigTypeDef,
+    TimeRangeTypeDef,
+    TriggerConfigUnionTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
     GetOnPremisesInstanceOutputTypeDef,
+    AlarmConfigurationUnionTypeDef,
     TargetInstancesOutputTypeDef,
+    EC2TagSetUnionTypeDef,
     TargetInstancesTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
     BatchGetApplicationRevisionsInputRequestTypeDef,
     GetApplicationRevisionInputRequestTypeDef,
@@ -558,34 +562,38 @@
     ListApplicationRevisionsOutputTypeDef,
     RegisterApplicationRevisionInputRequestTypeDef,
     RevisionInfoTypeDef,
     LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
     CreateDeploymentConfigInputRequestTypeDef,
     DeploymentConfigInfoTypeDef,
+    ListDeploymentsInputListDeploymentsPaginateTypeDef,
+    ListDeploymentsInputRequestTypeDef,
     CreateDeploymentInputRequestTypeDef,
+    TargetInstancesUnionTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
     CreateDeploymentGroupInputRequestTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     UpdateDeploymentGroupInputRequestTypeDef,
     GetDeploymentConfigOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     GetDeploymentTargetOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     GetDeploymentOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/mypy_boto3_codedeploy.egg-info/SOURCES.txt` & `mypy-boto3-codedeploy-1.28.16/mypy_boto3_codedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.15.post1/setup.py` & `mypy-boto3-codedeploy-1.28.16/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codedeploy",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_codedeploy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeDeploy 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CodeDeploy 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 codedeploy type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 codedeploy type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codedeploy": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

