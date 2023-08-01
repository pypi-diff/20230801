# Comparing `tmp/mypy-boto3-application-autoscaling-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-application-autoscaling-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-autoscaling-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:31 2023, max compression
+gzip compressed data, was "mypy-boto3-application-autoscaling-1.28.16.tar", last modified: Tue Aug  1 11:36:11 2023, max compression
```

## Comparing `mypy-boto3-application-autoscaling-1.28.15.post1.tar` & `mypy-boto3-application-autoscaling-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.025007 mypy-boto3-application-autoscaling-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-29 10:02:31.021007 mypy-boto3-application-autoscaling-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.021007 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26057 2023-07-29 09:38:15.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26008 2023-07-29 09:38:15.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.021007 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:31.025007 mypy-boto3-application-autoscaling-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.884950 mypy-boto3-application-autoscaling-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-08-01 11:36:11.884950 mypy-boto3-application-autoscaling-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.872950 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26538 2023-08-01 11:10:46.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26489 2023-08-01 11:10:46.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.884950 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-08-01 11:36:11.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 11:36:11.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:11.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 11:36:11.000000 mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:11.884950 mypy-boto3-application-autoscaling-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-01 11:10:45.000000 mypy-boto3-application-autoscaling-1.28.16/setup.py
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/LICENSE` & `mypy-boto3-application-autoscaling-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/PKG-INFO` & `mypy-boto3-application-autoscaling-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 application-autoscaling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 application-autoscaling type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-autoscaling)](https://pepy.tech/project/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
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
@@ -338,20 +338,20 @@
 )
 
 
 def check_value(value: AdjustmentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_application_autoscaling.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_application_autoscaling.type_defs import (
     AlarmTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
@@ -362,53 +362,56 @@
     DescribeScalingActivitiesRequestRequestTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotScaledReasonTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
+    TimestampTypeDef,
     SuspendedStateTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
     DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
-    PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
+    PutScheduledActionRequestRequestTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricOutputTypeDef,
     TargetTrackingMetricTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     DescribeScalableTargetsResponseTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
     TargetTrackingMetricStatOutputTypeDef,
     TargetTrackingMetricStatTypeDef,
     TargetTrackingMetricDataQueryOutputTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
     CustomizedMetricSpecificationOutputTypeDef,
     CustomizedMetricSpecificationTypeDef,
     TargetTrackingScalingPolicyConfigurationOutputTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
     ScalingPolicyTypeDef,
     PutScalingPolicyRequestRequestTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
 )
 
 
-def get_structure() -> AlarmTypeDef:
+def get_value() -> AlarmTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/README.md` & `mypy-boto3-application-autoscaling-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-autoscaling)](https://pepy.tech/project/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
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
@@ -306,20 +306,20 @@
 )
 
 
 def check_value(value: AdjustmentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_application_autoscaling.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_application_autoscaling.type_defs import (
     AlarmTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
@@ -330,53 +330,56 @@
     DescribeScalingActivitiesRequestRequestTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotScaledReasonTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
+    TimestampTypeDef,
     SuspendedStateTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
     DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
-    PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
+    PutScheduledActionRequestRequestTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricOutputTypeDef,
     TargetTrackingMetricTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     DescribeScalableTargetsResponseTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
     TargetTrackingMetricStatOutputTypeDef,
     TargetTrackingMetricStatTypeDef,
     TargetTrackingMetricDataQueryOutputTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
     CustomizedMetricSpecificationOutputTypeDef,
     CustomizedMetricSpecificationTypeDef,
     TargetTrackingScalingPolicyConfigurationOutputTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
     ScalingPolicyTypeDef,
     PutScalingPolicyRequestRequestTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
 )
 
 
-def get_structure() -> AlarmTypeDef:
+def get_value() -> AlarmTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__init__.py` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__init__.pyi` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__main__.py` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationAutoScaling 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ApplicationAutoScaling 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
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

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/client.py` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_application_autoscaling.client import ApplicationAutoScalingClient
 
     session = Session()
     client: ApplicationAutoScalingClient = session.client("application-autoscaling")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PolicyTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import (
     DescribeScalableTargetsPaginator,
     DescribeScalingActivitiesPaginator,
@@ -31,51 +30,46 @@
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
-    StepScalingPolicyConfigurationOutputTypeDef,
-    StepScalingPolicyConfigurationTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
     SuspendedStateTypeDef,
-    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
-    TargetTrackingScalingPolicyConfigurationTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ApplicationAutoScalingClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConcurrentUpdateException: Type[BotocoreClientError]
     FailedResourceAccessException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ObjectNotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class ApplicationAutoScalingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/)
     """
 
     meta: ClientMeta
@@ -84,31 +78,28 @@
     def exceptions(self) -> Exceptions:
         """
         ApplicationAutoScalingClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#close)
         """
-
     def delete_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
@@ -116,15 +107,14 @@
         """
         Deletes the specified scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#delete_scaling_policy)
         """
-
     def delete_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
@@ -132,30 +122,28 @@
         """
         Deletes the specified scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#delete_scheduled_action)
         """
-
     def deregister_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
     ) -> Dict[str, Any]:
         """
         Deregisters an Application Auto Scaling scalable target when you have finished
         using it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.deregister_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#deregister_scalable_target)
         """
-
     def describe_scalable_targets(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
@@ -163,15 +151,14 @@
     ) -> DescribeScalableTargetsResponseTypeDef:
         """
         Gets information about the scalable targets in the specified namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scalable_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scalable_targets)
         """
-
     def describe_scaling_activities(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
@@ -181,15 +168,14 @@
         """
         Provides descriptive information about the scaling activities in the specified
         namespace from the previous six weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_activities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scaling_activities)
         """
-
     def describe_scaling_policies(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
@@ -199,15 +185,14 @@
         """
         Describes the Application Auto Scaling scaling policies for the specified
         service namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scaling_policies)
         """
-
     def describe_scheduled_actions(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
@@ -217,82 +202,72 @@
         """
         Describes the Application Auto Scaling scheduled actions for the specified
         service namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scheduled_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scheduled_actions)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#generate_presigned_url)
         """
-
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns all the tags on the specified Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#list_tags_for_resource)
         """
