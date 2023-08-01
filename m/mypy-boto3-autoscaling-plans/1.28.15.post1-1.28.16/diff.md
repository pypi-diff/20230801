# Comparing `tmp/mypy-boto3-autoscaling-plans-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-autoscaling-plans-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-plans-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-plans-1.28.16.tar", last modified: Tue Aug  1 11:36:15 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1.tar` & `mypy-boto3-autoscaling-plans-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.605022 mypy-boto3-autoscaling-plans-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-29 10:02:34.601022 mypy-boto3-autoscaling-plans-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.593021 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-29 09:38:53.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-07-29 09:38:52.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-07-29 09:38:53.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-07-29 09:38:53.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.601022 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.605022 mypy-boto3-autoscaling-plans-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.360945 mypy-boto3-autoscaling-plans-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-08-01 11:36:15.356945 mypy-boto3-autoscaling-plans-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.356945 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-08-01 11:11:26.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-08-01 11:11:26.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.356945 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:15.360945 mypy-boto3-autoscaling-plans-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-plans-1.28.16/setup.py
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/LICENSE` & `mypy-boto3-autoscaling-plans-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AutoScalingPlans 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 autoscaling-plans type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 autoscaling-plans type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling-plans)](https://pepy.tech/project/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
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
@@ -332,60 +332,63 @@
 )
 
 
 def check_value(value: DescribeScalingPlanResourcesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
     TagFilterOutputTypeDef,
     TagFilterTypeDef,
     ResponseMetadataTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
-    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    TimestampTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
     ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
     CreateScalingPlanResponseTypeDef,
     CustomizedLoadMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
     CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
     DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
-    DescribeScalingPlansRequestRequestTypeDef,
+    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    ApplicationSourceUnionTypeDef,
     TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
+    DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
+    DescribeScalingPlansRequestRequestTypeDef,
     ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
     ScalingInstructionTypeDef,
     ScalingPlanTypeDef,
     ScalingPlanResourceTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
+    ScalingInstructionUnionTypeDef,
     DescribeScalingPlansResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
+    CreateScalingPlanRequestRequestTypeDef,
+    UpdateScalingPlanRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagFilterOutputTypeDef:
+def get_value() -> TagFilterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/README.md` & `mypy-boto3-autoscaling-plans-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling-plans)](https://pepy.tech/project/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
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
@@ -300,60 +300,63 @@
 )
 
 
 def check_value(value: DescribeScalingPlanResourcesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
     TagFilterOutputTypeDef,
     TagFilterTypeDef,
     ResponseMetadataTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
-    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    TimestampTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
     ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
     CreateScalingPlanResponseTypeDef,
     CustomizedLoadMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
     CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
     DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
-    DescribeScalingPlansRequestRequestTypeDef,
+    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    ApplicationSourceUnionTypeDef,
     TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
+    DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
+    DescribeScalingPlansRequestRequestTypeDef,
     ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
     ScalingInstructionTypeDef,
     ScalingPlanTypeDef,
     ScalingPlanResourceTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
+    ScalingInstructionUnionTypeDef,
     DescribeScalingPlansResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
+    CreateScalingPlanRequestRequestTypeDef,
+    UpdateScalingPlanRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagFilterOutputTypeDef:
+def get_value() -> TagFilterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__init__.py` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__init__.pyi` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__main__.py` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScalingPlans 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AutoScalingPlans 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans\nOther"
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

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/client.py` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,28 @@
     from mypy_boto3_autoscaling_plans.client import AutoScalingPlansClient
 
     session = Session()
     client: AutoScalingPlansClient = session.client("autoscaling-plans")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ForecastDataTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import DescribeScalingPlanResourcesPaginator, DescribeScalingPlansPaginator
 from .type_defs import (
-    ApplicationSourceOutputTypeDef,
-    ApplicationSourceTypeDef,
+    ApplicationSourceUnionTypeDef,
     CreateScalingPlanResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
-    ScalingInstructionOutputTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -92,18 +90,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#close)
         """
 
     def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
-        ApplicationSource: Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef],
-        ScalingInstructions: Sequence[
-            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
-        ]
+        ApplicationSource: ApplicationSourceUnionTypeDef,
+        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef]
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -134,17 +130,15 @@
         """
 
     def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[
-            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-        ] = ...,
+        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
@@ -170,33 +164,31 @@
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         ForecastDataType: ForecastDataTypeType,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str]
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef
     ) -> GetScalingPlanResourceForecastDataResponseTypeDef:
         """
         Retrieves the forecast data for a scalable resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.get_scaling_plan_resource_forecast_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#get_scaling_plan_resource_forecast_data)
         """
 
     def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        ApplicationSource: Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef] = ...,
