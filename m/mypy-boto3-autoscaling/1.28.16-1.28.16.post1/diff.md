# Comparing `tmp/mypy-boto3-autoscaling-1.28.16.tar.gz` & `tmp/mypy-boto3-autoscaling-1.28.16.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-1.28.16.post1.tar", last modified: Tue Aug  1 11:36:15 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-1.28.16.tar` & `mypy-boto3-autoscaling-1.28.16.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53486 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53403 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86691 2023-07-31 19:32:08.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86554 2023-07-31 19:32:07.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.300945 mypy-boto3-autoscaling-1.28.16.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24006 2023-08-01 11:36:15.296945 mypy-boto3-autoscaling-1.28.16.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22500 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.288945 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52911 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52828 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    87518 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87381 2023-08-01 11:11:23.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.296945 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24006 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:15.300945 mypy-boto3-autoscaling-1.28.16.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/setup.py
```

### Comparing `mypy-boto3-autoscaling-1.28.16/LICENSE` & `mypy-boto3-autoscaling-1.28.16.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16/PKG-INFO` & `mypy-boto3-autoscaling-1.28.16.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.16
-Summary: Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 autoscaling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 autoscaling type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
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
@@ -383,20 +383,20 @@
 )
 
 
 def check_value(value: AcceleratorManufacturerType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_autoscaling.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     ResponseMetadataTypeDef,
@@ -413,15 +413,14 @@
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
-    ScheduledUpdateGroupActionRequestTypeDef,
     EbsTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
@@ -443,27 +442,26 @@
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
     DescribePoliciesTypeRequestTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
-    DescribeScheduledActionsTypeRequestTypeDef,
+    TimestampTypeDef,
     DescribeTrafficSourcesRequestRequestTypeDef,
     TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
-    GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
@@ -476,15 +474,14 @@
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
-    PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
@@ -513,49 +510,54 @@
     AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
     DescribeTagsTypeDescribeTagsPaginateTypeDef,
     DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
     LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
-    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    DescribeScheduledActionsTypeRequestTypeDef,
+    GetPredictiveScalingForecastTypeRequestTypeDef,
+    PutScheduledUpdateGroupActionTypeRequestTypeDef,
+    ScheduledUpdateGroupActionRequestTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
     InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
     PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
+    RefreshPreferencesUnionTypeDef,
     AutoScalingInstancesTypeTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
     MetricStatOutputTypeDef,
     TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
+    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     RollbackDetailsTypeDef,
     LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
     MetricDataQueryOutputTypeDef,
     TargetTrackingMetricDataQueryOutputTypeDef,
@@ -577,30 +579,34 @@
     TargetTrackingConfigurationOutputTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
     TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
     DesiredConfigurationOutputTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
     PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
     AutoScalingGroupsTypeTypeDef,
     InstanceRefreshTypeDef,
+    DesiredConfigurationUnionTypeDef,
     StartInstanceRefreshTypeRequestTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     ScalingPolicyTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
     PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestTypeDef:
+def get_value() -> AcceleratorCountRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-1.28.16/README.md` & `mypy-boto3-autoscaling-1.28.16.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
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
@@ -351,20 +351,20 @@
 )
 
 
 def check_value(value: AcceleratorManufacturerType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_autoscaling.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     ResponseMetadataTypeDef,
@@ -381,15 +381,14 @@
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
-    ScheduledUpdateGroupActionRequestTypeDef,
     EbsTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
@@ -411,27 +410,26 @@
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
     DescribePoliciesTypeRequestTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
-    DescribeScheduledActionsTypeRequestTypeDef,
+    TimestampTypeDef,
     DescribeTrafficSourcesRequestRequestTypeDef,
     TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
-    GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
@@ -444,15 +442,14 @@
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
-    PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
@@ -481,49 +478,54 @@
     AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
     DescribeTagsTypeDescribeTagsPaginateTypeDef,
     DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
     LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
-    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    DescribeScheduledActionsTypeRequestTypeDef,
+    GetPredictiveScalingForecastTypeRequestTypeDef,
+    PutScheduledUpdateGroupActionTypeRequestTypeDef,
+    ScheduledUpdateGroupActionRequestTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
     InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
     PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
+    RefreshPreferencesUnionTypeDef,
     AutoScalingInstancesTypeTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
     MetricStatOutputTypeDef,
     TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
+    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     RollbackDetailsTypeDef,
     LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
     MetricDataQueryOutputTypeDef,
     TargetTrackingMetricDataQueryOutputTypeDef,
@@ -545,30 +547,34 @@
     TargetTrackingConfigurationOutputTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
     TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
     DesiredConfigurationOutputTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
     PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
     AutoScalingGroupsTypeTypeDef,
     InstanceRefreshTypeDef,
+    DesiredConfigurationUnionTypeDef,
     StartInstanceRefreshTypeRequestTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     ScalingPolicyTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
     PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestTypeDef:
+def get_value() -> AcceleratorCountRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__init__.py` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__init__.pyi` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__main__.py` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScaling 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.AutoScaling 1.28.16\nVersion:         1.28.16.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.16.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/client.py` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_autoscaling.client import AutoScalingClient
 
     session = Session()
     client: AutoScalingClient = session.client("autoscaling")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import WarmPoolStateType
 from .paginator import (
     DescribeAutoScalingGroupsPaginator,
     DescribeAutoScalingInstancesPaginator,
@@ -51,80 +50,72 @@
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
-    DesiredConfigurationOutputTypeDef,
-    DesiredConfigurationTypeDef,
+    DesiredConfigurationUnionTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     InstanceReusePolicyTypeDef,
     LaunchConfigurationsTypeTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
-    MixedInstancesPolicyOutputTypeDef,
-    MixedInstancesPolicyTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
-    PredictiveScalingConfigurationOutputTypeDef,
-    PredictiveScalingConfigurationTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
     ProcessesTypeTypeDef,
-    RefreshPreferencesOutputTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesUnionTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
-    TargetTrackingConfigurationOutputTypeDef,
-    TargetTrackingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
+    TimestampTypeDef,
     TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AutoScalingClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ActiveInstanceRefreshNotFoundFault: Type[BotocoreClientError]
     AlreadyExistsFault: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InstanceRefreshInProgressFault: Type[BotocoreClientError]
     InvalidNextToken: Type[BotocoreClientError]
     IrreversibleInstanceRefreshFault: Type[BotocoreClientError]
     LimitExceededFault: Type[BotocoreClientError]
     ResourceContentionFault: Type[BotocoreClientError]
     ResourceInUseFault: Type[BotocoreClientError]
     ScalingActivityInProgressFault: Type[BotocoreClientError]
     ServiceLinkedRoleFailure: Type[BotocoreClientError]
 
-
 class AutoScalingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/)
     """
 
     meta: ClientMeta
@@ -133,105 +124,95 @@
     def exceptions(self) -> Exceptions:
         """
         AutoScalingClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#exceptions)
         """
-
     def attach_instances(
         self, *, AutoScalingGroupName: str, InstanceIds: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches one or more EC2 instances to the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_instances)
         """
-
     def attach_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, TargetGroupARNs: Sequence[str]
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_load_balancer_target_groups)
         """
-
     def attach_load_balancers(
         self, *, AutoScalingGroupName: str, LoadBalancerNames: Sequence[str]
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_load_balancers)
         """
-
     def attach_traffic_sources(
         self, *, AutoScalingGroupName: str, TrafficSources: Sequence[TrafficSourceIdentifierTypeDef]
     ) -> Dict[str, Any]:
         """
         Attaches one or more traffic sources to the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_traffic_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_traffic_sources)
         """
-
     def batch_delete_scheduled_action(
         self, *, AutoScalingGroupName: str, ScheduledActionNames: Sequence[str]
     ) -> BatchDeleteScheduledActionAnswerTypeDef:
         """
         Deletes one or more scheduled actions for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.batch_delete_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#batch_delete_scheduled_action)
         """
-
     def batch_put_scheduled_update_group_action(
         self,
         *,
         AutoScalingGroupName: str,
         ScheduledUpdateGroupActions: Sequence[ScheduledUpdateGroupActionRequestTypeDef]
     ) -> BatchPutScheduledUpdateGroupActionAnswerTypeDef:
         """
         Creates or updates one or more scheduled scaling actions for an Auto Scaling
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.batch_put_scheduled_update_group_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#batch_put_scheduled_update_group_action)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#can_paginate)
         """
-
     def cancel_instance_refresh(
         self, *, AutoScalingGroupName: str
     ) -> CancelInstanceRefreshAnswerTypeDef:
         """
         Cancels an instance refresh or rollback that is in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.cancel_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#cancel_instance_refresh)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#close)
         """
-
     def complete_lifecycle_action(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleActionResult: str,
         LifecycleActionToken: str = ...,
@@ -240,26 +221,23 @@
         """
         Completes the lifecycle action for the specified token or instance with the
         specified result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.complete_lifecycle_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#complete_lifecycle_action)
         """
-
     def create_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         MinSize: int,
         MaxSize: int,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: Union[
-            MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
-        ] = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
         InstanceId: str = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         LoadBalancerNames: Sequence[str] = ...,
         TargetGroupARNs: Sequence[str] = ...,
         HealthCheckType: str = ...,
@@ -282,15 +260,14 @@
         **We strongly recommend using a launch template when calling this operation to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Creates
         an Auto Scaling group with the specified name and attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_auto_scaling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#create_auto_scaling_group)
         """
-
     def create_launch_configuration(
         self,
         *,
         LaunchConfigurationName: str,
         ImageId: str = ...,
         KeyName: str = ...,
         SecurityGroups: Sequence[str] = ...,
@@ -312,153 +289,138 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a launch configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#create_launch_configuration)
         """
-
     def create_or_update_tags(self, *, Tags: Sequence[TagTypeDef]) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates tags for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_or_update_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#create_or_update_tags)
         """
-
     def delete_auto_scaling_group(
         self, *, AutoScalingGroupName: str, ForceDelete: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_auto_scaling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_auto_scaling_group)
         """
-
     def delete_launch_configuration(
         self, *, LaunchConfigurationName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified launch configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_launch_configuration)
         """
-
     def delete_lifecycle_hook(
         self, *, LifecycleHookName: str, AutoScalingGroupName: str
     ) -> Dict[str, Any]:
         """
         Deletes the specified lifecycle hook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_lifecycle_hook)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_lifecycle_hook)
         """
-
     def delete_notification_configuration(
         self, *, AutoScalingGroupName: str, TopicARN: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_notification_configuration)
         """
-
     def delete_policy(
         self, *, PolicyName: str, AutoScalingGroupName: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified scaling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_policy)
         """
-
     def delete_scheduled_action(
         self, *, AutoScalingGroupName: str, ScheduledActionName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_scheduled_action)
         """
-
     def delete_tags(self, *, Tags: Sequence[TagTypeDef]) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_tags)
         """
-
     def delete_warm_pool(
         self, *, AutoScalingGroupName: str, ForceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the warm pool for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_warm_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_warm_pool)
         """
-
     def describe_account_limits(self) -> DescribeAccountLimitsAnswerTypeDef:
         """
         Describes the current Amazon EC2 Auto Scaling resource quotas for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_account_limits)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_account_limits)
         """
-
     def describe_adjustment_types(self) -> DescribeAdjustmentTypesAnswerTypeDef:
         """
         Describes the available adjustment types for step scaling and simple scaling
         policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_adjustment_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_adjustment_types)
         """
-
     def describe_auto_scaling_groups(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...,
         Filters: Sequence[FilterTypeDef] = ...
     ) -> AutoScalingGroupsTypeTypeDef:
         """
         Gets information about the Auto Scaling groups in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_auto_scaling_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_auto_scaling_groups)
         """
-
     def describe_auto_scaling_instances(
         self, *, InstanceIds: Sequence[str] = ..., MaxRecords: int = ..., NextToken: str = ...
     ) -> AutoScalingInstancesTypeTypeDef:
         """
         Gets information about the Auto Scaling instances in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_auto_scaling_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_auto_scaling_instances)
         """
-
     def describe_auto_scaling_notification_types(
         self,
     ) -> DescribeAutoScalingNotificationTypesAnswerTypeDef:
         """
         Describes the notification types that are supported by Amazon EC2 Auto Scaling.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_auto_scaling_notification_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_auto_scaling_notification_types)
         """
-
     def describe_instance_refreshes(
         self,
         *,
         AutoScalingGroupName: str,
         InstanceRefreshIds: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
@@ -466,90 +428,82 @@
         """
         Gets information about the instance refreshes for the specified Auto Scaling
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_instance_refreshes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_instance_refreshes)
         """
-
     def describe_launch_configurations(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> LaunchConfigurationsTypeTypeDef:
         """
         Gets information about the launch configurations in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_launch_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_launch_configurations)
         """
-
     def describe_lifecycle_hook_types(self) -> DescribeLifecycleHookTypesAnswerTypeDef:
         """
         Describes the available types of lifecycle hooks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_lifecycle_hook_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_lifecycle_hook_types)
         """
-
     def describe_lifecycle_hooks(
         self, *, AutoScalingGroupName: str, LifecycleHookNames: Sequence[str] = ...
     ) -> DescribeLifecycleHooksAnswerTypeDef:
         """
         Gets information about the lifecycle hooks for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_lifecycle_hooks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_lifecycle_hooks)
         """
-
     def describe_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, NextToken: str = ..., MaxRecords: int = ...
     ) -> DescribeLoadBalancerTargetGroupsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_load_balancer_target_groups)
         """
-
     def describe_load_balancers(
         self, *, AutoScalingGroupName: str, NextToken: str = ..., MaxRecords: int = ...
     ) -> DescribeLoadBalancersResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_load_balancers)
         """
-
     def describe_metric_collection_types(self) -> DescribeMetricCollectionTypesAnswerTypeDef:
         """
         Describes the available CloudWatch metrics for Amazon EC2 Auto Scaling.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_metric_collection_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_metric_collection_types)
         """
