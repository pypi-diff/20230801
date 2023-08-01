# Comparing `tmp/mypy-boto3-devops-guru-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-devops-guru-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devops-guru-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:55 2023, max compression
+gzip compressed data, was "mypy-boto3-devops-guru-1.28.16.tar", last modified: Tue Aug  1 11:36:36 2023, max compression
```

## Comparing `mypy-boto3-devops-guru-1.28.15.post1.tar` & `mypy-boto3-devops-guru-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.885101 mypy-boto3-devops-guru-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23372 2023-07-29 10:02:55.877101 mypy-boto3-devops-guru-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21864 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.877101 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31416 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31364 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64825 2023-07-29 09:42:22.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64758 2023-07-29 09:42:21.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.877101 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23372 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:55.885101 mypy-boto3-devops-guru-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-29 09:42:18.000000 mypy-boto3-devops-guru-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.988912 mypy-boto3-devops-guru-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23483 2023-08-01 11:36:35.980912 mypy-boto3-devops-guru-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.972912 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-08-01 11:14:53.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-08-01 11:14:53.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65246 2023-08-01 11:14:54.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65179 2023-08-01 11:14:54.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.980912 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23483 2023-08-01 11:36:35.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-01 11:36:35.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:35.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:36:35.000000 mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:35.988912 mypy-boto3-devops-guru-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-01 11:14:52.000000 mypy-boto3-devops-guru-1.28.16/setup.py
```

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/LICENSE` & `mypy-boto3-devops-guru-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/PKG-INFO` & `mypy-boto3-devops-guru-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DevOpsGuru 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 devops-guru type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 devops-guru type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devops-guru)](https://pepy.tech/project/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
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
@@ -397,20 +397,20 @@
 )
 
 
 def check_value(value: AnomalySeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
     ResponseMetadataTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
@@ -425,35 +425,31 @@
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
     TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DescribeAccountOverviewRequestRequestTypeDef,
+    TimestampTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
     InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
-    DescribeOrganizationOverviewRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
-    EndTimeRangeTypeDef,
     EventResourceTypeDef,
-    EventTimeRangeTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
-    StartTimeRangeTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
@@ -486,26 +482,29 @@
     DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
     CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
+    DescribeAccountOverviewRequestRequestTypeDef,
+    DescribeOrganizationOverviewRequestRequestTypeDef,
+    EndTimeRangeTypeDef,
+    EventTimeRangeTypeDef,
+    StartTimeRangeTypeDef,
     DescribeFeedbackResponseTypeDef,
     PutFeedbackRequestRequestTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListRecommendationsRequestListRecommendationsPaginateTypeDef,
-    ListInsightsClosedStatusFilterTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
-    ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
     NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
     ServiceIntegrationConfigTypeDef,
@@ -517,21 +516,24 @@
     ResourceCollectionTypeDef,
     ServiceHealthTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     UpdateEventSourcesConfigRequestRequestTypeDef,
     CloudWatchMetricsDetailTypeDef,
     GetCostEstimationResponseTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     StartCostEstimationRequestRequestTypeDef,
+    ListInsightsClosedStatusFilterTypeDef,
+    ListInsightsAnyStatusFilterTypeDef,
     ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     ListAnomaliesForInsightRequestRequestTypeDef,
-    ListInsightsStatusFilterTypeDef,
     AnomalousLogGroupTypeDef,
     NotificationChannelTypeDef,
     AddNotificationChannelRequestRequestTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     UpdateServiceIntegrationRequestRequestTypeDef,
     DescribeServiceIntegrationResponseTypeDef,
     PerformanceInsightsReferenceMetricTypeDef,
     RecommendationRelatedAnomalyTypeDef,
     GetResourceCollectionResponseTypeDef,
     EventTypeDef,
     MonitoredResourceIdentifierTypeDef,
@@ -543,18 +545,15 @@
     ReactiveOrganizationInsightSummaryTypeDef,
     ListEventsFiltersTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     DescribeOrganizationResourceCollectionHealthResponseTypeDef,
     DescribeResourceCollectionHealthResponseTypeDef,
     UpdateResourceCollectionRequestRequestTypeDef,
-    ListInsightsRequestListInsightsPaginateTypeDef,
-    ListInsightsRequestRequestTypeDef,
-    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    ListOrganizationInsightsRequestRequestTypeDef,
+    ListInsightsStatusFilterTypeDef,
     ListAnomalousLogGroupsResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     PerformanceInsightsReferenceComparisonValuesTypeDef,
     RecommendationTypeDef,
     ListEventsResponseTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListInsightsResponseTypeDef,
@@ -564,28 +563,32 @@
     ListOrganizationInsightsResponseTypeDef,
     ListEventsRequestListEventsPaginateTypeDef,
     ListEventsRequestRequestTypeDef,
     SearchInsightsRequestRequestTypeDef,
     SearchInsightsRequestSearchInsightsPaginateTypeDef,
     SearchOrganizationInsightsRequestRequestTypeDef,
     SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
+    ListInsightsRequestListInsightsPaginateTypeDef,
+    ListInsightsRequestRequestTypeDef,
+    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    ListOrganizationInsightsRequestRequestTypeDef,
     PerformanceInsightsReferenceDataTypeDef,
     ListRecommendationsResponseTypeDef,
     PerformanceInsightsMetricsDetailTypeDef,
     AnomalySourceDetailsTypeDef,
     ProactiveAnomalySummaryTypeDef,
     ProactiveAnomalyTypeDef,
     ReactiveAnomalySummaryTypeDef,
     ReactiveAnomalyTypeDef,
     ListAnomaliesForInsightResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
 )
 
 
-def get_structure() -> AccountInsightHealthTypeDef:
+def get_value() -> AccountInsightHealthTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/README.md` & `mypy-boto3-devops-guru-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devops-guru)](https://pepy.tech/project/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
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
@@ -365,20 +365,20 @@
 )
 
 
 def check_value(value: AnomalySeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
     ResponseMetadataTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
@@ -393,35 +393,31 @@
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
     TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DescribeAccountOverviewRequestRequestTypeDef,
+    TimestampTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
     InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
-    DescribeOrganizationOverviewRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
-    EndTimeRangeTypeDef,
     EventResourceTypeDef,
-    EventTimeRangeTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
-    StartTimeRangeTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
@@ -454,26 +450,29 @@
     DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
     CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
+    DescribeAccountOverviewRequestRequestTypeDef,
+    DescribeOrganizationOverviewRequestRequestTypeDef,
+    EndTimeRangeTypeDef,
+    EventTimeRangeTypeDef,
+    StartTimeRangeTypeDef,
     DescribeFeedbackResponseTypeDef,
     PutFeedbackRequestRequestTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListRecommendationsRequestListRecommendationsPaginateTypeDef,
-    ListInsightsClosedStatusFilterTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
-    ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
     NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
     ServiceIntegrationConfigTypeDef,
@@ -485,21 +484,24 @@
     ResourceCollectionTypeDef,
     ServiceHealthTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     UpdateEventSourcesConfigRequestRequestTypeDef,
     CloudWatchMetricsDetailTypeDef,
     GetCostEstimationResponseTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     StartCostEstimationRequestRequestTypeDef,
+    ListInsightsClosedStatusFilterTypeDef,
+    ListInsightsAnyStatusFilterTypeDef,
     ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     ListAnomaliesForInsightRequestRequestTypeDef,
-    ListInsightsStatusFilterTypeDef,
     AnomalousLogGroupTypeDef,
     NotificationChannelTypeDef,
     AddNotificationChannelRequestRequestTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     UpdateServiceIntegrationRequestRequestTypeDef,
     DescribeServiceIntegrationResponseTypeDef,
     PerformanceInsightsReferenceMetricTypeDef,
     RecommendationRelatedAnomalyTypeDef,
     GetResourceCollectionResponseTypeDef,
     EventTypeDef,
     MonitoredResourceIdentifierTypeDef,
@@ -511,18 +513,15 @@
     ReactiveOrganizationInsightSummaryTypeDef,
     ListEventsFiltersTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     DescribeOrganizationResourceCollectionHealthResponseTypeDef,
     DescribeResourceCollectionHealthResponseTypeDef,
     UpdateResourceCollectionRequestRequestTypeDef,
-    ListInsightsRequestListInsightsPaginateTypeDef,
-    ListInsightsRequestRequestTypeDef,
-    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    ListOrganizationInsightsRequestRequestTypeDef,
+    ListInsightsStatusFilterTypeDef,
     ListAnomalousLogGroupsResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     PerformanceInsightsReferenceComparisonValuesTypeDef,
     RecommendationTypeDef,
     ListEventsResponseTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListInsightsResponseTypeDef,
@@ -532,28 +531,32 @@
     ListOrganizationInsightsResponseTypeDef,
     ListEventsRequestListEventsPaginateTypeDef,
     ListEventsRequestRequestTypeDef,
     SearchInsightsRequestRequestTypeDef,
     SearchInsightsRequestSearchInsightsPaginateTypeDef,
     SearchOrganizationInsightsRequestRequestTypeDef,
     SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
+    ListInsightsRequestListInsightsPaginateTypeDef,
+    ListInsightsRequestRequestTypeDef,
+    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    ListOrganizationInsightsRequestRequestTypeDef,
     PerformanceInsightsReferenceDataTypeDef,
     ListRecommendationsResponseTypeDef,
     PerformanceInsightsMetricsDetailTypeDef,
     AnomalySourceDetailsTypeDef,
     ProactiveAnomalySummaryTypeDef,
     ProactiveAnomalyTypeDef,
     ReactiveAnomalySummaryTypeDef,
     ReactiveAnomalyTypeDef,
     ListAnomaliesForInsightResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
 )
 
 
-def get_structure() -> AccountInsightHealthTypeDef:
+def get_value() -> AccountInsightHealthTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__init__.py` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__init__.pyi` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__main__.py` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DevOpsGuru 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.DevOpsGuru 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru\nOther"
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

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/client.py` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_devops_guru.client import DevOpsGuruClient
 
     session = Session()
     client: DevOpsGuruClient = session.client("devops-guru")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     InsightTypeType,
     LocaleType,
     OrganizationResourceCollectionTypeType,
@@ -40,16 +39,15 @@
     ListOrganizationInsightsPaginator,
     ListRecommendationsPaginator,
     SearchInsightsPaginator,
     SearchOrganizationInsightsPaginator,
 )
 from .type_defs import (
     AddNotificationChannelResponseTypeDef,
-    CostEstimationResourceCollectionFilterOutputTypeDef,
-    CostEstimationResourceCollectionFilterTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     DescribeFeedbackResponseTypeDef,
     DescribeInsightResponseTypeDef,
     DescribeOrganizationHealthResponseTypeDef,
@@ -69,21 +67,21 @@
     ListInsightsResponseTypeDef,
     ListInsightsStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
     ListRecommendationsResponseTypeDef,
-    NotificationChannelConfigOutputTypeDef,
-    NotificationChannelConfigTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     StartTimeRangeTypeDef,
+    TimestampTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -126,17 +124,15 @@
         DevOpsGuruClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#exceptions)
         """
 
     def add_notification_channel(
-        self,
-        *,
-        Config: Union[NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef]
+        self, *, Config: NotificationChannelConfigUnionTypeDef
     ) -> AddNotificationChannelResponseTypeDef:
         """
         Adds a notification channel to DevOps Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.add_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#add_notification_channel)
         """
@@ -173,15 +169,15 @@
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_account_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#describe_account_health)
         """
 
     def describe_account_overview(
-        self, *, FromTime: Union[datetime, str], ToTime: Union[datetime, str] = ...
+        self, *, FromTime: TimestampTypeDef, ToTime: TimestampTypeDef = ...
     ) -> DescribeAccountOverviewResponseTypeDef:
         """
         For the time range passed in, returns the number of open reactive insight that
         were created, the number of open proactive insights that were created, and the
         Mean Time to Recover (MTTR) for all closed reactive insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_account_overview)
@@ -232,16 +228,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_organization_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#describe_organization_health)
         """
 
     def describe_organization_overview(
         self,
         *,
-        FromTime: Union[datetime, str],
-        ToTime: Union[datetime, str] = ...,
+        FromTime: TimestampTypeDef,
+        ToTime: TimestampTypeDef = ...,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...
     ) -> DescribeOrganizationOverviewResponseTypeDef:
         """
         Returns an overview of your organization's history based on the specified time
         range.
 
@@ -481,18 +477,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#search_organization_insights)
         """
 
     def start_cost_estimation(
         self,
         *,
-        ResourceCollection: Union[
-            CostEstimationResourceCollectionFilterTypeDef,
-            CostEstimationResourceCollectionFilterOutputTypeDef,
-        ],
+        ResourceCollection: CostEstimationResourceCollectionFilterUnionTypeDef,
         ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
```

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/client.pyi` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_devops_guru.client import DevOpsGuruClient
 
     session = Session()
     client: DevOpsGuruClient = session.client("devops-guru")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     InsightTypeType,
     LocaleType,
     OrganizationResourceCollectionTypeType,
@@ -40,16 +39,15 @@
     ListOrganizationInsightsPaginator,
     ListRecommendationsPaginator,
     SearchInsightsPaginator,
     SearchOrganizationInsightsPaginator,
 )
 from .type_defs import (
     AddNotificationChannelResponseTypeDef,
-    CostEstimationResourceCollectionFilterOutputTypeDef,
-    CostEstimationResourceCollectionFilterTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     DescribeFeedbackResponseTypeDef,
     DescribeInsightResponseTypeDef,
     DescribeOrganizationHealthResponseTypeDef,
@@ -69,21 +67,21 @@
     ListInsightsResponseTypeDef,
     ListInsightsStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
     ListRecommendationsResponseTypeDef,
-    NotificationChannelConfigOutputTypeDef,
-    NotificationChannelConfigTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     StartTimeRangeTypeDef,
+    TimestampTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -121,17 +119,15 @@
         """
         DevOpsGuruClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#exceptions)
         """
     def add_notification_channel(
-        self,
-        *,
-        Config: Union[NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef]
+        self, *, Config: NotificationChannelConfigUnionTypeDef
     ) -> AddNotificationChannelResponseTypeDef:
         """
         Adds a notification channel to DevOps Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.add_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#add_notification_channel)
         """
@@ -163,15 +159,15 @@
         insights, and the number of metrics analyzed in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_account_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#describe_account_health)
         """
     def describe_account_overview(
-        self, *, FromTime: Union[datetime, str], ToTime: Union[datetime, str] = ...
+        self, *, FromTime: TimestampTypeDef, ToTime: TimestampTypeDef = ...
     ) -> DescribeAccountOverviewResponseTypeDef:
         """
         For the time range passed in, returns the number of open reactive insight that
         were created, the number of open proactive insights that were created, and the
         Mean Time to Recover (MTTR) for all closed reactive insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_account_overview)
@@ -216,16 +212,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_organization_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#describe_organization_health)
         """
     def describe_organization_overview(
         self,
         *,
-        FromTime: Union[datetime, str],
-        ToTime: Union[datetime, str] = ...,
+        FromTime: TimestampTypeDef,
+        ToTime: TimestampTypeDef = ...,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...
     ) -> DescribeOrganizationOverviewResponseTypeDef:
         """
         Returns an overview of your organization's history based on the specified time
         range.
 
@@ -446,18 +442,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#search_organization_insights)
         """
     def start_cost_estimation(
         self,
         *,
-        ResourceCollection: Union[
-            CostEstimationResourceCollectionFilterTypeDef,
-            CostEstimationResourceCollectionFilterOutputTypeDef,
-        ],
+        ResourceCollection: CostEstimationResourceCollectionFilterUnionTypeDef,
         ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
```

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/literals.py` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/literals.pyi` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/paginator.py` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/paginator.pyi` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/type_defs.py` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_devops_guru.type_defs import AccountInsightHealthTypeDef
 
-    data: AccountInsightHealthTypeDef = {...}
+    data: AccountInsightHealthTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -65,35 +65,31 @@
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
     "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
-    "DescribeAccountOverviewRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
     "InsightFeedbackTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
-    "DescribeOrganizationOverviewRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     "DescribeResourceCollectionHealthRequestRequestTypeDef",
-    "EndTimeRangeTypeDef",
     "EventResourceTypeDef",
-    "EventTimeRangeTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
     "InsightTimeRangeTypeDef",
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
-    "StartTimeRangeTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
@@ -126,26 +122,29 @@
     "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
     "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
+    "DescribeAccountOverviewRequestRequestTypeDef",
+    "DescribeOrganizationOverviewRequestRequestTypeDef",
+    "EndTimeRangeTypeDef",
+    "EventTimeRangeTypeDef",
+    "StartTimeRangeTypeDef",
     "DescribeFeedbackResponseTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    "ListInsightsClosedStatusFilterTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
-    "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
     "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
     "UpdateServiceIntegrationConfigTypeDef",
     "ServiceIntegrationConfigTypeDef",
@@ -157,21 +156,24 @@
     "ResourceCollectionTypeDef",
     "ServiceHealthTypeDef",
     "UpdateResourceCollectionFilterTypeDef",
     "DescribeEventSourcesConfigResponseTypeDef",
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     "CloudWatchMetricsDetailTypeDef",
     "GetCostEstimationResponseTypeDef",
+    "CostEstimationResourceCollectionFilterUnionTypeDef",
     "StartCostEstimationRequestRequestTypeDef",
+    "ListInsightsClosedStatusFilterTypeDef",
+    "ListInsightsAnyStatusFilterTypeDef",
     "ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     "ListAnomaliesForInsightRequestRequestTypeDef",
-    "ListInsightsStatusFilterTypeDef",
     "AnomalousLogGroupTypeDef",
     "NotificationChannelTypeDef",
     "AddNotificationChannelRequestRequestTypeDef",
+    "NotificationChannelConfigUnionTypeDef",
     "UpdateServiceIntegrationRequestRequestTypeDef",
     "DescribeServiceIntegrationResponseTypeDef",
     "PerformanceInsightsReferenceMetricTypeDef",
     "RecommendationRelatedAnomalyTypeDef",
     "GetResourceCollectionResponseTypeDef",
     "EventTypeDef",
     "MonitoredResourceIdentifierTypeDef",
@@ -183,18 +185,15 @@
     "ReactiveOrganizationInsightSummaryTypeDef",
     "ListEventsFiltersTypeDef",
     "SearchInsightsFiltersTypeDef",
     "SearchOrganizationInsightsFiltersTypeDef",
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     "DescribeResourceCollectionHealthResponseTypeDef",
     "UpdateResourceCollectionRequestRequestTypeDef",
-    "ListInsightsRequestListInsightsPaginateTypeDef",
-    "ListInsightsRequestRequestTypeDef",
-    "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    "ListOrganizationInsightsRequestRequestTypeDef",
+    "ListInsightsStatusFilterTypeDef",
     "ListAnomalousLogGroupsResponseTypeDef",
     "ListNotificationChannelsResponseTypeDef",
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     "RecommendationTypeDef",
     "ListEventsResponseTypeDef",
     "ListMonitoredResourcesResponseTypeDef",
     "ListInsightsResponseTypeDef",
@@ -204,14 +203,18 @@
     "ListOrganizationInsightsResponseTypeDef",
     "ListEventsRequestListEventsPaginateTypeDef",
     "ListEventsRequestRequestTypeDef",
     "SearchInsightsRequestRequestTypeDef",
     "SearchInsightsRequestSearchInsightsPaginateTypeDef",
     "SearchOrganizationInsightsRequestRequestTypeDef",
     "SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
+    "ListInsightsRequestListInsightsPaginateTypeDef",
+    "ListInsightsRequestRequestTypeDef",
+    "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    "ListOrganizationInsightsRequestRequestTypeDef",
     "PerformanceInsightsReferenceDataTypeDef",
     "ListRecommendationsResponseTypeDef",
     "PerformanceInsightsMetricsDetailTypeDef",
     "AnomalySourceDetailsTypeDef",
     "ProactiveAnomalySummaryTypeDef",
     "ProactiveAnomalyTypeDef",
     "ReactiveAnomalySummaryTypeDef",
@@ -403,36 +406,15 @@
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-    },
-)
-_OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
-    {
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class DescribeAccountOverviewRequestRequestTypeDef(
-    _RequiredDescribeAccountOverviewRequestRequestTypeDef,
-    _OptionalDescribeAccountOverviewRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDescribeAnomalyRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAnomalyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribeAnomalyRequestRequestTypeDef = TypedDict(
@@ -493,38 +475,14 @@
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
-_RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-    },
-)
-_OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationOverviewRequestRequestTypeDef",
-    {
-        "ToTime": Union[datetime, str],
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-    },
-    total=False,
-)
-
-
-class DescribeOrganizationOverviewRequestRequestTypeDef(
-    _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
-    _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
-):
-    pass
-
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -574,41 +532,24 @@
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
 
-EndTimeRangeTypeDef = TypedDict(
-    "EndTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 EventResourceTypeDef = TypedDict(
     "EventResourceTypeDef",
     {
         "Type": str,
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-EventTimeRangeTypeDef = TypedDict(
-    "EventTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-)
-
 GetCostEstimationRequestRequestTypeDef = TypedDict(
     "GetCostEstimationRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -690,23 +631,14 @@
     "ServiceCollectionTypeDef",
     {
         "ServiceNames": Sequence[ServiceNameType],
     },
     total=False,
 )
 
-StartTimeRangeTypeDef = TypedDict(
-    "StartTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -1095,14 +1027,86 @@
     {
         "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterTypeDef,
         "Tags": Sequence[TagCostEstimationResourceCollectionFilterTypeDef],
     },
     total=False,
 )
 
+_RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+    },
+)
+_OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
+    {
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeAccountOverviewRequestRequestTypeDef(
+    _RequiredDescribeAccountOverviewRequestRequestTypeDef,
+    _OptionalDescribeAccountOverviewRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+    },
+)
+_OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationOverviewRequestRequestTypeDef",
+    {
+        "ToTime": TimestampTypeDef,
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+    },
+    total=False,
+)
+
+
+class DescribeOrganizationOverviewRequestRequestTypeDef(
+    _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
+    _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
+):
+    pass
+
+
+EndTimeRangeTypeDef = TypedDict(
+    "EndTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EventTimeRangeTypeDef = TypedDict(
+    "EventTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+)
+
+StartTimeRangeTypeDef = TypedDict(
+    "StartTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1242,38 +1246,22 @@
 class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
     _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
     _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
 ):
     pass
 
 
-ListInsightsClosedStatusFilterTypeDef = TypedDict(
-    "ListInsightsClosedStatusFilterTypeDef",
-    {
-        "Type": InsightTypeType,
-        "EndTimeRange": EndTimeRangeTypeDef,
-    },
-)
-
 ListAnomaliesForInsightFiltersTypeDef = TypedDict(
     "ListAnomaliesForInsightFiltersTypeDef",
     {
         "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
-ListInsightsAnyStatusFilterTypeDef = TypedDict(
-    "ListInsightsAnyStatusFilterTypeDef",
-    {
-        "Type": InsightTypeType,
-        "StartTimeRange": StartTimeRangeTypeDef,
-    },
-)
-
 ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef = TypedDict(
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     {
         "Filters": ListMonitoredResourcesFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1471,14 +1459,18 @@
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CostEstimationResourceCollectionFilterUnionTypeDef = Union[
+    CostEstimationResourceCollectionFilterTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
+]
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
     },
 )
 _OptionalStartCostEstimationRequestRequestTypeDef = TypedDict(
@@ -1493,14 +1485,30 @@
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
 
+ListInsightsClosedStatusFilterTypeDef = TypedDict(
+    "ListInsightsClosedStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "EndTimeRange": EndTimeRangeTypeDef,
+    },
+)
+
+ListInsightsAnyStatusFilterTypeDef = TypedDict(
+    "ListInsightsAnyStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "StartTimeRange": StartTimeRangeTypeDef,
+    },
+)
+
 _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
@@ -1544,24 +1552,14 @@
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
 
-ListInsightsStatusFilterTypeDef = TypedDict(
-    "ListInsightsStatusFilterTypeDef",
-    {
-        "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
-        "Closed": ListInsightsClosedStatusFilterTypeDef,
-        "Any": ListInsightsAnyStatusFilterTypeDef,
-    },
-    total=False,
-)
-
 AnomalousLogGroupTypeDef = TypedDict(
     "AnomalousLogGroupTypeDef",
     {
         "LogGroupName": str,
         "ImpactStartTime": datetime,
         "ImpactEndTime": datetime,
         "NumberOfLogLinesScanned": int,
@@ -1582,14 +1580,17 @@
 AddNotificationChannelRequestRequestTypeDef = TypedDict(
     "AddNotificationChannelRequestRequestTypeDef",
     {
         "Config": NotificationChannelConfigTypeDef,
     },
 )
 
+NotificationChannelConfigUnionTypeDef = Union[
+    NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef
+]
 UpdateServiceIntegrationRequestRequestTypeDef = TypedDict(
     "UpdateServiceIntegrationRequestRequestTypeDef",
     {
         "ServiceIntegration": UpdateServiceIntegrationConfigTypeDef,
     },
 )
 
@@ -1812,107 +1813,24 @@
     "UpdateResourceCollectionRequestRequestTypeDef",
     {
         "Action": UpdateResourceCollectionActionType,
         "ResourceCollection": UpdateResourceCollectionFilterTypeDef,
     },
 )
 
-_RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
-    "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
-    "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListInsightsRequestListInsightsPaginateTypeDef(
-    _RequiredListInsightsRequestListInsightsPaginateTypeDef,
-    _OptionalListInsightsRequestListInsightsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListInsightsRequestRequestTypeDef = TypedDict(
-    "_RequiredListInsightsRequestRequestTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListInsightsRequestRequestTypeDef = TypedDict(
-    "_OptionalListInsightsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class ListInsightsRequestRequestTypeDef(
-    _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
-    "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
-    "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
-    _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
-    "_RequiredListOrganizationInsightsRequestRequestTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
-    "_OptionalListOrganizationInsightsRequestRequestTypeDef",
+ListInsightsStatusFilterTypeDef = TypedDict(
+    "ListInsightsStatusFilterTypeDef",
     {
-        "MaxResults": int,
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "NextToken": str,
+        "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
+        "Closed": ListInsightsClosedStatusFilterTypeDef,
+        "Any": ListInsightsAnyStatusFilterTypeDef,
     },
     total=False,
 )
 
-
-class ListOrganizationInsightsRequestRequestTypeDef(
-    _RequiredListOrganizationInsightsRequestRequestTypeDef,
-    _OptionalListOrganizationInsightsRequestRequestTypeDef,
-):
-    pass
-
-
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2159,14 +2077,107 @@
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
 
+_RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
+    "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
+    "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInsightsRequestListInsightsPaginateTypeDef(
+    _RequiredListInsightsRequestListInsightsPaginateTypeDef,
+    _OptionalListInsightsRequestListInsightsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListInsightsRequestRequestTypeDef = TypedDict(
+    "_RequiredListInsightsRequestRequestTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListInsightsRequestRequestTypeDef = TypedDict(
+    "_OptionalListInsightsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListInsightsRequestRequestTypeDef(
+    _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
+    "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
+    "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
+    _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
+    "_RequiredListOrganizationInsightsRequestRequestTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
+    "_OptionalListOrganizationInsightsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListOrganizationInsightsRequestRequestTypeDef(
+    _RequiredListOrganizationInsightsRequestRequestTypeDef,
+    _OptionalListOrganizationInsightsRequestRequestTypeDef,
+):
+    pass
+
+
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/type_defs.pyi` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_devops_guru.type_defs import AccountInsightHealthTypeDef
 