-        ScalingInstructions: Sequence[
-            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
-        ] = ...
+        ApplicationSource: ApplicationSourceUnionTypeDef = ...,
+        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/client.pyi` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -10,30 +10,28 @@
     from mypy_boto3_autoscaling_plans.client import AutoScalingPlansClient
 
     session = Session()
     client: AutoScalingPlansClient = session.client("autoscaling-plans")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ForecastDataTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import DescribeScalingPlanResourcesPaginator, DescribeScalingPlansPaginator
 from .type_defs import (
-    ApplicationSourceOutputTypeDef,
-    ApplicationSourceTypeDef,
+    ApplicationSourceUnionTypeDef,
     CreateScalingPlanResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
-    ScalingInstructionOutputTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -85,18 +83,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#close)
         """
     def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
-        ApplicationSource: Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef],
-        ScalingInstructions: Sequence[
-            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
-        ]
+        ApplicationSource: ApplicationSourceUnionTypeDef,
+        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef]
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -124,17 +120,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#describe_scaling_plan_resources)
         """
     def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[
-            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-        ] = ...,
+        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
@@ -158,32 +152,30 @@
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         ForecastDataType: ForecastDataTypeType,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str]
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef
     ) -> GetScalingPlanResourceForecastDataResponseTypeDef:
         """
         Retrieves the forecast data for a scalable resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.get_scaling_plan_resource_forecast_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#get_scaling_plan_resource_forecast_data)
         """
     def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        ApplicationSource: Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef] = ...,
-        ScalingInstructions: Sequence[
-            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
-        ] = ...
+        ApplicationSource: ApplicationSourceUnionTypeDef = ...,
+        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/literals.py` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/literals.pyi` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/paginator.py` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,20 @@
     session = Session()
     client: AutoScalingPlansClient = session.client("autoscaling-plans")
 
     describe_scaling_plan_resources_paginator: DescribeScalingPlanResourcesPaginator = client.get_paginator("describe_scaling_plan_resources")
     describe_scaling_plans_paginator: DescribeScalingPlansPaginator = client.get_paginator("describe_scaling_plans")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ApplicationSourceOutputTypeDef,
-    ApplicationSourceTypeDef,
+    ApplicationSourceUnionTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeScalingPlanResourcesPaginator", "DescribeScalingPlansPaginator")
 
@@ -72,16 +71,14 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[
-            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-        ] = ...,
+        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/paginator.pyi` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,20 @@
     session = Session()
     client: AutoScalingPlansClient = session.client("autoscaling-plans")
 
     describe_scaling_plan_resources_paginator: DescribeScalingPlanResourcesPaginator = client.get_paginator("describe_scaling_plan_resources")
     describe_scaling_plans_paginator: DescribeScalingPlansPaginator = client.get_paginator("describe_scaling_plans")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ApplicationSourceOutputTypeDef,
-    ApplicationSourceTypeDef,
+    ApplicationSourceUnionTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeScalingPlanResourcesPaginator", "DescribeScalingPlansPaginator")
 
@@ -68,16 +67,14 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[
-            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-        ] = ...,
+        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/type_defs.py` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_autoscaling_plans.type_defs import TagFilterOutputTypeDef
 
-    data: TagFilterOutputTypeDef = {...}
+    data: TagFilterOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -44,39 +44,42 @@
     "TagFilterTypeDef",
     "ResponseMetadataTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
-    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
     "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
     "CreateScalingPlanResponseTypeDef",
     "CustomizedLoadMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
     "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
-    "DescribeScalingPlansRequestRequestTypeDef",
+    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
+    "ApplicationSourceUnionTypeDef",
     "TargetTrackingConfigurationOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