-
     def describe_notification_configurations(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> DescribeNotificationConfigurationsAnswerTypeDef:
         """
         Gets information about the Amazon SNS notifications that are configured for one
         or more Auto Scaling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_notification_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_notification_configurations)
         """
-
     def describe_policies(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
         NextToken: str = ...,
@@ -557,15 +511,14 @@
     ) -> PoliciesTypeTypeDef:
         """
         Gets information about the scaling policies in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_policies)
         """
-
     def describe_scaling_activities(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
         MaxRecords: int = ...,
@@ -573,163 +526,149 @@
     ) -> ActivitiesTypeTypeDef:
         """
         Gets information about the scaling activities in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scaling_activities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_scaling_activities)
         """
-
     def describe_scaling_process_types(self) -> ProcessesTypeTypeDef:
         """
         Describes the scaling process types for use with the  ResumeProcesses and
         SuspendProcesses APIs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scaling_process_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_scaling_process_types)
         """
-
     def describe_scheduled_actions(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> ScheduledActionsTypeTypeDef:
         """
         Gets information about the scheduled actions that haven't run or that have not
         reached their end time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scheduled_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_scheduled_actions)
         """
-
     def describe_tags(
         self, *, Filters: Sequence[FilterTypeDef] = ..., NextToken: str = ..., MaxRecords: int = ...
     ) -> TagsTypeTypeDef:
         """
         Describes the specified tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_tags)
         """
-
     def describe_termination_policy_types(self) -> DescribeTerminationPolicyTypesAnswerTypeDef:
         """
         Describes the termination policies supported by Amazon EC2 Auto Scaling.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_termination_policy_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_termination_policy_types)
         """
-
     def describe_traffic_sources(
         self,
         *,
         AutoScalingGroupName: str,
         TrafficSourceType: str = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> DescribeTrafficSourcesResponseTypeDef:
         """
         Gets information about the traffic sources for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_traffic_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_traffic_sources)
         """
-
     def describe_warm_pool(
         self, *, AutoScalingGroupName: str, MaxRecords: int = ..., NextToken: str = ...
     ) -> DescribeWarmPoolAnswerTypeDef:
         """
         Gets information about a warm pool and its instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_warm_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_warm_pool)
         """
-
     def detach_instances(
         self,
         *,
         AutoScalingGroupName: str,
         ShouldDecrementDesiredCapacity: bool,
         InstanceIds: Sequence[str] = ...
     ) -> DetachInstancesAnswerTypeDef:
         """
         Removes one or more instances from the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_instances)
         """
-
     def detach_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, TargetGroupARNs: Sequence[str]
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_load_balancer_target_groups)
         """
-
     def detach_load_balancers(
         self, *, AutoScalingGroupName: str, LoadBalancerNames: Sequence[str]
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_load_balancers)
         """
-
     def detach_traffic_sources(
         self, *, AutoScalingGroupName: str, TrafficSources: Sequence[TrafficSourceIdentifierTypeDef]
     ) -> Dict[str, Any]:
         """
         Detaches one or more traffic sources from the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_traffic_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_traffic_sources)
         """
-
     def disable_metrics_collection(
         self, *, AutoScalingGroupName: str, Metrics: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disables group metrics collection for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.disable_metrics_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#disable_metrics_collection)
         """
-
     def enable_metrics_collection(
         self, *, AutoScalingGroupName: str, Granularity: str, Metrics: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables group metrics collection for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.enable_metrics_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#enable_metrics_collection)
         """
-
     def enter_standby(
         self,
         *,
         AutoScalingGroupName: str,
         ShouldDecrementDesiredCapacity: bool,
         InstanceIds: Sequence[str] = ...
     ) -> EnterStandbyAnswerTypeDef:
         """
         Moves the specified instances into the standby state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.enter_standby)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#enter_standby)
         """
-
     def execute_policy(
         self,
         *,
         PolicyName: str,
         AutoScalingGroupName: str = ...,
         HonorCooldown: bool = ...,
         MetricValue: float = ...,
@@ -737,54 +676,50 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Executes the specified policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.execute_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#execute_policy)
         """
-
     def exit_standby(
         self, *, AutoScalingGroupName: str, InstanceIds: Sequence[str] = ...
     ) -> ExitStandbyAnswerTypeDef:
         """
         Moves the specified instances out of the standby state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.exit_standby)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#exit_standby)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#generate_presigned_url)
         """
-
     def get_predictive_scaling_forecast(
         self,
         *,
         AutoScalingGroupName: str,
         PolicyName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str]
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef
     ) -> GetPredictiveScalingForecastAnswerTypeDef:
         """
         Retrieves the forecast data for a predictive scaling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_predictive_scaling_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_predictive_scaling_forecast)
         """
-
     def put_lifecycle_hook(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleTransition: str = ...,
         RoleARN: str = ...,
@@ -795,76 +730,68 @@
     ) -> Dict[str, Any]:
         """
         Creates or updates a lifecycle hook for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_lifecycle_hook)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_lifecycle_hook)
         """
-
     def put_notification_configuration(
         self, *, AutoScalingGroupName: str, TopicARN: str, NotificationTypes: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Configures an Auto Scaling group to send notifications when specified events
         take place.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_notification_configuration)
         """
-
     def put_scaling_policy(
         self,
         *,
         AutoScalingGroupName: str,
         PolicyName: str,
         PolicyType: str = ...,
         AdjustmentType: str = ...,
         MinAdjustmentStep: int = ...,
         MinAdjustmentMagnitude: int = ...,
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
-        TargetTrackingConfiguration: Union[
-            TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
-        ] = ...,
+        TargetTrackingConfiguration: TargetTrackingConfigurationUnionTypeDef = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: Union[
-            PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
-        ] = ...
+        PredictiveScalingConfiguration: PredictiveScalingConfigurationUnionTypeDef = ...
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_scaling_policy)
         """
-
     def put_scheduled_update_group_action(
         self,
         *,
         AutoScalingGroupName: str,
         ScheduledActionName: str,
-        Time: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        Time: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Recurrence: str = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         TimeZone: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a scheduled scaling action for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scheduled_update_group_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_scheduled_update_group_action)
         """
-
     def put_warm_pool(
         self,
         *,
         AutoScalingGroupName: str,
         MaxGroupPreparedCapacity: int = ...,
         MinSize: int = ...,
         PoolState: WarmPoolStateType = ...,
@@ -872,15 +799,14 @@
     ) -> Dict[str, Any]:
         """
         Creates or updates a warm pool for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_warm_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_warm_pool)
         """
-
     def record_lifecycle_action_heartbeat(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleActionToken: str = ...,
         InstanceId: str = ...
@@ -888,114 +814,101 @@
         """
         Records a heartbeat for the lifecycle action associated with the specified token
         or instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.record_lifecycle_action_heartbeat)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#record_lifecycle_action_heartbeat)
         """
-
     def resume_processes(
         self, *, AutoScalingGroupName: str, ScalingProcesses: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Resumes the specified suspended auto scaling processes, or all suspended
         process, for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.resume_processes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#resume_processes)
         """
-
     def rollback_instance_refresh(
         self, *, AutoScalingGroupName: str
     ) -> RollbackInstanceRefreshAnswerTypeDef:
         """
         Cancels an instance refresh that is in progress and rolls back any changes that
         it made.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.rollback_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#rollback_instance_refresh)
         """
-
     def set_desired_capacity(
         self, *, AutoScalingGroupName: str, DesiredCapacity: int, HonorCooldown: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the size of the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.set_desired_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#set_desired_capacity)
         """
-
     def set_instance_health(
         self, *, InstanceId: str, HealthStatus: str, ShouldRespectGracePeriod: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the health status of the specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.set_instance_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#set_instance_health)
         """
-
     def set_instance_protection(
         self, *, InstanceIds: Sequence[str], AutoScalingGroupName: str, ProtectedFromScaleIn: bool
     ) -> Dict[str, Any]:
         """
         Updates the instance protection settings of the specified instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.set_instance_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#set_instance_protection)
         """
-
     def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
-        DesiredConfiguration: Union[
-            DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
-        ] = ...,
-        Preferences: Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef] = ...
+        DesiredConfiguration: DesiredConfigurationUnionTypeDef = ...,
+        Preferences: RefreshPreferencesUnionTypeDef = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#start_instance_refresh)
         """
-
     def suspend_processes(
         self, *, AutoScalingGroupName: str, ScalingProcesses: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Suspends the specified auto scaling processes, or all processes, for the
         specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.suspend_processes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#suspend_processes)
         """
-
     def terminate_instance_in_auto_scaling_group(
         self, *, InstanceId: str, ShouldDecrementDesiredCapacity: bool
     ) -> ActivityTypeTypeDef:
         """
         Terminates the specified instance and optionally adjusts the desired group size.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.terminate_instance_in_auto_scaling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#terminate_instance_in_auto_scaling_group)
         """
-
     def update_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: Union[
-            MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
-        ] = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         HealthCheckType: str = ...,
         HealthCheckGracePeriod: int = ...,
@@ -1014,103 +927,92 @@
         **We strongly recommend that all Auto Scaling groups use launch templates to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Updates
         the configuration for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.update_auto_scaling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#update_auto_scaling_group)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_auto_scaling_groups"]
     ) -> DescribeAutoScalingGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_auto_scaling_instances"]
     ) -> DescribeAutoScalingInstancesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_launch_configurations"]
     ) -> DescribeLaunchConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_load_balancer_target_groups"]
     ) -> DescribeLoadBalancerTargetGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_load_balancers"]
     ) -> DescribeLoadBalancersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_notification_configurations"]
     ) -> DescribeNotificationConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_policies"]
     ) -> DescribePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_activities"]
     ) -> DescribeScalingActivitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scheduled_actions"]
     ) -> DescribeScheduledActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["describe_tags"]) -> DescribeTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_warm_pool"]
     ) -> DescribeWarmPoolPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
```

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/client.pyi` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_autoscaling.client import AutoScalingClient
 
     session = Session()
     client: AutoScalingClient = session.client("autoscaling")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import WarmPoolStateType
 from .paginator import (
     DescribeAutoScalingGroupsPaginator,
     DescribeAutoScalingInstancesPaginator,
@@ -51,76 +50,76 @@
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
-    DesiredConfigurationOutputTypeDef,
-    DesiredConfigurationTypeDef,
+    DesiredConfigurationUnionTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     InstanceReusePolicyTypeDef,
     LaunchConfigurationsTypeTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
-    MixedInstancesPolicyOutputTypeDef,
-    MixedInstancesPolicyTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
-    PredictiveScalingConfigurationOutputTypeDef,
-    PredictiveScalingConfigurationTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
     ProcessesTypeTypeDef,
-    RefreshPreferencesOutputTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesUnionTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
-    TargetTrackingConfigurationOutputTypeDef,
-    TargetTrackingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
+    TimestampTypeDef,
     TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("AutoScalingClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ActiveInstanceRefreshNotFoundFault: Type[BotocoreClientError]
     AlreadyExistsFault: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InstanceRefreshInProgressFault: Type[BotocoreClientError]
     InvalidNextToken: Type[BotocoreClientError]
     IrreversibleInstanceRefreshFault: Type[BotocoreClientError]
     LimitExceededFault: Type[BotocoreClientError]
     ResourceContentionFault: Type[BotocoreClientError]
     ResourceInUseFault: Type[BotocoreClientError]
     ScalingActivityInProgressFault: Type[BotocoreClientError]
     ServiceLinkedRoleFailure: Type[BotocoreClientError]
 
+
 class AutoScalingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/)
     """
 
     meta: ClientMeta
@@ -129,95 +128,105 @@
     def exceptions(self) -> Exceptions:
         """
         AutoScalingClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#exceptions)
         """
+
     def attach_instances(
         self, *, AutoScalingGroupName: str, InstanceIds: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches one or more EC2 instances to the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_instances)
         """
+
     def attach_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, TargetGroupARNs: Sequence[str]
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_load_balancer_target_groups)
         """
+
     def attach_load_balancers(
         self, *, AutoScalingGroupName: str, LoadBalancerNames: Sequence[str]
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_load_balancers)
         """
+
     def attach_traffic_sources(
         self, *, AutoScalingGroupName: str, TrafficSources: Sequence[TrafficSourceIdentifierTypeDef]
     ) -> Dict[str, Any]:
         """
         Attaches one or more traffic sources to the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_traffic_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_traffic_sources)
         """
+
     def batch_delete_scheduled_action(
         self, *, AutoScalingGroupName: str, ScheduledActionNames: Sequence[str]
     ) -> BatchDeleteScheduledActionAnswerTypeDef:
         """
         Deletes one or more scheduled actions for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.batch_delete_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#batch_delete_scheduled_action)
         """
+
     def batch_put_scheduled_update_group_action(
         self,
         *,
         AutoScalingGroupName: str,
         ScheduledUpdateGroupActions: Sequence[ScheduledUpdateGroupActionRequestTypeDef]
     ) -> BatchPutScheduledUpdateGroupActionAnswerTypeDef:
         """
         Creates or updates one or more scheduled scaling actions for an Auto Scaling
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.batch_put_scheduled_update_group_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#batch_put_scheduled_update_group_action)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#can_paginate)
         """
+
     def cancel_instance_refresh(
         self, *, AutoScalingGroupName: str
     ) -> CancelInstanceRefreshAnswerTypeDef:
         """
         Cancels an instance refresh or rollback that is in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.cancel_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#cancel_instance_refresh)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#close)
         """
+
     def complete_lifecycle_action(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleActionResult: str,
         LifecycleActionToken: str = ...,
@@ -226,25 +235,24 @@
         """
         Completes the lifecycle action for the specified token or instance with the
         specified result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.complete_lifecycle_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#complete_lifecycle_action)
         """
+
     def create_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         MinSize: int,
         MaxSize: int,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: Union[
-            MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
-        ] = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
         InstanceId: str = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         LoadBalancerNames: Sequence[str] = ...,
         TargetGroupARNs: Sequence[str] = ...,
         HealthCheckType: str = ...,
@@ -267,14 +275,15 @@
         **We strongly recommend using a launch template when calling this operation to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Creates
         an Auto Scaling group with the specified name and attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_auto_scaling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#create_auto_scaling_group)
         """
+
     def create_launch_configuration(
         self,
         *,
         LaunchConfigurationName: str,
         ImageId: str = ...,
         KeyName: str = ...,
         SecurityGroups: Sequence[str] = ...,
@@ -296,138 +305,153 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a launch configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#create_launch_configuration)
         """
+
     def create_or_update_tags(self, *, Tags: Sequence[TagTypeDef]) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates tags for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_or_update_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#create_or_update_tags)
         """
+
     def delete_auto_scaling_group(
         self, *, AutoScalingGroupName: str, ForceDelete: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_auto_scaling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_auto_scaling_group)
         """
+
     def delete_launch_configuration(
         self, *, LaunchConfigurationName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified launch configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_launch_configuration)
         """
+
     def delete_lifecycle_hook(
         self, *, LifecycleHookName: str, AutoScalingGroupName: str
     ) -> Dict[str, Any]:
         """
         Deletes the specified lifecycle hook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_lifecycle_hook)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_lifecycle_hook)
         """
+
     def delete_notification_configuration(
         self, *, AutoScalingGroupName: str, TopicARN: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_notification_configuration)
         """
+
     def delete_policy(
         self, *, PolicyName: str, AutoScalingGroupName: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified scaling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_policy)
         """
+
     def delete_scheduled_action(
         self, *, AutoScalingGroupName: str, ScheduledActionName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_scheduled_action)
         """
+
     def delete_tags(self, *, Tags: Sequence[TagTypeDef]) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_tags)
         """
+
     def delete_warm_pool(
         self, *, AutoScalingGroupName: str, ForceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the warm pool for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.delete_warm_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#delete_warm_pool)
         """
+
     def describe_account_limits(self) -> DescribeAccountLimitsAnswerTypeDef:
         """
         Describes the current Amazon EC2 Auto Scaling resource quotas for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_account_limits)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_account_limits)
         """
+
     def describe_adjustment_types(self) -> DescribeAdjustmentTypesAnswerTypeDef:
         """
         Describes the available adjustment types for step scaling and simple scaling
         policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_adjustment_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_adjustment_types)
         """
+
     def describe_auto_scaling_groups(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...,
         Filters: Sequence[FilterTypeDef] = ...
     ) -> AutoScalingGroupsTypeTypeDef:
         """
         Gets information about the Auto Scaling groups in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_auto_scaling_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_auto_scaling_groups)
         """
+
     def describe_auto_scaling_instances(
         self, *, InstanceIds: Sequence[str] = ..., MaxRecords: int = ..., NextToken: str = ...
     ) -> AutoScalingInstancesTypeTypeDef:
         """
         Gets information about the Auto Scaling instances in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_auto_scaling_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_auto_scaling_instances)
         """
+
     def describe_auto_scaling_notification_types(
         self,
     ) -> DescribeAutoScalingNotificationTypesAnswerTypeDef:
         """
         Describes the notification types that are supported by Amazon EC2 Auto Scaling.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_auto_scaling_notification_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_auto_scaling_notification_types)
         """
+
     def describe_instance_refreshes(
         self,
         *,
         AutoScalingGroupName: str,
         InstanceRefreshIds: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
@@ -435,82 +459,90 @@
         """
         Gets information about the instance refreshes for the specified Auto Scaling
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_instance_refreshes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_instance_refreshes)
         """
+
     def describe_launch_configurations(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> LaunchConfigurationsTypeTypeDef:
         """
         Gets information about the launch configurations in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_launch_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_launch_configurations)
         """
+
     def describe_lifecycle_hook_types(self) -> DescribeLifecycleHookTypesAnswerTypeDef:
         """
         Describes the available types of lifecycle hooks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_lifecycle_hook_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_lifecycle_hook_types)
         """
+
     def describe_lifecycle_hooks(
         self, *, AutoScalingGroupName: str, LifecycleHookNames: Sequence[str] = ...
     ) -> DescribeLifecycleHooksAnswerTypeDef:
         """
         Gets information about the lifecycle hooks for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_lifecycle_hooks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_lifecycle_hooks)
         """
+
     def describe_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, NextToken: str = ..., MaxRecords: int = ...
     ) -> DescribeLoadBalancerTargetGroupsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_load_balancer_target_groups)
         """