-    data: AccountInsightHealthTypeDef = {...}
+    data: AccountInsightHealthTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -64,35 +64,31 @@
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
     "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
-    "DescribeAccountOverviewRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
     "InsightFeedbackTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
-    "DescribeOrganizationOverviewRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     "DescribeResourceCollectionHealthRequestRequestTypeDef",
-    "EndTimeRangeTypeDef",
     "EventResourceTypeDef",
-    "EventTimeRangeTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
     "InsightTimeRangeTypeDef",
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
-    "StartTimeRangeTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
@@ -125,26 +121,29 @@
     "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
     "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
+    "DescribeAccountOverviewRequestRequestTypeDef",
+    "DescribeOrganizationOverviewRequestRequestTypeDef",
+    "EndTimeRangeTypeDef",
+    "EventTimeRangeTypeDef",
+    "StartTimeRangeTypeDef",
     "DescribeFeedbackResponseTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    "ListInsightsClosedStatusFilterTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
-    "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
     "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
     "UpdateServiceIntegrationConfigTypeDef",
     "ServiceIntegrationConfigTypeDef",
@@ -156,21 +155,24 @@
     "ResourceCollectionTypeDef",
     "ServiceHealthTypeDef",
     "UpdateResourceCollectionFilterTypeDef",
     "DescribeEventSourcesConfigResponseTypeDef",
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     "CloudWatchMetricsDetailTypeDef",
     "GetCostEstimationResponseTypeDef",
