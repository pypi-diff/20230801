# Comparing `tmp/mypy-boto3-ce-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ce-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ce-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:37 2023, max compression
+gzip compressed data, was "mypy-boto3-ce-1.28.16.tar", last modified: Tue Aug  1 11:36:18 2023, max compression
```

## Comparing `mypy-boto3-ce-1.28.15.post1.tar` & `mypy-boto3-ce-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.969035 mypy-boto3-ce-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-07-29 10:02:37.965036 mypy-boto3-ce-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.961035 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33450 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33405 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68807 2023-07-29 09:39:16.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68734 2023-07-29 09:39:15.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.965036 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:37.969035 mypy-boto3-ce-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.804939 mypy-boto3-ce-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-08-01 11:36:18.804939 mypy-boto3-ce-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17883 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.788939 mypy-boto3-ce-1.28.16/mypy_boto3_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32681 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32636 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-08-01 11:11:47.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-08-01 11:11:47.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69108 2023-08-01 11:11:49.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69035 2023-08-01 11:11:48.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.788939 mypy-boto3-ce-1.28.16/mypy_boto3_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-08-01 11:36:18.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-01 11:36:18.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:18.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 11:36:18.000000 mypy-boto3-ce-1.28.16/mypy_boto3_ce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:18.804939 mypy-boto3-ce-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:11:46.000000 mypy-boto3-ce-1.28.16/setup.py
```

### Comparing `mypy-boto3-ce-1.28.15.post1/LICENSE` & `mypy-boto3-ce-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.15.post1/PKG-INFO` & `mypy-boto3-ce-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CostExplorer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ce type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ce type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -320,20 +320,20 @@
 )
 
 
 def check_value(value: AccountScopeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ce.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
     SubscriberTypeDef,
@@ -366,14 +366,15 @@
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
     TagValuesTypeDef,
+    ExpressionUnionTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     SortDefinitionTypeDef,
     MetricValueTypeDef,
@@ -459,34 +460,36 @@
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
+    AnomalySubscriptionUnionTypeDef,
     CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomaliesResponseTypeDef,
     ListCostCategoryDefinitionsResponseTypeDef,
     CostCategoryTypeDef,
-    CreateCostCategoryDefinitionRequestRequestTypeDef,
-    UpdateCostCategoryDefinitionRequestRequestTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     GetCostForecastResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     ReservationCoverageGroupTypeDef,
     ResourceUtilizationTypeDef,
     GetReservationPurchaseRecommendationRequestRequestTypeDef,
     ResultByTimeTypeDef,
     UtilizationByTimeTypeDef,
     ReservationPurchaseRecommendationDetailTypeDef,
     GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     SavingsPlansPurchaseRecommendationTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
+    CreateCostCategoryDefinitionRequestRequestTypeDef,
+    UpdateCostCategoryDefinitionRequestRequestTypeDef,
     CoverageByTimeTypeDef,
     CurrentInstanceTypeDef,
     TargetInstanceTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     ReservationPurchaseRecommendationTypeDef,
@@ -495,15 +498,15 @@
     ModifyRecommendationDetailTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     RightsizingRecommendationTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
 )
 
 
-def get_structure() -> AnomalyDateIntervalTypeDef:
+def get_value() -> AnomalyDateIntervalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ce-1.28.15.post1/README.md` & `mypy-boto3-ce-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -288,20 +288,20 @@
 )
 
 
 def check_value(value: AccountScopeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ce.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
     SubscriberTypeDef,
@@ -334,14 +334,15 @@
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
     TagValuesTypeDef,
+    ExpressionUnionTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     SortDefinitionTypeDef,
     MetricValueTypeDef,
@@ -427,34 +428,36 @@
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
+    AnomalySubscriptionUnionTypeDef,
     CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomaliesResponseTypeDef,
     ListCostCategoryDefinitionsResponseTypeDef,
     CostCategoryTypeDef,
-    CreateCostCategoryDefinitionRequestRequestTypeDef,
-    UpdateCostCategoryDefinitionRequestRequestTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     GetCostForecastResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     ReservationCoverageGroupTypeDef,
     ResourceUtilizationTypeDef,
     GetReservationPurchaseRecommendationRequestRequestTypeDef,
     ResultByTimeTypeDef,
     UtilizationByTimeTypeDef,
     ReservationPurchaseRecommendationDetailTypeDef,
     GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     SavingsPlansPurchaseRecommendationTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
+    CreateCostCategoryDefinitionRequestRequestTypeDef,
+    UpdateCostCategoryDefinitionRequestRequestTypeDef,
     CoverageByTimeTypeDef,
     CurrentInstanceTypeDef,
     TargetInstanceTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     ReservationPurchaseRecommendationTypeDef,
@@ -463,15 +466,15 @@
     ModifyRecommendationDetailTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     RightsizingRecommendationTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
 )
 
 