+
     def describe_load_balancers(
         self, *, AutoScalingGroupName: str, NextToken: str = ..., MaxRecords: int = ...
     ) -> DescribeLoadBalancersResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_load_balancers)
         """
+
     def describe_metric_collection_types(self) -> DescribeMetricCollectionTypesAnswerTypeDef:
         """
         Describes the available CloudWatch metrics for Amazon EC2 Auto Scaling.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_metric_collection_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_metric_collection_types)
         """
+
     def describe_notification_configurations(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> DescribeNotificationConfigurationsAnswerTypeDef:
         """
         Gets information about the Amazon SNS notifications that are configured for one
         or more Auto Scaling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_notification_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_notification_configurations)
         """
+
     def describe_policies(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
         NextToken: str = ...,
@@ -518,14 +550,15 @@
     ) -> PoliciesTypeTypeDef:
         """
         Gets information about the scaling policies in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_policies)
         """
+
     def describe_scaling_activities(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
         MaxRecords: int = ...,
@@ -533,149 +566,163 @@
     ) -> ActivitiesTypeTypeDef:
         """
         Gets information about the scaling activities in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scaling_activities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_scaling_activities)
         """
+
     def describe_scaling_process_types(self) -> ProcessesTypeTypeDef:
         """
         Describes the scaling process types for use with the  ResumeProcesses and
         SuspendProcesses APIs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scaling_process_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_scaling_process_types)
         """
+
     def describe_scheduled_actions(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> ScheduledActionsTypeTypeDef:
         """
         Gets information about the scheduled actions that haven't run or that have not
         reached their end time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scheduled_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_scheduled_actions)
         """
+
     def describe_tags(
         self, *, Filters: Sequence[FilterTypeDef] = ..., NextToken: str = ..., MaxRecords: int = ...
     ) -> TagsTypeTypeDef:
         """
         Describes the specified tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_tags)
         """
+
     def describe_termination_policy_types(self) -> DescribeTerminationPolicyTypesAnswerTypeDef:
         """
         Describes the termination policies supported by Amazon EC2 Auto Scaling.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_termination_policy_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_termination_policy_types)
         """
+
     def describe_traffic_sources(
         self,
         *,
         AutoScalingGroupName: str,
         TrafficSourceType: str = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> DescribeTrafficSourcesResponseTypeDef:
         """
         Gets information about the traffic sources for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_traffic_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_traffic_sources)
         """
+
     def describe_warm_pool(
         self, *, AutoScalingGroupName: str, MaxRecords: int = ..., NextToken: str = ...
     ) -> DescribeWarmPoolAnswerTypeDef:
         """
         Gets information about a warm pool and its instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_warm_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_warm_pool)
         """
+
     def detach_instances(
         self,
         *,
         AutoScalingGroupName: str,
         ShouldDecrementDesiredCapacity: bool,
         InstanceIds: Sequence[str] = ...
     ) -> DetachInstancesAnswerTypeDef:
         """
         Removes one or more instances from the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_instances)
         """
+
     def detach_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, TargetGroupARNs: Sequence[str]
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_load_balancer_target_groups)
         """
+
     def detach_load_balancers(
         self, *, AutoScalingGroupName: str, LoadBalancerNames: Sequence[str]
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_load_balancers)
         """
+
     def detach_traffic_sources(
         self, *, AutoScalingGroupName: str, TrafficSources: Sequence[TrafficSourceIdentifierTypeDef]
     ) -> Dict[str, Any]:
         """
         Detaches one or more traffic sources from the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_traffic_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_traffic_sources)
         """
+
     def disable_metrics_collection(
         self, *, AutoScalingGroupName: str, Metrics: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disables group metrics collection for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.disable_metrics_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#disable_metrics_collection)
         """
+
     def enable_metrics_collection(
         self, *, AutoScalingGroupName: str, Granularity: str, Metrics: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables group metrics collection for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.enable_metrics_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#enable_metrics_collection)
         """
+
     def enter_standby(
         self,
         *,
         AutoScalingGroupName: str,
         ShouldDecrementDesiredCapacity: bool,
         InstanceIds: Sequence[str] = ...
     ) -> EnterStandbyAnswerTypeDef:
         """
         Moves the specified instances into the standby state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.enter_standby)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#enter_standby)
         """
+
     def execute_policy(
         self,
         *,
         PolicyName: str,
         AutoScalingGroupName: str = ...,
         HonorCooldown: bool = ...,
         MetricValue: float = ...,
@@ -683,50 +730,54 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Executes the specified policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.execute_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#execute_policy)
         """
+
     def exit_standby(
         self, *, AutoScalingGroupName: str, InstanceIds: Sequence[str] = ...
     ) -> ExitStandbyAnswerTypeDef:
         """
         Moves the specified instances out of the standby state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.exit_standby)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#exit_standby)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#generate_presigned_url)
         """
+
     def get_predictive_scaling_forecast(
         self,
         *,
         AutoScalingGroupName: str,
         PolicyName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str]
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef
     ) -> GetPredictiveScalingForecastAnswerTypeDef:
         """
         Retrieves the forecast data for a predictive scaling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_predictive_scaling_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_predictive_scaling_forecast)
         """
+
     def put_lifecycle_hook(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleTransition: str = ...,
         RoleARN: str = ...,
@@ -737,72 +788,72 @@
     ) -> Dict[str, Any]:
         """
         Creates or updates a lifecycle hook for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_lifecycle_hook)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_lifecycle_hook)
         """
+
     def put_notification_configuration(
         self, *, AutoScalingGroupName: str, TopicARN: str, NotificationTypes: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Configures an Auto Scaling group to send notifications when specified events
         take place.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_notification_configuration)
         """
+
     def put_scaling_policy(
         self,
         *,
         AutoScalingGroupName: str,
         PolicyName: str,
         PolicyType: str = ...,
         AdjustmentType: str = ...,
         MinAdjustmentStep: int = ...,
         MinAdjustmentMagnitude: int = ...,
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
-        TargetTrackingConfiguration: Union[
-            TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
-        ] = ...,
+        TargetTrackingConfiguration: TargetTrackingConfigurationUnionTypeDef = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: Union[
-            PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
-        ] = ...
+        PredictiveScalingConfiguration: PredictiveScalingConfigurationUnionTypeDef = ...
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_scaling_policy)
         """
+
     def put_scheduled_update_group_action(
         self,
         *,
         AutoScalingGroupName: str,
         ScheduledActionName: str,
-        Time: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        Time: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Recurrence: str = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         TimeZone: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a scheduled scaling action for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scheduled_update_group_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_scheduled_update_group_action)
         """
+
     def put_warm_pool(
         self,
         *,
         AutoScalingGroupName: str,
         MaxGroupPreparedCapacity: int = ...,
         MinSize: int = ...,
         PoolState: WarmPoolStateType = ...,
@@ -810,14 +861,15 @@
     ) -> Dict[str, Any]:
         """
         Creates or updates a warm pool for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_warm_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_warm_pool)
         """
+
     def record_lifecycle_action_heartbeat(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleActionToken: str = ...,
         InstanceId: str = ...
@@ -825,105 +877,110 @@
         """
         Records a heartbeat for the lifecycle action associated with the specified token
         or instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.record_lifecycle_action_heartbeat)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#record_lifecycle_action_heartbeat)
         """
+
     def resume_processes(
         self, *, AutoScalingGroupName: str, ScalingProcesses: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Resumes the specified suspended auto scaling processes, or all suspended
         process, for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.resume_processes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#resume_processes)
         """
+
     def rollback_instance_refresh(
         self, *, AutoScalingGroupName: str
     ) -> RollbackInstanceRefreshAnswerTypeDef:
         """
         Cancels an instance refresh that is in progress and rolls back any changes that
         it made.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.rollback_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#rollback_instance_refresh)
         """
+
     def set_desired_capacity(
         self, *, AutoScalingGroupName: str, DesiredCapacity: int, HonorCooldown: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the size of the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.set_desired_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#set_desired_capacity)
         """
+
     def set_instance_health(
         self, *, InstanceId: str, HealthStatus: str, ShouldRespectGracePeriod: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the health status of the specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.set_instance_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#set_instance_health)
         """
+
     def set_instance_protection(
         self, *, InstanceIds: Sequence[str], AutoScalingGroupName: str, ProtectedFromScaleIn: bool
     ) -> Dict[str, Any]:
         """
         Updates the instance protection settings of the specified instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.set_instance_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#set_instance_protection)
         """
+
     def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
-        DesiredConfiguration: Union[
-            DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
-        ] = ...,
-        Preferences: Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef] = ...
+        DesiredConfiguration: DesiredConfigurationUnionTypeDef = ...,
+        Preferences: RefreshPreferencesUnionTypeDef = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#start_instance_refresh)
         """
+
     def suspend_processes(
         self, *, AutoScalingGroupName: str, ScalingProcesses: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Suspends the specified auto scaling processes, or all processes, for the
         specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.suspend_processes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#suspend_processes)
         """
+
     def terminate_instance_in_auto_scaling_group(
         self, *, InstanceId: str, ShouldDecrementDesiredCapacity: bool
     ) -> ActivityTypeTypeDef:
         """
         Terminates the specified instance and optionally adjusts the desired group size.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.terminate_instance_in_auto_scaling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#terminate_instance_in_auto_scaling_group)
         """
+
     def update_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: Union[
-            MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
-        ] = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         HealthCheckType: str = ...,
         HealthCheckGracePeriod: int = ...,
@@ -942,92 +999,103 @@
         **We strongly recommend that all Auto Scaling groups use launch templates to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Updates
         the configuration for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.update_auto_scaling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#update_auto_scaling_group)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_auto_scaling_groups"]
     ) -> DescribeAutoScalingGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_auto_scaling_instances"]
     ) -> DescribeAutoScalingInstancesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_launch_configurations"]
     ) -> DescribeLaunchConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_load_balancer_target_groups"]
     ) -> DescribeLoadBalancerTargetGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_load_balancers"]
     ) -> DescribeLoadBalancersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_notification_configurations"]
     ) -> DescribeNotificationConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_policies"]
     ) -> DescribePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_activities"]
     ) -> DescribeScalingActivitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scheduled_actions"]
     ) -> DescribeScheduledActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["describe_tags"]) -> DescribeTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_warm_pool"]
     ) -> DescribeWarmPoolPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