+    "CostEstimationResourceCollectionFilterUnionTypeDef",
     "StartCostEstimationRequestRequestTypeDef",
+    "ListInsightsClosedStatusFilterTypeDef",
+    "ListInsightsAnyStatusFilterTypeDef",
     "ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     "ListAnomaliesForInsightRequestRequestTypeDef",
-    "ListInsightsStatusFilterTypeDef",
     "AnomalousLogGroupTypeDef",
     "NotificationChannelTypeDef",
     "AddNotificationChannelRequestRequestTypeDef",
+    "NotificationChannelConfigUnionTypeDef",
     "UpdateServiceIntegrationRequestRequestTypeDef",
     "DescribeServiceIntegrationResponseTypeDef",
     "PerformanceInsightsReferenceMetricTypeDef",
     "RecommendationRelatedAnomalyTypeDef",
     "GetResourceCollectionResponseTypeDef",
     "EventTypeDef",
     "MonitoredResourceIdentifierTypeDef",
@@ -182,18 +184,15 @@
     "ReactiveOrganizationInsightSummaryTypeDef",
     "ListEventsFiltersTypeDef",
     "SearchInsightsFiltersTypeDef",
     "SearchOrganizationInsightsFiltersTypeDef",
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     "DescribeResourceCollectionHealthResponseTypeDef",
     "UpdateResourceCollectionRequestRequestTypeDef",