-def get_structure() -> AnomalyDateIntervalTypeDef:
+def get_value() -> AnomalyDateIntervalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/__main__.py` & `mypy-boto3-ce-1.28.16/mypy_boto3_ce/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostExplorer 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CostExplorer 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
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

### Comparing `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/client.py` & `mypy-boto3-ce-1.28.16/mypy_boto3_ce/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ce.client import CostExplorerClient
 
     session = Session()
     client: CostExplorerClient = session.client("ce")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
@@ -34,28 +34,25 @@
     SavingsPlansDataTypeType,
     SupportedSavingsPlansTypeType,
     TermInYearsType,
 )
 from .type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
-    AnomalySubscriptionOutputTypeDef,
-    AnomalySubscriptionTypeDef,
+    AnomalySubscriptionUnionTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostCategoryRuleTypeDef,
-    CostCategorySplitChargeRuleOutputTypeDef,
-    CostCategorySplitChargeRuleTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     CreateAnomalyMonitorResponseTypeDef,
     CreateAnomalySubscriptionResponseTypeDef,
     CreateCostCategoryDefinitionResponseTypeDef,
     DateIntervalTypeDef,
     DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
-    ExpressionOutputTypeDef,
-    ExpressionTypeDef,
+    ExpressionUnionTypeDef,
     GetAnomaliesResponseTypeDef,
     GetAnomalyMonitorsResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
@@ -169,15 +166,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_anomaly_monitor)
         """
 
     def create_anomaly_subscription(
         self,
         *,
-        AnomalySubscription: Union[AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef],
+        AnomalySubscription: AnomalySubscriptionUnionTypeDef,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_anomaly_subscription)
@@ -187,17 +184,15 @@
         self,
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[
-            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
-        ] = ...,
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_cost_category_definition)
@@ -303,15 +298,15 @@
 
     def get_cost_and_usage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
@@ -319,15 +314,15 @@
         """
 
     def get_cost_and_usage_with_resources(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"],
+        Filter: ExpressionUnionTypeDef,
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
@@ -337,15 +332,15 @@
 
     def get_cost_categories(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
@@ -355,15 +350,15 @@
 
     def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
@@ -373,15 +368,15 @@
     def get_dimension_values(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
@@ -392,15 +387,15 @@
 
     def get_reservation_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
         MaxResults: int = ...
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
@@ -413,15 +408,15 @@
         """
 
     def get_reservation_purchase_recommendation(
         self,
         *,
         Service: str,
         AccountId: str = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
@@ -435,15 +430,15 @@
 
     def get_reservation_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
@@ -451,15 +446,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_reservation_utilization)
         """
 
     def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
@@ -480,15 +475,15 @@
 
     def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
@@ -503,44 +498,44 @@
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...
+        Filter: ExpressionUnionTypeDef = ...
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_purchase_recommendation)
         """
 
     def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges with
         daily or monthly granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_utilization)
         """
 
     def get_savings_plans_utilization_details(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for a
@@ -552,15 +547,15 @@
 
     def get_tags(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
@@ -570,15 +565,15 @@
 
     def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will use
         over the forecast time period that you select, based on your past usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
@@ -690,15 +685,15 @@
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...
+        ThresholdExpression: ExpressionUnionTypeDef = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_anomaly_subscription)
         """
@@ -717,17 +712,15 @@
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[
-            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
-        ] = ...
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_cost_category_definition)
         """
```

### Comparing `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/client.pyi` & `mypy-boto3-ce-1.28.16/mypy_boto3_ce/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ce.client import CostExplorerClient
 
     session = Session()
     client: CostExplorerClient = session.client("ce")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
@@ -34,28 +34,25 @@
     SavingsPlansDataTypeType,
     SupportedSavingsPlansTypeType,
     TermInYearsType,
 )
 from .type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
-    AnomalySubscriptionOutputTypeDef,
-    AnomalySubscriptionTypeDef,
+    AnomalySubscriptionUnionTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostCategoryRuleTypeDef,
-    CostCategorySplitChargeRuleOutputTypeDef,
-    CostCategorySplitChargeRuleTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     CreateAnomalyMonitorResponseTypeDef,
     CreateAnomalySubscriptionResponseTypeDef,
     CreateCostCategoryDefinitionResponseTypeDef,
     DateIntervalTypeDef,
     DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
-    ExpressionOutputTypeDef,
-    ExpressionTypeDef,
+    ExpressionUnionTypeDef,
     GetAnomaliesResponseTypeDef,
     GetAnomalyMonitorsResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
@@ -161,15 +158,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_anomaly_monitor)
         """
     def create_anomaly_subscription(
         self,
         *,
-        AnomalySubscription: Union[AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef],
+        AnomalySubscription: AnomalySubscriptionUnionTypeDef,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_anomaly_subscription)
@@ -178,17 +175,15 @@
         self,
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[
-            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
-        ] = ...,
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_cost_category_definition)
@@ -285,30 +280,30 @@
         """
     def get_cost_and_usage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_cost_and_usage)
         """
     def get_cost_and_usage_with_resources(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"],
+        Filter: ExpressionUnionTypeDef,
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
@@ -317,15 +312,15 @@
         """
     def get_cost_categories(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
@@ -334,15 +329,15 @@
         """
     def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
@@ -351,15 +346,15 @@
     def get_dimension_values(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
@@ -369,15 +364,15 @@
         """
     def get_reservation_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
         MaxResults: int = ...
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
@@ -389,15 +384,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_reservation_coverage)
         """
     def get_reservation_purchase_recommendation(
         self,
         *,
         Service: str,
         AccountId: str = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
@@ -410,30 +405,30 @@
         """
     def get_reservation_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_utilization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_reservation_utilization)
         """
     def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
@@ -452,15 +447,15 @@
         """
     def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