```

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/literals.py` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/literals.pyi` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/paginator.py` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
     describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
     describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ActivitiesTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
@@ -54,14 +53,15 @@
     DescribeWarmPoolAnswerTypeDef,
     FilterTypeDef,
     LaunchConfigurationsTypeTypeDef,
     PaginatorConfigTypeDef,
     PoliciesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     TagsTypeTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeAutoScalingGroupsPaginator",
     "DescribeAutoScalingInstancesPaginator",
     "DescribeLaunchConfigurationsPaginator",
     "DescribeLoadBalancerTargetGroupsPaginator",
@@ -232,16 +232,16 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/paginator.pyi` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,15 @@
     describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
     describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ActivitiesTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
@@ -54,14 +53,15 @@
     DescribeWarmPoolAnswerTypeDef,
     FilterTypeDef,
     LaunchConfigurationsTypeTypeDef,
     PaginatorConfigTypeDef,
     PoliciesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     TagsTypeTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeAutoScalingGroupsPaginator",
     "DescribeAutoScalingInstancesPaginator",
     "DescribeLaunchConfigurationsPaginator",
     "DescribeLoadBalancerTargetGroupsPaginator",
@@ -221,16 +221,16 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/type_defs.py` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestTypeDef
 
-    data: AcceleratorCountRequestTypeDef = {...}
+    data: AcceleratorCountRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -47,15 +47,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmSpecificationOutputTypeDef",
@@ -70,15 +69,14 @@
     "EnabledMetricTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
-    "ScheduledUpdateGroupActionRequestTypeDef",
     "EbsTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
@@ -100,27 +98,26 @@
     "LoadBalancerStateTypeDef",
     "MetricCollectionTypeTypeDef",
     "MetricGranularityTypeTypeDef",
     "NotificationConfigurationTypeDef",
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
     "DescribePoliciesTypeRequestTypeDef",
     "DescribeScalingActivitiesTypeRequestTypeDef",
-    "DescribeScheduledActionsTypeRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeTrafficSourcesRequestRequestTypeDef",
     "TrafficSourceStateTypeDef",
     "DescribeWarmPoolTypeRequestTypeDef",
     "DetachInstancesQueryRequestTypeDef",
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
-    "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
@@ -133,15 +130,14 @@
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
-    "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
@@ -170,49 +166,54 @@
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     "DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
-    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
     "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    "DescribeScheduledActionsTypeRequestTypeDef",
+    "GetPredictiveScalingForecastTypeRequestTypeDef",
+    "PutScheduledUpdateGroupActionTypeRequestTypeDef",
+    "ScheduledUpdateGroupActionRequestTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
     "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
     "ScheduledActionsTypeTypeDef",
+    "RefreshPreferencesUnionTypeDef",
     "AutoScalingInstancesTypeTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
     "MetricStatOutputTypeDef",
     "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
+    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RollbackDetailsTypeDef",
     "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
     "MetricDataQueryOutputTypeDef",
     "TargetTrackingMetricDataQueryOutputTypeDef",
@@ -234,23 +235,27 @@
     "TargetTrackingConfigurationOutputTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
     "DesiredConfigurationOutputTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
+    "MixedInstancesPolicyUnionTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
     "PredictiveScalingConfigurationOutputTypeDef",
     "PredictiveScalingConfigurationTypeDef",
+    "TargetTrackingConfigurationUnionTypeDef",
     "AutoScalingGroupsTypeTypeDef",
     "InstanceRefreshTypeDef",
+    "DesiredConfigurationUnionTypeDef",
     "StartInstanceRefreshTypeRequestTypeDef",
     "GetPredictiveScalingForecastAnswerTypeDef",
     "ScalingPolicyTypeDef",
+    "PredictiveScalingConfigurationUnionTypeDef",
     "PutScalingPolicyTypeRequestTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
@@ -290,19 +295,17 @@
         "Details": str,
         "AutoScalingGroupState": str,
         "AutoScalingGroupARN": str,
     },
     total=False,
 )
 
-
 class ActivityTypeDef(_RequiredActivityTypeDef, _OptionalActivityTypeDef):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -353,21 +356,19 @@
     "_OptionalAttachInstancesQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class AttachInstancesQueryRequestTypeDef(
     _RequiredAttachInstancesQueryRequestTypeDef, _OptionalAttachInstancesQueryRequestTypeDef
 ):
     pass
 
-
 AttachLoadBalancerTargetGroupsTypeRequestTypeDef = TypedDict(
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TargetGroupARNs": Sequence[str],
     },
 )
@@ -390,21 +391,19 @@
     "_OptionalTrafficSourceIdentifierTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-
 class TrafficSourceIdentifierTypeDef(
     _RequiredTrafficSourceIdentifierTypeDef, _OptionalTrafficSourceIdentifierTypeDef
 ):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -480,58 +479,28 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-
 class FailedScheduledUpdateGroupActionRequestTypeDef(
     _RequiredFailedScheduledUpdateGroupActionRequestTypeDef,
     _OptionalFailedScheduledUpdateGroupActionRequestTypeDef,
 ):
     pass
 
-
 BatchDeleteScheduledActionTypeRequestTypeDef = TypedDict(
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionNames": Sequence[str],
     },
 )
 
-_RequiredScheduledUpdateGroupActionRequestTypeDef = TypedDict(
-    "_RequiredScheduledUpdateGroupActionRequestTypeDef",
-    {
-        "ScheduledActionName": str,
-    },
-)
-_OptionalScheduledUpdateGroupActionRequestTypeDef = TypedDict(
-    "_OptionalScheduledUpdateGroupActionRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Recurrence": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "DesiredCapacity": int,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-
-class ScheduledUpdateGroupActionRequestTypeDef(
-    _RequiredScheduledUpdateGroupActionRequestTypeDef,
-    _OptionalScheduledUpdateGroupActionRequestTypeDef,
-):
-    pass
-
-
 EbsTypeDef = TypedDict(
     "EbsTypeDef",
     {
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
         "DeleteOnTermination": bool,
@@ -570,22 +539,20 @@
     {
         "LifecycleActionToken": str,
         "InstanceId": str,
     },
     total=False,
 )
 
-
 class CompleteLifecycleActionTypeRequestTypeDef(
     _RequiredCompleteLifecycleActionTypeRequestTypeDef,
     _OptionalCompleteLifecycleActionTypeRequestTypeDef,
 ):
     pass
 
-
 _RequiredLifecycleHookSpecificationTypeDef = TypedDict(
     "_RequiredLifecycleHookSpecificationTypeDef",
     {
         "LifecycleHookName": str,
         "LifecycleTransition": str,
     },
 )
@@ -597,21 +564,19 @@
         "DefaultResult": str,
         "NotificationTargetARN": str,
         "RoleARN": str,
     },
     total=False,
 )
 
-
 class LifecycleHookSpecificationTypeDef(
     _RequiredLifecycleHookSpecificationTypeDef, _OptionalLifecycleHookSpecificationTypeDef
 ):
     pass
 
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -621,19 +586,17 @@
         "ResourceType": str,
         "Value": str,
         "PropagateAtLaunch": bool,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 InstanceMetadataOptionsTypeDef = TypedDict(
     "InstanceMetadataOptionsTypeDef",
     {
         "HttpTokens": InstanceMetadataHttpTokensStateType,
         "HttpPutResponseHopLimit": int,
         "HttpEndpoint": InstanceMetadataEndpointStateType,
     },
@@ -666,22 +629,20 @@
     "_OptionalDeleteAutoScalingGroupTypeRequestTypeDef",
     {
         "ForceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteAutoScalingGroupTypeRequestTypeDef(
     _RequiredDeleteAutoScalingGroupTypeRequestTypeDef,
     _OptionalDeleteAutoScalingGroupTypeRequestTypeDef,
 ):
     pass
 
-
 DeleteLifecycleHookTypeRequestTypeDef = TypedDict(
     "DeleteLifecycleHookTypeRequestTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
     },
 )
@@ -704,21 +665,19 @@
     "_OptionalDeletePolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
     total=False,
 )
 
-
 class DeletePolicyTypeRequestTypeDef(
     _RequiredDeletePolicyTypeRequestTypeDef, _OptionalDeletePolicyTypeRequestTypeDef
 ):
     pass
 
-
 DeleteScheduledActionTypeRequestTypeDef = TypedDict(
     "DeleteScheduledActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionName": str,
     },
 )
@@ -733,21 +692,19 @@
     "_OptionalDeleteWarmPoolTypeRequestTypeDef",
     {
         "ForceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteWarmPoolTypeRequestTypeDef(
     _RequiredDeleteWarmPoolTypeRequestTypeDef, _OptionalDeleteWarmPoolTypeRequestTypeDef
 ):
     pass
 
-
 DescribeAutoScalingInstancesTypeRequestTypeDef = TypedDict(
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "MaxRecords": int,
         "NextToken": str,
     },
@@ -766,22 +723,20 @@
         "InstanceRefreshIds": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeInstanceRefreshesTypeRequestTypeDef(
     _RequiredDescribeInstanceRefreshesTypeRequestTypeDef,
     _OptionalDescribeInstanceRefreshesTypeRequestTypeDef,
 ):
     pass
 