-    "ListInsightsRequestListInsightsPaginateTypeDef",
-    "ListInsightsRequestRequestTypeDef",
-    "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    "ListOrganizationInsightsRequestRequestTypeDef",
+    "ListInsightsStatusFilterTypeDef",
     "ListAnomalousLogGroupsResponseTypeDef",
     "ListNotificationChannelsResponseTypeDef",
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     "RecommendationTypeDef",
     "ListEventsResponseTypeDef",
     "ListMonitoredResourcesResponseTypeDef",
     "ListInsightsResponseTypeDef",
@@ -203,14 +202,18 @@
     "ListOrganizationInsightsResponseTypeDef",
     "ListEventsRequestListEventsPaginateTypeDef",
     "ListEventsRequestRequestTypeDef",
     "SearchInsightsRequestRequestTypeDef",
     "SearchInsightsRequestSearchInsightsPaginateTypeDef",
     "SearchOrganizationInsightsRequestRequestTypeDef",
     "SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
+    "ListInsightsRequestListInsightsPaginateTypeDef",
+    "ListInsightsRequestRequestTypeDef",
+    "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    "ListOrganizationInsightsRequestRequestTypeDef",
     "PerformanceInsightsReferenceDataTypeDef",
     "ListRecommendationsResponseTypeDef",
     "PerformanceInsightsMetricsDetailTypeDef",
     "AnomalySourceDetailsTypeDef",
     "ProactiveAnomalySummaryTypeDef",
     "ProactiveAnomalyTypeDef",
     "ReactiveAnomalySummaryTypeDef",