@@ -474,42 +469,42 @@
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...
+        Filter: ExpressionUnionTypeDef = ...
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_purchase_recommendation)
         """
     def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges with
         daily or monthly granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_utilization)
         """
     def get_savings_plans_utilization_details(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for a
@@ -520,15 +515,15 @@
         """
     def get_tags(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
@@ -537,15 +532,15 @@
         """
     def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will use
         over the forecast time period that you select, based on your past usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
@@ -647,15 +642,15 @@
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...
+        ThresholdExpression: ExpressionUnionTypeDef = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_anomaly_subscription)
         """
@@ -672,17 +667,15 @@
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[
-            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
-        ] = ...
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_cost_category_definition)
         """
```

### Comparing `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/literals.py` & `mypy-boto3-ce-1.28.16/mypy_boto3_ce/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/literals.pyi` & `mypy-boto3-ce-1.28.16/mypy_boto3_ce/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/type_defs.py` & `mypy-boto3-ce-1.28.16/mypy_boto3_ce/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ce.type_defs import AnomalyDateIntervalTypeDef
 
-    data: AnomalyDateIntervalTypeDef = {...}
+    data: AnomalyDateIntervalTypeDef = ...
     ```
 """
 import sys
 from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
     AccountScopeType,
@@ -92,14 +92,15 @@
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
     "TagValuesTypeDef",
+    "ExpressionUnionTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "SortDefinitionTypeDef",
     "MetricValueTypeDef",
@@ -185,34 +186,36 @@
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     "GetAnomalySubscriptionsResponseTypeDef",
+    "AnomalySubscriptionUnionTypeDef",
     "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomaliesResponseTypeDef",
     "ListCostCategoryDefinitionsResponseTypeDef",
     "CostCategoryTypeDef",
-    "CreateCostCategoryDefinitionRequestRequestTypeDef",
-    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
+    "CostCategorySplitChargeRuleUnionTypeDef",
     "GetCostForecastResponseTypeDef",
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
     "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
+    "CreateCostCategoryDefinitionRequestRequestTypeDef",
+    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
     "TargetInstanceTypeDef",
     "GetCostAndUsageResponseTypeDef",
     "GetCostAndUsageWithResourcesResponseTypeDef",
     "GetReservationUtilizationResponseTypeDef",
     "ReservationPurchaseRecommendationTypeDef",
@@ -636,14 +639,15 @@
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
     total=False,
 )
 
+ExpressionUnionTypeDef = Union["ExpressionTypeDef", "ExpressionOutputTypeDef"]
 GenerationSummaryTypeDef = TypedDict(
     "GenerationSummaryTypeDef",
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
@@ -2030,14 +2034,17 @@
     {
         "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AnomalySubscriptionUnionTypeDef = Union[
+    AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef
+]
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
     },
 )
 _OptionalCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
@@ -2096,71 +2103,17 @@
 )
 
 
 class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
     pass
 
 
-_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[
-            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
-        ],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "CostCategoryArn": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[
-            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
+CostCategorySplitChargeRuleUnionTypeDef = Union[
+    CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef
+]
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2329,14 +2282,67 @@
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "CostCategoryArn": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
```

