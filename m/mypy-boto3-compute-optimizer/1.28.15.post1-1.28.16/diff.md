# Comparing `tmp/mypy-boto3-compute-optimizer-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-compute-optimizer-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-compute-optimizer-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:51 2023, max compression
+gzip compressed data, was "mypy-boto3-compute-optimizer-1.28.16.tar", last modified: Tue Aug  1 11:36:31 2023, max compression
```

## Comparing `mypy-boto3-compute-optimizer-1.28.15.post1.tar` & `mypy-boto3-compute-optimizer-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.437087 mypy-boto3-compute-optimizer-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:16.000000 mypy-boto3-compute-optimizer-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-07-29 10:02:51.433087 mypy-boto3-compute-optimizer-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-29 09:41:16.000000 mypy-boto3-compute-optimizer-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.429087 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-29 09:41:16.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-29 09:41:16.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:41:16.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-07-29 09:41:17.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-29 09:41:16.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-07-29 09:41:18.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-07-29 09:41:18.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-29 09:41:17.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-07-29 09:41:17.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:16.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41985 2023-07-29 09:41:19.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41962 2023-07-29 09:41:19.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:16.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.433087 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-07-29 10:02:51.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 10:02:51.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:51.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:02:51.000000 mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:51.437087 mypy-boto3-compute-optimizer-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:41:16.000000 mypy-boto3-compute-optimizer-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:31.932918 mypy-boto3-compute-optimizer-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:48.000000 mypy-boto3-compute-optimizer-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-08-01 11:36:31.932918 mypy-boto3-compute-optimizer-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-08-01 11:13:48.000000 mypy-boto3-compute-optimizer-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:31.932918 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-01 11:13:48.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-01 11:13:48.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 11:13:50.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24700 2023-08-01 11:13:50.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24667 2023-08-01 11:13:50.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-08-01 11:13:50.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-08-01 11:13:50.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-08-01 11:13:50.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-08-01 11:13:50.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:50.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42031 2023-08-01 11:13:51.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42008 2023-08-01 11:13:51.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:48.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:31.932918 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-08-01 11:36:31.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 11:36:31.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:31.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:31.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:31.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:36:31.000000 mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:31.932918 mypy-boto3-compute-optimizer-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 11:13:48.000000 mypy-boto3-compute-optimizer-1.28.16/setup.py
```

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/LICENSE` & `mypy-boto3-compute-optimizer-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/PKG-INFO` & `mypy-boto3-compute-optimizer-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ComputeOptimizer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ComputeOptimizer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 compute-optimizer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 compute-optimizer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-compute-optimizer)](https://pepy.tech/project/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
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
 
 
 def check_value(value: AutoScalingConfigurationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_compute_optimizer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_compute_optimizer.type_defs import (
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
@@ -418,15 +418,15 @@
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
     GetRecommendationErrorTypeDef,
-    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
@@ -452,28 +452,29 @@
     RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
-    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsRequestRequestTypeDef,
     ExportEBSVolumeRecommendationsRequestRequestTypeDef,
     ExportEC2InstanceRecommendationsRequestRequestTypeDef,
     ExportECSServiceRecommendationsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsResponseTypeDef,
     ExportDestinationTypeDef,
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
+    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
     GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
@@ -494,15 +495,15 @@
     GetECSServiceRecommendationsResponseTypeDef,
     GetEC2InstanceRecommendationsResponseTypeDef,
     GetLambdaFunctionRecommendationsResponseTypeDef,
     GetEBSVolumeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountEnrollmentStatusTypeDef:
+def get_value() -> AccountEnrollmentStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/README.md` & `mypy-boto3-compute-optimizer-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-compute-optimizer)](https://pepy.tech/project/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
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
 
 
 def check_value(value: AutoScalingConfigurationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_compute_optimizer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_compute_optimizer.type_defs import (
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
@@ -386,15 +386,15 @@
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
     GetRecommendationErrorTypeDef,
-    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
@@ -420,28 +420,29 @@
     RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
-    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsRequestRequestTypeDef,
     ExportEBSVolumeRecommendationsRequestRequestTypeDef,
     ExportEC2InstanceRecommendationsRequestRequestTypeDef,
     ExportECSServiceRecommendationsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsResponseTypeDef,
     ExportDestinationTypeDef,
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
+    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
     GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
@@ -462,15 +463,15 @@
     GetECSServiceRecommendationsResponseTypeDef,
     GetEC2InstanceRecommendationsResponseTypeDef,
     GetLambdaFunctionRecommendationsResponseTypeDef,
     GetEBSVolumeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountEnrollmentStatusTypeDef:
+def get_value() -> AccountEnrollmentStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/__init__.py` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/__init__.pyi` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/__main__.py` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComputeOptimizer 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ComputeOptimizer 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer\nOther"
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

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/client.py` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_compute_optimizer.client import ComputeOptimizerClient
 
     session = Session()
     client: ComputeOptimizerClient = session.client("compute-optimizer")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     EnhancedInfrastructureMetricsType,
     ExportableAutoScalingGroupFieldType,
     ExportableECSServiceFieldType,
@@ -64,14 +63,15 @@
     GetRecommendationPreferencesResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
     JobFilterTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     ScopeTypeDef,
+    TimestampTypeDef,
     UpdateEnrollmentStatusResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -316,16 +316,16 @@
 
     def get_ec2_recommendation_projected_metrics(
         self,
         *,
         instanceArn: str,
         stat: MetricStatisticType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         recommendationPreferences: RecommendationPreferencesTypeDef = ...
     ) -> GetEC2RecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected utilization metrics of Amazon EC2 instance
         recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_recommendation_projected_metrics)
@@ -334,16 +334,16 @@
 
     def get_ecs_service_recommendation_projected_metrics(
         self,
         *,
         serviceArn: str,
         stat: MetricStatisticType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str]
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef
     ) -> GetECSServiceRecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected metrics of Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendation_projected_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/client/#get_ecs_service_recommendation_projected_metrics)
         """
```

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/client.pyi` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_compute_optimizer.client import ComputeOptimizerClient
 
     session = Session()
     client: ComputeOptimizerClient = session.client("compute-optimizer")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     EnhancedInfrastructureMetricsType,
     ExportableAutoScalingGroupFieldType,
     ExportableECSServiceFieldType,
@@ -64,14 +63,15 @@
     GetRecommendationPreferencesResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
     JobFilterTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     ScopeTypeDef,
+    TimestampTypeDef,
     UpdateEnrollmentStatusResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -298,16 +298,16 @@
         """
     def get_ec2_recommendation_projected_metrics(
         self,
         *,
         instanceArn: str,
         stat: MetricStatisticType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         recommendationPreferences: RecommendationPreferencesTypeDef = ...
     ) -> GetEC2RecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected utilization metrics of Amazon EC2 instance
         recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_recommendation_projected_metrics)
@@ -315,16 +315,16 @@
         """
     def get_ecs_service_recommendation_projected_metrics(
         self,
         *,
         serviceArn: str,
         stat: MetricStatisticType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str]
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef
     ) -> GetECSServiceRecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected metrics of Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendation_projected_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/client/#get_ecs_service_recommendation_projected_metrics)
         """
```

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/literals.py` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/literals.pyi` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/paginator.py` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/paginator.pyi` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/type_defs.py` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_compute_optimizer.type_defs import AccountEnrollmentStatusTypeDef
 
-    data: AccountEnrollmentStatusTypeDef = {...}
+    data: AccountEnrollmentStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -95,15 +95,15 @@
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
     "ExternalMetricStatusTypeDef",
     "GetRecommendationErrorTypeDef",
-    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
@@ -129,28 +129,29 @@
     "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
-    "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "ExportEBSVolumeRecommendationsRequestRequestTypeDef",
     "ExportEC2InstanceRecommendationsRequestRequestTypeDef",
     "ExportECSServiceRecommendationsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     "ExportDestinationTypeDef",
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     "ExportECSServiceRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
+    "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "RecommendedOptionProjectedMetricTypeDef",
     "SummaryTypeDef",
     "ServiceConfigurationTypeDef",
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationOptionTypeDef",
     "ECSServiceRecommendationOptionTypeDef",
@@ -420,25 +421,15 @@
         "identifier": str,
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "serviceArn": str,
-        "stat": MetricStatisticType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 GetEffectiveRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -836,40 +827,14 @@
         "filters": Sequence[FilterTypeDef],
         "accountIds": Sequence[str],
         "recommendationPreferences": RecommendationPreferencesTypeDef,
     },
     total=False,
 )
 
-_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "instanceArn": str,
-        "stat": MetricStatisticType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "recommendationPreferences": RecommendationPreferencesTypeDef,
-    },
-    total=False,
-)
-
-
-class GetEC2RecommendationProjectedMetricsRequestRequestTypeDef(
-    _RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
-    _OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredExportAutoScalingGroupRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
     },
 )
 _OptionalExportAutoScalingGroupRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1070,14 +1035,51 @@
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "instanceArn": str,
+        "stat": MetricStatisticType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "recommendationPreferences": RecommendationPreferencesTypeDef,
+    },
+    total=False,
+)
+
+
+class GetEC2RecommendationProjectedMetricsRequestRequestTypeDef(
+    _RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    _OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+):
+    pass
+
+
+GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "serviceArn": str,
+        "stat": MetricStatisticType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
 RecommendedOptionProjectedMetricTypeDef = TypedDict(
     "RecommendedOptionProjectedMetricTypeDef",
     {
         "recommendedInstanceType": str,
         "rank": int,
         "projectedMetrics": List[ProjectedMetricTypeDef],
     },
```

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer/type_defs.pyi` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_compute_optimizer.type_defs import AccountEnrollmentStatusTypeDef
 
-    data: AccountEnrollmentStatusTypeDef = {...}
+    data: AccountEnrollmentStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -94,15 +94,15 @@
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
     "ExternalMetricStatusTypeDef",
     "GetRecommendationErrorTypeDef",
-    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
@@ -128,28 +128,29 @@
     "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
-    "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "ExportEBSVolumeRecommendationsRequestRequestTypeDef",
     "ExportEC2InstanceRecommendationsRequestRequestTypeDef",
     "ExportECSServiceRecommendationsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     "ExportDestinationTypeDef",
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     "ExportECSServiceRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
+    "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "RecommendedOptionProjectedMetricTypeDef",
     "SummaryTypeDef",
     "ServiceConfigurationTypeDef",
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationOptionTypeDef",
     "ECSServiceRecommendationOptionTypeDef",
@@ -419,25 +420,15 @@
         "identifier": str,
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "serviceArn": str,
-        "stat": MetricStatisticType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 GetEffectiveRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -825,38 +816,14 @@
         "filters": Sequence[FilterTypeDef],
         "accountIds": Sequence[str],
         "recommendationPreferences": RecommendationPreferencesTypeDef,
     },
     total=False,
 )
 
-_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "instanceArn": str,
-        "stat": MetricStatisticType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "recommendationPreferences": RecommendationPreferencesTypeDef,
-    },
-    total=False,
-)
-
-class GetEC2RecommendationProjectedMetricsRequestRequestTypeDef(
-    _RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
-    _OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
-):
-    pass
-
 _RequiredExportAutoScalingGroupRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
     },
 )
 _OptionalExportAutoScalingGroupRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1047,14 +1014,49 @@
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "instanceArn": str,
+        "stat": MetricStatisticType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "recommendationPreferences": RecommendationPreferencesTypeDef,
+    },
+    total=False,
+)
+
+class GetEC2RecommendationProjectedMetricsRequestRequestTypeDef(
+    _RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    _OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+):
+    pass
+
+GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "serviceArn": str,
+        "stat": MetricStatisticType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
 RecommendedOptionProjectedMetricTypeDef = TypedDict(
     "RecommendedOptionProjectedMetricTypeDef",
     {
         "recommendedInstanceType": str,
         "rank": int,
         "projectedMetrics": List[ProjectedMetricTypeDef],
     },
```

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer.egg-info/PKG-INFO` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ComputeOptimizer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ComputeOptimizer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 compute-optimizer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 compute-optimizer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-compute-optimizer)](https://pepy.tech/project/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
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
 
 
 def check_value(value: AutoScalingConfigurationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_compute_optimizer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_compute_optimizer.type_defs import (
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
@@ -418,15 +418,15 @@
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
     GetRecommendationErrorTypeDef,
-    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
@@ -452,28 +452,29 @@
     RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
-    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsRequestRequestTypeDef,
     ExportEBSVolumeRecommendationsRequestRequestTypeDef,
     ExportEC2InstanceRecommendationsRequestRequestTypeDef,
     ExportECSServiceRecommendationsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsResponseTypeDef,
     ExportDestinationTypeDef,
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
+    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
     GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
@@ -494,15 +495,15 @@
     GetECSServiceRecommendationsResponseTypeDef,
     GetEC2InstanceRecommendationsResponseTypeDef,
     GetLambdaFunctionRecommendationsResponseTypeDef,
     GetEBSVolumeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountEnrollmentStatusTypeDef:
+def get_value() -> AccountEnrollmentStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt` & `mypy-boto3-compute-optimizer-1.28.16/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.15.post1/setup.py` & `mypy-boto3-compute-optimizer-1.28.16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-compute-optimizer",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_compute_optimizer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComputeOptimizer 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ComputeOptimizer 1.28.16 service generated with"
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
-    keywords="boto3 compute-optimizer type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 compute-optimizer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_compute_optimizer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