-
     def put_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
-        StepScalingPolicyConfiguration: Union[
-            StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
-        ] = ...,
-        TargetTrackingScalingPolicyConfiguration: Union[
-            TargetTrackingScalingPolicyConfigurationTypeDef,
-            TargetTrackingScalingPolicyConfigurationOutputTypeDef,
-        ] = ...
+        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationUnionTypeDef = ...,
+        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationUnionTypeDef = ...
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#put_scaling_policy)
         """
-
     def put_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         Schedule: str = ...,
         Timezone: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         ScalableTargetAction: ScalableTargetActionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#put_scheduled_action)
         """
-
     def register_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         MinCapacity: int = ...,
@@ -304,58 +279,52 @@
         """
         Registers or updates a scalable target, which is the resource that you want to
         scale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.register_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#register_scalable_target)
         """
-
     def tag_resource(self, *, ResourceARN: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds or edits tags on an Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes tags from an Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#untag_resource)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scalable_targets"]
     ) -> DescribeScalableTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_activities"]
     ) -> DescribeScalingActivitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_policies"]
     ) -> DescribeScalingPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scheduled_actions"]
     ) -> DescribeScheduledActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/client.pyi` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_application_autoscaling.client import ApplicationAutoScalingClient
 
     session = Session()
     client: ApplicationAutoScalingClient = session.client("application-autoscaling")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PolicyTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import (
     DescribeScalableTargetsPaginator,
     DescribeScalingActivitiesPaginator,
@@ -31,47 +30,50 @@
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
-    StepScalingPolicyConfigurationOutputTypeDef,
-    StepScalingPolicyConfigurationTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
     SuspendedStateTypeDef,
-    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
-    TargetTrackingScalingPolicyConfigurationTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ApplicationAutoScalingClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConcurrentUpdateException: Type[BotocoreClientError]
     FailedResourceAccessException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ObjectNotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class ApplicationAutoScalingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/)
     """
 
     meta: ClientMeta
@@ -80,28 +82,31 @@
     def exceptions(self) -> Exceptions:
         """
         ApplicationAutoScalingClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#close)
         """
+
     def delete_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
@@ -109,14 +114,15 @@
         """
         Deletes the specified scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#delete_scaling_policy)
         """
+
     def delete_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
@@ -124,28 +130,30 @@
         """
         Deletes the specified scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#delete_scheduled_action)
         """
+
     def deregister_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
     ) -> Dict[str, Any]:
         """
         Deregisters an Application Auto Scaling scalable target when you have finished
         using it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.deregister_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#deregister_scalable_target)
         """
+
     def describe_scalable_targets(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
@@ -153,14 +161,15 @@
     ) -> DescribeScalableTargetsResponseTypeDef:
         """
         Gets information about the scalable targets in the specified namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scalable_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scalable_targets)
         """
+
     def describe_scaling_activities(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
@@ -170,14 +179,15 @@
         """
         Provides descriptive information about the scaling activities in the specified
         namespace from the previous six weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_activities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scaling_activities)
         """
+
     def describe_scaling_policies(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
@@ -187,14 +197,15 @@
         """
         Describes the Application Auto Scaling scaling policies for the specified
         service namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scaling_policies)
         """
+
     def describe_scheduled_actions(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
@@ -204,77 +215,77 @@
         """
         Describes the Application Auto Scaling scheduled actions for the specified
         service namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scheduled_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scheduled_actions)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#generate_presigned_url)
         """
+
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns all the tags on the specified Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#list_tags_for_resource)
         """
+
     def put_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
-        StepScalingPolicyConfiguration: Union[
-            StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
-        ] = ...,
-        TargetTrackingScalingPolicyConfiguration: Union[
-            TargetTrackingScalingPolicyConfigurationTypeDef,
-            TargetTrackingScalingPolicyConfigurationOutputTypeDef,
-        ] = ...
+        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationUnionTypeDef = ...,
+        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationUnionTypeDef = ...
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#put_scaling_policy)
         """
+
     def put_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         Schedule: str = ...,
         Timezone: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         ScalableTargetAction: ScalableTargetActionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#put_scheduled_action)
         """
+
     def register_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         MinCapacity: int = ...,
@@ -286,52 +297,58 @@
         """
         Registers or updates a scalable target, which is the resource that you want to
         scale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.register_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#register_scalable_target)
         """
+
     def tag_resource(self, *, ResourceARN: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds or edits tags on an Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes tags from an Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#untag_resource)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scalable_targets"]
     ) -> DescribeScalableTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_activities"]
     ) -> DescribeScalingActivitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_policies"]
     ) -> DescribeScalingPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scheduled_actions"]
     ) -> DescribeScheduledActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/literals.py` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/literals.pyi` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/paginator.py` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/paginator.pyi` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/type_defs.py` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_application_autoscaling.type_defs import AlarmTypeDef
 