@@ -398,34 +401,15 @@
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-    },
-)
-_OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
-    {
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class DescribeAccountOverviewRequestRequestTypeDef(
-    _RequiredDescribeAccountOverviewRequestRequestTypeDef,
-    _OptionalDescribeAccountOverviewRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDescribeAnomalyRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAnomalyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribeAnomalyRequestRequestTypeDef = TypedDict(
@@ -482,36 +466,14 @@
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
-_RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-    },
-)
-_OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationOverviewRequestRequestTypeDef",
-    {
-        "ToTime": Union[datetime, str],
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-    },
-    total=False,
-)
-
-class DescribeOrganizationOverviewRequestRequestTypeDef(
-    _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
-    _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
-):
-    pass
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -557,41 +519,24 @@
 
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
-EndTimeRangeTypeDef = TypedDict(
-    "EndTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 EventResourceTypeDef = TypedDict(
     "EventResourceTypeDef",
     {
         "Type": str,
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-EventTimeRangeTypeDef = TypedDict(
-    "EventTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-)
-
 GetCostEstimationRequestRequestTypeDef = TypedDict(
     "GetCostEstimationRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -669,23 +614,14 @@
     "ServiceCollectionTypeDef",
     {
         "ServiceNames": Sequence[ServiceNameType],
     },
     total=False,
 )
 
-StartTimeRangeTypeDef = TypedDict(
-    "StartTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -1068,14 +1004,82 @@
     {
         "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterTypeDef,
         "Tags": Sequence[TagCostEstimationResourceCollectionFilterTypeDef],
     },
     total=False,
 )
 
+_RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+    },
+)
+_OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
+    {
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class DescribeAccountOverviewRequestRequestTypeDef(
+    _RequiredDescribeAccountOverviewRequestRequestTypeDef,
+    _OptionalDescribeAccountOverviewRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+    },
+)
+_OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationOverviewRequestRequestTypeDef",
+    {
+        "ToTime": TimestampTypeDef,
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+    },
+    total=False,
+)
+
+class DescribeOrganizationOverviewRequestRequestTypeDef(
+    _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
+    _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
+):
+    pass
+
+EndTimeRangeTypeDef = TypedDict(
+    "EndTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EventTimeRangeTypeDef = TypedDict(
+    "EventTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+)
+
+StartTimeRangeTypeDef = TypedDict(
+    "StartTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1205,38 +1209,22 @@
 
 class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
     _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
     _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
 ):
     pass
 
-ListInsightsClosedStatusFilterTypeDef = TypedDict(
-    "ListInsightsClosedStatusFilterTypeDef",
-    {
-        "Type": InsightTypeType,
-        "EndTimeRange": EndTimeRangeTypeDef,
-    },
-)
-
 ListAnomaliesForInsightFiltersTypeDef = TypedDict(
     "ListAnomaliesForInsightFiltersTypeDef",
     {
         "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
-ListInsightsAnyStatusFilterTypeDef = TypedDict(
-    "ListInsightsAnyStatusFilterTypeDef",
-    {
-        "Type": InsightTypeType,
-        "StartTimeRange": StartTimeRangeTypeDef,
-    },
-)
-
 ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef = TypedDict(
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     {
         "Filters": ListMonitoredResourcesFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1430,14 +1418,18 @@
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CostEstimationResourceCollectionFilterUnionTypeDef = Union[
+    CostEstimationResourceCollectionFilterTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
+]
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
     },
 )
 _OptionalStartCostEstimationRequestRequestTypeDef = TypedDict(
@@ -1450,14 +1442,30 @@
 
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
+ListInsightsClosedStatusFilterTypeDef = TypedDict(
+    "ListInsightsClosedStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "EndTimeRange": EndTimeRangeTypeDef,
+    },
+)
+
+ListInsightsAnyStatusFilterTypeDef = TypedDict(
+    "ListInsightsAnyStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "StartTimeRange": StartTimeRangeTypeDef,
+    },
+)
+
 _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
@@ -1497,24 +1505,14 @@
 
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
-ListInsightsStatusFilterTypeDef = TypedDict(
-    "ListInsightsStatusFilterTypeDef",
-    {
-        "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
-        "Closed": ListInsightsClosedStatusFilterTypeDef,
-        "Any": ListInsightsAnyStatusFilterTypeDef,
-    },
-    total=False,
-)
-
 AnomalousLogGroupTypeDef = TypedDict(
     "AnomalousLogGroupTypeDef",
     {
         "LogGroupName": str,
         "ImpactStartTime": datetime,
         "ImpactEndTime": datetime,
         "NumberOfLogLinesScanned": int,
@@ -1535,14 +1533,17 @@
 AddNotificationChannelRequestRequestTypeDef = TypedDict(
     "AddNotificationChannelRequestRequestTypeDef",
     {
         "Config": NotificationChannelConfigTypeDef,
     },
 )
 
+NotificationChannelConfigUnionTypeDef = Union[
+    NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef
+]
 UpdateServiceIntegrationRequestRequestTypeDef = TypedDict(
     "UpdateServiceIntegrationRequestRequestTypeDef",
     {
         "ServiceIntegration": UpdateServiceIntegrationConfigTypeDef,
     },
 )
 
@@ -1765,99 +1766,24 @@
     "UpdateResourceCollectionRequestRequestTypeDef",
     {
         "Action": UpdateResourceCollectionActionType,
         "ResourceCollection": UpdateResourceCollectionFilterTypeDef,
     },
 )
 
-_RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
-    "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
-    "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListInsightsRequestListInsightsPaginateTypeDef(
-    _RequiredListInsightsRequestListInsightsPaginateTypeDef,
-    _OptionalListInsightsRequestListInsightsPaginateTypeDef,
-):
-    pass
-
-_RequiredListInsightsRequestRequestTypeDef = TypedDict(
-    "_RequiredListInsightsRequestRequestTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListInsightsRequestRequestTypeDef = TypedDict(
-    "_OptionalListInsightsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class ListInsightsRequestRequestTypeDef(
-    _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
-):
-    pass
-
-_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
-    "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
-    "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
-    _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-):
-    pass
-
-_RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
-    "_RequiredListOrganizationInsightsRequestRequestTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
-    "_OptionalListOrganizationInsightsRequestRequestTypeDef",
+ListInsightsStatusFilterTypeDef = TypedDict(
+    "ListInsightsStatusFilterTypeDef",
     {
-        "MaxResults": int,
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "NextToken": str,
+        "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
+        "Closed": ListInsightsClosedStatusFilterTypeDef,
+        "Any": ListInsightsAnyStatusFilterTypeDef,
     },
     total=False,
 )
 
-class ListOrganizationInsightsRequestRequestTypeDef(
-    _RequiredListOrganizationInsightsRequestRequestTypeDef,
-    _OptionalListOrganizationInsightsRequestRequestTypeDef,
-):
-    pass
-
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2092,14 +2018,99 @@
 
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
+_RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
+    "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
+    "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInsightsRequestListInsightsPaginateTypeDef(
+    _RequiredListInsightsRequestListInsightsPaginateTypeDef,
+    _OptionalListInsightsRequestListInsightsPaginateTypeDef,
+):
+    pass
+
+_RequiredListInsightsRequestRequestTypeDef = TypedDict(
+    "_RequiredListInsightsRequestRequestTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListInsightsRequestRequestTypeDef = TypedDict(
+    "_OptionalListInsightsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListInsightsRequestRequestTypeDef(
+    _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
+    "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
+    "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
+    _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+):
+    pass
+
+_RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
+    "_RequiredListOrganizationInsightsRequestRequestTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
+    "_OptionalListOrganizationInsightsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListOrganizationInsightsRequestRequestTypeDef(
+    _RequiredListOrganizationInsightsRequestRequestTypeDef,
+    _OptionalListOrganizationInsightsRequestRequestTypeDef,
+):
+    pass
+
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/PKG-INFO` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DevOpsGuru 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 devops-guru type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 devops-guru type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devops-guru)](https://pepy.tech/project/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
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
@@ -397,20 +397,20 @@
 )
 
 
 def check_value(value: AnomalySeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
     ResponseMetadataTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
@@ -425,35 +425,31 @@
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
     TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DescribeAccountOverviewRequestRequestTypeDef,
+    TimestampTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
     InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
-    DescribeOrganizationOverviewRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
-    EndTimeRangeTypeDef,
     EventResourceTypeDef,
-    EventTimeRangeTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
-    StartTimeRangeTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
@@ -486,26 +482,29 @@
     DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
     CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
+    DescribeAccountOverviewRequestRequestTypeDef,
+    DescribeOrganizationOverviewRequestRequestTypeDef,
+    EndTimeRangeTypeDef,
+    EventTimeRangeTypeDef,
+    StartTimeRangeTypeDef,
     DescribeFeedbackResponseTypeDef,
     PutFeedbackRequestRequestTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListRecommendationsRequestListRecommendationsPaginateTypeDef,
-    ListInsightsClosedStatusFilterTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
-    ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
     NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
     ServiceIntegrationConfigTypeDef,
@@ -517,21 +516,24 @@
     ResourceCollectionTypeDef,
     ServiceHealthTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     UpdateEventSourcesConfigRequestRequestTypeDef,
     CloudWatchMetricsDetailTypeDef,
     GetCostEstimationResponseTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     StartCostEstimationRequestRequestTypeDef,
+    ListInsightsClosedStatusFilterTypeDef,
+    ListInsightsAnyStatusFilterTypeDef,
     ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     ListAnomaliesForInsightRequestRequestTypeDef,
-    ListInsightsStatusFilterTypeDef,
     AnomalousLogGroupTypeDef,
     NotificationChannelTypeDef,
     AddNotificationChannelRequestRequestTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     UpdateServiceIntegrationRequestRequestTypeDef,
     DescribeServiceIntegrationResponseTypeDef,
     PerformanceInsightsReferenceMetricTypeDef,
     RecommendationRelatedAnomalyTypeDef,
     GetResourceCollectionResponseTypeDef,
     EventTypeDef,
     MonitoredResourceIdentifierTypeDef,
@@ -543,18 +545,15 @@
     ReactiveOrganizationInsightSummaryTypeDef,
     ListEventsFiltersTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     DescribeOrganizationResourceCollectionHealthResponseTypeDef,
     DescribeResourceCollectionHealthResponseTypeDef,
     UpdateResourceCollectionRequestRequestTypeDef,
-    ListInsightsRequestListInsightsPaginateTypeDef,
-    ListInsightsRequestRequestTypeDef,
-    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    ListOrganizationInsightsRequestRequestTypeDef,
+    ListInsightsStatusFilterTypeDef,
     ListAnomalousLogGroupsResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     PerformanceInsightsReferenceComparisonValuesTypeDef,
     RecommendationTypeDef,
     ListEventsResponseTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListInsightsResponseTypeDef,
@@ -564,28 +563,32 @@
     ListOrganizationInsightsResponseTypeDef,
     ListEventsRequestListEventsPaginateTypeDef,
     ListEventsRequestRequestTypeDef,
     SearchInsightsRequestRequestTypeDef,
     SearchInsightsRequestSearchInsightsPaginateTypeDef,
     SearchOrganizationInsightsRequestRequestTypeDef,
     SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
+    ListInsightsRequestListInsightsPaginateTypeDef,
+    ListInsightsRequestRequestTypeDef,
+    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    ListOrganizationInsightsRequestRequestTypeDef,
     PerformanceInsightsReferenceDataTypeDef,
     ListRecommendationsResponseTypeDef,
     PerformanceInsightsMetricsDetailTypeDef,
     AnomalySourceDetailsTypeDef,
     ProactiveAnomalySummaryTypeDef,
     ProactiveAnomalyTypeDef,
     ReactiveAnomalySummaryTypeDef,
     ReactiveAnomalyTypeDef,
     ListAnomaliesForInsightResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
 )
 
 
-def get_structure() -> AccountInsightHealthTypeDef:
+def get_value() -> AccountInsightHealthTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/SOURCES.txt` & `mypy-boto3-devops-guru-1.28.16/mypy_boto3_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15.post1/setup.py` & `mypy-boto3-devops-guru-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devops-guru",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.DevOpsGuru 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 devops-guru type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 devops-guru type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_devops_guru": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