-
 LifecycleHookTypeDef = TypedDict(
     "LifecycleHookTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
         "LifecycleTransition": str,
         "NotificationTargetARN": str,
@@ -804,22 +759,20 @@
     "_OptionalDescribeLifecycleHooksTypeRequestTypeDef",
     {
         "LifecycleHookNames": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeLifecycleHooksTypeRequestTypeDef(
     _RequiredDescribeLifecycleHooksTypeRequestTypeDef,
     _OptionalDescribeLifecycleHooksTypeRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
@@ -827,22 +780,20 @@
     {
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeLoadBalancerTargetGroupsRequestRequestTypeDef(
     _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 LoadBalancerTargetGroupStateTypeDef = TypedDict(
     "LoadBalancerTargetGroupStateTypeDef",
     {
         "LoadBalancerTargetGroupARN": str,
         "State": str,
     },
     total=False,
@@ -859,22 +810,20 @@
     {
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeLoadBalancersRequestRequestTypeDef(
     _RequiredDescribeLoadBalancersRequestRequestTypeDef,
     _OptionalDescribeLoadBalancersRequestRequestTypeDef,
 ):
     pass
 
-
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "LoadBalancerName": str,
         "State": str,
     },
     total=False,
@@ -936,27 +885,15 @@
         "IncludeDeletedGroups": bool,
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxRecords": int,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTrafficSourcesRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
@@ -965,22 +902,20 @@
         "TrafficSourceType": str,
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeTrafficSourcesRequestRequestTypeDef(
     _RequiredDescribeTrafficSourcesRequestRequestTypeDef,
     _OptionalDescribeTrafficSourcesRequestRequestTypeDef,
 ):
     pass
 
-
 TrafficSourceStateTypeDef = TypedDict(
     "TrafficSourceStateTypeDef",
     {
         "TrafficSource": str,
         "State": str,
         "Identifier": str,
         "Type": str,
@@ -999,21 +934,19 @@
     {
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeWarmPoolTypeRequestTypeDef(
     _RequiredDescribeWarmPoolTypeRequestTypeDef, _OptionalDescribeWarmPoolTypeRequestTypeDef
 ):
     pass
 
-
 _RequiredDetachInstancesQueryRequestTypeDef = TypedDict(
     "_RequiredDetachInstancesQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
@@ -1021,21 +954,19 @@
     "_OptionalDetachInstancesQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class DetachInstancesQueryRequestTypeDef(
     _RequiredDetachInstancesQueryRequestTypeDef, _OptionalDetachInstancesQueryRequestTypeDef
 ):
     pass
 
-
 DetachLoadBalancerTargetGroupsTypeRequestTypeDef = TypedDict(
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TargetGroupARNs": Sequence[str],
     },
 )
@@ -1058,22 +989,20 @@
     "_OptionalDisableMetricsCollectionQueryRequestTypeDef",
     {
         "Metrics": Sequence[str],
     },
     total=False,
 )
 
-
 class DisableMetricsCollectionQueryRequestTypeDef(
     _RequiredDisableMetricsCollectionQueryRequestTypeDef,
     _OptionalDisableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
-
 _RequiredEnableMetricsCollectionQueryRequestTypeDef = TypedDict(
     "_RequiredEnableMetricsCollectionQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "Granularity": str,
     },
 )
@@ -1081,22 +1010,20 @@
     "_OptionalEnableMetricsCollectionQueryRequestTypeDef",
     {
         "Metrics": Sequence[str],
     },
     total=False,
 )
 
-
 class EnableMetricsCollectionQueryRequestTypeDef(
     _RequiredEnableMetricsCollectionQueryRequestTypeDef,
     _OptionalEnableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
-
 _RequiredEnterStandbyQueryRequestTypeDef = TypedDict(
     "_RequiredEnterStandbyQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
@@ -1104,21 +1031,19 @@
     "_OptionalEnterStandbyQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class EnterStandbyQueryRequestTypeDef(
     _RequiredEnterStandbyQueryRequestTypeDef, _OptionalEnterStandbyQueryRequestTypeDef
 ):
     pass
 
-
 _RequiredExecutePolicyTypeRequestTypeDef = TypedDict(
     "_RequiredExecutePolicyTypeRequestTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalExecutePolicyTypeRequestTypeDef = TypedDict(
@@ -1128,52 +1053,38 @@
         "HonorCooldown": bool,
         "MetricValue": float,
         "BreachThreshold": float,
     },
     total=False,
 )
 
-
 class ExecutePolicyTypeRequestTypeDef(
     _RequiredExecutePolicyTypeRequestTypeDef, _OptionalExecutePolicyTypeRequestTypeDef
 ):
     pass
 
-
 _RequiredExitStandbyQueryRequestTypeDef = TypedDict(
     "_RequiredExitStandbyQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalExitStandbyQueryRequestTypeDef = TypedDict(
     "_OptionalExitStandbyQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ExitStandbyQueryRequestTypeDef(
     _RequiredExitStandbyQueryRequestTypeDef, _OptionalExitStandbyQueryRequestTypeDef
 ):
     pass
 
-
-GetPredictiveScalingForecastTypeRequestTypeDef = TypedDict(
-    "GetPredictiveScalingForecastTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
 InstanceRefreshLivePoolProgressTypeDef = TypedDict(
     "InstanceRefreshLivePoolProgressTypeDef",
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
@@ -1207,19 +1118,17 @@
     "_OptionalMemoryMiBRequestTypeDef",
     {
         "Max": int,
     },
     total=False,
 )
 
-
 class MemoryMiBRequestTypeDef(_RequiredMemoryMiBRequestTypeDef, _OptionalMemoryMiBRequestTypeDef):
     pass
 
-
 NetworkBandwidthGbpsRequestTypeDef = TypedDict(
     "NetworkBandwidthGbpsRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1253,19 +1162,17 @@
     "_OptionalVCpuCountRequestTypeDef",
     {
         "Max": int,
     },
     total=False,
 )
 
-
 class VCpuCountRequestTypeDef(_RequiredVCpuCountRequestTypeDef, _OptionalVCpuCountRequestTypeDef):
     pass
 
-
 InstanceReusePolicyTypeDef = TypedDict(
     "InstanceReusePolicyTypeDef",
     {
         "ReuseOnScaleIn": bool,
     },
     total=False,
 )
@@ -1310,87 +1217,79 @@
     "_OptionalPredefinedMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
-
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
-
 _RequiredPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedLoadMetricTypeDef",
     {
         "PredefinedMetricType": PredefinedLoadMetricTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
     "_OptionalPredictiveScalingPredefinedLoadMetricTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
-
 class PredictiveScalingPredefinedLoadMetricTypeDef(
     _RequiredPredictiveScalingPredefinedLoadMetricTypeDef,
     _OptionalPredictiveScalingPredefinedLoadMetricTypeDef,
 ):
     pass
 
-
 _RequiredPredictiveScalingPredefinedMetricPairTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedMetricPairTypeDef",
     {
         "PredefinedMetricType": PredefinedMetricPairTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedMetricPairTypeDef = TypedDict(
     "_OptionalPredictiveScalingPredefinedMetricPairTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
-
 class PredictiveScalingPredefinedMetricPairTypeDef(
     _RequiredPredictiveScalingPredefinedMetricPairTypeDef,
     _OptionalPredictiveScalingPredefinedMetricPairTypeDef,
 ):
     pass
 
-
 _RequiredPredictiveScalingPredefinedScalingMetricTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedScalingMetricTypeDef",
     {
         "PredefinedMetricType": PredefinedScalingMetricTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedScalingMetricTypeDef = TypedDict(
     "_OptionalPredictiveScalingPredefinedScalingMetricTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
-
 class PredictiveScalingPredefinedScalingMetricTypeDef(
     _RequiredPredictiveScalingPredefinedScalingMetricTypeDef,
     _OptionalPredictiveScalingPredefinedScalingMetricTypeDef,
 ):
     pass
 
-
 ProcessTypeTypeDef = TypedDict(
     "ProcessTypeTypeDef",
     {
         "ProcessName": str,
     },
 )
 
@@ -1410,21 +1309,19 @@
         "NotificationMetadata": str,
         "HeartbeatTimeout": int,
         "DefaultResult": str,
     },
     total=False,
 )
 
-
 class PutLifecycleHookTypeRequestTypeDef(
     _RequiredPutLifecycleHookTypeRequestTypeDef, _OptionalPutLifecycleHookTypeRequestTypeDef
 ):
     pass
 
-
 PutNotificationConfigurationTypeRequestTypeDef = TypedDict(
     "PutNotificationConfigurationTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TopicARN": str,
         "NotificationTypes": Sequence[str],
     },
@@ -1441,49 +1338,17 @@
     {
         "MetricIntervalLowerBound": float,
         "MetricIntervalUpperBound": float,
     },
     total=False,
 )
 
-
 class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
     pass
 
-
-_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionName": str,
-    },
-)
-_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "Time": Union[datetime, str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Recurrence": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "DesiredCapacity": int,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-
-class PutScheduledUpdateGroupActionTypeRequestTypeDef(
-    _RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef,
-    _OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef,
-):
-    pass
-
-
 _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef = TypedDict(
     "_RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
     },
 )
@@ -1492,22 +1357,20 @@
     {
         "LifecycleActionToken": str,
         "InstanceId": str,
     },
     total=False,
 )
 
-
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
 ):
     pass
 
-
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -1521,21 +1384,19 @@
     "_OptionalScalingProcessQueryRequestTypeDef",
     {
         "ScalingProcesses": Sequence[str],
     },
     total=False,
 )
 
-
 class ScalingProcessQueryRequestTypeDef(
     _RequiredScalingProcessQueryRequestTypeDef, _OptionalScalingProcessQueryRequestTypeDef
 ):
     pass
 
-
 ScheduledUpdateGroupActionTypeDef = TypedDict(
     "ScheduledUpdateGroupActionTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionName": str,
         "ScheduledActionARN": str,
         "Time": datetime,
@@ -1561,21 +1422,19 @@
     "_OptionalSetDesiredCapacityTypeRequestTypeDef",
     {
         "HonorCooldown": bool,
     },
     total=False,
 )
 
-
 class SetDesiredCapacityTypeRequestTypeDef(
     _RequiredSetDesiredCapacityTypeRequestTypeDef, _OptionalSetDesiredCapacityTypeRequestTypeDef
 ):
     pass
 
-
 _RequiredSetInstanceHealthQueryRequestTypeDef = TypedDict(
     "_RequiredSetInstanceHealthQueryRequestTypeDef",
     {
         "InstanceId": str,
         "HealthStatus": str,
     },
 )
@@ -1583,21 +1442,19 @@
     "_OptionalSetInstanceHealthQueryRequestTypeDef",
     {
         "ShouldRespectGracePeriod": bool,
     },
     total=False,
 )
 
-
 class SetInstanceHealthQueryRequestTypeDef(
     _RequiredSetInstanceHealthQueryRequestTypeDef, _OptionalSetInstanceHealthQueryRequestTypeDef
 ):
     pass
 
-
 SetInstanceProtectionQueryRequestTypeDef = TypedDict(
     "SetInstanceProtectionQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "AutoScalingGroupName": str,
         "ProtectedFromScaleIn": bool,
     },
@@ -1833,44 +1690,40 @@
     "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
     _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
     "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
     _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
 ):
     pass
 
-
 DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
     "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1894,26 +1747,14 @@
         "AutoScalingGroupName": str,
         "IncludeDeletedGroups": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeTagsTypeDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1929,22 +1770,20 @@
     "_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef(
     _RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
     _OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
 ):
     pass
 
-
 LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1968,21 +1807,19 @@
         "LaunchConfigurationName": str,
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
-
 class AutoScalingInstanceDetailsTypeDef(
     _RequiredAutoScalingInstanceDetailsTypeDef, _OptionalAutoScalingInstanceDetailsTypeDef
 ):
     pass
 
-
 _RequiredInstanceTypeDef = TypedDict(
     "_RequiredInstanceTypeDef",
     {
         "InstanceId": str,
         "AvailabilityZone": str,
         "LifecycleState": LifecycleStateType,
         "HealthStatus": str,
@@ -1996,19 +1833,17 @@
         "LaunchConfigurationName": str,
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
-
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
     pass
 
-
 TagsTypeTypeDef = TypedDict(
     "TagsTypeTypeDef",
     {
         "Tags": List[TagDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2026,22 +1861,14 @@
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     {
         "FailedScheduledUpdateGroupActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
-    },
-)
-
 _RequiredBlockDeviceMappingTypeDef = TypedDict(
     "_RequiredBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
     },
 )
 _OptionalBlockDeviceMappingTypeDef = TypedDict(
@@ -2050,21 +1877,19 @@
         "VirtualName": str,
         "Ebs": EbsTypeDef,
         "NoDevice": bool,
     },
     total=False,
 )
 
-
 class BlockDeviceMappingTypeDef(
     _RequiredBlockDeviceMappingTypeDef, _OptionalBlockDeviceMappingTypeDef
 ):
     pass
 
-
 CreateOrUpdateTagsTypeRequestTypeDef = TypedDict(
     "CreateOrUpdateTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
@@ -2086,19 +1911,17 @@
     "_OptionalMetricOutputTypeDef",
     {
         "Dimensions": List[MetricDimensionTypeDef],
     },
     total=False,
 )
 
-
 class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
     pass
 
-
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
@@ -2106,19 +1929,17 @@
     "_OptionalMetricTypeDef",
     {
         "Dimensions": Sequence[MetricDimensionTypeDef],
     },
     total=False,
 )
 
-
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
-
 DescribeLifecycleHooksAnswerTypeDef = TypedDict(
     "DescribeLifecycleHooksAnswerTypeDef",
     {
         "LifecycleHooks": List[LifecycleHookTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2155,14 +1976,103 @@
     {
         "NotificationConfigurations": List[NotificationConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxRecords": int,
+    },
+    total=False,
+)
+
+GetPredictiveScalingForecastTypeRequestTypeDef = TypedDict(
+    "GetPredictiveScalingForecastTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionName": str,
+    },
+)
+_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "Time": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Recurrence": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "DesiredCapacity": int,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+class PutScheduledUpdateGroupActionTypeRequestTypeDef(
+    _RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef,
+    _OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef,
+):
+    pass
+
+_RequiredScheduledUpdateGroupActionRequestTypeDef = TypedDict(
+    "_RequiredScheduledUpdateGroupActionRequestTypeDef",
+    {
+        "ScheduledActionName": str,
+    },
+)
+_OptionalScheduledUpdateGroupActionRequestTypeDef = TypedDict(
+    "_OptionalScheduledUpdateGroupActionRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Recurrence": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "DesiredCapacity": int,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+class ScheduledUpdateGroupActionRequestTypeDef(
+    _RequiredScheduledUpdateGroupActionRequestTypeDef,
+    _OptionalScheduledUpdateGroupActionRequestTypeDef,
+):
+    pass
+
 DescribeTrafficSourcesResponseTypeDef = TypedDict(
     "DescribeTrafficSourcesResponseTypeDef",
     {
         "TrafficSources": List[TrafficSourceStateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2208,21 +2118,19 @@
         "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
         "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
         "AllowedInstanceTypes": List[str],
     },
     total=False,
 )
 
-
 class InstanceRequirementsOutputTypeDef(
     _RequiredInstanceRequirementsOutputTypeDef, _OptionalInstanceRequirementsOutputTypeDef
 ):
     pass
 
-
 _RequiredInstanceRequirementsTypeDef = TypedDict(
     "_RequiredInstanceRequirementsTypeDef",
     {
         "VCpuCount": VCpuCountRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -2250,21 +2158,19 @@
         "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
         "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
         "AllowedInstanceTypes": Sequence[str],
     },
     total=False,
 )
 
-
 class InstanceRequirementsTypeDef(
     _RequiredInstanceRequirementsTypeDef, _OptionalInstanceRequirementsTypeDef
 ):
     pass
 
-
 _RequiredPutWarmPoolTypeRequestTypeDef = TypedDict(
     "_RequiredPutWarmPoolTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalPutWarmPoolTypeRequestTypeDef = TypedDict(
@@ -2274,21 +2180,19 @@
         "MinSize": int,
         "PoolState": WarmPoolStateType,
         "InstanceReusePolicy": InstanceReusePolicyTypeDef,
     },
     total=False,
 )
 
-
 class PutWarmPoolTypeRequestTypeDef(
     _RequiredPutWarmPoolTypeRequestTypeDef, _OptionalPutWarmPoolTypeRequestTypeDef
 ):
     pass
 
-
 WarmPoolConfigurationTypeDef = TypedDict(
     "WarmPoolConfigurationTypeDef",
     {
         "MaxGroupPreparedCapacity": int,
         "MinSize": int,
         "PoolState": WarmPoolStateType,
         "Status": Literal["PendingDelete"],
@@ -2310,14 +2214,15 @@
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RefreshPreferencesUnionTypeDef = Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef]
 AutoScalingInstancesTypeTypeDef = TypedDict(
     "AutoScalingInstancesTypeTypeDef",
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2350,22 +2255,20 @@
         "AssociatePublicIpAddress": bool,
         "PlacementTenancy": str,
         "MetadataOptions": InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
-
 class CreateLaunchConfigurationTypeRequestTypeDef(
     _RequiredCreateLaunchConfigurationTypeRequestTypeDef,
     _OptionalCreateLaunchConfigurationTypeRequestTypeDef,
 ):
     pass
 
-
 _RequiredLaunchConfigurationTypeDef = TypedDict(
     "_RequiredLaunchConfigurationTypeDef",
     {
         "LaunchConfigurationName": str,
         "ImageId": str,
         "InstanceType": str,
         "CreatedTime": datetime,
@@ -2390,21 +2293,19 @@
         "AssociatePublicIpAddress": bool,
         "PlacementTenancy": str,
         "MetadataOptions": InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
-
 class LaunchConfigurationTypeDef(
     _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
-
 _RequiredMetricStatOutputTypeDef = TypedDict(
     "_RequiredMetricStatOutputTypeDef",
     {
         "Metric": MetricOutputTypeDef,
         "Stat": str,
     },
 )
@@ -2412,19 +2313,17 @@
     "_OptionalMetricStatOutputTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
-
 class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
     pass
 
-
 _RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatOutputTypeDef",
     {
         "Metric": MetricOutputTypeDef,
         "Stat": str,
     },
 )
@@ -2432,21 +2331,19 @@
     "_OptionalTargetTrackingMetricStatOutputTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricStatOutputTypeDef(
     _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
 ):
     pass
 
-
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
@@ -2454,19 +2351,17 @@
     "_OptionalMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
-
 class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
-
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
@@ -2474,20 +2369,26 @@
     "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
+BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
+    },
+)
 
 RollbackDetailsTypeDef = TypedDict(
     "RollbackDetailsTypeDef",
     {
         "RollbackReason": str,
         "RollbackStartTime": datetime,
         "PercentageCompleteOnRollback": int,
@@ -2551,21 +2452,19 @@
         "MetricStat": MetricStatOutputTypeDef,
         "Label": str,
         "ReturnData": bool,
     },
     total=False,
 )
 
-
 class MetricDataQueryOutputTypeDef(
     _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
 ):
     pass
 
-
 _RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
@@ -2575,22 +2474,20 @@
         "MetricStat": TargetTrackingMetricStatOutputTypeDef,
         "Label": str,
         "ReturnData": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricDataQueryOutputTypeDef(
     _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
     _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
 ):
     pass
 
-
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -2600,19 +2497,17 @@
         "MetricStat": MetricStatTypeDef,
         "Label": str,
         "ReturnData": bool,
     },
     total=False,
 )
 
-
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
-
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
@@ -2622,21 +2517,19 @@
         "MetricStat": TargetTrackingMetricStatTypeDef,
         "Label": str,
         "ReturnData": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
-
 LaunchTemplateOutputTypeDef = TypedDict(
     "LaunchTemplateOutputTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
     },
     total=False,
@@ -2756,22 +2649,20 @@
         "CustomizedCapacityMetricSpecification": (
             PredictiveScalingCustomizedCapacityMetricOutputTypeDef
         ),
     },
     total=False,
 )
 
-
 class PredictiveScalingMetricSpecificationOutputTypeDef(
     _RequiredPredictiveScalingMetricSpecificationOutputTypeDef,
     _OptionalPredictiveScalingMetricSpecificationOutputTypeDef,
 ):
     pass
 
-
 _RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationOutputTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
@@ -2780,22 +2671,20 @@
         "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
         "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingConfigurationOutputTypeDef(
     _RequiredTargetTrackingConfigurationOutputTypeDef,
     _OptionalTargetTrackingConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredPredictiveScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredictiveScalingMetricSpecificationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationTypeDef = TypedDict(
@@ -2807,22 +2696,20 @@
         "CustomizedScalingMetricSpecification": PredictiveScalingCustomizedScalingMetricTypeDef,
         "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricTypeDef,
         "CustomizedCapacityMetricSpecification": PredictiveScalingCustomizedCapacityMetricTypeDef,
     },
     total=False,
 )
 