-    data: AlarmTypeDef = {...}
+    data: AlarmTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -44,48 +44,51 @@
     "DescribeScalingActivitiesRequestRequestTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotScaledReasonTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
+    "TimestampTypeDef",
     "SuspendedStateTypeDef",
     "StepAdjustmentTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
     "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
-    "PutScheduledActionRequestRequestTypeDef",
     "ScheduledActionTypeDef",
+    "PutScheduledActionRequestRequestTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
     "StepScalingPolicyConfigurationOutputTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
     "TargetTrackingMetricOutputTypeDef",
     "TargetTrackingMetricTypeDef",
     "DescribeScalingActivitiesResponseTypeDef",
     "DescribeScheduledActionsResponseTypeDef",
     "DescribeScalableTargetsResponseTypeDef",
+    "StepScalingPolicyConfigurationUnionTypeDef",
     "TargetTrackingMetricStatOutputTypeDef",
     "TargetTrackingMetricStatTypeDef",
     "TargetTrackingMetricDataQueryOutputTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
     "CustomizedMetricSpecificationOutputTypeDef",
     "CustomizedMetricSpecificationTypeDef",
     "TargetTrackingScalingPolicyConfigurationOutputTypeDef",
     "TargetTrackingScalingPolicyConfigurationTypeDef",
     "ScalingPolicyTypeDef",
     "PutScalingPolicyRequestRequestTypeDef",
+    "TargetTrackingScalingPolicyConfigurationUnionTypeDef",
     "DescribeScalingPoliciesResponseTypeDef",
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
@@ -308,14 +311,15 @@
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 SuspendedStateTypeDef = TypedDict(
     "SuspendedStateTypeDef",
     {
         "DynamicScalingInSuspended": bool,
         "DynamicScalingOutSuspended": bool,
         "ScheduledScalingSuspended": bool,
     },
@@ -515,68 +519,68 @@
 )
 
 
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
 