+    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
+    "DescribeScalingPlansRequestRequestTypeDef",
     "ScalingInstructionOutputTypeDef",
     "ScalingPolicyTypeDef",
     "ScalingInstructionTypeDef",
     "ScalingPlanTypeDef",
     "ScalingPlanResourceTypeDef",
-    "CreateScalingPlanRequestRequestTypeDef",
-    "UpdateScalingPlanRequestRequestTypeDef",
+    "ScalingInstructionUnionTypeDef",
     "DescribeScalingPlansResponseTypeDef",
     "DescribeScalingPlanResourcesResponseTypeDef",
+    "CreateScalingPlanRequestRequestTypeDef",
+    "UpdateScalingPlanRequestRequestTypeDef",
 )
 
 TagFilterOutputTypeDef = TypedDict(
     "TagFilterOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
@@ -159,28 +162,15 @@
 class DescribeScalingPlanResourcesRequestRequestTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
-    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-        "ServiceNamespace": ServiceNamespaceType,
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "ForecastDataType": ForecastDataTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
@@ -374,41 +364,29 @@
 class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
 ):
     pass
 
 
-DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
-    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
-    {
-        "ScalingPlanNames": Sequence[str],
-        "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[
-            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-        ],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeScalingPlansRequestRequestTypeDef = TypedDict(
-    "DescribeScalingPlansRequestRequestTypeDef",
+GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
+    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     {
-        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[
-            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-        ],
-        "MaxResults": int,
-        "NextToken": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "ForecastDataType": ForecastDataTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
-    total=False,
 )
 
+ApplicationSourceUnionTypeDef = Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
 _RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationOutputTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
@@ -454,14 +432,37 @@
 
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
 
+DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
+    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
+    {
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScalingPlansRequestRequestTypeDef = TypedDict(
+    "DescribeScalingPlansRequestRequestTypeDef",
+    {
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 _RequiredScalingInstructionOutputTypeDef = TypedDict(
     "_RequiredScalingInstructionOutputTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
@@ -592,60 +593,56 @@
 
 class ScalingPlanResourceTypeDef(
     _RequiredScalingPlanResourceTypeDef, _OptionalScalingPlanResourceTypeDef
 ):
     pass
 
 
+ScalingInstructionUnionTypeDef = Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+DescribeScalingPlansResponseTypeDef = TypedDict(
+    "DescribeScalingPlansResponseTypeDef",
+    {
+        "ScalingPlans": List[ScalingPlanTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
+    "DescribeScalingPlanResourcesResponseTypeDef",
+    {
+        "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateScalingPlanRequestRequestTypeDef = TypedDict(
     "CreateScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[
-            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
-        ],
+        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
     },
 )
 
 _RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 _OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateScalingPlanRequestRequestTypeDef",
     {
         "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[
-            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
-        ],
+        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
     },
     total=False,
 )
 
 
 class UpdateScalingPlanRequestRequestTypeDef(
     _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
 ):
     pass
-
-
-DescribeScalingPlansResponseTypeDef = TypedDict(
-    "DescribeScalingPlansResponseTypeDef",
-    {
-        "ScalingPlans": List[ScalingPlanTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
-    "DescribeScalingPlanResourcesResponseTypeDef",
-    {
-        "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/type_defs.pyi` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_autoscaling_plans.type_defs import TagFilterOutputTypeDef
 
-    data: TagFilterOutputTypeDef = {...}
+    data: TagFilterOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -43,39 +43,42 @@
     "TagFilterTypeDef",
     "ResponseMetadataTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
-    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
     "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
     "CreateScalingPlanResponseTypeDef",
     "CustomizedLoadMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
     "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
-    "DescribeScalingPlansRequestRequestTypeDef",
+    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
+    "ApplicationSourceUnionTypeDef",
     "TargetTrackingConfigurationOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
+    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
+    "DescribeScalingPlansRequestRequestTypeDef",
     "ScalingInstructionOutputTypeDef",
     "ScalingPolicyTypeDef",
     "ScalingInstructionTypeDef",
     "ScalingPlanTypeDef",
     "ScalingPlanResourceTypeDef",
-    "CreateScalingPlanRequestRequestTypeDef",
-    "UpdateScalingPlanRequestRequestTypeDef",
+    "ScalingInstructionUnionTypeDef",
     "DescribeScalingPlansResponseTypeDef",
     "DescribeScalingPlanResourcesResponseTypeDef",
+    "CreateScalingPlanRequestRequestTypeDef",
+    "UpdateScalingPlanRequestRequestTypeDef",
 )
 
 TagFilterOutputTypeDef = TypedDict(
     "TagFilterOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
@@ -156,28 +159,15 @@
 
 class DescribeScalingPlanResourcesRequestRequestTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestRequestTypeDef,
 ):
     pass
 
-GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
-    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-        "ServiceNamespace": ServiceNamespaceType,
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "ForecastDataType": ForecastDataTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
@@ -357,41 +347,29 @@
 
 class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
 ):
     pass
 
-DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
-    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
-    {
-        "ScalingPlanNames": Sequence[str],
-        "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[
-            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-        ],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeScalingPlansRequestRequestTypeDef = TypedDict(
-    "DescribeScalingPlansRequestRequestTypeDef",
+GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
+    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     {
-        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[
-            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-        ],
-        "MaxResults": int,
-        "NextToken": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "ForecastDataType": ForecastDataTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
-    total=False,
 )
 
+ApplicationSourceUnionTypeDef = Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
 _RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationOutputTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
@@ -433,14 +411,37 @@
 )
 
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
+DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
+    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
+    {
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScalingPlansRequestRequestTypeDef = TypedDict(
+    "DescribeScalingPlansRequestRequestTypeDef",
+    {
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 _RequiredScalingInstructionOutputTypeDef = TypedDict(
     "_RequiredScalingInstructionOutputTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
@@ -561,58 +562,55 @@
 )
 
 class ScalingPlanResourceTypeDef(
     _RequiredScalingPlanResourceTypeDef, _OptionalScalingPlanResourceTypeDef
 ):
     pass
 
+ScalingInstructionUnionTypeDef = Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+DescribeScalingPlansResponseTypeDef = TypedDict(
+    "DescribeScalingPlansResponseTypeDef",
+    {
+        "ScalingPlans": List[ScalingPlanTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
+    "DescribeScalingPlanResourcesResponseTypeDef",
+    {
+        "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateScalingPlanRequestRequestTypeDef = TypedDict(
     "CreateScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[
-            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
-        ],
+        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
     },
 )
 
 _RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 _OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateScalingPlanRequestRequestTypeDef",
     {
         "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[
-            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
-        ],
+        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
     },
     total=False,
 )
 
 class UpdateScalingPlanRequestRequestTypeDef(
     _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
 ):
     pass
-
-DescribeScalingPlansResponseTypeDef = TypedDict(
-    "DescribeScalingPlansResponseTypeDef",
-    {
-        "ScalingPlans": List[ScalingPlanTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
-    "DescribeScalingPlanResourcesResponseTypeDef",
-    {
-        "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AutoScalingPlans 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 autoscaling-plans type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 autoscaling-plans type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling-plans)](https://pepy.tech/project/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
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
@@ -332,60 +332,63 @@
 )
 
 
 def check_value(value: DescribeScalingPlanResourcesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
     TagFilterOutputTypeDef,
     TagFilterTypeDef,
     ResponseMetadataTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
-    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    TimestampTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
     ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
     CreateScalingPlanResponseTypeDef,
     CustomizedLoadMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
     CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
     DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
-    DescribeScalingPlansRequestRequestTypeDef,
+    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    ApplicationSourceUnionTypeDef,
     TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
+    DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
+    DescribeScalingPlansRequestRequestTypeDef,
     ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
     ScalingInstructionTypeDef,
     ScalingPlanTypeDef,
     ScalingPlanResourceTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
+    ScalingInstructionUnionTypeDef,
     DescribeScalingPlansResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
+    CreateScalingPlanRequestRequestTypeDef,
+    UpdateScalingPlanRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagFilterOutputTypeDef:
+def get_value() -> TagFilterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-plans-1.28.16/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15.post1/setup.py` & `mypy-boto3-autoscaling-plans-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling-plans",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_autoscaling_plans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.AutoScalingPlans 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 autoscaling-plans type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 autoscaling-plans type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_autoscaling_plans": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