-
 class PredictiveScalingMetricSpecificationTypeDef(
     _RequiredPredictiveScalingMetricSpecificationTypeDef,
     _OptionalPredictiveScalingMetricSpecificationTypeDef,
 ):
     pass
 
-
 _RequiredTargetTrackingConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationTypeDef = TypedDict(
@@ -2831,21 +2718,19 @@
         "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
         "CustomizedMetricSpecification": CustomizedMetricSpecificationTypeDef,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
-
 _RequiredAutoScalingGroupTypeDef = TypedDict(
     "_RequiredAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
         "DesiredCapacity": int,
@@ -2884,19 +2769,17 @@
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
         "TrafficSources": List[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
-
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
-
 DesiredConfigurationOutputTypeDef = TypedDict(
     "DesiredConfigurationOutputTypeDef",
     {
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
     },
     total=False,
@@ -2937,31 +2820,32 @@
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
         "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
-
 class CreateAutoScalingGroupTypeRequestTypeDef(
     _RequiredCreateAutoScalingGroupTypeRequestTypeDef,
     _OptionalCreateAutoScalingGroupTypeRequestTypeDef,
 ):
     pass
 
-
 DesiredConfigurationTypeDef = TypedDict(
     "DesiredConfigurationTypeDef",
     {
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
     },
     total=False,
 )
 
+MixedInstancesPolicyUnionTypeDef = Union[
+    MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
+]
 _RequiredUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredUpdateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
@@ -2987,22 +2871,20 @@
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
     },
     total=False,
 )
 
-
 class UpdateAutoScalingGroupTypeRequestTypeDef(
     _RequiredUpdateAutoScalingGroupTypeRequestTypeDef,
     _OptionalUpdateAutoScalingGroupTypeRequestTypeDef,
 ):
     pass
 
-
 LoadForecastTypeDef = TypedDict(
     "LoadForecastTypeDef",
     {
         "Timestamps": List[datetime],
         "Values": List[float],
         "MetricSpecification": PredictiveScalingMetricSpecificationOutputTypeDef,
     },
@@ -3021,22 +2903,20 @@
         "SchedulingBufferTime": int,
         "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
         "MaxCapacityBuffer": int,
     },
     total=False,
 )
 
-
 class PredictiveScalingConfigurationOutputTypeDef(
     _RequiredPredictiveScalingConfigurationOutputTypeDef,
     _OptionalPredictiveScalingConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredPredictiveScalingConfigurationTypeDef = TypedDict(
     "_RequiredPredictiveScalingConfigurationTypeDef",
     {
         "MetricSpecifications": Sequence[PredictiveScalingMetricSpecificationTypeDef],
     },
 )
 _OptionalPredictiveScalingConfigurationTypeDef = TypedDict(
@@ -3046,21 +2926,22 @@
         "SchedulingBufferTime": int,
         "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
         "MaxCapacityBuffer": int,
     },
     total=False,
 )
 
-
 class PredictiveScalingConfigurationTypeDef(
     _RequiredPredictiveScalingConfigurationTypeDef, _OptionalPredictiveScalingConfigurationTypeDef
 ):
     pass
 
-
+TargetTrackingConfigurationUnionTypeDef = Union[
+    TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
+]
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3081,14 +2962,17 @@
         "Preferences": RefreshPreferencesOutputTypeDef,
         "DesiredConfiguration": DesiredConfigurationOutputTypeDef,
         "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
+DesiredConfigurationUnionTypeDef = Union[
+    DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
+]
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalStartInstanceRefreshTypeRequestTypeDef = TypedDict(
@@ -3097,21 +2981,19 @@
         "Strategy": Literal["Rolling"],
         "DesiredConfiguration": DesiredConfigurationTypeDef,
         "Preferences": RefreshPreferencesTypeDef,
     },
     total=False,
 )
 
-
 class StartInstanceRefreshTypeRequestTypeDef(
     _RequiredStartInstanceRefreshTypeRequestTypeDef, _OptionalStartInstanceRefreshTypeRequestTypeDef
 ):
     pass
 
-
 GetPredictiveScalingForecastAnswerTypeDef = TypedDict(
     "GetPredictiveScalingForecastAnswerTypeDef",
     {
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3137,14 +3019,17 @@
         "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+PredictiveScalingConfigurationUnionTypeDef = Union[
+    PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
+]
 _RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
     },
 )
@@ -3163,21 +3048,19 @@
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class PutScalingPolicyTypeRequestTypeDef(
     _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
 ):
     pass
 