-_RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutScheduledActionRequestRequestTypeDef",
+_RequiredScheduledActionTypeDef = TypedDict(
+    "_RequiredScheduledActionTypeDef",
     {
-        "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
+        "ScheduledActionARN": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "Schedule": str,
         "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
+        "CreationTime": datetime,
     },
 )
-_OptionalPutScheduledActionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutScheduledActionRequestRequestTypeDef",
+_OptionalScheduledActionTypeDef = TypedDict(
+    "_OptionalScheduledActionTypeDef",
     {
-        "Schedule": str,
         "Timezone": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "ScalableDimension": ScalableDimensionType,
+        "StartTime": datetime,
+        "EndTime": datetime,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
 
-class PutScheduledActionRequestRequestTypeDef(
-    _RequiredPutScheduledActionRequestRequestTypeDef,
-    _OptionalPutScheduledActionRequestRequestTypeDef,
-):
+class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
     pass
 
 
-_RequiredScheduledActionTypeDef = TypedDict(
-    "_RequiredScheduledActionTypeDef",
+_RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
-        "ScheduledActionName": str,
-        "ScheduledActionARN": str,
         "ServiceNamespace": ServiceNamespaceType,
-        "Schedule": str,
+        "ScheduledActionName": str,
         "ResourceId": str,
-        "CreationTime": datetime,
+        "ScalableDimension": ScalableDimensionType,
     },
 )
-_OptionalScheduledActionTypeDef = TypedDict(
-    "_OptionalScheduledActionTypeDef",
+_OptionalPutScheduledActionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutScheduledActionRequestRequestTypeDef",
     {
+        "Schedule": str,
         "Timezone": str,
-        "ScalableDimension": ScalableDimensionType,
-        "StartTime": datetime,
-        "EndTime": datetime,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
 
-class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
+class PutScheduledActionRequestRequestTypeDef(
+    _RequiredPutScheduledActionRequestRequestTypeDef,
+    _OptionalPutScheduledActionRequestRequestTypeDef,
+):
     pass
 
 
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
@@ -697,14 +701,17 @@
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StepScalingPolicyConfigurationUnionTypeDef = Union[
+    StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
+]
 _RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatOutputTypeDef",
     {
         "Metric": TargetTrackingMetricOutputTypeDef,
         "Stat": str,
     },
 )
@@ -923,14 +930,18 @@
 
 class PutScalingPolicyRequestRequestTypeDef(
     _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
 ):
     pass
 
 
+TargetTrackingScalingPolicyConfigurationUnionTypeDef = Union[
+    TargetTrackingScalingPolicyConfigurationTypeDef,
+    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
+]
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/type_defs.pyi` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_application_autoscaling.type_defs import AlarmTypeDef
 
-    data: AlarmTypeDef = {...}
+    data: AlarmTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -43,48 +43,51 @@
     "DescribeScalingActivitiesRequestRequestTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotScaledReasonTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
+    "TimestampTypeDef",
     "SuspendedStateTypeDef",
     "StepAdjustmentTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
     "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
-    "PutScheduledActionRequestRequestTypeDef",
     "ScheduledActionTypeDef",
+    "PutScheduledActionRequestRequestTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
     "StepScalingPolicyConfigurationOutputTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
     "TargetTrackingMetricOutputTypeDef",
     "TargetTrackingMetricTypeDef",
     "DescribeScalingActivitiesResponseTypeDef",
     "DescribeScheduledActionsResponseTypeDef",
     "DescribeScalableTargetsResponseTypeDef",
+    "StepScalingPolicyConfigurationUnionTypeDef",
     "TargetTrackingMetricStatOutputTypeDef",
     "TargetTrackingMetricStatTypeDef",
     "TargetTrackingMetricDataQueryOutputTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
     "CustomizedMetricSpecificationOutputTypeDef",
     "CustomizedMetricSpecificationTypeDef",
     "TargetTrackingScalingPolicyConfigurationOutputTypeDef",
     "TargetTrackingScalingPolicyConfigurationTypeDef",
     "ScalingPolicyTypeDef",
     "PutScalingPolicyRequestRequestTypeDef",
+    "TargetTrackingScalingPolicyConfigurationUnionTypeDef",
     "DescribeScalingPoliciesResponseTypeDef",
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
@@ -295,14 +298,15 @@
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 SuspendedStateTypeDef = TypedDict(
     "SuspendedStateTypeDef",
     {
         "DynamicScalingInSuspended": bool,
         "DynamicScalingOutSuspended": bool,
         "ScheduledScalingSuspended": bool,
     },
@@ -490,65 +494,65 @@
     },
     total=False,
 )
 
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
-_RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutScheduledActionRequestRequestTypeDef",
+_RequiredScheduledActionTypeDef = TypedDict(
+    "_RequiredScheduledActionTypeDef",
     {
-        "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
+        "ScheduledActionARN": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "Schedule": str,
         "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
+        "CreationTime": datetime,
     },
 )
-_OptionalPutScheduledActionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutScheduledActionRequestRequestTypeDef",
+_OptionalScheduledActionTypeDef = TypedDict(
+    "_OptionalScheduledActionTypeDef",
     {
-        "Schedule": str,
         "Timezone": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "ScalableDimension": ScalableDimensionType,
+        "StartTime": datetime,
+        "EndTime": datetime,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
-class PutScheduledActionRequestRequestTypeDef(
-    _RequiredPutScheduledActionRequestRequestTypeDef,
-    _OptionalPutScheduledActionRequestRequestTypeDef,
-):
+class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
     pass
 
-_RequiredScheduledActionTypeDef = TypedDict(
-    "_RequiredScheduledActionTypeDef",
+_RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
-        "ScheduledActionName": str,
-        "ScheduledActionARN": str,
         "ServiceNamespace": ServiceNamespaceType,
-        "Schedule": str,
+        "ScheduledActionName": str,
         "ResourceId": str,
-        "CreationTime": datetime,
+        "ScalableDimension": ScalableDimensionType,
     },
 )
-_OptionalScheduledActionTypeDef = TypedDict(
-    "_OptionalScheduledActionTypeDef",
+_OptionalPutScheduledActionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutScheduledActionRequestRequestTypeDef",
     {
+        "Schedule": str,
         "Timezone": str,
-        "ScalableDimension": ScalableDimensionType,
-        "StartTime": datetime,
-        "EndTime": datetime,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
-class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
+class PutScheduledActionRequestRequestTypeDef(
+    _RequiredPutScheduledActionRequestRequestTypeDef,
+    _OptionalPutScheduledActionRequestRequestTypeDef,
+):
     pass
 
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -664,14 +668,17 @@
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StepScalingPolicyConfigurationUnionTypeDef = Union[
+    StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
+]
 _RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatOutputTypeDef",
     {
         "Metric": TargetTrackingMetricOutputTypeDef,
         "Stat": str,
     },
 )
@@ -874,14 +881,18 @@
 )
 
 class PutScalingPolicyRequestRequestTypeDef(
     _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
 ):
     pass
 
+TargetTrackingScalingPolicyConfigurationUnionTypeDef = Union[
+    TargetTrackingScalingPolicyConfigurationTypeDef,
+    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
+]
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 application-autoscaling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 application-autoscaling type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-autoscaling)](https://pepy.tech/project/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
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
@@ -338,20 +338,20 @@
 )
 
 
 def check_value(value: AdjustmentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_application_autoscaling.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_application_autoscaling.type_defs import (
     AlarmTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
@@ -362,53 +362,56 @@
     DescribeScalingActivitiesRequestRequestTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotScaledReasonTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
+    TimestampTypeDef,
     SuspendedStateTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
     DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
-    PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
+    PutScheduledActionRequestRequestTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricOutputTypeDef,
     TargetTrackingMetricTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     DescribeScalableTargetsResponseTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
     TargetTrackingMetricStatOutputTypeDef,
     TargetTrackingMetricStatTypeDef,
     TargetTrackingMetricDataQueryOutputTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
     CustomizedMetricSpecificationOutputTypeDef,
     CustomizedMetricSpecificationTypeDef,
     TargetTrackingScalingPolicyConfigurationOutputTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
     ScalingPolicyTypeDef,
     PutScalingPolicyRequestRequestTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
 )
 
 
-def get_structure() -> AlarmTypeDef:
+def get_value() -> AlarmTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-application-autoscaling-1.28.16/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15.post1/setup.py` & `mypy-boto3-application-autoscaling-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-application-autoscaling",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ApplicationAutoScaling 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,17 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords=(
-        "boto3 application-autoscaling type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="boto3 application-autoscaling type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_application_autoscaling": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/"
```