### Comparing `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/type_defs.pyi` & `mypy-boto3-ce-1.28.16/mypy_boto3_ce/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ce.type_defs import AnomalyDateIntervalTypeDef
 
-    data: AnomalyDateIntervalTypeDef = {...}
+    data: AnomalyDateIntervalTypeDef = ...
     ```
 """
 import sys
 from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
     AccountScopeType,
@@ -91,14 +91,15 @@
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
     "TagValuesTypeDef",
+    "ExpressionUnionTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "SortDefinitionTypeDef",
     "MetricValueTypeDef",
@@ -184,34 +185,36 @@
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     "GetAnomalySubscriptionsResponseTypeDef",
+    "AnomalySubscriptionUnionTypeDef",
     "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomaliesResponseTypeDef",
     "ListCostCategoryDefinitionsResponseTypeDef",
     "CostCategoryTypeDef",
-    "CreateCostCategoryDefinitionRequestRequestTypeDef",
-    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
+    "CostCategorySplitChargeRuleUnionTypeDef",
     "GetCostForecastResponseTypeDef",
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
     "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
+    "CreateCostCategoryDefinitionRequestRequestTypeDef",
+    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
     "TargetInstanceTypeDef",
     "GetCostAndUsageResponseTypeDef",
     "GetCostAndUsageWithResourcesResponseTypeDef",
     "GetReservationUtilizationResponseTypeDef",
     "ReservationPurchaseRecommendationTypeDef",
@@ -627,14 +630,15 @@
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
     total=False,
 )
 
+ExpressionUnionTypeDef = Union["ExpressionTypeDef", "ExpressionOutputTypeDef"]
 GenerationSummaryTypeDef = TypedDict(
     "GenerationSummaryTypeDef",
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
@@ -1967,14 +1971,17 @@
     {
         "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AnomalySubscriptionUnionTypeDef = Union[
+    AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef
+]
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
     },
 )
 _OptionalCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
@@ -2029,67 +2036,17 @@
     },
     total=False,
 )
 
 class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
     pass
 
-_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[
-            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
-        ],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-    total=False,
-)
-
-class CreateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "CostCategoryArn": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[
-            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
+CostCategorySplitChargeRuleUnionTypeDef = Union[
+    CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef
+]
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2256,14 +2213,63 @@
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+    total=False,
+)
+
+class CreateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "CostCategoryArn": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
```

### Comparing `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/PKG-INFO` & `mypy-boto3-ce-1.28.16/mypy_boto3_ce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CostExplorer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ce type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ce type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -320,20 +320,20 @@
 )
 
 
 def check_value(value: AccountScopeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ce.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
     SubscriberTypeDef,
@@ -366,14 +366,15 @@
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
     TagValuesTypeDef,
+    ExpressionUnionTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     SortDefinitionTypeDef,
     MetricValueTypeDef,
@@ -459,34 +460,36 @@
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
+    AnomalySubscriptionUnionTypeDef,
     CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomaliesResponseTypeDef,
     ListCostCategoryDefinitionsResponseTypeDef,
     CostCategoryTypeDef,
-    CreateCostCategoryDefinitionRequestRequestTypeDef,
-    UpdateCostCategoryDefinitionRequestRequestTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     GetCostForecastResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     ReservationCoverageGroupTypeDef,
     ResourceUtilizationTypeDef,
     GetReservationPurchaseRecommendationRequestRequestTypeDef,
     ResultByTimeTypeDef,
     UtilizationByTimeTypeDef,
     ReservationPurchaseRecommendationDetailTypeDef,
     GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     SavingsPlansPurchaseRecommendationTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
+    CreateCostCategoryDefinitionRequestRequestTypeDef,
+    UpdateCostCategoryDefinitionRequestRequestTypeDef,
     CoverageByTimeTypeDef,
     CurrentInstanceTypeDef,
     TargetInstanceTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     ReservationPurchaseRecommendationTypeDef,
@@ -495,15 +498,15 @@
     ModifyRecommendationDetailTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     RightsizingRecommendationTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
 )
 
 
-def get_structure() -> AnomalyDateIntervalTypeDef:
+def get_value() -> AnomalyDateIntervalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/SOURCES.txt` & `mypy-boto3-ce-1.28.16/mypy_boto3_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.15.post1/setup.py` & `mypy-boto3-ce-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ce",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CostExplorer 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 ce type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ce type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ce": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