-
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/type_defs.pyi` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestTypeDef
 
-    data: AcceleratorCountRequestTypeDef = {...}
+    data: AcceleratorCountRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -47,14 +47,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmSpecificationOutputTypeDef",
@@ -69,15 +70,14 @@
     "EnabledMetricTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
-    "ScheduledUpdateGroupActionRequestTypeDef",
     "EbsTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
@@ -99,27 +99,26 @@
     "LoadBalancerStateTypeDef",
     "MetricCollectionTypeTypeDef",
     "MetricGranularityTypeTypeDef",
     "NotificationConfigurationTypeDef",
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
     "DescribePoliciesTypeRequestTypeDef",
     "DescribeScalingActivitiesTypeRequestTypeDef",
-    "DescribeScheduledActionsTypeRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeTrafficSourcesRequestRequestTypeDef",
     "TrafficSourceStateTypeDef",
     "DescribeWarmPoolTypeRequestTypeDef",
     "DetachInstancesQueryRequestTypeDef",
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
-    "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
@@ -132,15 +131,14 @@
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
-    "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
@@ -169,49 +167,54 @@
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     "DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
-    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
     "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    "DescribeScheduledActionsTypeRequestTypeDef",
+    "GetPredictiveScalingForecastTypeRequestTypeDef",
+    "PutScheduledUpdateGroupActionTypeRequestTypeDef",
+    "ScheduledUpdateGroupActionRequestTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
     "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
     "ScheduledActionsTypeTypeDef",
+    "RefreshPreferencesUnionTypeDef",
     "AutoScalingInstancesTypeTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
     "MetricStatOutputTypeDef",
     "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
+    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RollbackDetailsTypeDef",
     "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
     "MetricDataQueryOutputTypeDef",
     "TargetTrackingMetricDataQueryOutputTypeDef",
@@ -233,23 +236,27 @@
     "TargetTrackingConfigurationOutputTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
     "DesiredConfigurationOutputTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
+    "MixedInstancesPolicyUnionTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
     "PredictiveScalingConfigurationOutputTypeDef",
     "PredictiveScalingConfigurationTypeDef",
+    "TargetTrackingConfigurationUnionTypeDef",
     "AutoScalingGroupsTypeTypeDef",
     "InstanceRefreshTypeDef",
+    "DesiredConfigurationUnionTypeDef",
     "StartInstanceRefreshTypeRequestTypeDef",
     "GetPredictiveScalingForecastAnswerTypeDef",
     "ScalingPolicyTypeDef",
+    "PredictiveScalingConfigurationUnionTypeDef",
     "PutScalingPolicyTypeRequestTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
@@ -289,17 +296,19 @@
         "Details": str,
         "AutoScalingGroupState": str,
         "AutoScalingGroupARN": str,
     },
     total=False,
 )
 
+
 class ActivityTypeDef(_RequiredActivityTypeDef, _OptionalActivityTypeDef):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -350,19 +359,21 @@
     "_OptionalAttachInstancesQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class AttachInstancesQueryRequestTypeDef(
     _RequiredAttachInstancesQueryRequestTypeDef, _OptionalAttachInstancesQueryRequestTypeDef
 ):
     pass
 
+
 AttachLoadBalancerTargetGroupsTypeRequestTypeDef = TypedDict(
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TargetGroupARNs": Sequence[str],
     },
 )
@@ -385,19 +396,21 @@
     "_OptionalTrafficSourceIdentifierTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+
 class TrafficSourceIdentifierTypeDef(
     _RequiredTrafficSourceIdentifierTypeDef, _OptionalTrafficSourceIdentifierTypeDef
 ):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -473,54 +486,30 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+
 class FailedScheduledUpdateGroupActionRequestTypeDef(
     _RequiredFailedScheduledUpdateGroupActionRequestTypeDef,
     _OptionalFailedScheduledUpdateGroupActionRequestTypeDef,
 ):
     pass
 
+
 BatchDeleteScheduledActionTypeRequestTypeDef = TypedDict(
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionNames": Sequence[str],
     },
 )
 
-_RequiredScheduledUpdateGroupActionRequestTypeDef = TypedDict(
-    "_RequiredScheduledUpdateGroupActionRequestTypeDef",
-    {
-        "ScheduledActionName": str,
-    },
-)
-_OptionalScheduledUpdateGroupActionRequestTypeDef = TypedDict(
-    "_OptionalScheduledUpdateGroupActionRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Recurrence": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "DesiredCapacity": int,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-class ScheduledUpdateGroupActionRequestTypeDef(
-    _RequiredScheduledUpdateGroupActionRequestTypeDef,
-    _OptionalScheduledUpdateGroupActionRequestTypeDef,
-):
-    pass
-
 EbsTypeDef = TypedDict(
     "EbsTypeDef",
     {
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
         "DeleteOnTermination": bool,
@@ -559,20 +548,22 @@
     {
         "LifecycleActionToken": str,
         "InstanceId": str,
     },
     total=False,
 )
 
+
 class CompleteLifecycleActionTypeRequestTypeDef(
     _RequiredCompleteLifecycleActionTypeRequestTypeDef,
     _OptionalCompleteLifecycleActionTypeRequestTypeDef,
 ):
     pass
 
+
 _RequiredLifecycleHookSpecificationTypeDef = TypedDict(
     "_RequiredLifecycleHookSpecificationTypeDef",
     {
         "LifecycleHookName": str,
         "LifecycleTransition": str,
     },
 )
@@ -584,19 +575,21 @@
         "DefaultResult": str,
         "NotificationTargetARN": str,
         "RoleARN": str,
     },
     total=False,
 )
 
+
 class LifecycleHookSpecificationTypeDef(
     _RequiredLifecycleHookSpecificationTypeDef, _OptionalLifecycleHookSpecificationTypeDef
 ):
     pass
 
+
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -606,17 +599,19 @@
         "ResourceType": str,
         "Value": str,
         "PropagateAtLaunch": bool,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 InstanceMetadataOptionsTypeDef = TypedDict(
     "InstanceMetadataOptionsTypeDef",
     {
         "HttpTokens": InstanceMetadataHttpTokensStateType,
         "HttpPutResponseHopLimit": int,
         "HttpEndpoint": InstanceMetadataEndpointStateType,
     },
@@ -649,20 +644,22 @@
     "_OptionalDeleteAutoScalingGroupTypeRequestTypeDef",
     {
         "ForceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteAutoScalingGroupTypeRequestTypeDef(
     _RequiredDeleteAutoScalingGroupTypeRequestTypeDef,
     _OptionalDeleteAutoScalingGroupTypeRequestTypeDef,
 ):
     pass
 
+
 DeleteLifecycleHookTypeRequestTypeDef = TypedDict(
     "DeleteLifecycleHookTypeRequestTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
     },
 )
@@ -685,19 +682,21 @@
     "_OptionalDeletePolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
     total=False,
 )
 
+
 class DeletePolicyTypeRequestTypeDef(
     _RequiredDeletePolicyTypeRequestTypeDef, _OptionalDeletePolicyTypeRequestTypeDef
 ):
     pass
 
+
 DeleteScheduledActionTypeRequestTypeDef = TypedDict(
     "DeleteScheduledActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionName": str,
     },
 )
@@ -712,19 +711,21 @@
     "_OptionalDeleteWarmPoolTypeRequestTypeDef",
     {
         "ForceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteWarmPoolTypeRequestTypeDef(
     _RequiredDeleteWarmPoolTypeRequestTypeDef, _OptionalDeleteWarmPoolTypeRequestTypeDef
 ):
     pass
 
+
 DescribeAutoScalingInstancesTypeRequestTypeDef = TypedDict(
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "MaxRecords": int,
         "NextToken": str,
     },
@@ -743,20 +744,22 @@
         "InstanceRefreshIds": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeInstanceRefreshesTypeRequestTypeDef(
     _RequiredDescribeInstanceRefreshesTypeRequestTypeDef,
     _OptionalDescribeInstanceRefreshesTypeRequestTypeDef,
 ):
     pass
 
+
 LifecycleHookTypeDef = TypedDict(
     "LifecycleHookTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
         "LifecycleTransition": str,
         "NotificationTargetARN": str,
@@ -779,20 +782,22 @@
     "_OptionalDescribeLifecycleHooksTypeRequestTypeDef",
     {
         "LifecycleHookNames": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeLifecycleHooksTypeRequestTypeDef(
     _RequiredDescribeLifecycleHooksTypeRequestTypeDef,
     _OptionalDescribeLifecycleHooksTypeRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
@@ -800,20 +805,22 @@
     {
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeLoadBalancerTargetGroupsRequestRequestTypeDef(
     _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 LoadBalancerTargetGroupStateTypeDef = TypedDict(
     "LoadBalancerTargetGroupStateTypeDef",
     {
         "LoadBalancerTargetGroupARN": str,
         "State": str,
     },
     total=False,
@@ -830,20 +837,22 @@
     {
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeLoadBalancersRequestRequestTypeDef(
     _RequiredDescribeLoadBalancersRequestRequestTypeDef,
     _OptionalDescribeLoadBalancersRequestRequestTypeDef,
 ):
     pass
 
+
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "LoadBalancerName": str,
         "State": str,
     },
     total=False,
@@ -905,27 +914,15 @@
         "IncludeDeletedGroups": bool,
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxRecords": int,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTrafficSourcesRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
@@ -934,20 +931,22 @@
         "TrafficSourceType": str,
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeTrafficSourcesRequestRequestTypeDef(
     _RequiredDescribeTrafficSourcesRequestRequestTypeDef,
     _OptionalDescribeTrafficSourcesRequestRequestTypeDef,
 ):
     pass
 
+
 TrafficSourceStateTypeDef = TypedDict(
     "TrafficSourceStateTypeDef",
     {
         "TrafficSource": str,
         "State": str,
         "Identifier": str,
         "Type": str,
@@ -966,19 +965,21 @@
     {
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeWarmPoolTypeRequestTypeDef(
     _RequiredDescribeWarmPoolTypeRequestTypeDef, _OptionalDescribeWarmPoolTypeRequestTypeDef
 ):
     pass
 
+
 _RequiredDetachInstancesQueryRequestTypeDef = TypedDict(
     "_RequiredDetachInstancesQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
@@ -986,19 +987,21 @@
     "_OptionalDetachInstancesQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class DetachInstancesQueryRequestTypeDef(
     _RequiredDetachInstancesQueryRequestTypeDef, _OptionalDetachInstancesQueryRequestTypeDef
 ):
     pass
 
+
 DetachLoadBalancerTargetGroupsTypeRequestTypeDef = TypedDict(
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TargetGroupARNs": Sequence[str],
     },
 )
@@ -1021,20 +1024,22 @@
     "_OptionalDisableMetricsCollectionQueryRequestTypeDef",
     {
         "Metrics": Sequence[str],
     },
     total=False,
 )
 
+
 class DisableMetricsCollectionQueryRequestTypeDef(
     _RequiredDisableMetricsCollectionQueryRequestTypeDef,
     _OptionalDisableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
+
 _RequiredEnableMetricsCollectionQueryRequestTypeDef = TypedDict(
     "_RequiredEnableMetricsCollectionQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "Granularity": str,
     },
 )
@@ -1042,20 +1047,22 @@
     "_OptionalEnableMetricsCollectionQueryRequestTypeDef",
     {
         "Metrics": Sequence[str],
     },
     total=False,
 )
 
+
 class EnableMetricsCollectionQueryRequestTypeDef(
     _RequiredEnableMetricsCollectionQueryRequestTypeDef,
     _OptionalEnableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
+
 _RequiredEnterStandbyQueryRequestTypeDef = TypedDict(
     "_RequiredEnterStandbyQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
@@ -1063,19 +1070,21 @@
     "_OptionalEnterStandbyQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class EnterStandbyQueryRequestTypeDef(
     _RequiredEnterStandbyQueryRequestTypeDef, _OptionalEnterStandbyQueryRequestTypeDef
 ):
     pass
 
+
 _RequiredExecutePolicyTypeRequestTypeDef = TypedDict(
     "_RequiredExecutePolicyTypeRequestTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalExecutePolicyTypeRequestTypeDef = TypedDict(
@@ -1085,47 +1094,41 @@
         "HonorCooldown": bool,
         "MetricValue": float,
         "BreachThreshold": float,
     },
     total=False,
 )
 
+
 class ExecutePolicyTypeRequestTypeDef(
     _RequiredExecutePolicyTypeRequestTypeDef, _OptionalExecutePolicyTypeRequestTypeDef
 ):
     pass
 
+
 _RequiredExitStandbyQueryRequestTypeDef = TypedDict(
     "_RequiredExitStandbyQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalExitStandbyQueryRequestTypeDef = TypedDict(
     "_OptionalExitStandbyQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ExitStandbyQueryRequestTypeDef(
     _RequiredExitStandbyQueryRequestTypeDef, _OptionalExitStandbyQueryRequestTypeDef
 ):
     pass
 
-GetPredictiveScalingForecastTypeRequestTypeDef = TypedDict(
-    "GetPredictiveScalingForecastTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
 
 InstanceRefreshLivePoolProgressTypeDef = TypedDict(
     "InstanceRefreshLivePoolProgressTypeDef",
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
@@ -1160,17 +1163,19 @@
     "_OptionalMemoryMiBRequestTypeDef",
     {
         "Max": int,
     },
     total=False,
 )
 
+
 class MemoryMiBRequestTypeDef(_RequiredMemoryMiBRequestTypeDef, _OptionalMemoryMiBRequestTypeDef):
     pass
 
+
 NetworkBandwidthGbpsRequestTypeDef = TypedDict(
     "NetworkBandwidthGbpsRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1204,17 +1209,19 @@
     "_OptionalVCpuCountRequestTypeDef",
     {
         "Max": int,
     },
     total=False,
 )
 
+
 class VCpuCountRequestTypeDef(_RequiredVCpuCountRequestTypeDef, _OptionalVCpuCountRequestTypeDef):
     pass
 
+
 InstanceReusePolicyTypeDef = TypedDict(
     "InstanceReusePolicyTypeDef",
     {
         "ReuseOnScaleIn": bool,
     },
     total=False,
 )
@@ -1259,79 +1266,87 @@
     "_OptionalPredefinedMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
+
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
+
 _RequiredPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedLoadMetricTypeDef",
     {
         "PredefinedMetricType": PredefinedLoadMetricTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
     "_OptionalPredictiveScalingPredefinedLoadMetricTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
+
 class PredictiveScalingPredefinedLoadMetricTypeDef(
     _RequiredPredictiveScalingPredefinedLoadMetricTypeDef,
     _OptionalPredictiveScalingPredefinedLoadMetricTypeDef,
 ):
     pass
 
+
 _RequiredPredictiveScalingPredefinedMetricPairTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedMetricPairTypeDef",
     {
         "PredefinedMetricType": PredefinedMetricPairTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedMetricPairTypeDef = TypedDict(
     "_OptionalPredictiveScalingPredefinedMetricPairTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
+
 class PredictiveScalingPredefinedMetricPairTypeDef(
     _RequiredPredictiveScalingPredefinedMetricPairTypeDef,
     _OptionalPredictiveScalingPredefinedMetricPairTypeDef,
 ):
     pass
 
+
 _RequiredPredictiveScalingPredefinedScalingMetricTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedScalingMetricTypeDef",
     {
         "PredefinedMetricType": PredefinedScalingMetricTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedScalingMetricTypeDef = TypedDict(
     "_OptionalPredictiveScalingPredefinedScalingMetricTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
+
 class PredictiveScalingPredefinedScalingMetricTypeDef(
     _RequiredPredictiveScalingPredefinedScalingMetricTypeDef,
     _OptionalPredictiveScalingPredefinedScalingMetricTypeDef,
 ):
     pass
 
+
 ProcessTypeTypeDef = TypedDict(
     "ProcessTypeTypeDef",
     {
         "ProcessName": str,
     },
 )
 
@@ -1351,19 +1366,21 @@
         "NotificationMetadata": str,
         "HeartbeatTimeout": int,
         "DefaultResult": str,
     },
     total=False,
 )
 
+
 class PutLifecycleHookTypeRequestTypeDef(
     _RequiredPutLifecycleHookTypeRequestTypeDef, _OptionalPutLifecycleHookTypeRequestTypeDef
 ):
     pass
 
+
 PutNotificationConfigurationTypeRequestTypeDef = TypedDict(
     "PutNotificationConfigurationTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TopicARN": str,
         "NotificationTypes": Sequence[str],
     },
@@ -1380,44 +1397,18 @@
     {
         "MetricIntervalLowerBound": float,
         "MetricIntervalUpperBound": float,
     },
     total=False,
 )
 
+
 class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
     pass
 
-_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionName": str,
-    },
-)
-_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "Time": Union[datetime, str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Recurrence": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "DesiredCapacity": int,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-class PutScheduledUpdateGroupActionTypeRequestTypeDef(
-    _RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef,
-    _OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef,
-):
-    pass
 
 _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef = TypedDict(
     "_RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
     },
@@ -1427,20 +1418,22 @@
     {
         "LifecycleActionToken": str,
         "InstanceId": str,
     },
     total=False,
 )
 
+
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
 ):
     pass
 
+
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -1454,19 +1447,21 @@
     "_OptionalScalingProcessQueryRequestTypeDef",
     {
         "ScalingProcesses": Sequence[str],
     },
     total=False,
 )
 
+
 class ScalingProcessQueryRequestTypeDef(
     _RequiredScalingProcessQueryRequestTypeDef, _OptionalScalingProcessQueryRequestTypeDef
 ):
     pass
 
+
 ScheduledUpdateGroupActionTypeDef = TypedDict(
     "ScheduledUpdateGroupActionTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionName": str,
         "ScheduledActionARN": str,
         "Time": datetime,
@@ -1492,19 +1487,21 @@
     "_OptionalSetDesiredCapacityTypeRequestTypeDef",
     {
         "HonorCooldown": bool,
     },
     total=False,
 )
 
+
 class SetDesiredCapacityTypeRequestTypeDef(
     _RequiredSetDesiredCapacityTypeRequestTypeDef, _OptionalSetDesiredCapacityTypeRequestTypeDef
 ):
     pass
 
+
 _RequiredSetInstanceHealthQueryRequestTypeDef = TypedDict(
     "_RequiredSetInstanceHealthQueryRequestTypeDef",
     {
         "InstanceId": str,
         "HealthStatus": str,
     },
 )
@@ -1512,19 +1509,21 @@
     "_OptionalSetInstanceHealthQueryRequestTypeDef",
     {
         "ShouldRespectGracePeriod": bool,
     },
     total=False,
 )
 
+
 class SetInstanceHealthQueryRequestTypeDef(
     _RequiredSetInstanceHealthQueryRequestTypeDef, _OptionalSetInstanceHealthQueryRequestTypeDef
 ):
     pass
 
+
 SetInstanceProtectionQueryRequestTypeDef = TypedDict(
     "SetInstanceProtectionQueryRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "AutoScalingGroupName": str,
         "ProtectedFromScaleIn": bool,
     },
@@ -1760,40 +1759,44 @@
     "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
     _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
     "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
     _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
 ):
     pass
 
+
 DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
     "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1817,26 +1820,14 @@
         "AutoScalingGroupName": str,
         "IncludeDeletedGroups": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeTagsTypeDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1852,20 +1843,22 @@
     "_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef(
     _RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
     _OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
 ):
     pass
 
+
 LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1889,19 +1882,21 @@
         "LaunchConfigurationName": str,
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
+
 class AutoScalingInstanceDetailsTypeDef(
     _RequiredAutoScalingInstanceDetailsTypeDef, _OptionalAutoScalingInstanceDetailsTypeDef
 ):
     pass
 
+
 _RequiredInstanceTypeDef = TypedDict(
     "_RequiredInstanceTypeDef",
     {
         "InstanceId": str,
         "AvailabilityZone": str,
         "LifecycleState": LifecycleStateType,
         "HealthStatus": str,
@@ -1915,17 +1910,19 @@
         "LaunchConfigurationName": str,
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
+
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
     pass
 
+
 TagsTypeTypeDef = TypedDict(
     "TagsTypeTypeDef",
     {
         "Tags": List[TagDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1943,22 +1940,14 @@
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     {
         "FailedScheduledUpdateGroupActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
-    },
-)
-
 _RequiredBlockDeviceMappingTypeDef = TypedDict(
     "_RequiredBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
     },
 )
 _OptionalBlockDeviceMappingTypeDef = TypedDict(
@@ -1967,19 +1956,21 @@
         "VirtualName": str,
         "Ebs": EbsTypeDef,
         "NoDevice": bool,
     },
     total=False,
 )
 
+
 class BlockDeviceMappingTypeDef(
     _RequiredBlockDeviceMappingTypeDef, _OptionalBlockDeviceMappingTypeDef
 ):
     pass
 
+
 CreateOrUpdateTagsTypeRequestTypeDef = TypedDict(
     "CreateOrUpdateTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
@@ -2001,17 +1992,19 @@
     "_OptionalMetricOutputTypeDef",
     {
         "Dimensions": List[MetricDimensionTypeDef],
     },
     total=False,
 )
 
+
 class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
     pass
 
+
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
@@ -2019,17 +2012,19 @@
     "_OptionalMetricTypeDef",
     {
         "Dimensions": Sequence[MetricDimensionTypeDef],
     },
     total=False,
 )
 
+
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
+
 DescribeLifecycleHooksAnswerTypeDef = TypedDict(
     "DescribeLifecycleHooksAnswerTypeDef",
     {
         "LifecycleHooks": List[LifecycleHookTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2066,14 +2061,107 @@
     {
         "NotificationConfigurations": List[NotificationConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxRecords": int,
+    },
+    total=False,
+)
+
+GetPredictiveScalingForecastTypeRequestTypeDef = TypedDict(
+    "GetPredictiveScalingForecastTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionName": str,
+    },
+)
+_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "Time": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Recurrence": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "DesiredCapacity": int,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+
+class PutScheduledUpdateGroupActionTypeRequestTypeDef(
+    _RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef,
+    _OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef,
+):
+    pass
+
+
+_RequiredScheduledUpdateGroupActionRequestTypeDef = TypedDict(
+    "_RequiredScheduledUpdateGroupActionRequestTypeDef",
+    {
+        "ScheduledActionName": str,
+    },
+)
+_OptionalScheduledUpdateGroupActionRequestTypeDef = TypedDict(
+    "_OptionalScheduledUpdateGroupActionRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Recurrence": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "DesiredCapacity": int,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+
+class ScheduledUpdateGroupActionRequestTypeDef(
+    _RequiredScheduledUpdateGroupActionRequestTypeDef,
+    _OptionalScheduledUpdateGroupActionRequestTypeDef,
+):
+    pass
+
+
 DescribeTrafficSourcesResponseTypeDef = TypedDict(
     "DescribeTrafficSourcesResponseTypeDef",
     {
         "TrafficSources": List[TrafficSourceStateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2119,19 +2207,21 @@
         "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
         "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
         "AllowedInstanceTypes": List[str],
     },
     total=False,
 )
 
+
 class InstanceRequirementsOutputTypeDef(
     _RequiredInstanceRequirementsOutputTypeDef, _OptionalInstanceRequirementsOutputTypeDef
 ):
     pass
 
+
 _RequiredInstanceRequirementsTypeDef = TypedDict(
     "_RequiredInstanceRequirementsTypeDef",
     {
         "VCpuCount": VCpuCountRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -2159,19 +2249,21 @@
         "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
         "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
         "AllowedInstanceTypes": Sequence[str],
     },
     total=False,
 )
 
+
 class InstanceRequirementsTypeDef(
     _RequiredInstanceRequirementsTypeDef, _OptionalInstanceRequirementsTypeDef
 ):
     pass
 
+
 _RequiredPutWarmPoolTypeRequestTypeDef = TypedDict(
     "_RequiredPutWarmPoolTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalPutWarmPoolTypeRequestTypeDef = TypedDict(
@@ -2181,19 +2273,21 @@
         "MinSize": int,
         "PoolState": WarmPoolStateType,
         "InstanceReusePolicy": InstanceReusePolicyTypeDef,
     },
     total=False,
 )
 
+
 class PutWarmPoolTypeRequestTypeDef(
     _RequiredPutWarmPoolTypeRequestTypeDef, _OptionalPutWarmPoolTypeRequestTypeDef
 ):
     pass
 
+
 WarmPoolConfigurationTypeDef = TypedDict(
     "WarmPoolConfigurationTypeDef",
     {
         "MaxGroupPreparedCapacity": int,
         "MinSize": int,
         "PoolState": WarmPoolStateType,
         "Status": Literal["PendingDelete"],
@@ -2215,14 +2309,15 @@
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RefreshPreferencesUnionTypeDef = Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef]
 AutoScalingInstancesTypeTypeDef = TypedDict(
     "AutoScalingInstancesTypeTypeDef",
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2255,20 +2350,22 @@
         "AssociatePublicIpAddress": bool,
         "PlacementTenancy": str,
         "MetadataOptions": InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
+
 class CreateLaunchConfigurationTypeRequestTypeDef(
     _RequiredCreateLaunchConfigurationTypeRequestTypeDef,
     _OptionalCreateLaunchConfigurationTypeRequestTypeDef,
 ):
     pass
 
+
 _RequiredLaunchConfigurationTypeDef = TypedDict(
     "_RequiredLaunchConfigurationTypeDef",
     {
         "LaunchConfigurationName": str,
         "ImageId": str,
         "InstanceType": str,
         "CreatedTime": datetime,
@@ -2293,19 +2390,21 @@
         "AssociatePublicIpAddress": bool,
         "PlacementTenancy": str,
         "MetadataOptions": InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
+
 class LaunchConfigurationTypeDef(
     _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
+
 _RequiredMetricStatOutputTypeDef = TypedDict(
     "_RequiredMetricStatOutputTypeDef",
     {
         "Metric": MetricOutputTypeDef,
         "Stat": str,
     },
 )
@@ -2313,17 +2412,19 @@
     "_OptionalMetricStatOutputTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
+
 class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
     pass
 
+
 _RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatOutputTypeDef",
     {
         "Metric": MetricOutputTypeDef,
         "Stat": str,
     },
 )
@@ -2331,19 +2432,21 @@
     "_OptionalTargetTrackingMetricStatOutputTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricStatOutputTypeDef(
     _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
 ):
     pass
 
+
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
@@ -2351,17 +2454,19 @@
     "_OptionalMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
+
 class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
+
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
@@ -2369,19 +2474,29 @@
     "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
+
+BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
+    },
+)
+
 RollbackDetailsTypeDef = TypedDict(
     "RollbackDetailsTypeDef",
     {
         "RollbackReason": str,
         "RollbackStartTime": datetime,
         "PercentageCompleteOnRollback": int,
         "InstancesToUpdateOnRollback": int,
@@ -2444,19 +2559,21 @@
         "MetricStat": MetricStatOutputTypeDef,
         "Label": str,
         "ReturnData": bool,
     },
     total=False,
 )
 
+
 class MetricDataQueryOutputTypeDef(
     _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
 ):
     pass
 
+
 _RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
@@ -2466,20 +2583,22 @@
         "MetricStat": TargetTrackingMetricStatOutputTypeDef,
         "Label": str,
         "ReturnData": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricDataQueryOutputTypeDef(
     _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
     _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
 ):
     pass
 
+
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -2489,17 +2608,19 @@
         "MetricStat": MetricStatTypeDef,
         "Label": str,
         "ReturnData": bool,
     },
     total=False,
 )
 
+
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
+
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
@@ -2509,19 +2630,21 @@
         "MetricStat": TargetTrackingMetricStatTypeDef,
         "Label": str,
         "ReturnData": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
+
 LaunchTemplateOutputTypeDef = TypedDict(
     "LaunchTemplateOutputTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
     },
     total=False,
@@ -2641,20 +2764,22 @@
         "CustomizedCapacityMetricSpecification": (
             PredictiveScalingCustomizedCapacityMetricOutputTypeDef
         ),
     },
     total=False,
 )
 
+
 class PredictiveScalingMetricSpecificationOutputTypeDef(
     _RequiredPredictiveScalingMetricSpecificationOutputTypeDef,
     _OptionalPredictiveScalingMetricSpecificationOutputTypeDef,
 ):
     pass
 
+
 _RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationOutputTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
@@ -2663,20 +2788,22 @@
         "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
         "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingConfigurationOutputTypeDef(
     _RequiredTargetTrackingConfigurationOutputTypeDef,
     _OptionalTargetTrackingConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredPredictiveScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredictiveScalingMetricSpecificationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationTypeDef = TypedDict(
@@ -2688,20 +2815,22 @@
         "CustomizedScalingMetricSpecification": PredictiveScalingCustomizedScalingMetricTypeDef,
         "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricTypeDef,
         "CustomizedCapacityMetricSpecification": PredictiveScalingCustomizedCapacityMetricTypeDef,
     },
     total=False,
 )
 
+
 class PredictiveScalingMetricSpecificationTypeDef(
     _RequiredPredictiveScalingMetricSpecificationTypeDef,
     _OptionalPredictiveScalingMetricSpecificationTypeDef,
 ):
     pass
 
+
 _RequiredTargetTrackingConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationTypeDef = TypedDict(
@@ -2710,19 +2839,21 @@
         "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
         "CustomizedMetricSpecification": CustomizedMetricSpecificationTypeDef,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
+
 _RequiredAutoScalingGroupTypeDef = TypedDict(
     "_RequiredAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
         "DesiredCapacity": int,
@@ -2761,17 +2892,19 @@
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
         "TrafficSources": List[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
+
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
+
 DesiredConfigurationOutputTypeDef = TypedDict(
     "DesiredConfigurationOutputTypeDef",
     {
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
     },
     total=False,
@@ -2812,29 +2945,34 @@
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
         "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
+
 class CreateAutoScalingGroupTypeRequestTypeDef(
     _RequiredCreateAutoScalingGroupTypeRequestTypeDef,
     _OptionalCreateAutoScalingGroupTypeRequestTypeDef,
 ):
     pass
 
+
 DesiredConfigurationTypeDef = TypedDict(
     "DesiredConfigurationTypeDef",
     {
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
     },
     total=False,
 )
 
+MixedInstancesPolicyUnionTypeDef = Union[
+    MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
+]
 _RequiredUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredUpdateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
@@ -2860,20 +2998,22 @@
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
     },
     total=False,
 )
 
+
 class UpdateAutoScalingGroupTypeRequestTypeDef(
     _RequiredUpdateAutoScalingGroupTypeRequestTypeDef,
     _OptionalUpdateAutoScalingGroupTypeRequestTypeDef,
 ):
     pass
 
+
 LoadForecastTypeDef = TypedDict(
     "LoadForecastTypeDef",
     {
         "Timestamps": List[datetime],
         "Values": List[float],
         "MetricSpecification": PredictiveScalingMetricSpecificationOutputTypeDef,
     },
@@ -2892,20 +3032,22 @@
         "SchedulingBufferTime": int,
         "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
         "MaxCapacityBuffer": int,
     },
     total=False,
 )
 
+
 class PredictiveScalingConfigurationOutputTypeDef(
     _RequiredPredictiveScalingConfigurationOutputTypeDef,
     _OptionalPredictiveScalingConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredPredictiveScalingConfigurationTypeDef = TypedDict(
     "_RequiredPredictiveScalingConfigurationTypeDef",
     {
         "MetricSpecifications": Sequence[PredictiveScalingMetricSpecificationTypeDef],
     },
 )
 _OptionalPredictiveScalingConfigurationTypeDef = TypedDict(
@@ -2915,19 +3057,24 @@
         "SchedulingBufferTime": int,
         "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
         "MaxCapacityBuffer": int,
     },
     total=False,
 )
 
+
 class PredictiveScalingConfigurationTypeDef(
     _RequiredPredictiveScalingConfigurationTypeDef, _OptionalPredictiveScalingConfigurationTypeDef
 ):
     pass
 
+
+TargetTrackingConfigurationUnionTypeDef = Union[
+    TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
+]
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2948,14 +3095,17 @@
         "Preferences": RefreshPreferencesOutputTypeDef,
         "DesiredConfiguration": DesiredConfigurationOutputTypeDef,
         "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
+DesiredConfigurationUnionTypeDef = Union[
+    DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
+]
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalStartInstanceRefreshTypeRequestTypeDef = TypedDict(
@@ -2964,19 +3114,21 @@
         "Strategy": Literal["Rolling"],
         "DesiredConfiguration": DesiredConfigurationTypeDef,
         "Preferences": RefreshPreferencesTypeDef,
     },
     total=False,
 )
 
+
 class StartInstanceRefreshTypeRequestTypeDef(
     _RequiredStartInstanceRefreshTypeRequestTypeDef, _OptionalStartInstanceRefreshTypeRequestTypeDef
 ):
     pass
 
+
 GetPredictiveScalingForecastAnswerTypeDef = TypedDict(
     "GetPredictiveScalingForecastAnswerTypeDef",
     {
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3002,14 +3154,17 @@
         "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+PredictiveScalingConfigurationUnionTypeDef = Union[
+    PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
+]
 _RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
     },
 )
@@ -3028,19 +3183,21 @@
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class PutScalingPolicyTypeRequestTypeDef(
     _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
 ):
     pass
 
+
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.16
-Summary: Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 autoscaling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 autoscaling type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
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
@@ -383,20 +383,20 @@
 )
 
 
 def check_value(value: AcceleratorManufacturerType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_autoscaling.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     ResponseMetadataTypeDef,
@@ -413,15 +413,14 @@
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
-    ScheduledUpdateGroupActionRequestTypeDef,
     EbsTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
@@ -443,27 +442,26 @@
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
     DescribePoliciesTypeRequestTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
-    DescribeScheduledActionsTypeRequestTypeDef,
+    TimestampTypeDef,
     DescribeTrafficSourcesRequestRequestTypeDef,
     TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
-    GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
@@ -476,15 +474,14 @@
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
-    PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
@@ -513,49 +510,54 @@
     AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
     DescribeTagsTypeDescribeTagsPaginateTypeDef,
     DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
     LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
-    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    DescribeScheduledActionsTypeRequestTypeDef,
+    GetPredictiveScalingForecastTypeRequestTypeDef,
+    PutScheduledUpdateGroupActionTypeRequestTypeDef,
+    ScheduledUpdateGroupActionRequestTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
     InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
     PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
+    RefreshPreferencesUnionTypeDef,
     AutoScalingInstancesTypeTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
     MetricStatOutputTypeDef,
     TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
+    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     RollbackDetailsTypeDef,
     LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
     MetricDataQueryOutputTypeDef,
     TargetTrackingMetricDataQueryOutputTypeDef,
@@ -577,30 +579,34 @@
     TargetTrackingConfigurationOutputTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
     TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
     DesiredConfigurationOutputTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
     PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
     AutoScalingGroupsTypeTypeDef,
     InstanceRefreshTypeDef,
+    DesiredConfigurationUnionTypeDef,
     StartInstanceRefreshTypeRequestTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     ScalingPolicyTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
     PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestTypeDef:
+def get_value() -> AcceleratorCountRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16/setup.py` & `mypy-boto3-autoscaling-1.28.16.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling",
-    version="1.28.16",
+    version="1.28.16.post1",
     packages=["mypy_boto3_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder"
-        " 7.16.2"
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
-    keywords="boto3 autoscaling type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 autoscaling type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_autoscaling": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

